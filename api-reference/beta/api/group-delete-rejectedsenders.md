---
title: Удаление объекта rejectedSender
description: Удаление пользователя или группы из списка отклоненных отправителей.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 309a859fd45152fc4cd5e29e3d84db7e8c07664e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593323"
---
# <a name="remove-rejectedsender"></a>Удаление объекта rejectedSender

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаление пользователя или группы из списка отклоненных отправителей для указанной группы.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)  |
|:---------------------------------------|:-------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Group.ReadWrite.All  |  
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id={id}
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок         | Значение                      |
|:---------------|:---------------------------|
| Авторизация  | Bearer {токен}. Обязательный.  

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.

## <a name="examples"></a>Примеры
### <a name="example-1-remove-a-user-from-the-rejected-senders-list-of-the-group"></a>Пример 1: Удаление пользователя из списка отклоненных отправителей группы.
#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "remove_user_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}
```
#### <a name="response"></a>Отклик
Ниже приведен пример отклика. 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>Пример кода для SDK
# <a name="ctabcs"></a>[Языках](#tab/cs)
[!INCLUDE [sample-code](../includes/remove_user_from_rejectedsenderslist_of_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Язык](#tab/javascript)
[!INCLUDE [sample-code](../includes/remove_user_from_rejectedsenderslist_of_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-remove-a-group-from-the-rejected-senders-list-of-the-group"></a>Пример 2: Удаление группы из списка отклоненных отправителей группы.
#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "remove_group_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```

#### <a name="response"></a>Отклик
Ниже приведен пример отклика. 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>Пример кода для SDK
# <a name="ctabcs"></a>[Языках](#tab/cs)
[!INCLUDE [sample-code](../includes/remove_group_from_rejectedsenderslist_of_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Язык](#tab/javascript)
[!INCLUDE [sample-code](../includes/remove_group_from_rejectedsenderslist_of_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
