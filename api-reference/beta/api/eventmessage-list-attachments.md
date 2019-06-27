---
title: Список вложений
description: Получение списка объектов вложений.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a327ba6d0742689e5868afb708edebbd0534fe67
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259089"
---
# <a name="list-attachments"></a><span data-ttu-id="ae841-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="ae841-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae841-104">Получение списка объектов вложений.</span><span class="sxs-lookup"><span data-stu-id="ae841-104">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae841-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae841-105">Permissions</span></span>
<span data-ttu-id="ae841-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae841-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae841-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae841-108">Permission type</span></span>      | <span data-ttu-id="ae841-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae841-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae841-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae841-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae841-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ae841-111">Mail.Read</span></span>    |
|<span data-ttu-id="ae841-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae841-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae841-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ae841-113">Mail.Read</span></span>    |
|<span data-ttu-id="ae841-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae841-114">Application</span></span> | <span data-ttu-id="ae841-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ae841-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae841-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae841-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ae841-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ae841-117">Optional query parameters</span></span>
<span data-ttu-id="ae841-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ae841-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae841-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae841-119">Request headers</span></span>
| <span data-ttu-id="ae841-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ae841-120">Name</span></span>       | <span data-ttu-id="ae841-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ae841-121">Type</span></span> | <span data-ttu-id="ae841-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ae841-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ae841-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae841-123">Authorization</span></span>  | <span data-ttu-id="ae841-124">string</span><span class="sxs-lookup"><span data-stu-id="ae841-124">string</span></span>  | <span data-ttu-id="ae841-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae841-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae841-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ae841-127">Request body</span></span>
<span data-ttu-id="ae841-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae841-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae841-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae841-129">Response</span></span>

<span data-ttu-id="ae841-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ae841-130">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ae841-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ae841-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae841-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae841-132">Request</span></span>
<span data-ttu-id="ae841-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae841-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="ae841-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae841-134">Response</span></span>
<span data-ttu-id="ae841-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae841-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ae841-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="ae841-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ae841-139">C#</span><span class="sxs-lookup"><span data-stu-id="ae841-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_attachments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ae841-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="ae841-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_attachments-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ae841-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ae841-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_attachments-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/eventmessage-list-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/eventmessage-list-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/eventmessage-list-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
