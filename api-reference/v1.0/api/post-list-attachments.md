---
title: Список вложений
description: Получение списка объектов attachment, вложенных в запись.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: bd5e0e1cb324540f1c32a158501113b2bf274a3c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510783"
---
# <a name="list-attachments"></a><span data-ttu-id="ebb62-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="ebb62-103">List attachments</span></span>

<span data-ttu-id="ebb62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebb62-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ebb62-105">Получение списка объектов [attachment](../resources/attachment.md), вложенных в запись.</span><span class="sxs-lookup"><span data-stu-id="ebb62-105">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="ebb62-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ebb62-106">Permissions</span></span>
<span data-ttu-id="ebb62-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebb62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebb62-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebb62-109">Permission type</span></span>      | <span data-ttu-id="ebb62-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebb62-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebb62-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebb62-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ebb62-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebb62-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ebb62-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebb62-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebb62-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebb62-114">Not supported.</span></span>    |
|<span data-ttu-id="ebb62-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebb62-115">Application</span></span> | <span data-ttu-id="ebb62-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebb62-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebb62-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebb62-117">HTTP request</span></span>
<span data-ttu-id="ebb62-118">Получение вложений для [записи](../resources/post.md) в [conversationThread](../resources/conversationthread.md) группы.</span><span class="sxs-lookup"><span data-stu-id="ebb62-118">Get the attachments for a [post](../resources/post.md) in a [conversationThread](../resources/conversationthread.md) of a group.</span></span> <span data-ttu-id="ebb62-119">Указать родительскую [беседу](../resources/conversation.md) необязательно.</span><span class="sxs-lookup"><span data-stu-id="ebb62-119">Specifying the parent [conversation](../resources/conversation.md) is optional.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ebb62-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ebb62-120">Optional query parameters</span></span>
<span data-ttu-id="ebb62-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ebb62-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="ebb62-122">В частности, вы можете использовать параметр запроса $expand, чтобы включить все вложенные вложения со всеми остальными свойствами POST.</span><span class="sxs-lookup"><span data-stu-id="ebb62-122">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="ebb62-123">Например:</span><span class="sxs-lookup"><span data-stu-id="ebb62-123">For example:</span></span>

<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="ebb62-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebb62-124">Request headers</span></span>
| <span data-ttu-id="ebb62-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ebb62-125">Header</span></span>       | <span data-ttu-id="ebb62-126">Значение</span><span class="sxs-lookup"><span data-stu-id="ebb62-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ebb62-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ebb62-127">Authorization</span></span>  | <span data-ttu-id="ebb62-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebb62-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ebb62-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ebb62-130">Request body</span></span>
<span data-ttu-id="ebb62-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ebb62-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebb62-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ebb62-132">Response</span></span>

<span data-ttu-id="ebb62-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [вложений](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ebb62-133">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ebb62-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ebb62-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebb62-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebb62-135">Request</span></span>
<span data-ttu-id="ebb62-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebb62-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ebb62-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebb62-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_get_attachments_v1",
  "sampleKeys": ["1848753d-185d-4c08-a4e4-6ee40521d115","AAQkADJfolA==","AAMkADJ-aHAAA="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJfolA==/posts/AAMkADJ-aHAAA=/attachments
```
# <a name="c"></a>[<span data-ttu-id="ebb62-138">C#</span><span class="sxs-lookup"><span data-stu-id="ebb62-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-get-attachments-v1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ebb62-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebb62-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-get-attachments-v1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ebb62-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebb62-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-get-attachments-v1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ebb62-141">Java</span><span class="sxs-lookup"><span data-stu-id="ebb62-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-get-attachments-v1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ebb62-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebb62-142">Response</span></span>
<span data-ttu-id="ebb62-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ebb62-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
