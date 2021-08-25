---
title: тип ресурса localizedName
description: Представляет локализованное имя, используемого в магазине терминов, которое определяет имя на локализованном языке.
author: vishriv
localization_priority: Normal
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: eb515cea31fd092d2040edddcff806355829ab79
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2021
ms.locfileid: "58515050"
---
# <a name="localizedname-resource-type"></a>тип ресурса localizedName

Пространство имен: microsoft.graph.termStore

Представляет локализованное имя, используемого в магазине [терминов,]которое определяет имя на локализованном языке. Дополнительные сведения см. [в деле localizedLabel.]

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|LanguageTag|Строка|Тег языка для метки.|
|name|String|Имя на локализованных языках.|

## <a name="relationships"></a>Связи
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
[магазин]: ../resources/termstore-store.md
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


