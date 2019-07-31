---
title: 'directoryObject: Валидатепропертиес'
description: Убедитесь, что отображаемое имя или псевдоним почты группы Office 365 соответствует политикам именования.  Клиенты могут использовать API, чтобы определить, является ли отображаемое имя или псевдоним почты допустимым, прежде чем пытаться **создать** группу Office 365. Для проверки свойств существующей группы используйте функцию Валидатепропертиес для групп.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6ffc7200ed36d752d11f459c2ff7eab225d663b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957747"
---
# <a name="directoryobject-validateproperties"></a>directoryObject: Валидатепропертиес

Убедитесь, что отображаемое имя или псевдоним почты группы Office 365 соответствует политикам именования.  Клиенты могут использовать API, чтобы определить, является ли отображаемое имя или псевдоним почты допустимым, прежде чем пытаться **создать** группу Office 365. Для проверки свойств существующей группы используйте [функцию валидатепропертиес](group-validateproperties.md) для групп.

Для отображаемого имени и свойств псевдонима почты выполняются следующие проверки. 
1. Проверка политики именования префиксов и суффиксов
2. Проверка политики нестандартных запрещенных слов
3. Проверка уникальности псевдонима почты

Этот API возвращается при первом обнаружении ошибки. Если одно или несколько свойств не прошли несколько проверок, возвращается только свойство с первой ошибкой проверки. Тем не менее, вы можете проверить псевдоним почты и отображаемое имя и получить коллекцию ошибок проверки, если проверяется только политика именования префиксов и суффиксов.

## <a name="prerequisites"></a>Необходимые условия

Для выполнения этого API требуются следующие **разрешения** : *Group. Read. ALL*

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           | Описание      |
|:---------------|:-----------------|
| Авторизация  | Bearer {code}    |
| Content-Type   | application/json |

## <a name="request-body"></a>Тело запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|Сущности|String| `Group`— единственный поддерживаемый тип объекта. |
|displayName|Строка| Отображаемое имя группы, которую требуется проверить. Свойство не обязательно должно быть обязательным. Однако необходимо указать по крайней мере одно свойство (displayName или mailNickname). |
|mailNickname|String| Псевдоним почты для группы, которую требуется проверить. Свойство не обязательно должно быть обязательным. Однако необходимо указать по крайней мере одно свойство (displayName или mailNickname). |
|Онбехалфофусерид|GUID| Идентификатор объекта пользователя, который олицетворяет при вызове API. Результаты проверки предназначены для атрибутов и ролей Онбехалфофусерид. |

## <a name="response"></a>Отклик

При успешном выполнении и отсутствии ошибок проверки метод возвращает `204 No Content` код отклика. В тексте отклика не возвращается никаких данных.

Если запрос является недопустимым, метод возвращает `400 Bad Request` код отклика. В тексте отклика возвращается сообщение об ошибке со сведениями о недопустимом запросе.

При возникновении ошибки проверки метод возвращает `422 Unprocessable Entity` код отклика. В тексте отклика возвращается сообщение об ошибке и коллекция сведений об ошибке.

## <a name="examples"></a>Примеры

В этом примере показан успешный запрос на проверку.

### <a name="request"></a>Запрос

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Цель — C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

Это пример запроса с ошибками проверки.

### <a name="request"></a>Запрос
```http
POST https://graph.microsoft.com/beta/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a>Отклик
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
