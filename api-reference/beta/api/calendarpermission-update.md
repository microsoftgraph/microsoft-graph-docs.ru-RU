---
title: Обновление календарпермиссион
description: Обновление свойств объекта календарпермиссион.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d1cd959c4ee083ff6ec26914c5f99ccd3d8c3c8f
ms.sourcegitcommit: 1a3ca53422fc9a8254e78af7c058e876fc9f9ef8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2019
ms.locfileid: "37942643"
---
# <a name="update-calendarpermission"></a>Обновление Календарпермиссион

Обновление свойств объекта Календарпермиссион.

## <a name="permissions"></a>Разрешения

В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Календарь | Делегированные (рабочая или учебная учетная запись) | Делегированное (личная учетная запись Майкрософт) | Приложение |
|:-----|:-----|:-----|:-----|
| календарь пользователя | Calendars.ReadWrite | Calendars.ReadWrite | Calendars.ReadWrite |
| календарь группы | Group.ReadWrite.All | Не поддерживается. | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

Обновление указанных разрешений для основного календаря пользователя:
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
```

Обновление указанных разрешений для календаря группы:
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/calendar/calendarPermissions/{id}
```

Обновление указанных разрешений для календаря пользователя, содержащего идентифицированное событие:
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Авторизация | Bearer {token} |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|алловедролес|Коллекция строк| Список разрешенных для общего доступа уровней разрешений для календаря. Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|
|emailAddress|[emailAddress](../resources/email.md)| Представляет общую папку, у которой есть доступ к календарю. Для общего доступа к общему ресурсу "Моя организация" свойство **Address** имеет значение null. |
|id|String| Уникальный идентификатор пользователя (общего доступа), с которым открыт общий доступ к календарю. Только для чтения.|
|исинсидеорганизатион|Логический| Значение true, если пользователь в контексте (Share) находится в той же организации, что и владелец календаря.|
|"несъемный"|Логический| `True`, если пользователь может быть удален из списка общих папок для указанного календаря, `false` в противном случае. Пользователь "Моя организация" определяет разрешения, которые пользователи в организации имеют в указанном календаре. Вы не можете удалить "Моя организация" как общий доступ к календарю.|
|role|календарролетипе| Текущий уровень разрешений общего календаря. Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [календарпермиссион](../resources/calendarpermission.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_calendarpermission"
}-->

```http
PATCH https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
Content-type: application/json

{
  "emailAddress": {
    "name": "My Organization",
  },
  "isRemovable": true,
  "isInsideOrganization": true,
  "role": "write",
  "allowedRoles": [
    "none",
    "freeBusyRead",
    "limitedRead",
    "read",
    "write"
  ],
  "id": "RGVmYXVsdA=="
}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "emailAddress": {
    "name": "My Organization",
  },
  "isRemovable": true,
  "isInsideOrganization": true,
  "role": "write",
  "allowedRoles": [
    "none",
    "freeBusyRead",
    "limitedRead",
    "read",
    "write"
  ],
  "id": "RGVmYXVsdA=="
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update calendarpermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->