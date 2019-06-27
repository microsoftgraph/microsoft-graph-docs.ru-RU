---
title: checkMemberGroups
description: Проверка участия в указанном списке групп. Возвращает из списка те группы, в которых
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cb46306a7ea2298bec4abb9827d93787ca843f7e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274643"
---
# <a name="checkmembergroups"></a>checkMemberGroups

Проверка участия в указанном списке групп. Возвращает из списка те группы, в которых указанный пользователь состоит напрямую или транзитивно.

В одном запросе можно проверять до 20 групп. Эта функция поддерживает Office 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Office 365 не могут содержать групп. Следовательно, участие в группе Office 365 всегда непосредственное.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| Делегированное (рабочая или учебная учетная запись)     | ~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается.                                                                                                     |
| Для приложения                            | ~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All                             |

> **Примечание.** В настоящее время для вызова этого API требуется разрешение `Directory.Read.All` или выше. При использовании разрешений `User.Read.All` или `User.ReadWrite.All` возникает ошибка. Мы знаем об этой проблеме.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение                     |
| :------------ | :------------------------ |
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json          |

## <a name="request-body"></a>Тело запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр | Тип              | Описание           |
| :-------- | :---------------- | :-------------------- |
| groupIds  | Коллекция строк | Массив идентификаторов групп |

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.

## <a name="example"></a>Пример

Ниже приведен пример вызова этого API.

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a>Отклик

Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

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
    "string-value"
  ]
}
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/user_checkmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_checkmembergroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objective-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_checkmembergroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
