---
title: тип ресурсов educationResource
description: Суперкласс для всех объектов ресурса в системе.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f817740ff7879d20788b46debad0824499f56498
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442439"
---
# <a name="educationresource-resource-type"></a>тип ресурсов educationResource

Пространство имен: microsoft.graph

Суперкласс для всех объектов ресурса в системе. Ресурс связан с  назначением и/или отправкой, представляюще обучающий объект, который передается или передается. Вы не можете мгновенно получить ресурс напрямую; необходимо сделать подкласс, который будет представлять тип используемого ресурса.

Этот ресурс сохраняет общие свойства для всех типов ресурсов.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Человек, создавший ресурс.|
|createdDateTime|DateTimeOffset|Момент создания ресурса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|displayName|String|Отображение имени ресурса.|
|lastModifiedBy|[identitySet](identityset.md)|Последний пользователь, который изменит ресурс.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения ресурса.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationResource"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


