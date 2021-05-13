---
title: Создание accessReviewHistoryDefinition
description: Создайте новый объект accessReviewHistoryDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3c0a1309ae67a2f4aa3f066deb5fe8adeec84119
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474124"
---
# <a name="create-accessreviewhistorydefinition"></a><span data-ttu-id="48026-103">Создание accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="48026-103">Create accessReviewHistoryDefinition</span></span>

<span data-ttu-id="48026-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48026-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48026-105">Создайте новый [объект accessReviewHistoryDefinition.](../resources/accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="48026-105">Create a new [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="48026-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48026-106">Permissions</span></span>

<span data-ttu-id="48026-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48026-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48026-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48026-109">Permission type</span></span>|<span data-ttu-id="48026-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48026-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48026-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48026-111">Delegated (work or school account)</span></span>|<span data-ttu-id="48026-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48026-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="48026-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48026-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48026-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48026-114">Not supported.</span></span>|
|<span data-ttu-id="48026-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48026-115">Application</span></span>|<span data-ttu-id="48026-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48026-116">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="48026-117">В роли каталога должен также быть подписан пользователь, который позволяет им читать обзор доступа для получения любых данных.</span><span class="sxs-lookup"><span data-stu-id="48026-117">The signed-in user must also be in a directory role that permits them to read an access review to retrieve any data.</span></span>  <span data-ttu-id="48026-118">Дополнительные сведения см. в дополнительных сведениях о требованиях к роли и разрешению для [отзывов о доступе.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="48026-118">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="48026-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48026-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/historyDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="48026-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48026-120">Request headers</span></span>

|<span data-ttu-id="48026-121">Имя</span><span class="sxs-lookup"><span data-stu-id="48026-121">Name</span></span>|<span data-ttu-id="48026-122">Описание</span><span class="sxs-lookup"><span data-stu-id="48026-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="48026-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48026-123">Authorization</span></span>|<span data-ttu-id="48026-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48026-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="48026-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="48026-126">Content-Type</span></span>|<span data-ttu-id="48026-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48026-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="48026-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48026-129">Request body</span></span>

<span data-ttu-id="48026-130">В теле запроса поставляют представление JSON объекта [accessReviewHistoryDefinition.](../resources/accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="48026-130">In the request body, supply a JSON representation of the [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object.</span></span>

<span data-ttu-id="48026-131">В следующей таблице показаны необходимые свойства, используемые для создания [accessReviewHistoryDefinition.](../resources/accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="48026-131">The following table shows the required properties used to create an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md).</span></span>

|<span data-ttu-id="48026-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="48026-132">Property</span></span>|<span data-ttu-id="48026-133">Тип</span><span class="sxs-lookup"><span data-stu-id="48026-133">Type</span></span>|<span data-ttu-id="48026-134">Описание</span><span class="sxs-lookup"><span data-stu-id="48026-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48026-135">displayName</span><span class="sxs-lookup"><span data-stu-id="48026-135">displayName</span></span> | <span data-ttu-id="48026-136">String</span><span class="sxs-lookup"><span data-stu-id="48026-136">String</span></span>  | <span data-ttu-id="48026-137">Имя для сбора данных истории проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="48026-137">Name for the access review history data collection.</span></span> <span data-ttu-id="48026-138">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="48026-138">Required.</span></span> |
|<span data-ttu-id="48026-139">reviewHistoryPeriodStartDateTime</span><span class="sxs-lookup"><span data-stu-id="48026-139">reviewHistoryPeriodStartDateTime</span></span>  | <span data-ttu-id="48026-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48026-140">DateTimeOffset</span></span>  | <span data-ttu-id="48026-141">Timestamp, отзывы, начиная с этой даты или после нее, будут включены в извлеченные данные истории.</span><span class="sxs-lookup"><span data-stu-id="48026-141">Timestamp, reviews starting on or after this date will be included in the fetched history data.</span></span> <span data-ttu-id="48026-142">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="48026-142">Required.</span></span>  |
|<span data-ttu-id="48026-143">reviewHistoryPeriodEndDateTime</span><span class="sxs-lookup"><span data-stu-id="48026-143">reviewHistoryPeriodEndDateTime</span></span>  | <span data-ttu-id="48026-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48026-144">DateTimeOffset</span></span>  | <span data-ttu-id="48026-145">Timestamp, отзывы, начиная с этой даты или до этой даты, будут включены в извлеченные данные истории.</span><span class="sxs-lookup"><span data-stu-id="48026-145">Timestamp, reviews starting on or before this date will be included in the fetched history data.</span></span> <span data-ttu-id="48026-146">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48026-146">Required.</span></span>  |
|<span data-ttu-id="48026-147">scopes</span><span class="sxs-lookup"><span data-stu-id="48026-147">scopes</span></span>|<span data-ttu-id="48026-148">коллекция microsoft.graph.accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="48026-148">microsoft.graph.accessReviewQueryScope collection</span></span>| <span data-ttu-id="48026-149">Используется для фильтрации отзывов, включенных в извлеченные данные истории.</span><span class="sxs-lookup"><span data-stu-id="48026-149">Used to filter which reviews are included in the fetched history data.</span></span> <span data-ttu-id="48026-150">Извлекает отзывы, область которых совпадает с этой предоставленной областью.</span><span class="sxs-lookup"><span data-stu-id="48026-150">Fetches reviews whose scope matches with this provided scope.</span></span> <span data-ttu-id="48026-151">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="48026-151">Required.</span></span>  |

### <a name="supported-scope-queries-for-accessreviewhistorydefinition"></a><span data-ttu-id="48026-152">Поддерживаемые запросы области для accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="48026-152">Supported scope queries for accessReviewHistoryDefinition</span></span>

<span data-ttu-id="48026-153">Ниже приводится запросы, поддерживаемые [в accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) на основе [accessreviewqueryscope.](../resources/accessreviewqueryscope.md)</span><span class="sxs-lookup"><span data-stu-id="48026-153">The following are queries supported on an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) based on the [accessreviewqueryscope](../resources/accessreviewqueryscope.md).</span></span> <span data-ttu-id="48026-154">Эти области диктуют, какой тип данных истории отзывов входит в загружаемый CSV-файл, который создается при создания определения.</span><span class="sxs-lookup"><span data-stu-id="48026-154">These scopes dictate which type of review history data is included in the downloadable CSV file which is generated when the definition is created.</span></span>

|<span data-ttu-id="48026-155">Сценарий</span><span class="sxs-lookup"><span data-stu-id="48026-155">Scenario</span></span>| <span data-ttu-id="48026-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="48026-156">Query</span></span> |
|--|--|
| <span data-ttu-id="48026-157">Включайте каждый результат проверки для отдельных групп (исключает определения, охватываемые для всех Microsoft 365 `accessReviewScheduleDefinition` групп с гостевых пользователей)</span><span class="sxs-lookup"><span data-stu-id="48026-157">Include every `accessReviewScheduleDefinition` review result on individual groups (excludes definitions scoped to all Microsoft 365 groups with guest users)</span></span> | <span data-ttu-id="48026-158">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')"</span><span class="sxs-lookup"><span data-stu-id="48026-158">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')"</span></span> |
| <span data-ttu-id="48026-159">Включайте каждый результат проверки в определенную группу (исключает определения, охватываемые для всех Microsoft 365 `accessReviewScheduleDefinition` групп с гостевых пользователей)</span><span class="sxs-lookup"><span data-stu-id="48026-159">Include every `accessReviewScheduleDefinition` review result on a specific group (excludes definitions scoped to all Microsoft 365 groups with guest users)</span></span> | <span data-ttu-id="48026-160">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups/{group id}')</span><span class="sxs-lookup"><span data-stu-id="48026-160">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups/{group id}')</span></span> |
| <span data-ttu-id="48026-161">Включайте каждый результат проверки для `accessReviewScheduleDefinition` всех Microsoft 365 групп с гостевых пользователей</span><span class="sxs-lookup"><span data-stu-id="48026-161">Include every `accessReviewScheduleDefinition` review result scoped to all Microsoft 365 groups with guest users</span></span> | <span data-ttu-id="48026-162">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, './members')</span><span class="sxs-lookup"><span data-stu-id="48026-162">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, './members')</span></span> |
| <span data-ttu-id="48026-163">`accessReviewScheduleDefinition`Включи каждый результат проверки в пакет доступа</span><span class="sxs-lookup"><span data-stu-id="48026-163">Include every `accessReviewScheduleDefinition` review result on an access package</span></span> | <span data-ttu-id="48026-164">/identityGovernance/accessReviews/definitions?$filter=contains (scope/query, 'accessPackageAssignments')</span><span class="sxs-lookup"><span data-stu-id="48026-164">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')</span></span> |
| <span data-ttu-id="48026-165">`accessReviewScheduleDefinition`Включай каждый результат проверки для директоров служб, назначенных привилегированной роли</span><span class="sxs-lookup"><span data-stu-id="48026-165">Include every `accessReviewScheduleDefinition` review result for service principals assigned to privileged role</span></span> | <span data-ttu-id="48026-166">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'roleAssignmentScheduleInstances')</span><span class="sxs-lookup"><span data-stu-id="48026-166">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'roleAssignmentScheduleInstances')</span></span> |
| <span data-ttu-id="48026-167">`accessReviewScheduleDefinition`Включи каждый результат проверки для reivews определенной группы</span><span class="sxs-lookup"><span data-stu-id="48026-167">Include every `accessReviewScheduleDefinition` review result for reivews of a specific group</span></span> | <span data-ttu-id="48026-168">/identityGovernance/accessReviews/definitions?$filter=scope/query eq '/groups/a1382a9b-8320-4e9c-8f73-dfead37d7723/members'</span><span class="sxs-lookup"><span data-stu-id="48026-168">/identityGovernance/accessReviews/definitions?$filter=scope/query eq '/groups/a1382a9b-8320-4e9c-8f73-dfead37d7723/members'</span></span> |

## <a name="response"></a><span data-ttu-id="48026-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="48026-169">Response</span></span>

<span data-ttu-id="48026-170">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="48026-170">If successful, this method returns a `201 Created` response code and an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="48026-171">Примеры</span><span class="sxs-lookup"><span data-stu-id="48026-171">Examples</span></span>

<span data-ttu-id="48026-172">В следующем примере показано, как создать определение истории доступа для доступа к отзывам по пакетам и группам доступа, которое будет работать между датой начала 01/01/2021 и датой окончания 04/05/2021.</span><span class="sxs-lookup"><span data-stu-id="48026-172">The following example shows how to create an access review history definition scoped to access reviews on access packages and groups, running between the start date of 01/01/2021 and end date of 04/05/2021.</span></span>

### <a name="request"></a><span data-ttu-id="48026-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="48026-173">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="48026-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="48026-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessreviewhistorydefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions
Content-Type: application/json

{
  "displayName": "Last quarter's group reviews April 2021",
  "decisions": [
    "approve",
    "deny",
    "dontKnow",
    "notReviewed",
    "notNotified"
  ],
  "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
  "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
      "queryRoot": null
    },  
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
      "queryRoot": null
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="48026-175">C#</span><span class="sxs-lookup"><span data-stu-id="48026-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewhistorydefinition-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48026-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48026-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewhistorydefinition-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48026-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48026-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewhistorydefinition-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="48026-178">Java</span><span class="sxs-lookup"><span data-stu-id="48026-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewhistorydefinition-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="48026-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="48026-179">Response</span></span>
><span data-ttu-id="48026-180">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="48026-180">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
  "id": "b2cb022f-b7e1-40f3-9854-c65a40861c38",
  "displayName": "Last quarter's group reviews April 2021",
  "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
  "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
  "decisions": [
    "approve",
    "deny",
    "dontKnow",
    "notReviewed",
    "notNotified"
  ],
  "status": "requested",
  "createdDateTime": "2021-04-14T00:22:48.9392594Z",
  "fulfilledDateTime": null,
  "downloadUri": null,
  "createdBy": {
      "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
      "displayName": "MOD Administrator",
      "userPrincipalName": "admin@contoso.com"
  },
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
      "queryRoot": null
    },  
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
      "queryRoot": null
    }
  ]
}
```
