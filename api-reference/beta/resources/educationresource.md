---
title: Тип ресурса Едукатионресаурце
description: Суперкласс для всех объектов ресурсов в системе. Ресурс связан с **назначением** и/или **отправкой**, представляющим обучающий объект, который
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f48d9b0bab9fbabd7e76da7c8d4bc738de5a137b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979578"
---
# <a name="educationresource-resource-type"></a>Тип ресурса Едукатионресаурце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Суперкласс для всех объектов ресурсов в системе. Ресурс связан с **назначением** и/или **отправкой**, представляющим обучающий объект, который передается или передается. Невозможно напрямую создать экземпляр ресурса; необходимо создать подкласс, который будет представлять тип используемого ресурса.

В этом ресурсе хранятся общие свойства для всех типов ресурсов.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Кто создал ресурс.|
|createdDateTime|Момент создания ресурса.  DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|displayName|String|Отображаемое имя ресурса.|
|lastModifiedBy|[identitySet](identityset.md)|Кто последний пользователь изменил ресурс.|
|lastModifiedDateTime|DateTimeOffset|Момент времени последнего изменения ресурса.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

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


