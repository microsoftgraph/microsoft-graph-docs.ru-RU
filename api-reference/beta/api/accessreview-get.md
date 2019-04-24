---
title: Получение Акцессревиев
description: 'В функции рецензирования Access Azure AD извлеките объект Акцессревиев.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 26551f27fdf328865509cd02011f3ee2344f5e82
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458770"
---
# <a name="get-accessreview"></a><span data-ttu-id="1a9c8-103">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="1a9c8-103">Get accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a9c8-104">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD извлеките объект [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="1a9c8-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="1a9c8-105">Чтобы получить рецензентов проверки доступа, используйте API [List акцессревиев проверяющих](accessreview-listreviewers.md) .</span><span class="sxs-lookup"><span data-stu-id="1a9c8-105">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="1a9c8-106">Чтобы получить решение об анализе доступа, используйте API [List акцессревиев решений](accessreview-listdecisions.md) или перечислите мои API [решений акцессревиев](accessreview-listmydecisions.md) .</span><span class="sxs-lookup"><span data-stu-id="1a9c8-106">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="1a9c8-107">Если это проверка доступа повторяется, используйте `instances` связь для получения коллекции [акцессревиев](../resources/accessreview.md) из прошлых, текущих и будущих экземпляров проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="1a9c8-107">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a9c8-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a9c8-108">Permissions</span></span>
<span data-ttu-id="1a9c8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a9c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a9c8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a9c8-111">Permission type</span></span>                        | <span data-ttu-id="1a9c8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a9c8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a9c8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a9c8-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a9c8-114">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="1a9c8-114"></span></span>  <span data-ttu-id="1a9c8-115">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им читать и просматривать доступ, или назначить его в качестве проверяющего при проверке доступа.</span><span class="sxs-lookup"><span data-stu-id="1a9c8-115">The signed in user must also be in a directory role that permits them to read an access review, or assigned as a reviewer on the access review.</span></span> |
|<span data-ttu-id="1a9c8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a9c8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a9c8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a9c8-117">Not supported.</span></span> |
|<span data-ttu-id="1a9c8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a9c8-118">Application</span></span>                            | <span data-ttu-id="1a9c8-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a9c8-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a9c8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a9c8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="1a9c8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a9c8-121">Request headers</span></span>
| <span data-ttu-id="1a9c8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1a9c8-122">Name</span></span>         | <span data-ttu-id="1a9c8-123">Тип</span><span class="sxs-lookup"><span data-stu-id="1a9c8-123">Type</span></span>        | <span data-ttu-id="1a9c8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="1a9c8-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1a9c8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a9c8-125">Authorization</span></span> | <span data-ttu-id="1a9c8-126">string</span><span class="sxs-lookup"><span data-stu-id="1a9c8-126">string</span></span> | <span data-ttu-id="1a9c8-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a9c8-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a9c8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a9c8-129">Request body</span></span>
<span data-ttu-id="1a9c8-130">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="1a9c8-130">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="1a9c8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a9c8-131">Response</span></span>
<span data-ttu-id="1a9c8-132">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и объект [акцессревиев](../resources/accessreview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a9c8-132">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a9c8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1a9c8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a9c8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a9c8-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')
```

##### <a name="response"></a><span data-ttu-id="1a9c8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a9c8-135">Response</span></span>
><span data-ttu-id="1a9c8-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a9c8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"},
    "settings": {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval": true,
        "autoReviewEnabled": false,
        "activityDurationInDays": 30,
        "autoApplyReviewResultsEnabled": false,
        "accessRecommendationsEnabled": false,
        "recurrenceSettings": {
            "recurrenceType": "onetime",
            "recurrenceEndType": "endBy",
            "durationInDays": 0,
            "recurrenceCount": 0
        },
        "autoReviewSettings": {
            "notReviewedResult": "Deny"
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="1a9c8-138">См. также</span><span class="sxs-lookup"><span data-stu-id="1a9c8-138">See also</span></span>

| <span data-ttu-id="1a9c8-139">Метод</span><span class="sxs-lookup"><span data-stu-id="1a9c8-139">Method</span></span>           | <span data-ttu-id="1a9c8-140">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1a9c8-140">Return Type</span></span>    |<span data-ttu-id="1a9c8-141">Описание</span><span class="sxs-lookup"><span data-stu-id="1a9c8-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1a9c8-142">Создание Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="1a9c8-142">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="1a9c8-143">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="1a9c8-143">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="1a9c8-144">Создание нового Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="1a9c8-144">Create a new accessReview.</span></span> |
|[<span data-ttu-id="1a9c8-145">Список Програмконтролс</span><span class="sxs-lookup"><span data-stu-id="1a9c8-145">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="1a9c8-146">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="1a9c8-146">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="1a9c8-147">Список Програмконтролс в клиенте.</span><span class="sxs-lookup"><span data-stu-id="1a9c8-147">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="1a9c8-148">Список рецензентов Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="1a9c8-148">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="1a9c8-149">Коллекция [userIdentity](../resources/useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="1a9c8-149">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="1a9c8-150">Получение рецензентов объекта Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="1a9c8-150">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="1a9c8-151">Список решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="1a9c8-151">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="1a9c8-152">Коллекция [акцессревиевдеЦисион](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="1a9c8-152">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="1a9c8-153">Получение решений для Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="1a9c8-153">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="1a9c8-154">Список моих решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="1a9c8-154">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="1a9c8-155">Коллекция [акцессревиевдеЦисион](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="1a9c8-155">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="1a9c8-156">В качестве проверяющего получите мое решение Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="1a9c8-156">As a reviewer, get my decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
