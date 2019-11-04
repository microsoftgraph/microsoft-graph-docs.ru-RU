---
title: Удаление Календарпермиссион
description: Удаление Календарпермиссион.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 13756f6a5c84b999b7322341b65030767535807c
ms.sourcegitcommit: 1a3ca53422fc9a8254e78af7c058e876fc9f9ef8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2019
ms.locfileid: "37942652"
---
# <a name="delete-calendarpermission"></a>Удаление Календарпермиссион

Удаление Календарпермиссион.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Calendars.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Calendars.ReadWrite    |
|Для приложений | Calendars.ReadWrite |
## <a name="http-request"></a>HTTP-запрос

Удаление указанных разрешений для основного календаря пользователя:
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/calendar/calendarPermissions/{id}
```

Удаление указанных разрешений для календаря группы:
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/calendar/calendarPermissions/{id}
```

Удаление указанных разрешений для календаря пользователя, содержащего идентифицированное событие:
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {token} |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "delete_calendarpermission"
}-->

```http
DELETE https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
```

### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete calendarPermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->