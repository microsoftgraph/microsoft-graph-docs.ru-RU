---
title: Тип ресурса Контентинфо
description: Представляет текущее состояние некоторых сведений, которые необходимо подписать.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d7e0c159d46cb680329efc6a93896ca3df7270f7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998923"
---
# <a name="contentinfo-resource-type"></a>Тип ресурса Контентинфо

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние некоторых сведений, которые необходимо подписать. **контентинфо** передается в API [евалуатеремовал](../api/informationprotectionlabel-evaluateRemoval.md), [ЕВАЛУАТЕАППЛИКАТИОН](../api/informationprotectionlabel-evaluateApplication.md)и [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateClassificationResults.md) для описания API текущего состояния информации. В этом **контентинфо** подробные сведения о том, какие метаданные, маркировка содержимого и защита должны добавляться или удаляться при применении, обновлении или удалении метки. 

## <a name="properties"></a>Свойства

| Свойство   | Тип                                       | Описание                                                                                                                     |
| :--------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| format     | String                                     | Возможные значения: `default`, `email`.                                                                                        |
| идентификатор | String                                     | Идентификатор, используемый для аналитики Azure Information Protection.                                                                     |
| метаданных   | Коллекция [keyValuePair](keyvaluepair.md) | Существующие метаданные Microsoft Information Protection передаются в виде пар "ключ-значение", где ключ — это MSIP_Label_GUID_PropName. |
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

