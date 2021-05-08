---
title: Создание accessReviewHistoryDefinition
description: Создайте новый объект accessReviewHistoryDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1ecb35c0c56d0db937aca60fa00d3559f0a063c4
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232953"
---
# <a name="create-accessreviewhistorydefinition"></a><span data-ttu-id="55ab3-103">Создание accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="55ab3-103">Create accessReviewHistoryDefinition</span></span>

<span data-ttu-id="55ab3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55ab3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55ab3-105">Создайте новый [объект accessReviewHistoryDefinition.](../resources/accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="55ab3-105">Create a new [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="55ab3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55ab3-106">Permissions</span></span>

<span data-ttu-id="55ab3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55ab3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55ab3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55ab3-109">Permission type</span></span>|<span data-ttu-id="55ab3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55ab3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55ab3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55ab3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="55ab3-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55ab3-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="55ab3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55ab3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55ab3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55ab3-114">Not supported.</span></span>|
|<span data-ttu-id="55ab3-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="55ab3-115">Application</span></span>|<span data-ttu-id="55ab3-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55ab3-116">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="55ab3-117">В роли каталога должен также быть подписан пользователь, который позволяет им читать обзор доступа для получения любых данных.</span><span class="sxs-lookup"><span data-stu-id="55ab3-117">The signed-in user must also be in a directory role that permits them to read an access review to retrieve any data.</span></span>  <span data-ttu-id="55ab3-118">Дополнительные сведения см. в дополнительных сведениях о требованиях к роли и разрешению для [отзывов о доступе.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="55ab3-118">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="55ab3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55ab3-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/historyDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="55ab3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55ab3-120">Request headers</span></span>

|<span data-ttu-id="55ab3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="55ab3-121">Name</span></span>|<span data-ttu-id="55ab3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="55ab3-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="55ab3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55ab3-123">Authorization</span></span>|<span data-ttu-id="55ab3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55ab3-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="55ab3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="55ab3-126">Content-Type</span></span>|<span data-ttu-id="55ab3-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55ab3-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="55ab3-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55ab3-129">Request body</span></span>

<span data-ttu-id="55ab3-130">В теле запроса поставляют представление JSON объекта [accessReviewHistoryDefinition.](../resources/accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="55ab3-130">In the request body, supply a JSON representation of the [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object.</span></span>

<span data-ttu-id="55ab3-131">В следующей таблице показаны необходимые свойства, используемые для создания [accessReviewHistoryDefinition.](../resources/accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="55ab3-131">The following table shows the required properties used to create an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md).</span></span>

|<span data-ttu-id="55ab3-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="55ab3-132">Property</span></span>|<span data-ttu-id="55ab3-133">Тип</span><span class="sxs-lookup"><span data-stu-id="55ab3-133">Type</span></span>|<span data-ttu-id="55ab3-134">Описание</span><span class="sxs-lookup"><span data-stu-id="55ab3-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55ab3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="55ab3-135">displayName</span></span> | <span data-ttu-id="55ab3-136">String</span><span class="sxs-lookup"><span data-stu-id="55ab3-136">String</span></span>  | <span data-ttu-id="55ab3-137">Имя для сбора данных истории проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="55ab3-137">Name for the access review history data collection.</span></span> <span data-ttu-id="55ab3-138">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="55ab3-138">Required.</span></span> |
|<span data-ttu-id="55ab3-139">reviewHistoryPeriodStartDateTime</span><span class="sxs-lookup"><span data-stu-id="55ab3-139">reviewHistoryPeriodStartDateTime</span></span>  | <span data-ttu-id="55ab3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55ab3-140">DateTimeOffset</span></span>  | <span data-ttu-id="55ab3-141">Timestamp, отзывы, начиная с этой даты или после нее, будут включены в извлеченные данные истории.</span><span class="sxs-lookup"><span data-stu-id="55ab3-141">Timestamp, reviews starting on or after this date will be included in the fetched history data.</span></span> <span data-ttu-id="55ab3-142">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="55ab3-142">Required.</span></span>  |
|<span data-ttu-id="55ab3-143">reviewHistoryPeriodEndDateTime</span><span class="sxs-lookup"><span data-stu-id="55ab3-143">reviewHistoryPeriodEndDateTime</span></span>  | <span data-ttu-id="55ab3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55ab3-144">DateTimeOffset</span></span>  | <span data-ttu-id="55ab3-145">Timestamp, отзывы, начиная с этой даты или до этой даты, будут включены в извлеченные данные истории.</span><span class="sxs-lookup"><span data-stu-id="55ab3-145">Timestamp, reviews starting on or before this date will be included in the fetched history data.</span></span> <span data-ttu-id="55ab3-146">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55ab3-146">Required.</span></span>  |
|<span data-ttu-id="55ab3-147">scopes</span><span class="sxs-lookup"><span data-stu-id="55ab3-147">scopes</span></span>|<span data-ttu-id="55ab3-148">коллекция microsoft.graph.accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="55ab3-148">microsoft.graph.accessReviewQueryScope collection</span></span>| <span data-ttu-id="55ab3-149">Используется для фильтрации отзывов, включенных в извлеченные данные истории.</span><span class="sxs-lookup"><span data-stu-id="55ab3-149">Used to filter which reviews are included in the fetched history data.</span></span> <span data-ttu-id="55ab3-150">Извлекает отзывы, область которых совпадает с этой предоставленной областью.</span><span class="sxs-lookup"><span data-stu-id="55ab3-150">Fetches reviews whose scope matches with this provided scope.</span></span> <span data-ttu-id="55ab3-151">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="55ab3-151">Required.</span></span>  |

### <a name="supported-scope-queries-for-accessreviewhistorydefinition"></a><span data-ttu-id="55ab3-152">Поддерживаемые запросы области для accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="55ab3-152">Supported scope queries for accessReviewHistoryDefinition</span></span>

<span data-ttu-id="55ab3-153">Ниже приводится запросы, поддерживаемые [в accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) на основе [accessreviewqueryscope.](../resources/accessreviewqueryscope.md)</span><span class="sxs-lookup"><span data-stu-id="55ab3-153">The following are queries supported on an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) based on the [accessreviewqueryscope](../resources/accessreviewqueryscope.md).</span></span> <span data-ttu-id="55ab3-154">Эти области диктуют, какой тип данных истории отзывов входит в загружаемый CSV-файл, который создается при создания определения.</span><span class="sxs-lookup"><span data-stu-id="55ab3-154">These scopes dictate which type of review history data is included in the downloadable CSV file which is generated when the definition is created.</span></span>

|<span data-ttu-id="55ab3-155">Сценарий</span><span class="sxs-lookup"><span data-stu-id="55ab3-155">Scenario</span></span>| <span data-ttu-id="55ab3-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="55ab3-156">Query</span></span> |
|--|--|
| <span data-ttu-id="55ab3-157">Включайте каждый результат проверки для отдельных групп (исключает определения, охватываемые для всех Microsoft 365 `accessReviewScheduleDefinition` групп с гостевых пользователей)</span><span class="sxs-lookup"><span data-stu-id="55ab3-157">Include every `accessReviewScheduleDefinition` review result on individual groups (excludes definitions scoped to all Microsoft 365 groups with guest users)</span></span> | <span data-ttu-id="55ab3-158">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')"</span><span class="sxs-lookup"><span data-stu-id="55ab3-158">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')"</span></span> |
| <span data-ttu-id="55ab3-159">Включайте каждый результат проверки в определенную группу (исключает определения, охватываемые для всех Microsoft 365 `accessReviewScheduleDefinition` групп с гостевых пользователей)</span><span class="sxs-lookup"><span data-stu-id="55ab3-159">Include every `accessReviewScheduleDefinition` review result on a specific group (excludes definitions scoped to all Microsoft 365 groups with guest users)</span></span> | <span data-ttu-id="55ab3-160">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups/{group id}')</span><span class="sxs-lookup"><span data-stu-id="55ab3-160">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups/{group id}')</span></span> |
| <span data-ttu-id="55ab3-161">Включайте каждый результат проверки для `accessReviewScheduleDefinition` всех Microsoft 365 групп с гостевых пользователей</span><span class="sxs-lookup"><span data-stu-id="55ab3-161">Include every `accessReviewScheduleDefinition` review result scoped to all Microsoft 365 groups with guest users</span></span> | <span data-ttu-id="55ab3-162">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, './members')</span><span class="sxs-lookup"><span data-stu-id="55ab3-162">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, './members')</span></span> |
| <span data-ttu-id="55ab3-163">`accessReviewScheduleDefinition`Включи каждый результат проверки в пакет доступа</span><span class="sxs-lookup"><span data-stu-id="55ab3-163">Include every `accessReviewScheduleDefinition` review result on an access package</span></span> | <span data-ttu-id="55ab3-164">/identityGovernance/accessReviews/definitions?$filter=contains (scope/query, 'accessPackageAssignments')</span><span class="sxs-lookup"><span data-stu-id="55ab3-164">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')</span></span> |
| <span data-ttu-id="55ab3-165">`accessReviewScheduleDefinition`Включай каждый результат проверки для директоров служб, назначенных привилегированной роли</span><span class="sxs-lookup"><span data-stu-id="55ab3-165">Include every `accessReviewScheduleDefinition` review result for service principals assigned to privileged role</span></span> | <span data-ttu-id="55ab3-166">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'roleAssignmentScheduleInstances')</span><span class="sxs-lookup"><span data-stu-id="55ab3-166">/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'roleAssignmentScheduleInstances')</span></span> |
| <span data-ttu-id="55ab3-167">`accessReviewScheduleDefinition`Включи каждый результат проверки для reivews определенной группы</span><span class="sxs-lookup"><span data-stu-id="55ab3-167">Include every `accessReviewScheduleDefinition` review result for reivews of a specific group</span></span> | <span data-ttu-id="55ab3-168">/identityGovernance/accessReviews/definitions?$filter=scope/query eq '/groups/a1382a9b-8320-4e9c-8f73-dfead37d7723/members'</span><span class="sxs-lookup"><span data-stu-id="55ab3-168">/identityGovernance/accessReviews/definitions?$filter=scope/query eq '/groups/a1382a9b-8320-4e9c-8f73-dfead37d7723/members'</span></span> |

## <a name="response"></a><span data-ttu-id="55ab3-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="55ab3-169">Response</span></span>

<span data-ttu-id="55ab3-170">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="55ab3-170">If successful, this method returns a `201 Created` response code and an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55ab3-171">Примеры</span><span class="sxs-lookup"><span data-stu-id="55ab3-171">Examples</span></span>

<span data-ttu-id="55ab3-172">В следующем примере показано, как создать определение истории доступа для доступа к отзывам по пакетам и группам доступа, которое будет работать между датой начала 01/01/2021 и датой окончания 04/05/2021.</span><span class="sxs-lookup"><span data-stu-id="55ab3-172">The following example shows how to create an access review history definition scoped to access reviews on access packages and groups, running between the start date of 01/01/2021 and end date of 04/05/2021.</span></span>

### <a name="request"></a><span data-ttu-id="55ab3-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="55ab3-173">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="55ab3-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="55ab3-174">Response</span></span>
><span data-ttu-id="55ab3-175">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="55ab3-175">**Note:** The response object shown here might be shortened for readability.</span></span>
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
