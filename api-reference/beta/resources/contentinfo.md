---
title: тип ресурса contentInfo
description: Представляет текущее состояние некоторых сведений, которые должны быть помечены.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 939d7730c0de2ffb13d4dbdcade6f7c2fbce5de4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962653"
---
# <a name="contentinfo-resource-type"></a>тип ресурса contentInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние некоторых сведений, которые должны быть помечены. **contentInfo** передается в a [evaluateRemoval,](../api/informationprotectionlabel-evaluateRemoval.md) [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md)и [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) API, чтобы описать API текущее состояние информации. В **этом содержимогоInfo** приводится информация о том, какие метаданные, маркировка контента и защита должны быть добавлены или удалены при нанесении, обновлении или удалении метки. 

## <a name="properties"></a>Свойства

| Свойство   | Тип                                       | Описание                                                                                                                     |
| :--------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| format     | String                                     | Возможные значения: `default`, `email`.                                                                                        |
| идентификатор | Строка                                     | Идентификатор, используемый для Azure Information Protection Analytics.                                                                     |
| метаданные   | Коллекция [keyValuePair](keyvaluepair.md) | Существующие метаданные Microsoft Information Protection передаются в виде пар ключей и значений, где ключом является MSIP_Label_GUID_PropName. |
| state      | String                                     | Возможные значения: `rest`, `motion`, `use`.                                                                                   |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.contentInfo",
  "baseType": null
}-->

```json
{
  "format": "String",
  "identifier": "String",
  "metadata": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contentInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

