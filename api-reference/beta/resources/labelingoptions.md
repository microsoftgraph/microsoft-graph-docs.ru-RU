---
title: Тип ресурса labelingOptions
description: Представляет параметры маркировки, которые могут быть предоставлены API оценки.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 7d2409bf538de3d37ca32cdf2fd1afb78a659817
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950309"
---
# <a name="labelingoptions-resource-type"></a>Тип ресурса labelingOptions

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры маркировки, которые могут быть предоставлены API оценки. **LabelingOptions** необходимо передать в API [evaluateApplication,](../api/informationprotectionlabel-evaluateapplication.md) чтобы указать сведения о метки, которая должна быть применена. 

## <a name="properties"></a>Свойства

| Свойство               | Тип                                                | Описание                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| assignmentMethod       | Строка                                              | Возможные значения: `standard`, `privileged`, `auto`.                                                                        |
| downgradeJustification | [downgradeJustification](downgradejustification.md) | Объект обоснования понижения, который указывает, было ли понижение оправдано, и если да, то причина.                          |
| расширенные свойства     | Коллекция [keyValuePair](keyvaluepair.md)          | Расширенные свойства будут разобрано и возвращены в стандартном формате метаданных MIP с меткой в качестве части сведений о метки. |
| labelId                | Guid                                                | GUID метки, которая должна применяться к данным.                                                              |

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

