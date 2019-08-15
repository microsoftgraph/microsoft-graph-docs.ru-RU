---
title: Получение Акцессревиев
description: 'В функции рецензирования Access Azure AD извлеките объект Акцессревиев.  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f8e628c2ba8835d42f00116e46b4dfa0527765fe
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408841"
---
# <a name="get-accessreview"></a><span data-ttu-id="2caa0-103">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="2caa0-103">Get accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2caa0-104">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD извлеките объект [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="2caa0-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="2caa0-105">Чтобы получить рецензентов проверки доступа, используйте API [List акцессревиев проверяющих](accessreview-listreviewers.md) .</span><span class="sxs-lookup"><span data-stu-id="2caa0-105">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="2caa0-106">Чтобы получить решение об анализе доступа, используйте API [List акцессревиев решений](accessreview-listdecisions.md) или перечислите мои API [решений акцессревиев](accessreview-listmydecisions.md) .</span><span class="sxs-lookup"><span data-stu-id="2caa0-106">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="2caa0-107">Если это проверка доступа повторяется, используйте `instances` связь для получения коллекции [акцессревиев](../resources/accessreview.md) из прошлых, текущих и будущих экземпляров проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="2caa0-107">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="2caa0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2caa0-108">Permissions</span></span>
<span data-ttu-id="2caa0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2caa0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2caa0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2caa0-111">Permission type</span></span>                        | <span data-ttu-id="2caa0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2caa0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2caa0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2caa0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="2caa0-114">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2caa0-114">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="2caa0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2caa0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2caa0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2caa0-116">Not supported.</span></span> |
|<span data-ttu-id="2caa0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2caa0-117">Application</span></span>                            | <span data-ttu-id="2caa0-118">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="2caa0-118">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |

<span data-ttu-id="2caa0-119">Чтобы вызвать этот API, пользователь, вошедшего в систему, должен быть включен в роль каталога, которая разрешает им читать проверку доступа, или пользователь может быть назначен в качестве проверяющего при проверке доступа.</span><span class="sxs-lookup"><span data-stu-id="2caa0-119">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="2caa0-120">Более подробную информацию можно узнать в статье требования к ролям и разрешениям для [рецензирования Access](../resources/accessreviews-root.md).</span><span class="sxs-lookup"><span data-stu-id="2caa0-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="2caa0-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2caa0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="2caa0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2caa0-122">Request headers</span></span>
| <span data-ttu-id="2caa0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="2caa0-123">Name</span></span>         | <span data-ttu-id="2caa0-124">Тип</span><span class="sxs-lookup"><span data-stu-id="2caa0-124">Type</span></span>        | <span data-ttu-id="2caa0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="2caa0-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2caa0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2caa0-126">Authorization</span></span> | <span data-ttu-id="2caa0-127">string</span><span class="sxs-lookup"><span data-stu-id="2caa0-127">string</span></span> | <span data-ttu-id="2caa0-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2caa0-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2caa0-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2caa0-130">Request body</span></span>
<span data-ttu-id="2caa0-131">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="2caa0-131">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="2caa0-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="2caa0-132">Response</span></span>
<span data-ttu-id="2caa0-133">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и объект [акцессревиев](../resources/accessreview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2caa0-133">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2caa0-134">Пример</span><span class="sxs-lookup"><span data-stu-id="2caa0-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2caa0-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="2caa0-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2caa0-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2caa0-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2caa0-137">C#</span><span class="sxs-lookup"><span data-stu-id="2caa0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2caa0-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2caa0-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2caa0-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2caa0-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2caa0-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2caa0-140">Response</span></span>
><span data-ttu-id="2caa0-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2caa0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="2caa0-143">См. также</span><span class="sxs-lookup"><span data-stu-id="2caa0-143">See also</span></span>

| <span data-ttu-id="2caa0-144">Метод</span><span class="sxs-lookup"><span data-stu-id="2caa0-144">Method</span></span>           | <span data-ttu-id="2caa0-145">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2caa0-145">Return Type</span></span>    |<span data-ttu-id="2caa0-146">Описание</span><span class="sxs-lookup"><span data-stu-id="2caa0-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2caa0-147">Создание Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="2caa0-147">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="2caa0-148">акцессревиев</span><span class="sxs-lookup"><span data-stu-id="2caa0-148">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="2caa0-149">Создание нового Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="2caa0-149">Create a new accessReview.</span></span> |
|[<span data-ttu-id="2caa0-150">Список Програмконтролс</span><span class="sxs-lookup"><span data-stu-id="2caa0-150">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="2caa0-151">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="2caa0-151">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="2caa0-152">Список Програмконтролс в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2caa0-152">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="2caa0-153">Список рецензентов Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="2caa0-153">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="2caa0-154">Коллекция [userIdentity](../resources/useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="2caa0-154">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="2caa0-155">Получение рецензентов объекта Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="2caa0-155">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="2caa0-156">Список решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="2caa0-156">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="2caa0-157">Коллекция [акцессревиевдеЦисион](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="2caa0-157">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="2caa0-158">Получение решений для Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="2caa0-158">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="2caa0-159">Список моих решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="2caa0-159">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="2caa0-160">Коллекция [акцессревиевдеЦисион](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="2caa0-160">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="2caa0-161">В качестве проверяющего получите мое решение Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="2caa0-161">As a reviewer, get my decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
