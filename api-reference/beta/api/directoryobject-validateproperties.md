---
title: 'directoryObject: validateProperties'
description: Проверьте, если группу Office 365 отображаемое имя или почты псевдонимов стандарту именования политик.  Клиенты могут использовать API-Интерфейс для определения отображаемое имя или псевдоним почты является допустимым перед попыткой **Создать** группу Office 365. Для проверки правильности свойств существующей группы, используйте функцию validateProperties для групп.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 515acb022150d091e7dcbbdecc1fb1adef849a88
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921320"
---
# <a name="directoryobject-validateproperties"></a>directoryObject: validateProperties

Проверьте, если группу Office 365 отображаемое имя или почты псевдонимов стандарту именования политик.  Клиенты могут использовать API-Интерфейс для определения отображаемое имя или псевдоним почты является допустимым перед попыткой **Создать** группу Office 365. Для проверки правильности свойств существующей группы, используйте [функцию validateProperties](group-validateproperties.md) для групп.

Для свойства отображаемое имя и почты псевдонимов выполняются следующие проверки: 
1. Проверка префикс и суффикс, политика именования
2. Проверка настраиваемых запрещенных словах политики
3. Проверка почты псевдонимов является уникальным

Этот интерфейс API возвращает с первого ошибка. Если одно или несколько свойств с ошибкой нескольких проверок, возвращается только свойства с первого сбой проверки. Тем не менее можно проверить псевдоним почты и отображаемое имя и получить коллекцию ошибок проверки, если выполняется только проверка префикс и суффикс, политика именования.

## <a name="prerequisites"></a>Необходимые компоненты

Для выполнения этот интерфейс API требуется следующее **разрешение** : *Group.Read.All*

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
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
|entityType|Строка| `Group`— Это тип только поддерживаемые сущности. |
|displayName|Строка| Отображаемое имя группы, чтобы проверить. Свойство не требуется по отдельности. Тем не менее по крайней мере одно свойство (отображаемое имя или mailNickname) является обязательным. |
|mailNickname|String| Псевдоним почты группы для проверки. Свойство не требуется по отдельности. Тем не менее по крайней мере одно свойство (отображаемое имя или mailNickname) является обязательным. |
|onBehalfOfUserId|Guid| Идентификатор объекта пользователя для олицетворения при вызове API. Результаты проверки используются атрибуты onBehalfOfUserId и роли. |

## <a name="response"></a>Ответ

В случае успешного выполнения и нет ошибок проверки, метод возвращает `204 No Content` код ответа. Он не возвращает все действия в теле ответа.

Если запрос является недопустимым, метод возвращает `400 Bad Request` код ответа. Сообщение об ошибке с подробными сведениями о недопустимый запрос возвращается в теле ответа.

Если ошибка проверки, метод возвращает `422 Unprocessable Entity` код ответа. Сообщение об ошибке и коллекцию сведений об ошибках, возвращается в теле ответа.

## <a name="examples"></a>Примеры

Это пример успешной проверки запроса.

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a>Ответ
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

Это пример запроса с ошибок проверки.

### <a name="request"></a>Запрос
```http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a>Ответ
```http
HTTP/1.1 422 
Content-Type: application/json

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "request-id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "displayName",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      },
      {
        "target": "mailNickname",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
