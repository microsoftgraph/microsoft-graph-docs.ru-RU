---
title: Получение accessReview
description: 'В Azure AD access дается обзор компонента, извлечение объекта accessReview.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: be946e07a7714dc744847d73ee49718237fac92e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926661"
---
# <a name="get-accessreview"></a><span data-ttu-id="5bcf8-103">Получение accessReview</span><span class="sxs-lookup"><span data-stu-id="5bcf8-103">Get accessReview</span></span>

> <span data-ttu-id="5bcf8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5bcf8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5bcf8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bcf8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5bcf8-106">В компоненте [дается обзор доступа](../resources/accessreviews-root.md) Azure AD извлечение объекта [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="5bcf8-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="5bcf8-107">Чтобы получить рецензентов проверки доступа, используйте [рецензентов accessReview список](accessreview-listreviewers.md) API.</span><span class="sxs-lookup"><span data-stu-id="5bcf8-107">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="5bcf8-108">Для получения решения проверки доступа, используйте API [решения accessReview списка](accessreview-listdecisions.md) или интерфейса API [Мои accessReview решения](accessreview-listmydecisions.md) .</span><span class="sxs-lookup"><span data-stu-id="5bcf8-108">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="5bcf8-109">Если это повторяющееся проверки доступа, используйте `instances` связь для получения коллекции [accessReview](../resources/accessreview.md) ранее, текущие и будущие экземпляры проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="5bcf8-109">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bcf8-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5bcf8-110">Permissions</span></span>
<span data-ttu-id="5bcf8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bcf8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bcf8-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5bcf8-113">Permission type</span></span>                        | <span data-ttu-id="5bcf8-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5bcf8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bcf8-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5bcf8-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="5bcf8-116">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="5bcf8-116"></span></span>  <span data-ttu-id="5bcf8-117">Также должен быть выполнен вход пользователя в роль каталог, который позволяет им читать проверки доступа или назначен в качестве проверяющего проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="5bcf8-117">The signed in user must also be in a directory role which permits them to read an access review, or assigned as a reviewer on the access review.</span></span> |
|<span data-ttu-id="5bcf8-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5bcf8-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bcf8-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bcf8-119">Not supported.</span></span> |
|<span data-ttu-id="5bcf8-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5bcf8-120">Application</span></span>                            | <span data-ttu-id="5bcf8-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bcf8-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5bcf8-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bcf8-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="5bcf8-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5bcf8-123">Request headers</span></span>
| <span data-ttu-id="5bcf8-124">Имя</span><span class="sxs-lookup"><span data-stu-id="5bcf8-124">Name</span></span>         | <span data-ttu-id="5bcf8-125">Тип</span><span class="sxs-lookup"><span data-stu-id="5bcf8-125">Type</span></span>        | <span data-ttu-id="5bcf8-126">Описание</span><span class="sxs-lookup"><span data-stu-id="5bcf8-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5bcf8-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bcf8-127">Authorization</span></span> | <span data-ttu-id="5bcf8-128">строка</span><span class="sxs-lookup"><span data-stu-id="5bcf8-128">string</span></span> | <span data-ttu-id="5bcf8-129">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="5bcf8-129">Bearer \{token\}.</span></span> <span data-ttu-id="5bcf8-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5bcf8-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bcf8-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5bcf8-131">Request body</span></span>
<span data-ttu-id="5bcf8-132">Нет текста запроса должен задаваться.</span><span class="sxs-lookup"><span data-stu-id="5bcf8-132">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="5bcf8-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="5bcf8-133">Response</span></span>
<span data-ttu-id="5bcf8-134">Успешно завершена, этот метод возвращает `200, OK` код ответа и объект [accessReview](../resources/accessreview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5bcf8-134">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bcf8-135">Пример</span><span class="sxs-lookup"><span data-stu-id="5bcf8-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5bcf8-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bcf8-136">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')
```

##### <a name="response"></a><span data-ttu-id="5bcf8-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bcf8-137">Response</span></span>
><span data-ttu-id="5bcf8-p106">**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5bcf8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
    "displayName": "review",
    "startDateTime": "2017-11-14T01:14:54.89Z",
    "endDateTime": "2017-12-14T01:14:54.89Z",
    "status": "InProgress",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "self",
    "description": "",
    "settings": {
        "reviewId": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval": true,
        "recurrenceSettings": {
            "recurrenceType": "onetime",
            "recurrenceEndType": "endBy",
            "durationInDays": 0,
            "recurrenceCount": 0
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="5bcf8-140">См. также</span><span class="sxs-lookup"><span data-stu-id="5bcf8-140">See also</span></span>

| <span data-ttu-id="5bcf8-141">Метод</span><span class="sxs-lookup"><span data-stu-id="5bcf8-141">Method</span></span>           | <span data-ttu-id="5bcf8-142">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5bcf8-142">Return Type</span></span>    |<span data-ttu-id="5bcf8-143">Описание</span><span class="sxs-lookup"><span data-stu-id="5bcf8-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5bcf8-144">Создание accessReview</span><span class="sxs-lookup"><span data-stu-id="5bcf8-144">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="5bcf8-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="5bcf8-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="5bcf8-146">Создание нового accessReview.</span><span class="sxs-lookup"><span data-stu-id="5bcf8-146">Create a new accessReview.</span></span> |
|[<span data-ttu-id="5bcf8-147">Список programControls</span><span class="sxs-lookup"><span data-stu-id="5bcf8-147">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="5bcf8-148">[programControl](../resources/programcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="5bcf8-148">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="5bcf8-149">Список programControls в клиент.</span><span class="sxs-lookup"><span data-stu-id="5bcf8-149">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="5bcf8-150">Список accessReview рецензентов</span><span class="sxs-lookup"><span data-stu-id="5bcf8-150">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="5bcf8-151">Коллекция [удостоверению пользователя](../resources/useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="5bcf8-151">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="5bcf8-152">Получите рецензентов accessReview.</span><span class="sxs-lookup"><span data-stu-id="5bcf8-152">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="5bcf8-153">Список accessReview решения</span><span class="sxs-lookup"><span data-stu-id="5bcf8-153">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="5bcf8-154">[accessReviewDecision](../resources/accessreviewdecision.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="5bcf8-154">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="5bcf8-155">Получите решения accessReview.</span><span class="sxs-lookup"><span data-stu-id="5bcf8-155">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="5bcf8-156">Мои accessReview решения</span><span class="sxs-lookup"><span data-stu-id="5bcf8-156">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="5bcf8-157">[accessReviewDecision](../resources/accessreviewdecision.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="5bcf8-157">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="5bcf8-158">В качестве читателя получите Мои решения accessReview.</span><span class="sxs-lookup"><span data-stu-id="5bcf8-158">As a reviewer, get my decisions of an accessReview.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
