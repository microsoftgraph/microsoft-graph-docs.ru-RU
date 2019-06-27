---
title: Список вложений
description: Получение списка объектов attachment, вложенных в запись.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a7ca9f0470e5ea97f7c0737087b6db282c90b740
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275168"
---
# <a name="list-attachments"></a><span data-ttu-id="a7006-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="a7006-103">List attachments</span></span>

<span data-ttu-id="a7006-104">Получение списка объектов [attachment](../resources/attachment.md), вложенных в запись.</span><span class="sxs-lookup"><span data-stu-id="a7006-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="a7006-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7006-105">Permissions</span></span>
<span data-ttu-id="a7006-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7006-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7006-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7006-108">Permission type</span></span>      | <span data-ttu-id="a7006-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7006-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7006-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7006-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a7006-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7006-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a7006-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7006-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7006-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7006-113">Not supported.</span></span>    |
|<span data-ttu-id="a7006-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7006-114">Application</span></span> | <span data-ttu-id="a7006-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7006-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7006-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7006-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a7006-117">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="a7006-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a7006-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a7006-118">Optional query parameters</span></span>
<span data-ttu-id="a7006-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a7006-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a7006-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7006-120">Request headers</span></span>
| <span data-ttu-id="a7006-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7006-121">Header</span></span>       | <span data-ttu-id="a7006-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a7006-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a7006-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7006-123">Authorization</span></span>  | <span data-ttu-id="a7006-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7006-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a7006-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a7006-126">Request body</span></span>
<span data-ttu-id="a7006-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7006-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7006-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7006-128">Response</span></span>

<span data-ttu-id="a7006-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a7006-129">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a7006-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a7006-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7006-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7006-131">Request</span></span>
<span data-ttu-id="a7006-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7006-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="a7006-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7006-133">Response</span></span>
<span data-ttu-id="a7006-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7006-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
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
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a7006-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="a7006-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a7006-138">C#</span><span class="sxs-lookup"><span data-stu-id="a7006-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_attachments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a7006-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="a7006-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_attachments-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a7006-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a7006-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_attachments-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/post-list-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/post-list-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/post-list-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
