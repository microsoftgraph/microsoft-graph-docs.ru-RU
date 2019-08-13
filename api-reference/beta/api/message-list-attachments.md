---
title: Список вложений
description: Получение списка объектов attachment, вложенных в сообщение.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4a5b9130a562ff15b1a9c13106c0528246805ce4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346914"
---
# <a name="list-attachments"></a><span data-ttu-id="30104-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="30104-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30104-104">Получение списка объектов [attachment](../resources/attachment.md), вложенных в сообщение.</span><span class="sxs-lookup"><span data-stu-id="30104-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="30104-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30104-105">Permissions</span></span>
<span data-ttu-id="30104-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30104-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30104-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30104-108">Permission type</span></span>      | <span data-ttu-id="30104-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30104-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30104-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30104-110">Delegated (work or school account)</span></span> | <span data-ttu-id="30104-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="30104-111">Mail.Read</span></span>    |
|<span data-ttu-id="30104-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30104-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30104-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="30104-113">Mail.Read</span></span>    |
|<span data-ttu-id="30104-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30104-114">Application</span></span> | <span data-ttu-id="30104-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="30104-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="30104-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30104-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="30104-117">Вложения [сообщения](../resources/message.md) в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="30104-117">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="30104-118">Вложения [сообщения](../resources/message.md) в папке [mailFolder](../resources/mailfolder.md) верхнего уровня в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="30104-118">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="30104-p102">Вложения [сообщения](../resources/message.md) в дочерней папке объекта [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя.  В приведенном ниже примере показан один уровень вложенности, но сообщение может находиться в папке, вложенной в дочернюю, и т. д.</span><span class="sxs-lookup"><span data-stu-id="30104-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="30104-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="30104-121">Optional query parameters</span></span>
<span data-ttu-id="30104-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="30104-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="30104-123">В частности, параметр запроса $expand можно использовать для включения всех вложений в сообщения, встроенных в остальные свойства сообщения.</span><span class="sxs-lookup"><span data-stu-id="30104-123">In particular, you can use the $expand query parameter to include all of the message attachments inline with the rest of the message properties.</span></span> <span data-ttu-id="30104-124">Пример:</span><span class="sxs-lookup"><span data-stu-id="30104-124">For example:</span></span>

```
GET https://graph.microsoft.com/beta/me/messages/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="30104-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30104-125">Request headers</span></span>
| <span data-ttu-id="30104-126">Имя</span><span class="sxs-lookup"><span data-stu-id="30104-126">Name</span></span>       | <span data-ttu-id="30104-127">Тип</span><span class="sxs-lookup"><span data-stu-id="30104-127">Type</span></span> | <span data-ttu-id="30104-128">Описание</span><span class="sxs-lookup"><span data-stu-id="30104-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="30104-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="30104-129">Authorization</span></span>  | <span data-ttu-id="30104-130">string</span><span class="sxs-lookup"><span data-stu-id="30104-130">string</span></span>  | <span data-ttu-id="30104-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30104-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30104-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="30104-133">Request body</span></span>
<span data-ttu-id="30104-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30104-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30104-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="30104-135">Response</span></span>

<span data-ttu-id="30104-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30104-136">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="30104-137">Пример</span><span class="sxs-lookup"><span data-stu-id="30104-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30104-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="30104-138">Request</span></span>
<span data-ttu-id="30104-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30104-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="30104-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="30104-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="30104-141">C#</span><span class="sxs-lookup"><span data-stu-id="30104-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="30104-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30104-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="30104-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="30104-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="30104-144">Java</span><span class="sxs-lookup"><span data-stu-id="30104-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-get-attachments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="30104-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="30104-145">Response</span></span>
<span data-ttu-id="30104-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30104-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
