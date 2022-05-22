---
title: Тип ресурса assignedPlan
description: Свойство **assignedPlans** объектов user и organization представляет собой коллекцию объектов **assignedPlan**.
ms.localizationpriority: medium
author: jconley76
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9338ae282f8c908aade2d0b2829c074c0f71f72e
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629212"
---
# <a name="assignedplan-resource-type"></a>Тип ресурса assignedPlan

Пространство имен: microsoft.graph

Свойство **assignedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **assignedPlan**.


## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assignedDateTime|DateTimeOffset|Дата и время назначения плана. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|capabilityStatus|String|Условие назначения возможностей. Возможные значения: `Enabled`, `Warning`, `Suspended`, `Deleted`. `LockedOut` См [. подробное описание](#capabilitystatus-values) каждого значения.|
|service|String|Имя службы; Например, `exchange`.|
|servicePlanId|Guid|Идентификатор GUID, определяющий план обслуживания. Полный список идентификаторов GUID и их эквивалентных понятных имен служб см. в разделе "Названия продуктов и идентификаторы планов обслуживания для [лицензирования"](/azure/active-directory/enterprise-users/licensing-service-plan-reference).|


### <a name="capabilitystatus-values"></a>Значения capabilityStatus

В следующей таблице описаны возможные состояния **для параметра capabilityStatus** подписки. Участники перечисляются в порядке перехода, если лицензия не продлена.

| Member | Описание  |
|:---------------|:--------|
| Включено | Доступно для обычного использования и назначения. |
| Предупреждение | Доступно для обычного использования и назначения, но находится в льготном периоде. |
| Suspended | Недоступно для назначения, но все данные, связанные с возможностью, должны быть сохранены. |
| LockedOut | Недоступно для всех администраторов и пользователей для назначения, но все данные, связанные с этой возможностью, должны быть сохранены. Это состояние после и `Suspended` , если лицензия не продлена, это конечное состояние перед началом плана `Deleted`. |
| Deleted | Недоступно, и все данные, связанные с этой возможностью, могут быть удалены. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedPlan"
}-->

```json
{
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "String",
  "service": "String",
  "servicePlanId": "Guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

