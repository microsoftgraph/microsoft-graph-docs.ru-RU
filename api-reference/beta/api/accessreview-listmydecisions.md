---
title: Список моих решений Акцессревиев
description: В функции рецензирования Access в Azure AD извлекаются решения объекта Акцессревиев для вызывающего пользователя как проверяющего.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a89e611b12c9aac8006c030e264cfd3514845ea0
ms.sourcegitcommit: 4bdcb5cd3227ff009e10868f2936b3153372b87a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/25/2019
ms.locfileid: "33299635"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="376fd-103">Список моих решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="376fd-103">List my accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="376fd-104">В функции рецензирования [Access](../resources/accessreviews-root.md) в Azure AD извлекаются решения объекта [акцессревиев](../resources/accessreview.md) для вызывающего пользователя как проверяющего.</span><span class="sxs-lookup"><span data-stu-id="376fd-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="376fd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="376fd-105">Permissions</span></span>
<span data-ttu-id="376fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="376fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="376fd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="376fd-108">Permission type</span></span>                        | <span data-ttu-id="376fd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="376fd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="376fd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="376fd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="376fd-111">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="376fd-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>   |
|<span data-ttu-id="376fd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="376fd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="376fd-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="376fd-113">Not supported.</span></span> |
|<span data-ttu-id="376fd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="376fd-114">Application</span></span>                            | <span data-ttu-id="376fd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="376fd-115">Not supported.</span></span> |

<span data-ttu-id="376fd-116">Кроме того, вошедшего в систему пользователь должен иметь разрешение на чтение этой конкретной проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="376fd-116">The signed in user must also be permitted to read this particular access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="376fd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="376fd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="376fd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="376fd-118">Request headers</span></span>
| <span data-ttu-id="376fd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="376fd-119">Name</span></span>         | <span data-ttu-id="376fd-120">Тип</span><span class="sxs-lookup"><span data-stu-id="376fd-120">Type</span></span>        | <span data-ttu-id="376fd-121">Описание</span><span class="sxs-lookup"><span data-stu-id="376fd-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="376fd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="376fd-122">Authorization</span></span> | <span data-ttu-id="376fd-123">string</span><span class="sxs-lookup"><span data-stu-id="376fd-123">string</span></span> | <span data-ttu-id="376fd-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="376fd-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="376fd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="376fd-126">Request body</span></span>
<span data-ttu-id="376fd-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="376fd-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="376fd-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="376fd-128">Response</span></span>
<span data-ttu-id="376fd-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [акцессревиевдеЦисион](../resources/accessreviewdecision.md) в теле отклика, для которого вызывающий пользователь является назначенным рецензентом.</span><span class="sxs-lookup"><span data-stu-id="376fd-129">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="376fd-130">Пример</span><span class="sxs-lookup"><span data-stu-id="376fd-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="376fd-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="376fd-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```

##### <a name="response"></a><span data-ttu-id="376fd-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="376fd-132">Response</span></span>
><span data-ttu-id="376fd-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="376fd-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="376fd-135">См. также</span><span class="sxs-lookup"><span data-stu-id="376fd-135">See also</span></span>

| <span data-ttu-id="376fd-136">Метод</span><span class="sxs-lookup"><span data-stu-id="376fd-136">Method</span></span>           | <span data-ttu-id="376fd-137">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="376fd-137">Return Type</span></span>    |<span data-ttu-id="376fd-138">Описание</span><span class="sxs-lookup"><span data-stu-id="376fd-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="376fd-139">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="376fd-139">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="376fd-140">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="376fd-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="376fd-141">Получение проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="376fd-141">Retrieve an access review.</span></span> |
|[<span data-ttu-id="376fd-142">Список решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="376fd-142">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="376fd-143">Коллекция [акцессревиевдеЦисион](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="376fd-143">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="376fd-144">Получение всех решений Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="376fd-144">Retrieve all the decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
