---
title: Получение Акцессревиевсчедуледефинитион
description: Получение объекта Акцессревиевсчедуледефинитион.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a6c5619222eb8a96fbf54a8f796abdc2d2bb85ec
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000991"
---
# <a name="get-accessreviewscheduledefinition"></a><span data-ttu-id="10b2a-103">Получение Акцессревиевсчедуледефинитион</span><span class="sxs-lookup"><span data-stu-id="10b2a-103">Get accessReviewScheduleDefinition</span></span>

<span data-ttu-id="10b2a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10b2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10b2a-105">Получение объекта [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="10b2a-105">Retrieve an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object by ID.</span></span> <span data-ttu-id="10b2a-106">Возвращает все свойства серии проверки доступа "запланированный доступ", за исключением связанного Акцессревиевинстанцес.</span><span class="sxs-lookup"><span data-stu-id="10b2a-106">This returns all properties of the scheduled access review series except for the associated accessReviewInstances.</span></span> <span data-ttu-id="10b2a-107">У каждого Акцессревиевсчедуледефинитион есть по крайней мере один экземпляр.</span><span class="sxs-lookup"><span data-stu-id="10b2a-107">Each accessReviewScheduleDefinition has at least one instance.</span></span> <span data-ttu-id="10b2a-108">Экземпляр представляет проверку для определенного ресурса (например, членов определенной группы), в течение одного экземпляра (например, Март 2021) повторяющейся проверки.</span><span class="sxs-lookup"><span data-stu-id="10b2a-108">An instance represents a review for a specific resource (such as a particular group's members), during one occurrence (e.g., March 2021) of a recurring review.</span></span>

<span data-ttu-id="10b2a-109">Чтобы получить экземпляры серии проверки доступа, используйте [акцессревиевинстанце API List](accessreviewinstance-list.md) .</span><span class="sxs-lookup"><span data-stu-id="10b2a-109">To retrieve the instances of the access review series, use the [list accessReviewInstance](accessreviewinstance-list.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="10b2a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10b2a-110">Permissions</span></span>
<span data-ttu-id="10b2a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10b2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10b2a-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10b2a-113">Permission type</span></span>                        | <span data-ttu-id="10b2a-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10b2a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="10b2a-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10b2a-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="10b2a-116">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="10b2a-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="10b2a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10b2a-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10b2a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10b2a-118">Not supported.</span></span>|
|<span data-ttu-id="10b2a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10b2a-119">Application</span></span>                            | <span data-ttu-id="10b2a-120">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="10b2a-120">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="10b2a-121">Чтобы вызвать этот API, вошедшего в систему пользователь должен также находиться в роли каталога, который позволяет им читать проверку доступа, или пользователь может быть назначен в качестве проверяющего при проверке доступа.</span><span class="sxs-lookup"><span data-stu-id="10b2a-121">To call this API, the signed-in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="10b2a-122">Более подробную информацию можно узнать в статье требования к ролям и разрешениям для [рецензирования Access](../resources/accessreviewsv2-root.md).</span><span class="sxs-lookup"><span data-stu-id="10b2a-122">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="10b2a-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10b2a-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="10b2a-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10b2a-124">Request headers</span></span>
<span data-ttu-id="10b2a-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="10b2a-125">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="10b2a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10b2a-126">Request body</span></span>
<span data-ttu-id="10b2a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10b2a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10b2a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="10b2a-128">Response</span></span>
<span data-ttu-id="10b2a-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [акцессревиевсчедуледефинитион](../resources/accessreviewscheduledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10b2a-129">If successful, this method returns a `200 OK` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10b2a-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="10b2a-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="10b2a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="10b2a-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReviewScheduleDefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
---

### <a name="response"></a><span data-ttu-id="10b2a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="10b2a-132">Response</span></span>
><span data-ttu-id="10b2a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10b2a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
        "userPrincipalName": "admin@microsoft.com"
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

## <a name="see-also"></a><span data-ttu-id="10b2a-135">См. также</span><span class="sxs-lookup"><span data-stu-id="10b2a-135">See also</span></span>

- [<span data-ttu-id="10b2a-136">Создание Акцессревиевсчедуледефинитион</span><span class="sxs-lookup"><span data-stu-id="10b2a-136">Create accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-create.md)
- [<span data-ttu-id="10b2a-137">Список Акцессревиевсчедуледефинитион</span><span class="sxs-lookup"><span data-stu-id="10b2a-137">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="10b2a-138">Список Акцессревиевинстанце</span><span class="sxs-lookup"><span data-stu-id="10b2a-138">List accessReviewInstance</span></span>](accessreviewinstance-list.md)


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
