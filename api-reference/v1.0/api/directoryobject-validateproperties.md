---
title: 'directoryObject: проверка Свойств'
description: Проверка соответствия отображаемого имени или почтового псевдонима группы Microsoft 365 политикам именования.
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 501ac437fed4870a7e5f40dd1297f9589b11dea3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016309"
---
# <a name="directoryobject-validateproperties"></a>directoryObject: проверка Свойств

Пространство имен: microsoft.graph

Проверка соответствия отображаемого имени или почтового псевдонима группы Microsoft 365 политикам именования.  Клиенты могут использовать этот API, чтобы определить, допустимо [](group-post-groups.md) ли имя или псевдоним почты перед попыткой создания Microsoft 365 группы. Чтобы проверить свойства существующей группы, используйте функцию [группы: validateProperties.](group-validateproperties.md)

Для свойств отображаемого имени и ником почты выполняются следующие проверки политики:
1. Проверка политики имен префикса и суффикса
2. Проверка настраиваемой политики запрещенных слов
3. Проверка уникальности псевдонима почты

Этот API возвращает только первый сбой проверки, с которым столкнулся. Если свойства не удается несколько проверки, возвращается только первая ошибка проверки. Однако вы можете проверить как имя почты, так и имя дисплея и получить коллекцию ошибок проверки, если вы только проверяете политику именования префикса и суффикса. Дополнительные новости о настройке политик имен см. в дополнительных подробной информации о политике [настройки имен.](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           | Описание      |
|:---------------|:-----------------|
| Авторизация  | Bearer {token}. Обязательный.    |
| Content-Type   | application/json |

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|entityType|String| Группа — это единственный поддерживаемый тип сущности. |
|displayName|Строка| Отображаемого имени группы для проверки. Свойство не требуется по отдельности. Однако требуется по крайней мере одно свойство **(displayName** или **mailNickname).** |
|mailNickname|String| Имя почты группы для проверки. Свойство не требуется по отдельности. Однако требуется по крайней мере одно свойство **(displayName** или **mailNickname).** |
|onBehalfOfUserId|Guid| ID пользователя, который должен выдать себя при вызове API. Результаты проверки для **атрибутов и ролей onBehalfOfUserId.** |

## <a name="response"></a>Отклик

В случае успешной проверки и без ошибок проверки метод возвращает `204 No Content` код ответа. Метод не возвращает данные в теле отклика.

Если запрос недействителен, метод возвращает `400 Bad Request` код ответа. Сообщение об ошибке с сведениями о недействительности запроса возвращается в тексте ответа.

При ошибке проверки метод возвращает `422 Unprocessable Entity` код ответа. Сообщение об ошибке и коллекция сведений об ошибках возвращаются в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-successful-validation-request"></a>Пример 1. Успешный запрос на проверку
Это пример успешного запроса на проверку.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/v1.0/directoryObjects/validateProperties
Content-type: application/json

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/directoryobject-validateproperties-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


### <a name="example-2-request-with-validation-errors"></a>Пример 2. Запрос с ошибками проверки
Это пример запроса с ошибками проверки.

#### <a name="request"></a>Запрос
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/validateProperties
Content-type: application/json

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

#### <a name="response"></a>Отклик
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

