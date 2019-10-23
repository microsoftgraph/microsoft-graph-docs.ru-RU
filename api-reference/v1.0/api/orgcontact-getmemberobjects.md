---
title: 'orgContact: getMemberObjects'
description: Возврат всех групп, членом которых является это организационное Контактное лицо. Это транзитивная проверка.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bbc577fe998d64a182051815124d364e9d3a7872
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37633931"
---
# <a name="orgcontact-getmemberobjects"></a>orgContact: getMemberObjects

Возврат всех групп, членом которых является это [организационное Контактное лицо](../resources/orgcontact.md) . Это транзитивная проверка. Организационные контакты не могут быть членами ролей каталогов. Роли каталога не возвращаются.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложения | OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Content-Type   | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|securityEnabledOnly|Логическое|Значение `false`. Возвращение лишь защищенных групп поддерживается только для пользователей.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос
Ниже приведен пример запроса.


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/contacts/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "groupID-value1"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
