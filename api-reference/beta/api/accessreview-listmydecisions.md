---
title: Мои accessReview решения
description: В компоненте обзоры доступа Azure AD извлечение решения объект accessReview для вызывающего пользователя в виде редактор.
localization_priority: Normal
ms.openlocfilehash: 27ae3129810b6019ecf47e23f1e4cc48362df6fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819014"
---
# <a name="list-my-accessreview-decisions"></a><span data-ttu-id="77a73-103">Мои accessReview решения</span><span class="sxs-lookup"><span data-stu-id="77a73-103">List my accessReview decisions</span></span>

> <span data-ttu-id="77a73-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="77a73-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77a73-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77a73-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77a73-106">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD извлечение решения объект [accessReview](../resources/accessreview.md) для вызывающего пользователя в виде редактор.</span><span class="sxs-lookup"><span data-stu-id="77a73-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object for the calling user as reviewer.</span></span>
## <a name="permissions"></a><span data-ttu-id="77a73-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77a73-107">Permissions</span></span>
<span data-ttu-id="77a73-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77a73-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77a73-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77a73-110">Permission type</span></span>                        | <span data-ttu-id="77a73-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77a73-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="77a73-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77a73-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="77a73-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="77a73-113"></span></span>  <span data-ttu-id="77a73-114">Выполнен вход пользователей необходимо также могут читать этот анализ конкретного клиента.</span><span class="sxs-lookup"><span data-stu-id="77a73-114">The signed in user must also be permitted to read this particular access review.</span></span> |
|<span data-ttu-id="77a73-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77a73-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77a73-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77a73-116">Not supported.</span></span> |
|<span data-ttu-id="77a73-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77a73-117">Application</span></span>                            | <span data-ttu-id="77a73-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77a73-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77a73-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77a73-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a><span data-ttu-id="77a73-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77a73-120">Request headers</span></span>
| <span data-ttu-id="77a73-121">Имя</span><span class="sxs-lookup"><span data-stu-id="77a73-121">Name</span></span>         | <span data-ttu-id="77a73-122">Тип</span><span class="sxs-lookup"><span data-stu-id="77a73-122">Type</span></span>        | <span data-ttu-id="77a73-123">Описание</span><span class="sxs-lookup"><span data-stu-id="77a73-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="77a73-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="77a73-124">Authorization</span></span> | <span data-ttu-id="77a73-125">string</span><span class="sxs-lookup"><span data-stu-id="77a73-125">string</span></span> | <span data-ttu-id="77a73-126">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="77a73-126">Bearer \{token\}.</span></span> <span data-ttu-id="77a73-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77a73-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77a73-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="77a73-128">Request body</span></span>
<span data-ttu-id="77a73-129">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="77a73-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="77a73-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="77a73-130">Response</span></span>
<span data-ttu-id="77a73-131">Успешно завершена, этот метод возвращает `200, OK` код ответа и массив объектов [accessReviewDecision](../resources/accessreviewdecision.md) в теле ответа, для которого вызывающего пользователя — это назначенный редактор.</span><span class="sxs-lookup"><span data-stu-id="77a73-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body, for which the calling user is an assigned reviewer.</span></span>

## <a name="example"></a><span data-ttu-id="77a73-132">Пример</span><span class="sxs-lookup"><span data-stu-id="77a73-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77a73-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="77a73-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/myDecisions
```

##### <a name="response"></a><span data-ttu-id="77a73-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="77a73-134">Response</span></span>
><span data-ttu-id="77a73-p105">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77a73-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="77a73-137">См. также</span><span class="sxs-lookup"><span data-stu-id="77a73-137">See also</span></span>

| <span data-ttu-id="77a73-138">Метод</span><span class="sxs-lookup"><span data-stu-id="77a73-138">Method</span></span>           | <span data-ttu-id="77a73-139">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="77a73-139">Return Type</span></span>    |<span data-ttu-id="77a73-140">Описание</span><span class="sxs-lookup"><span data-stu-id="77a73-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="77a73-141">Получение accessReview</span><span class="sxs-lookup"><span data-stu-id="77a73-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="77a73-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="77a73-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="77a73-143">Получите обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="77a73-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="77a73-144">Список accessReview решения</span><span class="sxs-lookup"><span data-stu-id="77a73-144">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="77a73-145">[accessReviewDecision](../resources/accessreviewdecision.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="77a73-145">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="77a73-146">Получите все решения accessReview.</span><span class="sxs-lookup"><span data-stu-id="77a73-146">Retrieve all the decisions of an accessReview.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
