---
title: 'group: validateProperties'
description: Проверка соответствия отображаемого имени или почтового псевдонима группы Microsoft 365 политикам именования.
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 96f3ea5420254a051feb3041b4d661a315305408
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209450"
---
# <a name="group-validateproperties"></a>group: validateProperties

Пространство имен: microsoft.graph

Проверка соответствия отображаемого имени или почтового псевдонима группы Microsoft 365 политикам именования. Клиенты могут использовать этот API, чтобы определить, является ли отображаемое имя или псевдоним почты допустимым, прежде чем пытаться обновить Microsoft 365 группу.[](group-update.md) Чтобы проверить свойства перед созданием группы, используйте [функцию directoryobject:validateProperties](directoryobject-validateproperties.md) .

Для свойств отображаемого имени и псевдонима почты выполняются следующие проверки политики:

1. Проверка политики именования префиксов и суффиксов
2. Проверка настраиваемой политики запрещенных слов

Этот API возвращает только первый обнаруженный сбой проверки. Если свойства не удается выполнить несколько проверк, возвращается только первый сбой проверки. Однако вы можете проверить псевдоним почты и отображаемое имя и получить коллекцию ошибок проверки, если проверяете только политику именования префиксов и суффиксов. Дополнительные сведения о настройке политик именования см. в разделе ["Настройка политики именования"](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Group.Read.All, Group.ReadWrite.All         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Приложение                            | Group.Read.All, Group.ReadWrite.All         |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {token}. Обязательный. |
| Content-Type  | application/json          |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр        | Тип   | Описание                                                                                                                                                              |
| :--------------- | :----- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| displayName      | Строка | Отображаемое имя проверяемой группы. Свойство не является обязательным по отдельности. Однако требуется по крайней мере одно свойство (**displayName** или **mailNickname**).  |
| mailNickname     | String | Псевдоним электронной почты проверяемой группы. Свойство не является обязательным по отдельности. Однако требуется по крайней мере одно свойство (**displayName** или **mailNickname**). |
| onBehalfOfUserId | Guid   | Идентификатор пользователя, олицетворяемого при вызове API. Результаты проверки предназначены для атрибутов и ролей **onBehalfOfUserId** .                                  |

## <a name="response"></a>Ответ

При успешном выполнении и отсутствии ошибок проверки метод возвращает `204 No Content` код отклика. Метод не возвращает данные в теле отклика.

Если запрос недопустим, метод возвращает код `400 Bad Request` ответа. В тексте ответа возвращается сообщение об ошибке с подробными сведениями о недопустимом запросе.

При возникновении ошибки проверки. Метод возвращает код `422 Unprocessable Entity` отклика. В тексте ответа возвращается сообщение об ошибке и коллекция сведений об ошибке.

## <a name="examples"></a>Примеры

### <a name="example-1-successful-validation-request"></a>Пример 1. Успешный запрос на проверку

Это пример успешного запроса на проверку.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json

{
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/group-validateproperties-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/group-validateproperties-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/group-validateproperties-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/group-validateproperties-powershell-snippets.md)]
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

### <a name="example-2-request-with-validation-errors"></a>Пример 2. Запрос с ошибками проверки

Это пример запроса с ошибками проверки.

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

#### <a name="response"></a>Отклик

```http
HTTP/1.1 422
Content-type: application/json

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
