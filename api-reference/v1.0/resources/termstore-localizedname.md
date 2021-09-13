---
title: тип ресурса localizedName
description: Представляет локализованное имя, используемого в магазине терминов, которое определяет имя на локализованном языке.
author: vishriv
ms.localizationpriority: medium
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: e4ef39aff45906c70195a92dfe6c4cabe87385e8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128048"
---
# <a name="localizedname-resource-type"></a>тип ресурса localizedName

Пространство имен: microsoft.graph.termStore

Представляет локализованное имя, используемого в магазине [терминов,]которое определяет имя на локализованном языке. Дополнительные сведения см. [в деле localizedLabel.]

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|LanguageTag|String|Тег языка для метки.|
|name|String|Имя на локализованных языках.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.termStore.localizedName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.localizedName",
  "name": "String",
  "languageTag": "String"
}
```

[microsoft.graph.termStore.localizedLabel]: termstore-localizedlabel.md
[microsoft.graph.termstore.store]: termstore-store.md
[store]: ../resources/termstore-store.md
[локализованнаяLabel]: ../resources/termstore-localizedlabel.md

<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedName is the facet for containing the name of termGroup",
  "keywords": "termLocalizedLNameFacet,facet,resource",
  "section": "documentation",
  "tocPath": "TermLocalizedNameFacet",
  "tocBookmarks": {
    "Resources/termStore.termLocalizedName&quot;: &quot;#"
  },
  "suppressions": []
}
-->


