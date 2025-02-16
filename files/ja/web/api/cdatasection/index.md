---
title: CDATASection
slug: Web/API/CDATASection
---

{{APIRef("DOM")}}

**`CDATA セクション`** 内では、通常の文字として XML 内に記述する場合に実態参照として記述する必要がある < や & など（※本来これらは `&lt;` や `&amp;` のように記述する必要がある）を、エスケープ無しでそのまま記述する事ができます。

構文は以下のような形となります。

```
<![CDATA[  ... ]]>
```

実際の使用例を以下に示します。

```xml
<foo>次の部分は CDATA セクションです: <![CDATA[  < > & ]]> ... その他にも、通常エスケープが必要な文字を全てエスケープ無しで記述可能。</foo>
```

`]]>` は CDATA セクション自体の終了部分として解釈される為、このシーケンスのみは CDATA セクションに記述する事が出来ません。例えば以下の様な記述はエラーとなるでしょう。

```xml
<![CDATA[  ]]> 任意のテキスト   ]]>
```

CDATA セクションは（非表示のものを除き）HTML 内で使用されるべきではないことに注意してください。XML でのみ使用可能です。

CDATA セクション自体は固有のプロパティやメソッドは持ちません。{{domxref("Text")}} インタフェースに実装されたメソッドとプロパティを利用する事ができます。

## 仕様

| 仕様                                                                                             | 状態                             | コメント                                                                    |
| ------------------------------------------------------------------------------------------------ | -------------------------------- | --------------------------------------------------------------------------- |
| {{SpecName('DOM WHATWG', '#dom-core-changes', 'CDATASection')}}             | {{Spec2('DOM WHATWG')}} | [issue #295](https://github.com/whatwg/dom/pull/295) のため再度追加された。 |
| {{SpecName('DOM3 Core', 'core.html#ID-667469212', 'CDATASection')}}         | {{Spec2('DOM3 Core')}}     | {{SpecName('DOM2 Core')}} からの変更なし。                           |
| {{SpecName('DOM2 Core', 'core.html#ID-667469212', 'CDATASection')}}         | {{Spec2('DOM2 Core')}}     | {{SpecName('DOM1')}} からの変更なし。                               |
| {{SpecName('DOM1', 'level-one-core.html#ID-667469212', 'CDATASection')}} | {{Spec2('DOM1')}}         | 最初の定義                                                                  |
