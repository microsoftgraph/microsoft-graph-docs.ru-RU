---
title: Список моих решений Акцессревиев
description: В функции рецензирования Access в Azure AD извлекаются решения объекта Акцессревиев для вызывающего пользователя как проверяющего.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e19e3b0581c995f1b0ef52369d3a3e7545696d1c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459453"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="36269-103">Список моих решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="36269-103">List my accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36269-104">В функции рецензирования [Access](../resources/accessreviews-root.md) в Azure AD извлекаются решения объекта [акцессревиев](../resources/accessreview.md) для вызывающего пользователя как проверяющего.</span><span class="sxs-lookup"><span data-stu-id="36269-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="36269-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36269-105">Permissions</span></span>
<span data-ttu-id="36269-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36269-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36269-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36269-108">Permission type</span></span>                        | <span data-ttu-id="36269-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36269-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="36269-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36269-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="36269-111">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="36269-111"></span></span>  <span data-ttu-id="36269-112">Кроме того, вошедшего в систему пользователь должен иметь разрешение на чтение этой конкретной проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="36269-112">The signed in user must also be permitted to read this particular access review.</span></span> |
|<span data-ttu-id="36269-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36269-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36269-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36269-114">Not supported.</span></span> |
|<span data-ttu-id="36269-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36269-115">Application</span></span>                            | <span data-ttu-id="36269-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36269-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36269-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36269-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="36269-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36269-118">Request headers</span></span>
| <span data-ttu-id="36269-119">Имя</span><span class="sxs-lookup"><span data-stu-id="36269-119">Name</span></span>         | <span data-ttu-id="36269-120">Тип</span><span class="sxs-lookup"><span data-stu-id="36269-120">Type</span></span>        | <span data-ttu-id="36269-121">Описание</span><span class="sxs-lookup"><span data-stu-id="36269-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="36269-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="36269-122">Authorization</span></span> | <span data-ttu-id="36269-123">string</span><span class="sxs-lookup"><span data-stu-id="36269-123">string</span></span> | <span data-ttu-id="36269-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36269-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36269-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36269-126">Request body</span></span>
<span data-ttu-id="36269-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="36269-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="36269-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="36269-128">Response</span></span>
<span data-ttu-id="36269-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [акцессревиевдеЦисион](../resources/accessreviewdecision.md) в теле отклика, для которого вызывающий пользователь является назначенным рецензентом.</span><span class="sxs-lookup"><span data-stu-id="36269-129">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="36269-130">Пример</span><span class="sxs-lookup"><span data-stu-id="36269-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36269-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="36269-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/myDecisions
```

##### <a name="response"></a><span data-ttu-id="36269-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="36269-132">Response</span></span>
><span data-ttu-id="36269-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36269-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="36269-135">См. также</span><span class="sxs-lookup"><span data-stu-id="36269-135">See also</span></span>

| <span data-ttu-id="36269-136">Метод</span><span class="sxs-lookup"><span data-stu-id="36269-136">Method</span></span>           | <span data-ttu-id="36269-137">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="36269-137">Return Type</span></span>    |<span data-ttu-id="36269-138">Описание</span><span class="sxs-lookup"><span data-stu-id="36269-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="36269-139">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="36269-139">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="36269-140">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="36269-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="36269-141">Получение проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="36269-141">Retrieve an access review.</span></span> |
|[<span data-ttu-id="36269-142">Список решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="36269-142">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="36269-143">Коллекция [акцессревиевдеЦисион](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="36269-143">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="36269-144">Получение всех решений Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="36269-144">Retrieve all the decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listmydecisions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
