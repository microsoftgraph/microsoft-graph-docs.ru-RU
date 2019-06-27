---
title: Удаление вложения
description: Удаление вложения из события календаря, сообщения, задачи Outlook или POST.
localization_priority: Normal
ms.openlocfilehash: 3ce9592699e3a870e5612d0c8fd7d96b0cfd1cd7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258326"
---
# <a name="delete-attachment"></a>Удаление вложения

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаление вложения из [события](../resources/event.md)календаря, [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [POST](../resources/post.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

* При доступе к вложениям в сообщениях: mail. ReadWrite
* При доступе к вложениям в событиях: Calendars. ReadWrite
* При доступе к вложениям в задачах Outlook: Tasks. ReadWrite
* При доступе к вложениям в записях групп: Group. ReadWrite. ALL

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a>HTTP-запрос

Вложения для [события](../resources/event.md).

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
-->

Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д.<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

Вложения для [задачи Outlook](../resources/outlooktask.md).
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/tasks/<id>/attachments/{id}
```

Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.
<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса на удаление вложения из данных, касающихся события.
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_attachment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_attachment-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_attachment-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/attachment-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/attachment-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/attachment-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
