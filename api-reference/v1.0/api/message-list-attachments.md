---
title: Список вложений
description: Получение списка объектов attachment, вложенных в сообщение.
author: abheek-das
ms.localizationpriority: high
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3d5a6e72c2db347ef97a6aaade0d14c34e4fe1d8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100746"
---
# <a name="list-attachments"></a>Список вложений

Пространство имен: microsoft.graph

Получение списка объектов [attachment](../resources/attachment.md), вложенных в сообщение.
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Mail.Read    |
|Делегированные (личная учетная запись Майкрософт) | Mail.Read    |
|Для приложений | Mail.Read |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д.
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_get_attachments_v1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-get-attachments-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-get-attachments-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-get-attachments-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-get-attachments-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/message-get-attachments-v1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/message-get-attachments-v1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик
Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "name": "message_get_attachments_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
