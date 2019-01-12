---
title: Список accessReview решения
description: В Azure AD access дается обзор компонента, извлечение решения accessReview объекта.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4f89fdbce1c87ce9ef8a6ba8c5b7f9b7be410617
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927011"
---
# <a name="list-accessreview-decisions"></a><span data-ttu-id="b1136-103">Список accessReview решения</span><span class="sxs-lookup"><span data-stu-id="b1136-103">List accessReview decisions</span></span>

> <span data-ttu-id="b1136-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b1136-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1136-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1136-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1136-106">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD извлечения решения [accessReview](../resources/accessreview.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="b1136-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the decisions of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="b1136-107">Обратите внимание, что повторяющиеся проверки доступа, не будут иметь `decisions` отношения.</span><span class="sxs-lookup"><span data-stu-id="b1136-107">Note that a recurring access review will not have a `decisions` relationship.</span></span>  <span data-ttu-id="b1136-108">Вместо этого необходимо перейти вызывающего `instance` отношения, чтобы найти `accessReview` объект для текущей или последние экземпляр проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="b1136-108">Instead, the caller must navigate the `instance` relationship to find an `accessReview` object for a current or past instance of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1136-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1136-109">Permissions</span></span>
<span data-ttu-id="b1136-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1136-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1136-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1136-112">Permission type</span></span>                        | <span data-ttu-id="b1136-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1136-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1136-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1136-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="b1136-115">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="b1136-115"></span></span>  <span data-ttu-id="b1136-116">Также должен быть выполнен вход пользователя в роль каталог, который позволяет им читать проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="b1136-116">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="b1136-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1136-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1136-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1136-118">Not supported.</span></span> |
|<span data-ttu-id="b1136-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1136-119">Application</span></span>                            | <span data-ttu-id="b1136-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1136-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1136-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1136-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a><span data-ttu-id="b1136-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1136-122">Request headers</span></span>
| <span data-ttu-id="b1136-123">Имя</span><span class="sxs-lookup"><span data-stu-id="b1136-123">Name</span></span>         | <span data-ttu-id="b1136-124">Тип</span><span class="sxs-lookup"><span data-stu-id="b1136-124">Type</span></span>        | <span data-ttu-id="b1136-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b1136-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b1136-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1136-126">Authorization</span></span> | <span data-ttu-id="b1136-127">string</span><span class="sxs-lookup"><span data-stu-id="b1136-127">string</span></span> | <span data-ttu-id="b1136-128">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="b1136-128">Bearer \{token\}.</span></span> <span data-ttu-id="b1136-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1136-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1136-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b1136-130">Request body</span></span>
<span data-ttu-id="b1136-131">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="b1136-131">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="b1136-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1136-132">Response</span></span>
<span data-ttu-id="b1136-133">Успешно завершена, этот метод возвращает `200, OK` код ответа и массив объектов [accessReviewDecision](../resources/accessreviewdecision.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b1136-133">If successful, this method returns a `200, OK` response code and an array of [accessReviewDecision](../resources/accessreviewdecision.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1136-134">Пример</span><span class="sxs-lookup"><span data-stu-id="b1136-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1136-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1136-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/decisions
```

##### <a name="response"></a><span data-ttu-id="b1136-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1136-136">Response</span></span>
><span data-ttu-id="b1136-p106">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1136-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="b1136-139">См. также</span><span class="sxs-lookup"><span data-stu-id="b1136-139">See also</span></span>

| <span data-ttu-id="b1136-140">Метод</span><span class="sxs-lookup"><span data-stu-id="b1136-140">Method</span></span>           | <span data-ttu-id="b1136-141">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b1136-141">Return Type</span></span>    |<span data-ttu-id="b1136-142">Описание</span><span class="sxs-lookup"><span data-stu-id="b1136-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b1136-143">Получение accessReview</span><span class="sxs-lookup"><span data-stu-id="b1136-143">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="b1136-144">accessReview</span><span class="sxs-lookup"><span data-stu-id="b1136-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="b1136-145">Получите обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="b1136-145">Retrieve an access review.</span></span> |
|[<span data-ttu-id="b1136-146">Мои accessReview решения</span><span class="sxs-lookup"><span data-stu-id="b1136-146">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="b1136-147">[accessReviewDecision](../resources/accessreviewdecision.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b1136-147">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="b1136-148">В качестве читателя получите Мои решения accessReview.</span><span class="sxs-lookup"><span data-stu-id="b1136-148">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="b1136-149">Отправлять напоминание accessReview</span><span class="sxs-lookup"><span data-stu-id="b1136-149">Send accessReview reminder</span></span>](accessreview-sendreminder.md) |       <span data-ttu-id="b1136-150">Нет.</span><span class="sxs-lookup"><span data-stu-id="b1136-150">None.</span></span>   |   <span data-ttu-id="b1136-151">Отправьте напоминание, чтобы проверяющие accessReview.</span><span class="sxs-lookup"><span data-stu-id="b1136-151">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="b1136-152">Остановка accessReview</span><span class="sxs-lookup"><span data-stu-id="b1136-152">Stop accessReview</span></span>](accessreview-stop.md) |        <span data-ttu-id="b1136-153">Нет.</span><span class="sxs-lookup"><span data-stu-id="b1136-153">None.</span></span>   |   <span data-ttu-id="b1136-154">Остановите accessReview.</span><span class="sxs-lookup"><span data-stu-id="b1136-154">Stop an accessReview.</span></span> |
|[<span data-ttu-id="b1136-155">Сброс accessReview решения</span><span class="sxs-lookup"><span data-stu-id="b1136-155">Reset accessReview decisions</span></span>](accessreview-reset.md) |        <span data-ttu-id="b1136-156">Нет.</span><span class="sxs-lookup"><span data-stu-id="b1136-156">None.</span></span>   |   <span data-ttu-id="b1136-157">Сброс решения, принимаемые при accessReview в хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="b1136-157">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="b1136-158">Применение accessReview решения</span><span class="sxs-lookup"><span data-stu-id="b1136-158">Apply accessReview decisions</span></span>](accessreview-apply.md) |        <span data-ttu-id="b1136-159">Нет.</span><span class="sxs-lookup"><span data-stu-id="b1136-159">None.</span></span>   |   <span data-ttu-id="b1136-160">Применение решения из завершенных accessReview.</span><span class="sxs-lookup"><span data-stu-id="b1136-160">Apply the decisions from a completed accessReview.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
