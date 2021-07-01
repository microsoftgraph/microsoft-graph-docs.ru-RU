---
title: Список accessReviewScheduleDefinitions
description: Получите список объектов accessReviewScheduleDefinition и их свойств.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 34c58be8c3fa0c580e91a74baee2ddafbed3e738
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208714"
---
# <a name="list-accessreviewscheduledefinitions"></a><span data-ttu-id="0a534-103">Список accessReviewScheduleDefinitions</span><span class="sxs-lookup"><span data-stu-id="0a534-103">List accessReviewScheduleDefinitions</span></span>
<span data-ttu-id="0a534-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a534-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0a534-105">Получите список объектов [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="0a534-105">Get a list of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects and their properties.</span></span>

>[!NOTE]
><span data-ttu-id="0a534-106">Размер страницы по умолчанию для этого API — 100 объектов accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="0a534-106">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="0a534-107">Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов.</span><span class="sxs-lookup"><span data-stu-id="0a534-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="0a534-108">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="0a534-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="0a534-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a534-109">Permissions</span></span>
<span data-ttu-id="0a534-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a534-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a534-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a534-112">Permission type</span></span>|<span data-ttu-id="0a534-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a534-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a534-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a534-114">Delegated (work or school account)</span></span>|<span data-ttu-id="0a534-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a534-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="0a534-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a534-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a534-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a534-117">Not supported.</span></span>|
|<span data-ttu-id="0a534-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="0a534-118">Application</span></span>|<span data-ttu-id="0a534-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a534-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

 <span data-ttu-id="0a534-120">В роли каталога должен также быть подписан пользователь, который позволяет им читать обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="0a534-120">The signed-in user must also be in a directory role that permits them to read an access review.</span></span> <span data-ttu-id="0a534-121">См. роль [обзора доступа и проверки авторизации разрешений приложений.](../resources/accessreviewsv2-root.md#role-and-application-permission-authorization-checks)</span><span class="sxs-lookup"><span data-stu-id="0a534-121">See access review [role and application permission authorization checks](../resources/accessreviewsv2-root.md#role-and-application-permission-authorization-checks).</span></span>

## <a name="http-request"></a><span data-ttu-id="0a534-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a534-122">HTTP request</span></span>

<span data-ttu-id="0a534-123">Чтобы перечислить все ваши accessReviewScheduleDefinitions:</span><span class="sxs-lookup"><span data-stu-id="0a534-123">To list all your accessReviewScheduleDefinitions:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0a534-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0a534-124">Optional query parameters</span></span>
<span data-ttu-id="0a534-125">Этот метод поддерживает `$select` параметры `$top` запроса , `$skip` , , и `$orderBy` `$filter` OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="0a534-125">This method supports the `$select`, `$top`, `$skip`,`$orderBy`, and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="0a534-126">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0a534-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="use-the-filter-query-parameter"></a><span data-ttu-id="0a534-127">Использование параметра $filter запроса</span><span class="sxs-lookup"><span data-stu-id="0a534-127">Use the $filter query parameter</span></span>
<span data-ttu-id="0a534-128">Параметр `$filter` запроса с `contains` оператором  поддерживается в свойстве области accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="0a534-128">The `$filter` query parameter with the `contains` operator is supported on the **scope** property of accessReviewScheduleDefinition.</span></span> <span data-ttu-id="0a534-129">Используйте следующий формат для запроса:</span><span class="sxs-lookup"><span data-stu-id="0a534-129">Use the following format for the request:</span></span>

```http
GET /identityGovernance/accessReviews/definitions?$filter=contains(scope/microsoft.graph.accessReviewQueryScope/query, '{object}')
```

<span data-ttu-id="0a534-130">Значение может `{object}` быть одним из следующих:</span><span class="sxs-lookup"><span data-stu-id="0a534-130">The value of `{object}` can be one of the following:</span></span>

|<span data-ttu-id="0a534-131">Значение</span><span class="sxs-lookup"><span data-stu-id="0a534-131">Value</span></span>|<span data-ttu-id="0a534-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0a534-132">Description</span></span>|
|:---     |:---       |
|`/groups`  |<span data-ttu-id="0a534-133">Список всех accessReviewScheduleDefinition в отдельных группах (исключает определения, Microsoft 365 группы с гостевых пользователей).</span><span class="sxs-lookup"><span data-stu-id="0a534-133">List every accessReviewScheduleDefinition on individual groups (excludes definitions scoped to all Microsoft 365 groups with guest users).</span></span>|
|`/groups/{group id}`  |<span data-ttu-id="0a534-134">Список всех accessReviewScheduleDefinition в определенной группе (исключает определения, Microsoft 365 группы с гостевых пользователей).</span><span class="sxs-lookup"><span data-stu-id="0a534-134">List every accessReviewScheduleDefinition on a specific group (excludes definitions scoped to all Microsoft 365 groups with guest users).</span></span>|
|`./members`  |<span data-ttu-id="0a534-135">Список всех accessReviewScheduleDefinition, Microsoft 365 групп с гостевых пользователей.</span><span class="sxs-lookup"><span data-stu-id="0a534-135">List every accessReviewScheduleDefinition scoped to all Microsoft 365 groups with guest users.</span></span>|
|`accessPackageAssignments`  |<span data-ttu-id="0a534-136">Список всех accessReviewScheduleDefinition в пакете доступа.</span><span class="sxs-lookup"><span data-stu-id="0a534-136">List every accessReviewScheduleDefinition on an access package.</span></span>|
|`roleAssignmentScheduleInstances`  |<span data-ttu-id="0a534-137">Список всех accessReviewScheduleDefinition для глав служб, присвоенных привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="0a534-137">List every accessReviewScheduleDefinition for service principals assigned to a privileged role.</span></span>|

<span data-ttu-id="0a534-138">Параметр `$filter` запроса не поддерживается в **accessReviewInactiveUserQueryScope** или **principalResourceMembershipScope.**</span><span class="sxs-lookup"><span data-stu-id="0a534-138">The `$filter` query parameter is not supported on **accessReviewInactiveUserQueryScope** or **principalResourceMembershipScope**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a534-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a534-139">Request headers</span></span>
|<span data-ttu-id="0a534-140">Имя</span><span class="sxs-lookup"><span data-stu-id="0a534-140">Name</span></span>|<span data-ttu-id="0a534-141">Описание</span><span class="sxs-lookup"><span data-stu-id="0a534-141">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0a534-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a534-142">Authorization</span></span>|<span data-ttu-id="0a534-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a534-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a534-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a534-145">Request body</span></span>
<span data-ttu-id="0a534-146">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0a534-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a534-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a534-147">Response</span></span>

<span data-ttu-id="0a534-148">В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [объектов accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0a534-148">If successful, this method returns a `200 OK` response code and a collection of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0a534-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="0a534-149">Examples</span></span>

### <a name="example-1-list-the-first-one-hundred-access-review-definitions"></a><span data-ttu-id="0a534-150">Пример 1. Список первой сотни определений обзоров доступа</span><span class="sxs-lookup"><span data-stu-id="0a534-150">Example 1: List the first one hundred access review definitions</span></span>

#### <a name="request"></a><span data-ttu-id="0a534-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a534-151">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0a534-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a534-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition"
}-->
```
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="0a534-153">C#</span><span class="sxs-lookup"><span data-stu-id="0a534-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a534-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a534-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a534-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a534-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a534-156">Java</span><span class="sxs-lookup"><span data-stu-id="0a534-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0a534-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a534-157">Response</span></span>
><span data-ttu-id="0a534-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0a534-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions",
    "@odata.count": 1,
    "value": [
        {
            "id": "98dcebed-c7f6-46f4-bcf3-4a3fccdb3e2a",
            "displayName": "Access Review",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/groups/119cc181-22f0-4e18-8537-264e7524ee0b/transitiveMembers",
                "queryType": "MicrosoftGraph"
            },
            "instanceEnumerationScope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
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

### <a name="example-2-retrieve-all-access-review-definitions-scoped-to-all-microsoft-365-groups-in-a-tenant"></a><span data-ttu-id="0a534-159">Пример 2. Извлечение всех определений обзоров доступа для всех Microsoft 365 групп клиента</span><span class="sxs-lookup"><span data-stu-id="0a534-159">Example 2: Retrieve all access review definitions scoped to all Microsoft 365 groups in a tenant</span></span>

#### <a name="request"></a><span data-ttu-id="0a534-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a534-160">Request</span></span>
<span data-ttu-id="0a534-161">В следующем примере показан запрос на извлечение всей серии обзоров доступа для всех Microsoft 365 групп клиента.</span><span class="sxs-lookup"><span data-stu-id="0a534-161">The following example shows a request to retrieve all the access review series scoped to all Microsoft 365 groups in a tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="0a534-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a534-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition_allgroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions?$filter=contains(scope/microsoft.graph.accessReviewQueryScope/query, './members')
```
# <a name="c"></a>[<span data-ttu-id="0a534-163">C#</span><span class="sxs-lookup"><span data-stu-id="0a534-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewscheduledefinition-allgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a534-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a534-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewscheduledefinition-allgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a534-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a534-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewscheduledefinition-allgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a534-166">Java</span><span class="sxs-lookup"><span data-stu-id="0a534-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewscheduledefinition-allgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0a534-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a534-167">Response</span></span>
><span data-ttu-id="0a534-168">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0a534-168">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions",
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
            "instances@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('cc701697-762c-439a-81f5-f58d680fde76')/instances",
            "instances": []
        }
    ]
}

```
