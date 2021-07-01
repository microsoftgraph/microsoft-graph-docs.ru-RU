---
title: Получить accessReviewScheduleDefinition
description: Ознакомьтесь с свойствами и отношениями объекта accessReviewScheduleDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b7eb33d56831e330883d833c3117187b7cc12b1c
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208664"
---
# <a name="get-accessreviewscheduledefinition"></a><span data-ttu-id="e0b6e-103">Получить accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="e0b6e-103">Get accessReviewScheduleDefinition</span></span>
<span data-ttu-id="e0b6e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0b6e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e0b6e-105">Ознакомьтесь с свойствами и отношениями [объекта accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e0b6e-105">Read the properties and relationships of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="e0b6e-106">Чтобы получить экземпляры серии обзоров доступа, используйте [API accessReviewInstance.](accessreviewinstance-list.md)</span><span class="sxs-lookup"><span data-stu-id="e0b6e-106">To retrieve the instances of the access review series, use the [list accessReviewInstance](accessreviewinstance-list.md) API.</span></span>   

## <a name="permissions"></a><span data-ttu-id="e0b6e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e0b6e-107">Permissions</span></span>
<span data-ttu-id="e0b6e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0b6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0b6e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0b6e-110">Permission type</span></span>|<span data-ttu-id="e0b6e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0b6e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0b6e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0b6e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0b6e-113">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0b6e-113">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="e0b6e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0b6e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0b6e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0b6e-115">Not supported.</span></span>|
|<span data-ttu-id="e0b6e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="e0b6e-116">Application</span></span>|<span data-ttu-id="e0b6e-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0b6e-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="e0b6e-118">Чтобы вызвать этот API, входив в каталог, пользователь должен также быть в роли каталога, которая позволяет ему читать обзор доступа, или пользователь может быть назначен в качестве рецензента в обзоре доступа.</span><span class="sxs-lookup"><span data-stu-id="e0b6e-118">To call this API, the signed-in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="e0b6e-119">Дополнительные сведения см. в дополнительных сведениях о требованиях к роли и разрешению для [отзывов о доступе.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="e0b6e-119">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="e0b6e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0b6e-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0b6e-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e0b6e-121">Optional query parameters</span></span>
<span data-ttu-id="e0b6e-122">Этот метод поддерживает `$select` параметр запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="e0b6e-122">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="e0b6e-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e0b6e-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0b6e-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0b6e-124">Request headers</span></span>
|<span data-ttu-id="e0b6e-125">Имя</span><span class="sxs-lookup"><span data-stu-id="e0b6e-125">Name</span></span>|<span data-ttu-id="e0b6e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="e0b6e-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e0b6e-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0b6e-127">Authorization</span></span>|<span data-ttu-id="e0b6e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0b6e-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0b6e-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e0b6e-130">Request body</span></span>
<span data-ttu-id="e0b6e-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e0b6e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0b6e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0b6e-132">Response</span></span>

<span data-ttu-id="e0b6e-133">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e0b6e-133">If successful, this method returns a `200 OK` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e0b6e-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="e0b6e-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e0b6e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0b6e-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e0b6e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0b6e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewscheduledefinition"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/3856fd6f-36e2-4152-97c9-76070d19f730
```
# <a name="c"></a>[<span data-ttu-id="e0b6e-137">C#</span><span class="sxs-lookup"><span data-stu-id="e0b6e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0b6e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0b6e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0b6e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0b6e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e0b6e-140">Java</span><span class="sxs-lookup"><span data-stu-id="e0b6e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e0b6e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0b6e-141">Response</span></span>
><span data-ttu-id="e0b6e-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e0b6e-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "d6bf2f6c-2f6c-d6bf-6c2f-bfd66c2fbfd6",
    "displayName": "Review example",
    "status": "Applying",
    "scope": {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/v1.0/groups/4444d821-ca3b-45cc-98ee-54c00a04deef/transitiveMembers/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
    },
    "reviewers": [
        {
            "query": "/v1.0/users/5555556e-fce3-4e2d-b28e-4ac0c7d2fa10",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "fallbackReviewers": [],
    "instanceEnumerationScope": {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/v1.0/groups/4444d821-ca3b-45cc-98ee-54c00a04deef",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
    },
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": false,
        "defaultDecisionEnabled": true,
        "defaultDecision": "Deny",
        "instanceDurationInDays": 10,
        "autoApplyDecisionsEnabled": false,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": null,
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-04-28",
                "endDate": "2021-05-08"
            }
        },
        "applyActions": [
            {
                "@odata.type": "#microsoft.graph.disableAndDeleteUserApplyAction"
            }
        ]
    }
  }
}
```

## <a name="see-also"></a><span data-ttu-id="e0b6e-143">См. также</span><span class="sxs-lookup"><span data-stu-id="e0b6e-143">See also</span></span>

- [<span data-ttu-id="e0b6e-144">Создание accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="e0b6e-144">Create accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-post.md)
- [<span data-ttu-id="e0b6e-145">Список accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="e0b6e-145">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="e0b6e-146">List accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="e0b6e-146">List accessReviewInstance</span></span>](accessreviewinstance-list.md)
