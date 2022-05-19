---
title: Тип ресурса assignedPlan
description: Свойство **assignedPlans** объектов user и organization представляет собой коллекцию объектов **assignedPlan**.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: directory-management
author: jconley76
ms.openlocfilehash: 245f11e099bf648e9f8e88e1136b168beb1f30b1
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549563"
---
# <a name="assignedplan-resource-type"></a>Тип ресурса assignedPlan

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Свойство **assignedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **assignedPlan**.


## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assignedDateTime|DateTimeOffset|Дата и время назначения плана; например: 2013-01-02T19:32:30Z. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|capabilityStatus|[capabilityStatus](#capabilitystatus-values)|Условие назначения возможностей. Возможные значения: `Enabled`, `Warning`, `Suspended`, `Deleted`. `LockedOut`|
|service|String|Имя службы; Например, `exchange`.|
|servicePlanId|Guid|Идентификатор GUID, определяющий план обслуживания. Полный список идентификаторов GUID и их эквивалентных понятных имен служб см. в разделе "Названия продуктов и идентификаторы планов обслуживания для [лицензирования"](/azure/active-directory/enterprise-users/licensing-service-plan-reference).|


### <a name="capabilitystatus-values"></a>Значения capabilityStatus

| Member | Описание  |
|:---------------|:--------|
| Включено | Доступно для обычного использования. |
| Предупреждение | Доступно для обычного использования, но находится в льготном периоде. |
| Suspended | Недоступно, но все данные, связанные с возможностью, должны быть сохранены. |
| Deleted | Недоступно, и все данные, связанные с этой возможностью, могут быть удалены. |
| LockedOut | Недоступно для всех администраторов и пользователей, но все данные, связанные с этой возможностью, должны быть сохранены. |

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
<!--
{
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


