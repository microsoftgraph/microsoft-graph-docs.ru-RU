---
title: Список accessReviewScheduleDefinitions
description: Извлечение объектов accessReviewScheduleDefinition.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: bbc014075f1dc72970ef64add9555d6067cbe0f0
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870026"
---
# <a name="list-accessreviewscheduledefinition"></a><span data-ttu-id="ec183-103">Список accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="ec183-103">List accessReviewScheduleDefinition</span></span>

<span data-ttu-id="ec183-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec183-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec183-105">Извлечение [объектов accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ec183-105">Retrieve the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects.</span></span> <span data-ttu-id="ec183-106">Возвращается список объектов accessReviewScheduleDefinition, включая все вложенные свойства, для каждой созданной серии обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="ec183-106">A list of zero or more accessReviewScheduleDefinition objects are returned, including all of their nested properties, for each access review series created.</span></span> <span data-ttu-id="ec183-107">Это не включает связанные объекты accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="ec183-107">This does not include the associated accessReviewInstance objects.</span></span>

>[!NOTE]
><span data-ttu-id="ec183-108">Размер страницы по умолчанию для этого API — 100 объектов accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="ec183-108">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="ec183-109">Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов.</span><span class="sxs-lookup"><span data-stu-id="ec183-109">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="ec183-110">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="ec183-110">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="ec183-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec183-111">Permissions</span></span>
<span data-ttu-id="ec183-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec183-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec183-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec183-114">Permission type</span></span>                        | <span data-ttu-id="ec183-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec183-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec183-116">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec183-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="ec183-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec183-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="ec183-118">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec183-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec183-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec183-119">Not supported.</span></span>|
|<span data-ttu-id="ec183-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="ec183-120">Application</span></span>                            | <span data-ttu-id="ec183-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec183-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

 <span data-ttu-id="ec183-122">В роли каталога должен также быть подписан пользователь, который позволяет им читать обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="ec183-122">The signed-in user must also be in a directory role that permits them to read an access review.</span></span> <span data-ttu-id="ec183-123">См. роль [обзора доступа и проверки авторизации разрешений приложений.](../resources/accessreviewsv2-root.md#role-and-application-permission-authorization-checks)</span><span class="sxs-lookup"><span data-stu-id="ec183-123">See access review [role and application permission authorization checks](../resources/accessreviewsv2-root.md#role-and-application-permission-authorization-checks).</span></span>

## <a name="http-request"></a><span data-ttu-id="ec183-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec183-124">HTTP request</span></span>

<span data-ttu-id="ec183-125">Чтобы перечислить все ваши accessReviewScheduleDefinitions:</span><span class="sxs-lookup"><span data-stu-id="ec183-125">To list all your accessReviewScheduleDefinitions:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ec183-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ec183-126">Optional query parameters</span></span>
<span data-ttu-id="ec183-127">Этот метод поддерживает `$select` параметры `$top` запросов , и `$skip` OData, чтобы помочь `$filter` настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="ec183-127">This method supports the `$select`, `$top`, `$skip`, and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="ec183-128">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ec183-128">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="use-the-filter-query-parameter"></a><span data-ttu-id="ec183-129">Использование параметра $filter запроса</span><span class="sxs-lookup"><span data-stu-id="ec183-129">Use the $filter query parameter</span></span>
<span data-ttu-id="ec183-130">Параметр `$filter` запроса с `contains` оператором  поддерживается в свойстве области accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="ec183-130">The `$filter` query parameter with the `contains` operator is supported on the **scope** property of accessReviewScheduleDefinition.</span></span> <span data-ttu-id="ec183-131">Используйте следующий формат для запроса:</span><span class="sxs-lookup"><span data-stu-id="ec183-131">Use the following format for the request:</span></span>

```http
GET /identityGovernance/accessReviews/definitions?$filter=contains(scope/microsoft.graph.accessReviewQueryScope/query, '{object}')
```

<span data-ttu-id="ec183-132">Значение может `{object}` быть одним из следующих:</span><span class="sxs-lookup"><span data-stu-id="ec183-132">The value of `{object}` can be one of the following:</span></span>

|<span data-ttu-id="ec183-133">Значение</span><span class="sxs-lookup"><span data-stu-id="ec183-133">Value</span></span>|<span data-ttu-id="ec183-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ec183-134">Description</span></span>|
|:---     |:---       |
|<span data-ttu-id="ec183-135">/groups</span><span class="sxs-lookup"><span data-stu-id="ec183-135">/groups</span></span>  |<span data-ttu-id="ec183-136">Список всех accessReviewScheduleDefinition в отдельных группах (исключает определения, Microsoft 365 группы с гостевых пользователей).</span><span class="sxs-lookup"><span data-stu-id="ec183-136">List every accessReviewScheduleDefinition on individual groups (excludes definitions scoped to all Microsoft 365 groups with guest users).</span></span>|
|<span data-ttu-id="ec183-137">/groups/{group id}</span><span class="sxs-lookup"><span data-stu-id="ec183-137">/groups/{group id}</span></span>  |<span data-ttu-id="ec183-138">Список всех accessReviewScheduleDefinition в определенной группе (исключает определения, Microsoft 365 группы с гостевых пользователей).</span><span class="sxs-lookup"><span data-stu-id="ec183-138">List every accessReviewScheduleDefinition on a specific group (excludes definitions scoped to all Microsoft 365 groups with guest users).</span></span>|
|<span data-ttu-id="ec183-139">./members</span><span class="sxs-lookup"><span data-stu-id="ec183-139">./members</span></span>  |<span data-ttu-id="ec183-140">Список всех accessReviewScheduleDefinition, Microsoft 365 групп с гостевых пользователей.</span><span class="sxs-lookup"><span data-stu-id="ec183-140">List every accessReviewScheduleDefinition scoped to all Microsoft 365 groups with guest users.</span></span>|
|<span data-ttu-id="ec183-141">accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="ec183-141">accessPackageAssignments</span></span>  |<span data-ttu-id="ec183-142">Список всех accessReviewScheduleDefinition в пакете доступа.</span><span class="sxs-lookup"><span data-stu-id="ec183-142">List every accessReviewScheduleDefinition on an access package.</span></span>|
|<span data-ttu-id="ec183-143">roleAssignmentScheduleInstances</span><span class="sxs-lookup"><span data-stu-id="ec183-143">roleAssignmentScheduleInstances</span></span>  |<span data-ttu-id="ec183-144">Список всех accessReviewScheduleDefinition для глав служб, присвоенных привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="ec183-144">List every accessReviewScheduleDefinition for service principals assigned to a privileged role.</span></span>|

<span data-ttu-id="ec183-145">Параметр `$filter` запроса не поддерживается в **accessReviewInactiveUserQueryScope** или **principalResourceMembershipScope.**</span><span class="sxs-lookup"><span data-stu-id="ec183-145">The `$filter` query parameter is not supported on **accessReviewInactiveUserQueryScope** or **principalResourceMembershipScope**.</span></span>


## <a name="request-headers"></a><span data-ttu-id="ec183-146">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec183-146">Request headers</span></span>
<span data-ttu-id="ec183-147">Нет.</span><span class="sxs-lookup"><span data-stu-id="ec183-147">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="ec183-148">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ec183-148">Request body</span></span>
<span data-ttu-id="ec183-149">Не поставляем тело запроса.</span><span class="sxs-lookup"><span data-stu-id="ec183-149">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="ec183-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec183-150">Response</span></span>
<span data-ttu-id="ec183-151">В случае успешной работы этот метод возвращает код отклика и массив `200 OK` [объектов accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ec183-151">If successful, this method returns a `200 OK` response code and an array of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ec183-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="ec183-152">Examples</span></span>

### <a name="example-1-list-the-first-one-hundred-access-review-definitions"></a><span data-ttu-id="ec183-153">Пример 1. Список первой сотни определений обзоров доступа</span><span class="sxs-lookup"><span data-stu-id="ec183-153">Example 1: List the first one hundred access review definitions</span></span>

#### <a name="request"></a><span data-ttu-id="ec183-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec183-154">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ec183-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec183-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="ec183-156">C#</span><span class="sxs-lookup"><span data-stu-id="ec183-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec183-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec183-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec183-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec183-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec183-159">Java</span><span class="sxs-lookup"><span data-stu-id="ec183-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ec183-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec183-160">Response</span></span>
><span data-ttu-id="ec183-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ec183-161">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions",
    "@odata.count": 1,
    "value": [
        {
            "id": "98dcebed-c7f6-46f4-bcf3-4a3fccdb3e2a",
            "displayName": "Access Review",
            "scope": {
                "query": "/groups/119cc181-22f0-4e18-8537-264e7524ee0b/transitiveMembers",
                "queryType": "MicrosoftGraph"
            },
            "instanceEnumerationScope": {
                "query": "/groups/119cc181-22f0-4e18-8537-264e7524ee0b",
                "queryType": "MicrosoftGraph"
            },
            "reviewers": [
                {
                    "query": "./manager",
                    "queryType": "MicrosoftGraph",
                    "queryRoot": "decisions"
                }
            ],
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
                        "startDate": "2020-09-11",
                        "endDate": "9999-12-31"
                    }
                }
            }
        }
    ]
}
```


### <a name="example-2-retrieve-all-access-review-definitions-scoped-to-all-microsoft-365-groups-in-a-tenant"></a><span data-ttu-id="ec183-162">Пример 2. Извлечение всех определений обзоров доступа для всех Microsoft 365 групп клиента</span><span class="sxs-lookup"><span data-stu-id="ec183-162">Example 2: Retrieve all access review definitions scoped to all Microsoft 365 groups in a tenant</span></span>

#### <a name="request"></a><span data-ttu-id="ec183-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec183-163">Request</span></span>
<span data-ttu-id="ec183-164">В следующем примере показан запрос на извлечение всей серии обзоров доступа для всех Microsoft 365 групп клиента.</span><span class="sxs-lookup"><span data-stu-id="ec183-164">The following example shows a request to retrieve all the access review series scoped to all Microsoft 365 groups in a tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="ec183-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec183-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition_allgroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions?$filter=contains(scope/microsoft.graph.accessReviewQueryScope/query, './members')
```
# <a name="c"></a>[<span data-ttu-id="ec183-166">C#</span><span class="sxs-lookup"><span data-stu-id="ec183-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewscheduledefinition-allgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec183-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec183-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewscheduledefinition-allgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec183-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec183-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewscheduledefinition-allgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec183-169">Java</span><span class="sxs-lookup"><span data-stu-id="ec183-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewscheduledefinition-allgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ec183-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec183-170">Response</span></span>
><span data-ttu-id="ec183-171">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ec183-171">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions",
    "@odata.count": 1,
    "value": [
        {
            "id": "cc701697-762c-439a-81f5-f58d680fde76",
            "displayName": "Review guest access across Microsoft 365 groups",
            "status": "InProgress",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph"
            },
            "instanceEnumerationScope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
                "queryType": "MicrosoftGraph"
            },
            "reviewers": [
                {
                    "query": "./manager",
                    "queryType": "MicrosoftGraph",
                    "queryRoot": "decisions"
                }
            ],
            "settings": {
                "mailNotificationsEnabled": true,
                "reminderNotificationsEnabled": true,
                "justificationRequiredOnApproval": true,
                "defaultDecisionEnabled": true,
                "defaultDecision": "Recommendation",
                "instanceDurationInDays": 25,
                "autoApplyDecisionsEnabled": true,
                "recommendationsEnabled": true,
                "recurrence": {
                    "pattern": {
                        "type": "absoluteMonthly",
                        "interval": 3,
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
                        "startDate": "2021-04-27",
                        "endDate": "9999-12-31"
                    }
                },
                "applyActions": [
                    {
                        "@odata.type": "#microsoft.graph.removeAccessApplyAction"
                    }
                ]
            },
            "instances@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('cc701697-762c-439a-81f5-f58d680fde76')/instances",
            "instances": []
        }
    ]
}

```


## <a name="see-also"></a><span data-ttu-id="ec183-172">См. также</span><span class="sxs-lookup"><span data-stu-id="ec183-172">See also</span></span>

- [<span data-ttu-id="ec183-173">Получить accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="ec183-173">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
