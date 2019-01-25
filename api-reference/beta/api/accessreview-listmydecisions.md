---
title: Мои accessReview решения
description: В компоненте обзоры доступа Azure AD извлечение решения объект accessReview для вызывающего пользователя в виде редактор.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e19e3b0581c995f1b0ef52369d3a3e7545696d1c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525327"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="98f24-103">Мои accessReview решения</span><span class="sxs-lookup"><span data-stu-id="98f24-103">List my accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98f24-104">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD извлечение решения объект [accessReview](../resources/accessreview.md) для вызывающего пользователя в виде редактор.</span><span class="sxs-lookup"><span data-stu-id="98f24-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="98f24-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98f24-105">Permissions</span></span>
<span data-ttu-id="98f24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98f24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98f24-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98f24-108">Permission type</span></span>                        | <span data-ttu-id="98f24-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98f24-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="98f24-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98f24-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="98f24-111">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="98f24-111"></span></span>  <span data-ttu-id="98f24-112">Выполнен вход пользователей необходимо также могут читать этот анализ конкретного клиента.</span><span class="sxs-lookup"><span data-stu-id="98f24-112">The signed in user must also be permitted to read this particular access review.</span></span> |
|<span data-ttu-id="98f24-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98f24-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98f24-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98f24-114">Not supported.</span></span> |
|<span data-ttu-id="98f24-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98f24-115">Application</span></span>                            | <span data-ttu-id="98f24-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98f24-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98f24-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98f24-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="98f24-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98f24-118">Request headers</span></span>
| <span data-ttu-id="98f24-119">Имя</span><span class="sxs-lookup"><span data-stu-id="98f24-119">Name</span></span>         | <span data-ttu-id="98f24-120">Тип</span><span class="sxs-lookup"><span data-stu-id="98f24-120">Type</span></span>        | <span data-ttu-id="98f24-121">Описание</span><span class="sxs-lookup"><span data-stu-id="98f24-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="98f24-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="98f24-122">Authorization</span></span> | <span data-ttu-id="98f24-123">string</span><span class="sxs-lookup"><span data-stu-id="98f24-123">string</span></span> | <span data-ttu-id="98f24-124">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="98f24-124">Bearer \{token\}.</span></span> <span data-ttu-id="98f24-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98f24-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98f24-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98f24-126">Request body</span></span>
<span data-ttu-id="98f24-127">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="98f24-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="98f24-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="98f24-128">Response</span></span>
<span data-ttu-id="98f24-129">Успешно завершена, этот метод возвращает `200, OK` код ответа и массив объектов [accessReviewDecision](../resources/accessreviewdecision.md) в теле ответа, для которого вызывающего пользователя — это назначенный редактор.</span><span class="sxs-lookup"><span data-stu-id="98f24-129">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="98f24-130">Пример</span><span class="sxs-lookup"><span data-stu-id="98f24-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98f24-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="98f24-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/myDecisions
```

##### <a name="response"></a><span data-ttu-id="98f24-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="98f24-132">Response</span></span>
><span data-ttu-id="98f24-p104">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98f24-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="98f24-135">См. также</span><span class="sxs-lookup"><span data-stu-id="98f24-135">See also</span></span>

| <span data-ttu-id="98f24-136">Метод</span><span class="sxs-lookup"><span data-stu-id="98f24-136">Method</span></span>           | <span data-ttu-id="98f24-137">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="98f24-137">Return Type</span></span>    |<span data-ttu-id="98f24-138">Описание</span><span class="sxs-lookup"><span data-stu-id="98f24-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="98f24-139">Получение accessReview</span><span class="sxs-lookup"><span data-stu-id="98f24-139">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="98f24-140">accessReview</span><span class="sxs-lookup"><span data-stu-id="98f24-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="98f24-141">Получите обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="98f24-141">Retrieve an access review.</span></span> |
|[<span data-ttu-id="98f24-142">Список accessReview решения</span><span class="sxs-lookup"><span data-stu-id="98f24-142">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="98f24-143">[accessReviewDecision](../resources/accessreviewdecision.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="98f24-143">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="98f24-144">Получите все решения accessReview.</span><span class="sxs-lookup"><span data-stu-id="98f24-144">Retrieve all the decisions of an accessReview.</span></span>|


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
