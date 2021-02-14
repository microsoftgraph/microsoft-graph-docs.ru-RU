---
title: Тип ресурса calendarPermission
description: Разрешения пользователя, которому совместно передается календарь.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8162220df0ebf6973f1b317c1e4c063dbc98de3e
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176705"
---
# <a name="calendarpermission-resource-type"></a>Тип ресурса calendarPermission

Разрешения пользователя, которому был передан календарь или которому делегирован доступ в клиенте Outlook.

Получать, обновлять и удалять разрешения календаря можно только от имени владельца календаря.

Получение разрешений календаря от имени пользователя или делегата возвращает пустую коллекцию разрешений календаря.

После того как для календаря настроены объекты [](../api/calendarpermission-update.md) sharee  или delegate, можно обновить только свойство роли, чтобы изменить разрешения sharee или delegate. Вы не **можете обновить** **свойство allowedRoles,** **emailAddress,** **isInsideOrganization** или **isRemovable.** Чтобы изменить эти свойства, [](../api/calendarpermission-delete.md) необходимо удалить соответствующий объект **calendarPermission** и создать в клиенте Outlook другого представителя или представителя.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Get calendarPermission](../api/calendarpermission-get.md) | [calendarPermission](calendarpermission.md) | Чтение свойств и связей объекта calendarPermission. |
| [Обновление](../api/calendarpermission-update.md) | [calendarPermission](calendarpermission.md) | Обновление объекта calendarPermission. |
| [удаление](../api/calendarpermission-delete.md); | Нет | Удаление объекта calendarPermission. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|allowedRoles|[Коллекция calendarRoleType](#calendarroletype-values)| Список разрешенных уровней разрешений общего доступа или делегирование для календаря. Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|
|emailAddress|[emailAddress](emailaddress.md)| Представляет делиться данными или делегатами, у которых есть доступ к календарю. Для обоймы "Моя организация" свойство **адреса** имеет null. Только для чтения. |
|id|String| Уникальный идентификатор пользователя (общего доступа или делегата), которому был передан календарь. Только для чтения.|
|isInsideOrganization|Логический| Имеет true, если пользователь в контексте (пользователь или делегат) находится в той же организации, что и владелец календаря.|
|isRemovable|Логический| `True` если пользователь может быть удален из списка sharees или делегатов для указанного календаря, в противном `false` случае. Пользователь "Моя организация" определяет разрешения, которые другие пользователи в организации имеют для данного календаря. Невозможно удалить "Моя организация" в качестве делиться в календаре.|
|role|[calendarRoleType](#calendarroletype-values)| Текущий уровень разрешений для доступа к календарю или делегата. |

### <a name="calendarroletype-values"></a>Значения calendarRoleType

| Member        | Описание |
|:--------------|:------------|
| Нет | Календарь не является общим для пользователя. |
| freeBusyRead | Пользователь — это пользователь, который может просматривать состояние занятости владельца в календаре. |
| limitedRead | Пользователь — это пользователь, который может просматривать состояние занятости, а также заголовки и расположения событий в календаре. |
| read | Пользователь — это пользователь, который может просматривать все сведения о событиях в календаре, кроме частных событий владельца. |
| write | Пользователь — это пользователь, который может просматривать все сведения (кроме частных событий) и редактировать события в календаре. |
| delegateWithoutPrivateEventAccess | Пользователь является делегатом, который имеет доступ на записи, но не может просматривать сведения о частных событиях владельца в календаре. |
| delegateWithPrivateEventAccess | Пользователь — это делегат, который имеет доступ на записи и может просматривать сведения о частных событиях владельца в календаре. |
| custom | Пользователь имеет настраиваемые разрешения на доступ к календарю. |


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.calendarPermission",
  "keyProperty": "id"
}-->

```json
{
  "allowedRoles": ["string"],
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "id": "String (identifier)",
  "isInsideOrganization": "boolean",
  "isRemovable": "boolean",
  "role": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendarPermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
