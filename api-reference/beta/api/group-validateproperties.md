---
title: 'Группа: Валидатепропертиес'
description: Убедитесь, что отображаемое имя или псевдоним почты группы Microsoft 365 соответствует политикам именования.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 08089b1a3f0737f854e21cd9d72b06f684f48bdd
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953665"
---
# <a name="group-validateproperties"></a>Группа: Валидатепропертиес

Пространство имен: microsoft.graph

Убедитесь, что отображаемое имя или псевдоним почты группы Microsoft 365 соответствует политикам именования. Клиенты могут использовать API, чтобы определить, является ли отображаемое имя или псевдоним почты допустимым, прежде чем пытаться **Обновить** группу Microsoft 365. Для проверки свойств перед созданием группы используйте [функцию валидатепропертиес](directoryobject-validateproperties.md) для объектов Directory.

Для отображаемого имени и свойств псевдонима почты выполняются следующие проверки. 
1. Проверка политики именования префиксов и суффиксов
2. Проверка политики нестандартных запрещенных слов

Этот API возвращается при первом обнаружении ошибки. Если одно или несколько свойств не прошли несколько проверок, возвращается только свойство с первой ошибкой проверки. Тем не менее, вы можете проверить псевдоним почты и отображаемое имя и получить коллекцию ошибок проверки, если проверяется только политика именования префиксов и суффиксов.

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
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           | Описание      |
|:---------------|:-----------------|
| Авторизация  | Bearer {code}    |
| Content-Type   | application/json |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|String| Отображаемое имя группы, которую требуется проверить. Свойство не обязательно должно быть обязательным. Однако необходимо указать по крайней мере одно свойство (displayName или mailNickname). |
|mailNickname|String| Псевдоним почты для группы, которую требуется проверить. Свойство не обязательно должно быть обязательным. Однако необходимо указать по крайней мере одно свойство (displayName или mailNickname). |
|онбехалфофусерид|Guid| Идентификатор объекта пользователя, который олицетворяет при вызове API. Результаты проверки предназначены для атрибутов и ролей Онбехалфофусерид. |

## <a name="response"></a>Отклик
При успешном выполнении и отсутствии ошибок проверки метод возвращает `204 No Content` код отклика. Метод не возвращает данные в теле отклика.

Если запрос является недопустимым, метод возвращает `400 Bad Request` код отклика. В тексте отклика возвращается сообщение об ошибке со сведениями о недопустимом запросе.

При возникновении ошибки проверки. Метод возвращает `422 Unprocessable Entity` код отклика. В тексте отклика возвращается сообщение об ошибке и коллекция сведений об ошибке.

## <a name="examples"></a>Примеры

В этом примере показан успешный запрос на проверку.

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

Это пример запроса с ошибками проверки.

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

### <a name="response"></a>Отклик
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
  "tocPath": "",
  "suppressions": [
  ]
}-->


