---
title: Список вложений
description: Получение списка объектов вложений.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 64b08f390e29f9ae58884284a609c961dfeaf292
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720629"
---
# <a name="list-attachments"></a><span data-ttu-id="a1923-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="a1923-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1923-104">Получение списка объектов вложений.</span><span class="sxs-lookup"><span data-stu-id="a1923-104">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="a1923-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1923-105">Permissions</span></span>
<span data-ttu-id="a1923-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1923-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1923-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1923-108">Permission type</span></span>      | <span data-ttu-id="a1923-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1923-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1923-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1923-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a1923-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a1923-111">Mail.Read</span></span>    |
|<span data-ttu-id="a1923-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1923-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1923-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a1923-113">Mail.Read</span></span>    |
|<span data-ttu-id="a1923-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1923-114">Application</span></span> | <span data-ttu-id="a1923-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a1923-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1923-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1923-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a1923-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a1923-117">Optional query parameters</span></span>
<span data-ttu-id="a1923-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a1923-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1923-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1923-119">Request headers</span></span>
| <span data-ttu-id="a1923-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a1923-120">Name</span></span>       | <span data-ttu-id="a1923-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a1923-121">Type</span></span> | <span data-ttu-id="a1923-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a1923-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a1923-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1923-123">Authorization</span></span>  | <span data-ttu-id="a1923-124">string</span><span class="sxs-lookup"><span data-stu-id="a1923-124">string</span></span>  | <span data-ttu-id="a1923-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1923-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1923-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1923-127">Request body</span></span>
<span data-ttu-id="a1923-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a1923-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1923-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1923-129">Response</span></span>

<span data-ttu-id="a1923-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a1923-130">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a1923-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a1923-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1923-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1923-132">Request</span></span>
<span data-ttu-id="a1923-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1923-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a1923-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1923-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "eventmessage_get_attachments_beta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a1923-135">C#</span><span class="sxs-lookup"><span data-stu-id="a1923-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/eventmessage-get-attachments-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a1923-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1923-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/eventmessage-get-attachments-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a1923-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a1923-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/eventmessage-get-attachments-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a1923-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1923-138">Response</span></span>
<span data-ttu-id="a1923-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1923-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "eventmessage_get_attachments_beta",
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
      "@odata.type":"#microsoft.graph.fileAttachment",
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
