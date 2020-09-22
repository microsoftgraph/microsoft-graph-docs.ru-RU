---
title: Тип ресурса Локализеднаме
description: Представляет локализованное имя, используемое в банке терминов, которое определяет имя на локализованном языке.
author: mohitpcad
ms.author: mopathak
localization_priority: Normal
ms.prod: sharepoint-taxonomy
doc_type: resourcePageType
ms.openlocfilehash: 5c9e6d4cd614c242e8f915fde71eadd07aa5de15
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973608"
---
# <a name="localizedname-resource-type"></a>Тип ресурса Локализеднаме

Пространство имен: Microsoft. Graph. банка

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет локализованное имя, используемое в [банке]терминов, которое определяет имя на локализованном языке. Дополнительные сведения см. в разделе [локализедлабел].

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|лангуажетаг|String|Тег языка для метки.|
|name|String|Имя на языке локализации.|

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
[store]: ../resources/termstore-store.md
[локализедлабел]: ../resources/termstore-localizedlabel.md

<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedName is the facet for containing the name of termGroup",
  "keywords": "termLocalizedLNameFacet,facet,resource",
  "section": "documentation",
  "tocPath": "TermLocalizedNameFacet",
  "tocBookmarks": {
    "Resources/termStore.termLocalizedName": "#"
  },
  "suppressions": []
}
-->


