---
title: 'Группа: validateProperties'
description: Проверьте, если группу Office 365 отображаемое имя или почты псевдонимов стандарту именования политик. Клиенты могут использовать API-Интерфейс для определения отображаемое имя или псевдоним почты является допустимым перед попыткой **обновления** группы с Office 365. Для проверки свойства перед созданием группы, используйте функцию validateProperties для объектов каталога.
localization_priority: Normal
ms.openlocfilehash: 0ffdf44f687ad047d952e00c268239432244006d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833903"
---
# <a name="group-validateproperties"></a>Группа: validateProperties

Проверьте, если группу Office 365 отображаемое имя или почты псевдонимов стандарту именования политик. Клиенты могут использовать API-Интерфейс для определения отображаемое имя или псевдоним почты является допустимым перед попыткой **обновления** группы с Office 365. Для проверки свойства перед созданием группы, используйте [функцию validateProperties](directoryobject-validateproperties.md) для объектов каталога.

Для свойства отображаемое имя и почты псевдонимов выполняются следующие проверки: 
1. Проверка префикс и суффикс, политика именования
2. Проверка настраиваемых запрещенных словах политики

Этот интерфейс API возвращает с первого ошибка. Если одно или несколько свойств с ошибкой нескольких проверок, возвращается только свойства с первого сбой проверки. Тем не менее можно проверить псевдоним почты и отображаемое имя и получить коллекцию ошибок проверки, если выполняется только проверка префикс и суффикс, политика именования.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Group.Read.All, Group.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Group.Read.All, Group.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/<id>/validateProperties
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           | Описание      |
|:---------------|:-----------------|
| Authorization  | Bearer {code}    |
| Content-Type   | application/json |

## <a name="request-body"></a>Тело запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|Строка| Отображаемое имя группы, чтобы проверить. Свойство не требуется по отдельности. Тем не менее по крайней мере одно свойство (отображаемое имя или mailNickname) является обязательным. |
|mailNickname|String| Псевдоним почты группы для проверки. Свойство не требуется по отдельности. Тем не менее по крайней мере одно свойство (отображаемое имя или mailNickname) является обязательным. |
|onBehalfOfUserId|Guid| Идентификатор объекта пользователя для олицетворения при вызове API. Результаты проверки используются атрибуты onBehalfOfUserId и роли. |

## <a name="response"></a>Ответ
В случае успешного выполнения и нет ошибок проверки, метод возвращает `204 No Content` код ответа. Он не возвращает все действия в теле ответа.

Если запрос является недопустимым, метод возвращает `400 Bad Request` код ответа. Сообщение об ошибке с подробными сведениями о недопустимый запрос возвращается в теле ответа.

В случае ошибки проверки. Метод возвращает `422 Unprocessable Entity` код ответа. Сообщение об ошибке и коллекцию сведений об ошибках, возвращается в теле ответа.

## <a name="examples"></a>Примеры

Это пример успешной проверки запроса.

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 132

{
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a>Ответ
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

Это пример запроса с ошибок проверки.

### <a name="request"></a>Запрос
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a>Ответ
```http
HTTP/1.1 422
Content-type: application/json
Content-length: 223

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "mailNickname",
        "code": "PropertyConflict",
        "message": "Another object with the same value for property mailNickname already exists."
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
