---
title: тип ресурса calendarPermission
description: Разрешения пользователя, с которым общий календарь.
author: Harini84
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e88ca527cd1f38a0db29083c34c80f2e7b81bca4
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763382"
---
# <a name="calendarpermission-resource-type"></a>тип ресурса calendarPermission

Пространство имен: microsoft.graph

Разрешения пользователя, с которым календарь был общим или делегирован в клиенте Outlook.

Список, создание, получения, обновления и удаления разрешений календаря поддерживается от имени только владельца календаря.

Получение разрешений календаря календаря от имени sharee или делегата возвращает пустой набор разрешений календаря.

После того как для календаря настроена доля [](../api/calendarpermission-update.md) или делегат, можно обновить только свойство роли, чтобы изменить разрешения sharee или delegate.  Вы не **можете обновить** **разрешенныеroles,** **emailAddress,** **isInsideOrganization** или **isRemovable** property. Чтобы изменить эти свойства, [](../api/calendarpermission-delete.md) необходимо удалить соответствующий объект **calendarPermission** и создать другой sharee или делегировать в Outlook клиента.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление](../api/calendar-list-calendarpermissions.md) | [calendarPermission](calendarpermission.md) | Получите коллекцию объектов calendarPermission, описывающих удостоверения и роли пользователей, с которыми указанный календарь был общим или делегирован. |
| [Создание](../api/calendar-post-calendarpermissions.md) | [calendarPermission](calendarpermission.md) | Создание объекта calendarPermission. |
| [Get calendarPermission](../api/calendarpermission-get.md) | [calendarPermission](calendarpermission.md) | Чтение свойств и связей объекта calendarPermission. |
| [Обновление](../api/calendarpermission-update.md) | [calendarPermission](calendarpermission.md) | Обновление объекта calendarPermission. |
| [удаление](../api/calendarpermission-delete.md); | Нет | Удаление объекта calendarPermission. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|allowedRoles|[коллекция calendarRoleType](#calendarroletype-values)| Список разрешенных уровней разрешений для календаря. Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|
|emailAddress|[emailAddress](emailaddress.md)| Представляет долю или делегат, у которого есть доступ к календарю. Для sharee "Моя организация" свойство **адресов** является null. Только для чтения. |
|id|String| Уникальный идентификатор пользователя (sharee или delegate), с которым был разделен календарь. Только для чтения.|
|isInsideOrganization|Логический| True, если пользователь в контексте (sharee или delegate) находится внутри той же организации, что и владелец календаря.|
|isRemovable|Логический| `True` если пользователь может быть удален из списка участников или делегатов для указанного календаря, в `false` противном случае. Пользователь "Моя организация" определяет разрешения, которые другие пользователи организации имеют в заданном календаре. Нельзя удалить "Моя организация" в качестве sharee в календаре.|
|role|[calendarRoleType](#calendarroletype-values)| Текущий уровень разрешений для делиться календарем или делегировать. |

### <a name="calendarroletype-values"></a>значения calendarRoleType

| Member        | Описание |
|:--------------|:------------|
| Нет | Календарь не является общим для пользователя. |
| freeBusyRead | Пользователь — это sharee, который может просматривать состояние свободного или занятого владельца в календаре. |
| limitedRead | Пользователь — это пользователь, который может просматривать состояние свободного/занятого, а также заголовки и расположения событий в календаре. |
| read | Пользователь — это пользователь, который может просматривать все сведения о событиях в календаре, за исключением частных событий владельца. |
| write | Пользователь — это пользователь, который может просматривать все сведения (за исключением частных событий) и изменять события в календаре. |
| delegateWithoutPrivateEventAccess | Пользователь — это делегат, который имеет доступ к записи, но не может просматривать сведения о частных событиях владельца в календаре. |
| delegateWithPrivateEventAccess | Пользователь — это делегат, который имеет доступ к записи и может просматривать сведения о частных событиях владельца в календаре. |
| настраиваемый | Пользователь имеет настраиваемые разрешения для календаря. |

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
