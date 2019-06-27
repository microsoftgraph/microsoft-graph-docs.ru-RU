---
title: Получение Акцессревиев
description: 'В функции рецензирования Access Azure AD извлеките объект Акцессревиев.  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 34236a1c8d80aa48976a4fcb65c503b5b7ab7a2c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258970"
---
# <a name="get-accessreview"></a><span data-ttu-id="44993-103">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="44993-103">Get accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44993-104">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD извлеките объект [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="44993-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="44993-105">Чтобы получить рецензентов проверки доступа, используйте API [List акцессревиев проверяющих](accessreview-listreviewers.md) .</span><span class="sxs-lookup"><span data-stu-id="44993-105">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="44993-106">Чтобы получить решение об анализе доступа, используйте API [List акцессревиев решений](accessreview-listdecisions.md) или перечислите мои API [решений акцессревиев](accessreview-listmydecisions.md) .</span><span class="sxs-lookup"><span data-stu-id="44993-106">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="44993-107">Если это проверка доступа повторяется, используйте `instances` связь для получения коллекции [акцессревиев](../resources/accessreview.md) из прошлых, текущих и будущих экземпляров проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="44993-107">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="44993-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44993-108">Permissions</span></span>
<span data-ttu-id="44993-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44993-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44993-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44993-111">Permission type</span></span>                        | <span data-ttu-id="44993-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44993-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="44993-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44993-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="44993-114">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="44993-114">AccessReview.Read.All</span></span>  |
|<span data-ttu-id="44993-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44993-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44993-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44993-116">Not supported.</span></span> |
|<span data-ttu-id="44993-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44993-117">Application</span></span>                            | <span data-ttu-id="44993-118">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="44993-118">AccessReview.Read.All</span></span>  |

<span data-ttu-id="44993-119">Чтобы вызвать этот API, пользователь, вошедшего в систему, должен быть включен в роль каталога, которая разрешает им читать проверку доступа, или пользователь может быть назначен в качестве проверяющего при проверке доступа.</span><span class="sxs-lookup"><span data-stu-id="44993-119">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="44993-120">Более подробную информацию можно узнать в статье требования к ролям и разрешениям для [рецензирования Access](../resources/accessreviews-root.md).</span><span class="sxs-lookup"><span data-stu-id="44993-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="44993-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44993-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="44993-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44993-122">Request headers</span></span>
| <span data-ttu-id="44993-123">Имя</span><span class="sxs-lookup"><span data-stu-id="44993-123">Name</span></span>         | <span data-ttu-id="44993-124">Тип</span><span class="sxs-lookup"><span data-stu-id="44993-124">Type</span></span>        | <span data-ttu-id="44993-125">Описание</span><span class="sxs-lookup"><span data-stu-id="44993-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="44993-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="44993-126">Authorization</span></span> | <span data-ttu-id="44993-127">string</span><span class="sxs-lookup"><span data-stu-id="44993-127">string</span></span> | <span data-ttu-id="44993-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44993-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44993-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="44993-130">Request body</span></span>
<span data-ttu-id="44993-131">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="44993-131">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="44993-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="44993-132">Response</span></span>
<span data-ttu-id="44993-133">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и объект [акцессревиев](../resources/accessreview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44993-133">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44993-134">Пример</span><span class="sxs-lookup"><span data-stu-id="44993-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44993-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="44993-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
```

##### <a name="response"></a><span data-ttu-id="44993-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="44993-136">Response</span></span>
><span data-ttu-id="44993-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44993-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="44993-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="44993-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="44993-140">C#</span><span class="sxs-lookup"><span data-stu-id="44993-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="44993-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="44993-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_accessReview-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="44993-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="44993-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_accessReview-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="44993-143">См. также</span><span class="sxs-lookup"><span data-stu-id="44993-143">See also</span></span>

| <span data-ttu-id="44993-144">Метод</span><span class="sxs-lookup"><span data-stu-id="44993-144">Method</span></span>           | <span data-ttu-id="44993-145">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="44993-145">Return Type</span></span>    |<span data-ttu-id="44993-146">Описание</span><span class="sxs-lookup"><span data-stu-id="44993-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="44993-147">Создание Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="44993-147">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="44993-148">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="44993-148">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="44993-149">Создание нового Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="44993-149">Create a new accessReview.</span></span> |
|[<span data-ttu-id="44993-150">Список Програмконтролс</span><span class="sxs-lookup"><span data-stu-id="44993-150">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="44993-151">Коллекция [програмконтрол](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="44993-151">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="44993-152">Список Програмконтролс в клиенте.</span><span class="sxs-lookup"><span data-stu-id="44993-152">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="44993-153">Список рецензентов Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="44993-153">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="44993-154">Коллекция [userIdentity](../resources/useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="44993-154">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="44993-155">Получение рецензентов объекта Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="44993-155">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="44993-156">Список решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="44993-156">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="44993-157">Коллекция [акцессревиевдеЦисион](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="44993-157">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="44993-158">Получение решений для Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="44993-158">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="44993-159">Список моих решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="44993-159">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="44993-160">Коллекция [акцессревиевдеЦисион](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="44993-160">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="44993-161">В качестве проверяющего получите мое решение Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="44993-161">As a reviewer, get my decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/accessreview-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
