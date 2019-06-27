---
title: Список моих решений Акцессревиев
description: В функции рецензирования Access в Azure AD извлекаются решения объекта Акцессревиев для вызывающего пользователя как проверяющего.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6b506ab17abe270bfd3ecc27ab70f7699487528a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258851"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="79cd4-103">Список моих решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="79cd4-103">List my accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79cd4-104">В функции рецензирования [Access](../resources/accessreviews-root.md) в Azure AD извлекаются решения объекта [акцессревиев](../resources/accessreview.md) для вызывающего пользователя как проверяющего.</span><span class="sxs-lookup"><span data-stu-id="79cd4-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="79cd4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79cd4-105">Permissions</span></span>
<span data-ttu-id="79cd4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79cd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79cd4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79cd4-108">Permission type</span></span>                        | <span data-ttu-id="79cd4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79cd4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="79cd4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79cd4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="79cd4-111">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="79cd4-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>   |
|<span data-ttu-id="79cd4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79cd4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79cd4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79cd4-113">Not supported.</span></span> |
|<span data-ttu-id="79cd4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79cd4-114">Application</span></span>                            | <span data-ttu-id="79cd4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79cd4-115">Not supported.</span></span> |

<span data-ttu-id="79cd4-116">Кроме того, вошедшего в систему пользователь должен иметь разрешение на чтение этой конкретной проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="79cd4-116">The signed in user must also be permitted to read this particular access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="79cd4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79cd4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="79cd4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79cd4-118">Request headers</span></span>
| <span data-ttu-id="79cd4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="79cd4-119">Name</span></span>         | <span data-ttu-id="79cd4-120">Тип</span><span class="sxs-lookup"><span data-stu-id="79cd4-120">Type</span></span>        | <span data-ttu-id="79cd4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="79cd4-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="79cd4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="79cd4-122">Authorization</span></span> | <span data-ttu-id="79cd4-123">string</span><span class="sxs-lookup"><span data-stu-id="79cd4-123">string</span></span> | <span data-ttu-id="79cd4-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79cd4-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79cd4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="79cd4-126">Request body</span></span>
<span data-ttu-id="79cd4-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="79cd4-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="79cd4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="79cd4-128">Response</span></span>
<span data-ttu-id="79cd4-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [акцессревиевдеЦисион](../resources/accessreviewdecision.md) в теле отклика, для которого вызывающий пользователь является назначенным рецензентом.</span><span class="sxs-lookup"><span data-stu-id="79cd4-129">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="79cd4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="79cd4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79cd4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="79cd4-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```

##### <a name="response"></a><span data-ttu-id="79cd4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="79cd4-132">Response</span></span>
><span data-ttu-id="79cd4-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79cd4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewDecision",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
            "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "accessReviewId": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "reviewResult": "Approve",
            "userPrincipalName": "alice@litware.com",
            "userId": "Alice Smith"
    }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="79cd4-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="79cd4-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="79cd4-136">C#</span><span class="sxs-lookup"><span data-stu-id="79cd4-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79cd4-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="79cd4-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="79cd4-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="79cd4-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="79cd4-139">См. также</span><span class="sxs-lookup"><span data-stu-id="79cd4-139">See also</span></span>

| <span data-ttu-id="79cd4-140">Метод</span><span class="sxs-lookup"><span data-stu-id="79cd4-140">Method</span></span>           | <span data-ttu-id="79cd4-141">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="79cd4-141">Return Type</span></span>    |<span data-ttu-id="79cd4-142">Описание</span><span class="sxs-lookup"><span data-stu-id="79cd4-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="79cd4-143">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="79cd4-143">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="79cd4-144">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="79cd4-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="79cd4-145">Получение проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="79cd4-145">Retrieve an access review.</span></span> |
|[<span data-ttu-id="79cd4-146">Список решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="79cd4-146">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="79cd4-147">Коллекция [акцессревиевдеЦисион](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="79cd4-147">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="79cd4-148">Получение всех решений Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="79cd4-148">Retrieve all the decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listmydecisions.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/accessreview-listmydecisions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-listmydecisions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
