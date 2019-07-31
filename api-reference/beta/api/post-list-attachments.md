---
title: Список вложений
description: Получение списка объектов attachment, вложенных в запись.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6a35aaf11f907de85e475af1ca2e5744311411d6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978849"
---
# <a name="list-attachments"></a><span data-ttu-id="6fb20-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="6fb20-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fb20-104">Получение списка объектов [attachment](../resources/attachment.md), вложенных в запись.</span><span class="sxs-lookup"><span data-stu-id="6fb20-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="6fb20-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6fb20-105">Permissions</span></span>
<span data-ttu-id="6fb20-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fb20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fb20-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6fb20-108">Permission type</span></span>      | <span data-ttu-id="6fb20-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6fb20-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fb20-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6fb20-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6fb20-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fb20-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6fb20-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6fb20-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fb20-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fb20-113">Not supported.</span></span>    |
|<span data-ttu-id="6fb20-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6fb20-114">Application</span></span> | <span data-ttu-id="6fb20-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fb20-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fb20-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6fb20-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="6fb20-117">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="6fb20-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6fb20-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6fb20-118">Optional query parameters</span></span>
<span data-ttu-id="6fb20-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6fb20-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="6fb20-120">В частности, вы можете использовать параметр запроса $expand, чтобы включить все вложенные вложения со всеми остальными свойствами POST.</span><span class="sxs-lookup"><span data-stu-id="6fb20-120">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="6fb20-121">Пример:</span><span class="sxs-lookup"><span data-stu-id="6fb20-121">For example:</span></span>

```
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="6fb20-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6fb20-122">Request headers</span></span>
| <span data-ttu-id="6fb20-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6fb20-123">Header</span></span>       | <span data-ttu-id="6fb20-124">Значение</span><span class="sxs-lookup"><span data-stu-id="6fb20-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6fb20-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6fb20-125">Authorization</span></span>  | <span data-ttu-id="6fb20-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6fb20-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6fb20-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6fb20-128">Request body</span></span>
<span data-ttu-id="6fb20-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6fb20-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fb20-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fb20-130">Response</span></span>

<span data-ttu-id="6fb20-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6fb20-131">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6fb20-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6fb20-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6fb20-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6fb20-133">Request</span></span>
<span data-ttu-id="6fb20-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6fb20-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6fb20-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fb20-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6fb20-136">C#</span><span class="sxs-lookup"><span data-stu-id="6fb20-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6fb20-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="6fb20-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6fb20-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6fb20-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6fb20-139">Java</span><span class="sxs-lookup"><span data-stu-id="6fb20-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-get-attachments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6fb20-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="6fb20-140">Response</span></span>
<span data-ttu-id="6fb20-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6fb20-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "isInline": false,
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
