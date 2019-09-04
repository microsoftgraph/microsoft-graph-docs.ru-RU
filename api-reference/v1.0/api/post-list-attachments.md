---
title: Список вложений
description: Получение списка объектов attachment, вложенных в запись.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 36bb1938c833abf6603c0579ce5ff6d1ebffb77a
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728470"
---
# <a name="list-attachments"></a><span data-ttu-id="c786a-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="c786a-103">List attachments</span></span>

<span data-ttu-id="c786a-104">Получение списка объектов [attachment](../resources/attachment.md), вложенных в запись.</span><span class="sxs-lookup"><span data-stu-id="c786a-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="c786a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c786a-105">Permissions</span></span>
<span data-ttu-id="c786a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c786a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c786a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c786a-108">Permission type</span></span>      | <span data-ttu-id="c786a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c786a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c786a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c786a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c786a-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c786a-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c786a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c786a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c786a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c786a-113">Not supported.</span></span>    |
|<span data-ttu-id="c786a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c786a-114">Application</span></span> | <span data-ttu-id="c786a-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c786a-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c786a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c786a-116">HTTP request</span></span>
<span data-ttu-id="c786a-117">Получение вложений для [записи](../resources/post.md) в [conversationThread](../resources/conversationthread.md) группы.</span><span class="sxs-lookup"><span data-stu-id="c786a-117">Get the attachments for a [post](../resources/post.md) in a [conversationThread](../resources/conversationthread.md) of a group.</span></span> <span data-ttu-id="c786a-118">Указать родительскую [беседу](../resources/conversation.md) необязательно.</span><span class="sxs-lookup"><span data-stu-id="c786a-118">Specifying the parent [conversation](../resources/conversation.md) is optional.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c786a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c786a-119">Optional query parameters</span></span>
<span data-ttu-id="c786a-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c786a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c786a-121">В частности, вы можете использовать параметр запроса $expand, чтобы включить все вложенные вложения со всеми остальными свойствами POST.</span><span class="sxs-lookup"><span data-stu-id="c786a-121">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="c786a-122">Пример:</span><span class="sxs-lookup"><span data-stu-id="c786a-122">For example:</span></span>

<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="c786a-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c786a-123">Request headers</span></span>
| <span data-ttu-id="c786a-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c786a-124">Header</span></span>       | <span data-ttu-id="c786a-125">Значение</span><span class="sxs-lookup"><span data-stu-id="c786a-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c786a-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c786a-126">Authorization</span></span>  | <span data-ttu-id="c786a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c786a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c786a-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c786a-129">Request body</span></span>
<span data-ttu-id="c786a-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c786a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c786a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c786a-131">Response</span></span>

<span data-ttu-id="c786a-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [вложений](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c786a-132">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c786a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c786a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c786a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c786a-134">Request</span></span>
<span data-ttu-id="c786a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c786a-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c786a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c786a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_get_attachments_v1",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJfolA==","AAMkADJ-aHAAA="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJfolA==/posts/AAMkADJ-aHAAA=/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c786a-137">C#</span><span class="sxs-lookup"><span data-stu-id="c786a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-get-attachments-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c786a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c786a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-get-attachments-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c786a-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c786a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-get-attachments-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c786a-140">Java</span><span class="sxs-lookup"><span data-stu-id="c786a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-get-attachments-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c786a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c786a-141">Response</span></span>
<span data-ttu-id="c786a-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c786a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "post_get_attachments_v1",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('1848753d-185d-4c08-a4e4-6ee40521d115')/threads('AAQkADJfolA%3D%3D')/posts('AAMkADJ-aHAAA%3D')/attachments",
    "value": [
        {
            "@odata.type": "#microsoft.graph.fileAttachment",
            "id": "AAMkADJ-aHAAABEgAQAO5ZYuLGBmNFnelXXQqAN6I=",
            "lastModifiedDateTime": "2019-08-23T01:53:41Z",
            "name": "FileAsAttachment.txt",
            "contentType": "text/plain",
            "size": 244,
            "isInline": false,
            "contentId": null,
            "contentLocation": null,
            "contentBytes": "VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu"
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
