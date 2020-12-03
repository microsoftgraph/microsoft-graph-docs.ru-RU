---
title: Тип ресурса assignedPlan
description: Свойство **assignedPlans** объектов user и organization представляет собой коллекцию объектов **assignedPlan**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: krbain
ms.openlocfilehash: fe546f2dd25ca7f65e1ce8299bfad9b9ce5be56d
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563424"
---
# <a name="assignedplan-resource-type"></a>Тип ресурса assignedPlan

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Свойство **assignedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **assignedPlan**.


## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|ассигнеддатетиме|DateTimeOffset|Дата и время назначения плана. Пример: 2013-01-02T19:32:30Z. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|капабилитистатус|[капабилитистатус](#capabilitystatus-values)|Условие назначения возможности. Возможные значения:,,, `Enabled` `Warning` `Suspended` `Deleted` , `LockedOut` .|
|service|String|Имя службы, например "Exchange".|
|сервицепланид|Guid|Идентификатор GUID, определяющий план обслуживания.|


### <a name="capabilitystatus-values"></a>значения Капабилитистатус

| Member | Описание  |
|:---------------|:--------|
| Включено | Доступен для обычного использования. |
| Предупреждение | Доступен для нормального использования, но находится в периоде отсрочки. |
| Suspended | Недоступно, но все данные, связанные с возможностью, должны быть сохранены. |
| Deleted | Все данные, связанные с возможностью, недоступны и могут быть удалены. |
| Блокировка | Недоступно для всех администраторов и пользователей, но все данные, связанные с этой возможностью, должны быть сохранены. |

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
  "capabilityStatus": "string",
  "service": "string",
  "servicePlanId": "guid"
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


