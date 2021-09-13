---
title: тип ресурса calendarPermission
description: Разрешения пользователя, с которым общий календарь.
ms.localizationpriority: medium
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 7d98bfb91cc1502fa8b2ae84027d824210f2010a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59027192"
---
# <a name="calendarpermission-resource-type"></a>тип ресурса calendarPermission

Пространство имен: microsoft.graph

Разрешения пользователя, с которым календарь был общим или делегирован в клиенте Outlook.

Получить, обновить и удалить разрешения календаря поддерживается от имени только владельца календаря.

Получение разрешений календаря календаря от имени sharee или делегата возвращает пустой набор разрешений календаря.

После того как для календаря настроена доля [](../api/calendarpermission-update.md) или делегат, можно обновить только свойство роли, чтобы изменить разрешения sharee или delegate.  Вы не **можете обновить** **разрешенныеroles,** **emailAddress,** **isInsideOrganization** или **isRemovable** property. Чтобы изменить эти свойства, [](../api/calendarpermission-delete.md) необходимо удалить соответствующий объект **calendarPermission** и создать другой sharee или делегировать в Outlook клиента.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Get calendarPermission](../api/calendarpermission-get.md) | [calendarPermission](calendarpermission.md) | Чтение свойств и связей объекта calendarPermission. |
| [Обновление](../api/calendarpermission-update.md) | [calendarPermission](calendarpermission.md) | Обновление объекта calendarPermission. |
| [удаление](../api/calendarpermission-delete.md); | Нет | Удаление объекта calendarPermission. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|allowedRoles|[коллекция calendarRoleType](#calendarroletype-values)| Список разрешенных уровней разрешений для календаря. Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|
|emailAddress|[emailAddress](emailaddress.md)| Представляет долю или делегат, у которого есть доступ к календарю. Для sharee "Моя организация" свойство **адресов** является null. Только для чтения. |
|id|String| Уникальный идентификатор пользователя (sharee или delegate), с которым был разделен календарь. Только для чтения.|
|isInsideOrganization|Boolean| True, если пользователь в контексте (sharee или delegate) находится внутри той же организации, что и владелец календаря.|
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

