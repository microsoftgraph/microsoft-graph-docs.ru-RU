---
title: Список accessReview решения
description: В Azure AD access дается обзор компонента, извлечение решения accessReview объекта.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: eeaa1374bbd44cfe9556e488d25e0fc2c7594cde
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521798"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="1cb54-103">Список accessReview решения</span><span class="sxs-lookup"><span data-stu-id="1cb54-103">List accessReview decisions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cb54-104">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD извлечения решения [accessReview](../resources/accessreview.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="1cb54-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="1cb54-105">Обратите внимание, что повторяющиеся проверки доступа, не будут иметь `decisions` отношения.</span><span class="sxs-lookup"><span data-stu-id="1cb54-105">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="1cb54-106">Вместо этого необходимо перейти вызывающего `instance` отношения, чтобы найти `accessReview` объект для текущей или последние экземпляр проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="1cb54-106">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cb54-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1cb54-107">Permissions</span></span>
<span data-ttu-id="1cb54-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cb54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cb54-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cb54-110">Permission type</span></span>                        | <span data-ttu-id="1cb54-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cb54-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cb54-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cb54-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1cb54-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="1cb54-113"></span></span>  <span data-ttu-id="1cb54-114">Также должен быть выполнен вход пользователя в роль каталог, который позволяет им читать проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="1cb54-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="1cb54-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cb54-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cb54-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cb54-116">Not supported.</span></span> |
|<span data-ttu-id="1cb54-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1cb54-117">Application</span></span>                            | <span data-ttu-id="1cb54-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cb54-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1cb54-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cb54-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="1cb54-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1cb54-120">Request headers</span></span>
| <span data-ttu-id="1cb54-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1cb54-121">Name</span></span>         | <span data-ttu-id="1cb54-122">Тип</span><span class="sxs-lookup"><span data-stu-id="1cb54-122">Type</span></span>        | <span data-ttu-id="1cb54-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1cb54-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1cb54-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cb54-124">Authorization</span></span> | <span data-ttu-id="1cb54-125">string</span><span class="sxs-lookup"><span data-stu-id="1cb54-125">string</span></span> | <span data-ttu-id="1cb54-126">Маркер носителя</span><span class="sxs-lookup"><span data-stu-id="1cb54-126">Bearer \{token\}.</span></span> <span data-ttu-id="1cb54-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1cb54-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cb54-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1cb54-128">Request body</span></span>
<span data-ttu-id="1cb54-129">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="1cb54-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="1cb54-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cb54-130">Response</span></span>
<span data-ttu-id="1cb54-131">Успешно завершена, этот метод возвращает `200, OK` код ответа и массив объектов [accessReviewDecision](../resources/accessreviewdecision.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1cb54-131">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cb54-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1cb54-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1cb54-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cb54-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/decisions
```

##### <a name="response"></a><span data-ttu-id="1cb54-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cb54-134">Response</span></span>
><span data-ttu-id="1cb54-p105">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1cb54-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="1cb54-137">См. также</span><span class="sxs-lookup"><span data-stu-id="1cb54-137">See also</span></span>

| <span data-ttu-id="1cb54-138">Метод</span><span class="sxs-lookup"><span data-stu-id="1cb54-138">Method</span></span>           | <span data-ttu-id="1cb54-139">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1cb54-139">Return Type</span></span>    |<span data-ttu-id="1cb54-140">Описание</span><span class="sxs-lookup"><span data-stu-id="1cb54-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1cb54-141">Получение accessReview</span><span class="sxs-lookup"><span data-stu-id="1cb54-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="1cb54-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="1cb54-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="1cb54-143">Получите обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="1cb54-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="1cb54-144">Мои accessReview решения</span><span class="sxs-lookup"><span data-stu-id="1cb54-144">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="1cb54-145">[accessReviewDecision](../resources/accessreviewdecision.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="1cb54-145">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="1cb54-146">В качестве читателя получите Мои решения accessReview.</span><span class="sxs-lookup"><span data-stu-id="1cb54-146">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="1cb54-147">Отправлять напоминание accessReview</span><span class="sxs-lookup"><span data-stu-id="1cb54-147">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="1cb54-148">Нет.</span><span class="sxs-lookup"><span data-stu-id="1cb54-148">None.</span></span>   |   <span data-ttu-id="1cb54-149">Отправьте напоминание, чтобы проверяющие accessReview.</span><span class="sxs-lookup"><span data-stu-id="1cb54-149">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="1cb54-150">Остановка accessReview</span><span class="sxs-lookup"><span data-stu-id="1cb54-150">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="1cb54-151">Нет.</span><span class="sxs-lookup"><span data-stu-id="1cb54-151">None.</span></span>   |   <span data-ttu-id="1cb54-152">Остановите accessReview.</span><span class="sxs-lookup"><span data-stu-id="1cb54-152">Stop an accessReview.</span></span> |
|[<span data-ttu-id="1cb54-153">Сброс accessReview решения</span><span class="sxs-lookup"><span data-stu-id="1cb54-153">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="1cb54-154">Нет.</span><span class="sxs-lookup"><span data-stu-id="1cb54-154">None.</span></span>   |   <span data-ttu-id="1cb54-155">Сброс решения, принимаемые при accessReview в хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="1cb54-155">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="1cb54-156">Применение accessReview решения</span><span class="sxs-lookup"><span data-stu-id="1cb54-156">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="1cb54-157">Нет.</span><span class="sxs-lookup"><span data-stu-id="1cb54-157">None.</span></span>   |   <span data-ttu-id="1cb54-158">Применение решения из завершенных accessReview.</span><span class="sxs-lookup"><span data-stu-id="1cb54-158">Apply the decisions from a completed accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listdecisions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
