---
title: Список вложений
description: Получение списка объектов attachment, вложенных в запись.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: eb5249592c6984ab20f4cad754f8b8d9eedf22bf
ms.sourcegitcommit: 36066afdced00f32838a03747d3e7760fc43683a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36453167"
---
# <a name="list-attachments"></a><span data-ttu-id="090db-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="090db-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="090db-104">Получение списка объектов [attachment](../resources/attachment.md), вложенных в запись.</span><span class="sxs-lookup"><span data-stu-id="090db-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="090db-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="090db-105">Permissions</span></span>
<span data-ttu-id="090db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="090db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="090db-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="090db-108">Permission type</span></span>      | <span data-ttu-id="090db-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="090db-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="090db-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="090db-110">Delegated (work or school account)</span></span> | <span data-ttu-id="090db-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="090db-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="090db-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="090db-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="090db-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="090db-113">Not supported.</span></span>    |
|<span data-ttu-id="090db-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="090db-114">Application</span></span> | <span data-ttu-id="090db-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="090db-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="090db-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="090db-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="090db-117">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="090db-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="090db-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="090db-118">Optional query parameters</span></span>
<span data-ttu-id="090db-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="090db-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="090db-120">В частности, вы можете использовать параметр запроса $expand, чтобы включить все вложенные вложения со всеми остальными свойствами POST.</span><span class="sxs-lookup"><span data-stu-id="090db-120">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="090db-121">Пример:</span><span class="sxs-lookup"><span data-stu-id="090db-121">For example:</span></span>

```
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="090db-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="090db-122">Request headers</span></span>
| <span data-ttu-id="090db-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="090db-123">Header</span></span>       | <span data-ttu-id="090db-124">Значение</span><span class="sxs-lookup"><span data-stu-id="090db-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="090db-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="090db-125">Authorization</span></span>  | <span data-ttu-id="090db-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="090db-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="090db-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="090db-128">Request body</span></span>
<span data-ttu-id="090db-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="090db-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="090db-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="090db-130">Response</span></span>

<span data-ttu-id="090db-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="090db-131">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="090db-132">Пример</span><span class="sxs-lookup"><span data-stu-id="090db-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="090db-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="090db-133">Request</span></span>
<span data-ttu-id="090db-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="090db-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="090db-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="090db-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_get_attachments_beta"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="090db-136">C#</span><span class="sxs-lookup"><span data-stu-id="090db-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="090db-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="090db-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="090db-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="090db-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="090db-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="090db-139">Response</span></span>
<span data-ttu-id="090db-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="090db-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "post_get_attachments_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
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
