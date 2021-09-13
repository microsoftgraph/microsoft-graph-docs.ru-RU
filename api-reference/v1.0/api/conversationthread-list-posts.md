---
title: Список публикаций
description: 'Получение публикаций из указанной цепочки. Можно указать родительский разговор и поток, или, '
ms.localizationpriority: medium
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 326737f5fe27e62aa7a455c70f892ace291ccec5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59050637"
---
# <a name="list-posts"></a>Список публикаций

Пространство имен: microsoft.graph

Получение записей из указанного потока. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Group.Read.All, Group.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Group.Read.All, Group.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{groupId}/threads/{threadId}/posts
GET /groups/{groupId}/conversations/{conversationId}/threads/{threadId}/posts

```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметр `$select` [запроса OData](/graph/query-parameters) для настройки ответа. `$expand` также поддерживается расширение определенных отношений, и только одно отношение может быть расширено в одном запросе.
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Post](../resources/post.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/02f3bafb-448c-487c-88c2-5fd65ce49a41/threads/AAQkADI5YzgxODgyLTExZDgtNDhkMS1iZDRjLTBhZGZiN2ExYWQxNwMkABAADW7fw6FZNEuyjrGA9R8SshAADW7fw6FZNEuyjrGA9R8Ssg==/posts
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-posts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-posts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-posts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-posts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик
Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('02f3bafb-448c-487c-88c2-5fd65ce49a41')/threads('AAQkADI5YzgxODgyLTExZDgtNDhkMS1iZDRjLTBhZGZiN2ExYWQxNwMkABAADW7fw6FZNEuyjrGA9R8SshAADW7fw6FZNEuyjrGA9R8Ssg%3D%3D')/posts",
  "value": [
    {
      "@odata.etag": "W/\"CQAAABYAAACWM1XFF4buR6Xp/9aBq6+wAAAAAAEK\"",
      "id": "AAMkADI5YzgxODgyLTExZDgtNDhkMS1iZDRjLTBhZGZiN2ExYWQxNwBGAAAAAAAmtAlgzc6xQZmiHzuqNLQ8BwCWM1XFF4buR6Xp-9aBq6_wAAAAAAEMAACWM1XFF4buR6Xp-9aBq6_wAAAAAAk9AAA=",
      "createdDateTime": "2021-04-14T07:01:07Z",
      "lastModifiedDateTime": "2021-04-14T07:01:08Z",
      "changeKey": "CQAAABYAAACWM1XFF4buR6Xp/9aBq6+wAAAAAAEK",
      "categories": [],
      "receivedDateTime": "2021-04-14T07:01:07Z",
      "hasAttachments": false,
      "body": {
        "contentType": "html",
        "content": "<html><body><div><div style=\"direction:ltr;\"><table border=\"0\" cellspacing=\"0\" cellpadding=\"0\" id=\"x_bodyTable\" style=\"vertical-align:top;width:100%;height:100%;border-spacing:0;border-collapse:collapse;margin:0;padding:0;border-width:0;box-sizing:border-box;\"><tr style=\"vertical-align:top;margin:0;padding:0;border-width:0;box-sizing:border-box;\"><td id=\"x_bodyCell\" style=\"vertical-align:top;direction:ltr;width:100%;height:100%;margin:0;padding:0;border-width:0;box-sizing:border-box;\"><table border=\"0\" cellspacing=\"0\" cellpadding=\"0\" id=\"x_content\" style=\"font-family:Segoe UI,Tahoma,Microsoft Sans Serif,Verdana,sans-serif;vertical-align:top;border-spacing:0;border-collapse:collapse;margin:0;padding:0;border-width:0;box-sizing:border-box;\"><tr style=\"vertical-align:top;margin:0;padding:0;border-width:0;box-sizing:border-box;\"><td style=\"font-family:Segoe UI,Tahoma,Microsoft Sans Serif,Verdana,sans-serif;vertical-align:top;height:64px;margin:0;padding:0 0 20px 0;border-width:0;box-sizing:border-box;\"><div style=\"color:#0072C6;font-size:18pt;vertical-align:top;margin:0;padding:0;border-width:0;box-sizing:border-box;\">Welcome to the Contoso Life group...."
      },
      "from": {
        "emailAddress": {
          "name": "Contoso Life",
          "address": "contosolife@M365x435773.onmicrosoft.com"
        }
      },
      "sender": {
        "emailAddress": {
          "name": "Contoso Life",
          "address": "contosolife@M365x435773.onmicrosoft.com"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
