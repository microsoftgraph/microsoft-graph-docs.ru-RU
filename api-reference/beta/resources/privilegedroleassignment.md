---
title: Тип ресурса privilegedRoleAssignment
description: 'Представляет назначение привилегированной ролей для определенного пользователя. '
localization_priority: Normal
ms.openlocfilehash: ec6bc34ecd56839c764592ff298475e8648f300b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823319"
---
# <a name="privilegedroleassignment-resource-type"></a>Тип ресурса privilegedRoleAssignment

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет назначение привилегированной ролей для определенного пользователя. 


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список privilegedRoleAssignment коллекции](../api/privilegedroleassignment-list.md) | [privilegedRoleAssignment](privilegedroleassignment.md) коллекции|Получите коллекцию объектов privilegedRoleAssignment.|
|[Получение privilegedRoleAssignment](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Чтение свойства и связи объекта privilegedRoleAssignment.|
|[Создание назначения](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| Создание нового назначения путем учета к коллекции назначений.|
|[Delete](../api/privilegedroleassignment-delete.md) | Нет |Удалите объект privilegedRoleAssignment. |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Сделайте как постоянное назначение ролей.|
|[makeEligible](../api/privilegedroleassignment-makeeligible.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Сделайте назначения ролей как подходящими.|
|[Мои](../api/privilegedroleassignment-my.md)|[privilegedRoleAssignment](privilegedroleassignment.md) коллекции|Получение назначения привилегированной роли текущего пользователя.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|expirationDateTime|dateTimeOffset|Даты-времени UTC при истечет назначения временные привилегированной роли. Для назначения постоянной роли значение null.|
|id|строка| Уникальный идентификатор для назначения привилегированной роли. Только для чтения. Это в формате «userId_roleId», где идентификатор пользователя — это строка идентификатора GUID для Azure AD идентификатор пользователя, а roleId — string GUID для идентификатора роль Azure администратора.|
|isElevated|boolean|**значение true,** если активирован назначения ролей. **значение false,** Если назначения ролей отключена.|
|resultMessage|string|Установка службы сообщения результата.|
|roleId|string|Идентификатор роли. В строковом формате GUID.|
|userId|string|Идентификатор пользователя. В строковом формате GUID.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| Только для чтения. Допускается значение null. Сведения о связанных ролей.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
}-->

```json
{
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isElevated": true,
  "resultMessage": "string",
  "roleId": "string",
  "userId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
