---
title: тип ресурса informationProtectionContentLabel
description: Описывает объект informationProtectionContentLabel, который определяет метаданные MIP на объекте.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: b4d113e0f8f6d8f057a93d9094533e7fa2d5be6c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962604"
---
# <a name="informationprotectioncontentlabel-resource-type"></a>тип ресурса informationProtectionContentLabel

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает объект informationProtectionContentLabel, который определяет метаданные MIP на объекте. **informationProtectionContentLabel** возвращается [решением API extractLabel](../api/informationprotectionlabel-extractLabel.md) на метку, которая в настоящее время применяется к файлу. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|assignmentMethod|Строка| Возможные значения: `standard`, `privileged`, `auto`.|
|creationDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|label|[labelDetails](labeldetails.md)| Сведения о мете, которая в настоящее время применяется к файлу. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.informationProtectionContentLabel",
  "baseType": null
}-->

```json
{
  "assignmentMethod": "String",
  "creationDateTime": "String (timestamp)",
  "label": {"@odata.type": "microsoft.graph.labelDetails"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionContentLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

