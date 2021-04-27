---
title: Получить accessReviewScheduleDefinition
description: Извлечение объекта accessReviewScheduleDefinition.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 572369a17288a584550c4d4f5bdda9cbf11e90e4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048360"
---
# <a name="get-accessreviewscheduledefinition"></a><span data-ttu-id="675eb-103">Получить accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="675eb-103">Get accessReviewScheduleDefinition</span></span>

<span data-ttu-id="675eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="675eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="675eb-105">Извлечение [объекта accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) по ID.</span><span class="sxs-lookup"><span data-stu-id="675eb-105">Retrieve an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object by ID.</span></span> <span data-ttu-id="675eb-106">Это возвращает все свойства серии запланированных обзоров доступа, за исключением связанных accessReviewInstances.</span><span class="sxs-lookup"><span data-stu-id="675eb-106">This returns all properties of the scheduled access review series except for the associated accessReviewInstances.</span></span> <span data-ttu-id="675eb-107">Каждый accessReviewScheduleDefinition имеет по крайней мере один экземпляр.</span><span class="sxs-lookup"><span data-stu-id="675eb-107">Each accessReviewScheduleDefinition has at least one instance.</span></span> <span data-ttu-id="675eb-108">Экземпляр представляет обзор для определенного ресурса (например, членов определенной группы) во время одного случая (например, в марте 2021 г.) повторяющегося обзора.</span><span class="sxs-lookup"><span data-stu-id="675eb-108">An instance represents a review for a specific resource (such as a particular group's members), during one occurrence (e.g., March 2021) of a recurring review.</span></span>

<span data-ttu-id="675eb-109">Чтобы получить экземпляры серии обзоров доступа, используйте [API accessReviewInstance.](accessreviewinstance-list.md)</span><span class="sxs-lookup"><span data-stu-id="675eb-109">To retrieve the instances of the access review series, use the [list accessReviewInstance](accessreviewinstance-list.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="675eb-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="675eb-110">Permissions</span></span>
<span data-ttu-id="675eb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="675eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="675eb-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="675eb-113">Permission type</span></span>                        | <span data-ttu-id="675eb-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="675eb-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="675eb-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="675eb-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="675eb-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="675eb-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="675eb-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="675eb-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="675eb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="675eb-118">Not supported.</span></span>|
|<span data-ttu-id="675eb-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="675eb-119">Application</span></span>                            | <span data-ttu-id="675eb-120">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="675eb-120">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="675eb-121">Чтобы вызвать этот API, входив в каталог, пользователь должен также быть в роли каталога, которая позволяет ему читать обзор доступа, или пользователь может быть назначен в качестве рецензента в обзоре доступа.</span><span class="sxs-lookup"><span data-stu-id="675eb-121">To call this API, the signed-in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="675eb-122">Дополнительные сведения см. в дополнительных сведениях о требованиях к роли и разрешению для [отзывов о доступе.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="675eb-122">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="675eb-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="675eb-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="675eb-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="675eb-124">Request headers</span></span>
<span data-ttu-id="675eb-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="675eb-125">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="675eb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="675eb-126">Request body</span></span>
<span data-ttu-id="675eb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="675eb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="675eb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="675eb-128">Response</span></span>
<span data-ttu-id="675eb-129">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="675eb-129">If successful, this method returns a `200 OK` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="675eb-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="675eb-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="675eb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="675eb-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="675eb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="675eb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviewScheduleDefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
# <a name="c"></a>[<span data-ttu-id="675eb-133">C#</span><span class="sxs-lookup"><span data-stu-id="675eb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="675eb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="675eb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="675eb-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="675eb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="675eb-136">Java</span><span class="sxs-lookup"><span data-stu-id="675eb-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="675eb-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="675eb-137">Response</span></span>
><span data-ttu-id="675eb-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="675eb-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "60860cdd-fb4d-4054-91ba-f7544443baa6",
    "displayName": "Test world",
    "createdDateTime": "2020-09-14T20:03:36.7391027Z",
    "lastModifiedDateTime": "2020-09-14T20:04:28Z",
    "status": "InProgress",
    "descriptionForAdmins": "",
    "descriptionForReviewers": "",
    "createdBy": {
        "id": "957f1027-c0ee-460d-4444-b8828e59e0fe",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@contoso.com"
    },
    "scope": {
        "query": "/groups/b7a059cb-038a-4802-8fc9-b944440cf11f/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups/b7a059cb-038a-4802-8fc9-b9d14444f11f",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "None",
        "instanceDurationInDays": 0,
        "autoApplyDecisionsEnabled": false,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": {
                "type": "weekly",
                "interval": 1,
                "month": 0,
                "dayOfMonth": 0,
                "daysOfWeek": [],
                "firstDayOfWeek": "sunday",
                "index": "first"
            },
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2020-09-15",
                "endDate": "9999-12-31"
            }
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="675eb-139">См. также</span><span class="sxs-lookup"><span data-stu-id="675eb-139">See also</span></span>

- [<span data-ttu-id="675eb-140">Создание accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="675eb-140">Create accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-create.md)
- [<span data-ttu-id="675eb-141">Список accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="675eb-141">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="675eb-142">List accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="675eb-142">List accessReviewInstance</span></span>](accessreviewinstance-list.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
