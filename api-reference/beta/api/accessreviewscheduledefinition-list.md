---
title: Список accessReviewScheduleDefinitions
description: Извлечение объектов accessReviewScheduleDefinition.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 769ebef6e056a9b2e345d7afad772f8893b50dda
ms.sourcegitcommit: 612e1d796023433c6e15a9d66ba99d9bdc424cee
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2021
ms.locfileid: "52703498"
---
# <a name="list-accessreviewscheduledefinition"></a><span data-ttu-id="0cf2c-103">Список accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="0cf2c-103">List accessReviewScheduleDefinition</span></span>

<span data-ttu-id="0cf2c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cf2c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cf2c-105">Извлечение [объектов accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0cf2c-105">Retrieve the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects.</span></span> <span data-ttu-id="0cf2c-106">Возвращается список объектов accessReviewScheduleDefinition, включая все вложенные свойства, для каждой созданной серии обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-106">A list of zero or more accessReviewScheduleDefinition objects are returned, including all of their nested properties, for each access review series created.</span></span> <span data-ttu-id="0cf2c-107">Это не включает связанные объекты accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-107">This does not include the associated accessReviewInstance objects.</span></span>

>[!NOTE]
><span data-ttu-id="0cf2c-108">Размер страницы по умолчанию для этого API — 100 объектов accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-108">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="0cf2c-109">Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-109">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="0cf2c-110">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="0cf2c-110">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="0cf2c-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0cf2c-111">Permissions</span></span>
<span data-ttu-id="0cf2c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cf2c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cf2c-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0cf2c-114">Permission type</span></span>                        | <span data-ttu-id="0cf2c-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0cf2c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cf2c-116">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0cf2c-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="0cf2c-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cf2c-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="0cf2c-118">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0cf2c-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cf2c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-119">Not supported.</span></span>|
|<span data-ttu-id="0cf2c-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="0cf2c-120">Application</span></span>                            | <span data-ttu-id="0cf2c-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cf2c-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

 <span data-ttu-id="0cf2c-122">В роли каталога должен также быть подписан пользователь, который позволяет им читать обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-122">The signed-in user must also be in a directory role that permits them to read an access review.</span></span> <span data-ttu-id="0cf2c-123">См. роль [обзора доступа и проверки авторизации разрешений приложений.](../resources/accessreviewsv2-root.md#role-and-application-permission-authorization-checks)</span><span class="sxs-lookup"><span data-stu-id="0cf2c-123">See access review [role and application permission authorization checks](../resources/accessreviewsv2-root.md#role-and-application-permission-authorization-checks).</span></span>

## <a name="http-request"></a><span data-ttu-id="0cf2c-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0cf2c-124">HTTP request</span></span>

<span data-ttu-id="0cf2c-125">Чтобы перечислить все ваши accessReviewScheduleDefinitions:</span><span class="sxs-lookup"><span data-stu-id="0cf2c-125">To list all your accessReviewScheduleDefinitions:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0cf2c-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0cf2c-126">Optional query parameters</span></span>
<span data-ttu-id="0cf2c-127">Этот метод поддерживает `$select` параметры `$top` запросов , и `$skip` OData, чтобы помочь `$filter` настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-127">This method supports the `$select`, `$top`, `$skip`, and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="0cf2c-128">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0cf2c-128">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="use-the-filter-query-parameter"></a><span data-ttu-id="0cf2c-129">Использование параметра $filter запроса</span><span class="sxs-lookup"><span data-stu-id="0cf2c-129">Use the $filter query parameter</span></span>
<span data-ttu-id="0cf2c-130">Параметр `$filter` запроса с `contains` оператором  поддерживается в свойстве области accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-130">The `$filter` query parameter with the `contains` operator is supported on the **scope** property of accessReviewScheduleDefinition.</span></span> <span data-ttu-id="0cf2c-131">Используйте следующий формат для запроса:</span><span class="sxs-lookup"><span data-stu-id="0cf2c-131">Use the following format for the request:</span></span>

```http
GET /identityGovernance/accessReviews/definitions?$filter=contains(scope/microsoft.graph.accessReviewQueryScope/query, '{object}')
```

<span data-ttu-id="0cf2c-132">Значение может `{object}` быть одним из следующих:</span><span class="sxs-lookup"><span data-stu-id="0cf2c-132">The value of `{object}` can be one of the following:</span></span>

|<span data-ttu-id="0cf2c-133">Значение</span><span class="sxs-lookup"><span data-stu-id="0cf2c-133">Value</span></span>|<span data-ttu-id="0cf2c-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0cf2c-134">Description</span></span>|
|:---     |:---       |
|`/groups`  |<span data-ttu-id="0cf2c-135">Список всех accessReviewScheduleDefinition в отдельных группах (исключает определения, Microsoft 365 группы с гостевых пользователей).</span><span class="sxs-lookup"><span data-stu-id="0cf2c-135">List every accessReviewScheduleDefinition on individual groups (excludes definitions scoped to all Microsoft 365 groups with guest users).</span></span>|
|`/groups/{group id}`  |<span data-ttu-id="0cf2c-136">Список всех accessReviewScheduleDefinition в определенной группе (исключает определения, Microsoft 365 группы с гостевых пользователей).</span><span class="sxs-lookup"><span data-stu-id="0cf2c-136">List every accessReviewScheduleDefinition on a specific group (excludes definitions scoped to all Microsoft 365 groups with guest users).</span></span>|
|`./members`  |<span data-ttu-id="0cf2c-137">Список всех accessReviewScheduleDefinition, Microsoft 365 групп с гостевых пользователей.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-137">List every accessReviewScheduleDefinition scoped to all Microsoft 365 groups with guest users.</span></span>|
|`accessPackageAssignments`  |<span data-ttu-id="0cf2c-138">Список всех accessReviewScheduleDefinition в пакете доступа.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-138">List every accessReviewScheduleDefinition on an access package.</span></span>|
|`roleAssignmentScheduleInstances`  |<span data-ttu-id="0cf2c-139">Список всех accessReviewScheduleDefinition для глав служб, присвоенных привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-139">List every accessReviewScheduleDefinition for service principals assigned to a privileged role.</span></span>|

<span data-ttu-id="0cf2c-140">Параметр `$filter` запроса не поддерживается в **accessReviewInactiveUserQueryScope** или **principalResourceMembershipScope.**</span><span class="sxs-lookup"><span data-stu-id="0cf2c-140">The `$filter` query parameter is not supported on **accessReviewInactiveUserQueryScope** or **principalResourceMembershipScope**.</span></span>


## <a name="request-headers"></a><span data-ttu-id="0cf2c-141">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0cf2c-141">Request headers</span></span>
<span data-ttu-id="0cf2c-142">Нет.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-142">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="0cf2c-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0cf2c-143">Request body</span></span>
<span data-ttu-id="0cf2c-144">Не поставляем тело запроса.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-144">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="0cf2c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cf2c-145">Response</span></span>
<span data-ttu-id="0cf2c-146">В случае успешной работы этот метод возвращает код отклика и массив `200 OK` [объектов accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-146">If successful, this method returns a `200 OK` response code and an array of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0cf2c-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="0cf2c-147">Examples</span></span>

### <a name="example-1-list-the-first-one-hundred-access-review-definitions"></a><span data-ttu-id="0cf2c-148">Пример 1. Список первой сотни определений обзоров доступа</span><span class="sxs-lookup"><span data-stu-id="0cf2c-148">Example 1: List the first one hundred access review definitions</span></span>

#### <a name="request"></a><span data-ttu-id="0cf2c-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cf2c-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0cf2c-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cf2c-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="0cf2c-151">C#</span><span class="sxs-lookup"><span data-stu-id="0cf2c-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cf2c-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cf2c-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cf2c-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cf2c-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0cf2c-154">Java</span><span class="sxs-lookup"><span data-stu-id="0cf2c-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="0cf2c-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cf2c-155">Response</span></span>
><span data-ttu-id="0cf2c-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-156">**Note:** The response object shown here might be shortened for readability.</span></span>
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


### <a name="example-2-retrieve-all-access-review-definitions-scoped-to-all-microsoft-365-groups-in-a-tenant"></a><span data-ttu-id="0cf2c-157">Пример 2. Извлечение всех определений обзоров доступа для всех Microsoft 365 групп клиента</span><span class="sxs-lookup"><span data-stu-id="0cf2c-157">Example 2: Retrieve all access review definitions scoped to all Microsoft 365 groups in a tenant</span></span>

#### <a name="request"></a><span data-ttu-id="0cf2c-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cf2c-158">Request</span></span>
<span data-ttu-id="0cf2c-159">В следующем примере показан запрос на извлечение всей серии обзоров доступа для всех Microsoft 365 групп клиента.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-159">The following example shows a request to retrieve all the access review series scoped to all Microsoft 365 groups in a tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition_allgroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions?$filter=contains(scope/microsoft.graph.accessReviewQueryScope/query, './members')
```

#### <a name="response"></a><span data-ttu-id="0cf2c-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cf2c-160">Response</span></span>
><span data-ttu-id="0cf2c-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0cf2c-161">**Note:** The response object shown here might be shortened for readability.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="0cf2c-162">См. также</span><span class="sxs-lookup"><span data-stu-id="0cf2c-162">See also</span></span>

- [<span data-ttu-id="0cf2c-163">Получить accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="0cf2c-163">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)


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
