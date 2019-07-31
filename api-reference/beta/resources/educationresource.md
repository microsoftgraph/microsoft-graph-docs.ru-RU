---
title: Тип ресурса Едукатионресаурце
description: Суперкласс для всех объектов ресурсов в системе. Ресурс связан с назначением **** и/или отправкой, представляющим обучающий объект, который ****
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8dfb996c863e3b2aa5e319fcd2b4dc6dd246751a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972609"
---
# <a name="educationresource-resource-type"></a>Тип ресурса Едукатионресаурце

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Суперкласс для всех объектов ресурсов в системе. Ресурс связан с назначением **** и/или отправкой, представляющим обучающий объект, который передается или передается. **** Невозможно напрямую создать экземпляр ресурса; необходимо создать подкласс, который будет представлять тип используемого ресурса.

В этом ресурсе хранятся общие свойства для всех типов ресурсов.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Кто создал ресурс.|
|createdDateTime|Момент создания ресурса.  DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|displayName|String|Отображаемое имя ресурса.|
|lastModifiedBy|[identitySet](identityset.md)|Кто последний пользователь изменил ресурс.|
|lastModifiedDateTime|DateTimeOffset|Момент времени последнего изменения ресурса.  Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|

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
