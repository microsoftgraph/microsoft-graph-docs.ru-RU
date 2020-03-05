---
title: Тип ресурса Лабелингоптионс
description: Представляет параметры меток, которые могут быть предоставлены API оценки.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 97557ad6e233506e5e074c408ffb04f83297f0af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523004"
---
# <a name="labelingoptions-resource-type"></a>Тип ресурса Лабелингоптионс

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры меток, которые могут быть предоставлены API оценки. **лабелингоптионс** необходимо передать в API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md) , чтобы указать сведения о метке, которую нужно применить. 

## <a name="properties"></a>Свойства

| Свойство               | Тип                                                | Описание                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| assignmentMethod       | String                                              | Возможные значения: `standard`, `privileged`, `auto`.                                                                        |
| довнградежустификатион | [довнградежустификатион](downgradejustification.md) | Объект выравнивания на более ранней версии, указывающий, было ли понижение по ширине, и, если да, то причина.                          |
| екстендедпропертиес     | Коллекция [keyValuePair](keyvaluepair.md)          | Расширенные свойства будут проанализированы и возвращены в стандартном формате метаданных МИП в составе сведений о метке. |
| лабелид                | GUID                                                | GUID метки, которая должна быть применена к данным.                                                              |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.labelingOptions",
  "baseType": null
}-->

```json
{
  "assignmentMethod": "String",
  "downgradeJustification": {"@odata.type": "microsoft.graph.downgradeJustification"},
  "extendedProperties": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "labelId": "Guid"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "labelingOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->