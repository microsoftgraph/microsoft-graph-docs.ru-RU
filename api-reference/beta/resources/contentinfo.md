---
title: Тип ресурса Контентинфо
description: Представляет текущее состояние некоторых сведений, которые необходимо подписать.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 04fcee1c95628782d4a959732afa88bf689e4ea7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507438"
---
# <a name="contentinfo-resource-type"></a>Тип ресурса Контентинфо

Пространство имен: Microsoft. Graph

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