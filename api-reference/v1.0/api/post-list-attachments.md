---
title: Список вложений
description: Получение списка объектов attachment, вложенных в запись.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2150f50d228dc0567152d5ccf233a76f71176d47
ms.sourcegitcommit: 36066afdced00f32838a03747d3e7760fc43683a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36453121"
---
# <a name="list-attachments"></a><span data-ttu-id="9b53c-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="9b53c-103">List attachments</span></span>

<span data-ttu-id="9b53c-104">Получение списка объектов [attachment](../resources/attachment.md), вложенных в запись.</span><span class="sxs-lookup"><span data-stu-id="9b53c-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="9b53c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9b53c-105">Permissions</span></span>
<span data-ttu-id="9b53c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b53c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b53c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b53c-108">Permission type</span></span>      | <span data-ttu-id="9b53c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b53c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b53c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b53c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9b53c-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b53c-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9b53c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b53c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b53c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b53c-113">Not supported.</span></span>    |
|<span data-ttu-id="9b53c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b53c-114">Application</span></span> | <span data-ttu-id="9b53c-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b53c-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b53c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b53c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="9b53c-117">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="9b53c-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9b53c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9b53c-118">Optional query parameters</span></span>
<span data-ttu-id="9b53c-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9b53c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9b53c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b53c-120">Request headers</span></span>
| <span data-ttu-id="9b53c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b53c-121">Header</span></span>       | <span data-ttu-id="9b53c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9b53c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9b53c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b53c-123">Authorization</span></span>  | <span data-ttu-id="9b53c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b53c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9b53c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9b53c-126">Request body</span></span>
<span data-ttu-id="9b53c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9b53c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b53c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b53c-128">Response</span></span>

<span data-ttu-id="9b53c-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9b53c-129">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9b53c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9b53c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9b53c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b53c-131">Request</span></span>
<span data-ttu-id="9b53c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b53c-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9b53c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b53c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_get_attachments_v1"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9b53c-134">C#</span><span class="sxs-lookup"><span data-stu-id="9b53c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9b53c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b53c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9b53c-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9b53c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9b53c-137">Java</span><span class="sxs-lookup"><span data-stu-id="9b53c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-get-attachments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9b53c-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="9b53c-138">Response</span></span>
<span data-ttu-id="9b53c-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b53c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "lastModifiedDateTime": "datetime-value",
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
