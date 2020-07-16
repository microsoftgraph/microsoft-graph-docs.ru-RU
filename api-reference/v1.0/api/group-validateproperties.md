---
title: 'Группа: Валидатепропертиес'
description: Убедитесь, что отображаемое имя или псевдоним почты группы Microsoft 365 соответствует политикам именования.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: acdc168df631a0db5eff277348cf4b0e43d85357
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897108"
---
# <a name="group-validateproperties"></a>Группа: Валидатепропертиес

Пространство имен: microsoft.graph

Убедитесь, что отображаемое имя или псевдоним почты группы Microsoft 365 соответствует политикам именования.  Клиенты могут использовать этот API, чтобы определить, является ли отображаемое имя или псевдоним почты допустимым, прежде чем пытаться [Обновить](group-update.md) группу Microsoft 365. Чтобы проверить свойства перед созданием группы, используйте функцию [directoryobject: валидатепропертиес](directoryobject-validateproperties.md) .

Для отображаемого имени и свойств псевдонима почты выполняются следующие проверки политик:
1. Проверка политики именования префиксов и суффиксов
2. Проверка политики нестандартных запрещенных слов

Этот API возвращает только первую обнаруженную ошибку проверки. Если свойства не прошли несколько проверок, возвращается только первый сбой проверки. Тем не менее, вы можете проверить псевдоним почты и отображаемое имя и получить коллекцию ошибок проверки, если проверяется только политика именования префиксов и суффиксов. Чтобы узнать больше о настройке политик именования, ознакомьтесь со статьей [Настройка политики именования](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Group.Read.All, Group.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Group.Read.All, Group.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           | Описание      |
|:---------------|:-----------------|
| Авторизация  | Bearer {токен}. Обязательный.    |
| Content-Type   | application/json |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|Строка| Отображаемое имя группы, которую требуется проверить. Свойство не обязательно должно быть обязательным. Однако необходимо указать по крайней мере одно свойство (**DisplayName** или **mailNickname**). |
|mailNickname|String| Псевдоним почты для группы, которую требуется проверить. Свойство не обязательно должно быть обязательным. Однако необходимо указать по крайней мере одно свойство (**DisplayName** или **mailNickname**). |
|онбехалфофусерид|Guid| Идентификатор пользователя, который олицетворяет при вызове API. Результаты проверки предназначены для атрибутов и ролей **онбехалфофусерид** . |

## <a name="response"></a>Отклик
При успешном выполнении и отсутствии ошибок проверки метод возвращает `204 No Content` код отклика. В тексте отклика не возвращается никаких данных.

Если запрос является недопустимым, метод возвращает `400 Bad Request` код отклика. В тексте отклика возвращается сообщение об ошибке со сведениями о недопустимом запросе.

При возникновении ошибки проверки. Метод возвращает `422 Unprocessable Entity` код отклика. В тексте отклика возвращается сообщение об ошибке и коллекция сведений об ошибке.

## <a name="examples"></a>Примеры

### <a name="example-1-successful-validation-request"></a>Пример 1: успешный запрос на проверку
В этом примере показан успешный запрос на проверку.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
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


#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-validation-errors"></a>Пример 2: запрос с ошибками проверки
Это пример запроса с ошибками проверки.

#### <a name="request"></a>Запросить
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

#### <a name="response"></a>Отклик
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
