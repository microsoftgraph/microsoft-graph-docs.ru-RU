---
title: Создание accessReviewHistoryDefinition
description: Создайте новый объект accessReviewHistoryDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f266276fae151bd8cc31455c4fd69eab193dd440
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629233"
---
# <a name="create-accessreviewhistorydefinition"></a><span data-ttu-id="eec21-103">Создание accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="eec21-103">Create accessReviewHistoryDefinition</span></span>

<span data-ttu-id="eec21-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eec21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eec21-105">Создайте новый [объект accessReviewHistoryDefinition.](../resources/accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="eec21-105">Create a new [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eec21-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eec21-106">Permissions</span></span>

<span data-ttu-id="eec21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eec21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eec21-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eec21-109">Permission type</span></span>|<span data-ttu-id="eec21-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eec21-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eec21-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eec21-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eec21-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eec21-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="eec21-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eec21-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eec21-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eec21-114">Not supported.</span></span>|
|<span data-ttu-id="eec21-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="eec21-115">Application</span></span>|<span data-ttu-id="eec21-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eec21-116">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="eec21-117">В роли каталога должен также быть подписан пользователь, который позволяет им читать обзор доступа для получения любых данных.</span><span class="sxs-lookup"><span data-stu-id="eec21-117">The signed-in user must also be in a directory role that permits them to read an access review to retrieve any data.</span></span>  <span data-ttu-id="eec21-118">Дополнительные сведения см. в дополнительных сведениях о требованиях к роли и разрешению для [отзывов о доступе.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="eec21-118">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="eec21-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eec21-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/historyDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="eec21-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eec21-120">Request headers</span></span>

|<span data-ttu-id="eec21-121">Имя</span><span class="sxs-lookup"><span data-stu-id="eec21-121">Name</span></span>|<span data-ttu-id="eec21-122">Описание</span><span class="sxs-lookup"><span data-stu-id="eec21-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eec21-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eec21-123">Authorization</span></span>|<span data-ttu-id="eec21-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eec21-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="eec21-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eec21-126">Content-Type</span></span>|<span data-ttu-id="eec21-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eec21-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eec21-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eec21-129">Request body</span></span>

<span data-ttu-id="eec21-130">В теле запроса поставляют представление JSON объекта [accessReviewHistoryDefinition.](../resources/accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="eec21-130">In the request body, supply a JSON representation of the [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object.</span></span>

<span data-ttu-id="eec21-131">В следующей таблице показаны необходимые свойства, используемые для создания [accessReviewHistoryDefinition.](../resources/accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="eec21-131">The following table shows the required properties used to create an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md).</span></span>

|<span data-ttu-id="eec21-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="eec21-132">Property</span></span>|<span data-ttu-id="eec21-133">Тип</span><span class="sxs-lookup"><span data-stu-id="eec21-133">Type</span></span>|<span data-ttu-id="eec21-134">Описание</span><span class="sxs-lookup"><span data-stu-id="eec21-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eec21-135">displayName</span><span class="sxs-lookup"><span data-stu-id="eec21-135">displayName</span></span> | <span data-ttu-id="eec21-136">Строка</span><span class="sxs-lookup"><span data-stu-id="eec21-136">String</span></span>  | <span data-ttu-id="eec21-137">Имя для сбора данных истории проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="eec21-137">Name for the access review history data collection.</span></span> <span data-ttu-id="eec21-138">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="eec21-138">Required.</span></span> |
|<span data-ttu-id="eec21-139">reviewHistoryPeriodStartDateTime</span><span class="sxs-lookup"><span data-stu-id="eec21-139">reviewHistoryPeriodStartDateTime</span></span>  | <span data-ttu-id="eec21-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eec21-140">DateTimeOffset</span></span>  | <span data-ttu-id="eec21-141">Timestamp, отзывы, начиная с этой даты или после нее, будут включены в извлеченные данные истории.</span><span class="sxs-lookup"><span data-stu-id="eec21-141">Timestamp, reviews starting on or after this date will be included in the fetched history data.</span></span> <span data-ttu-id="eec21-142">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="eec21-142">Required.</span></span>  |
|<span data-ttu-id="eec21-143">reviewHistoryPeriodEndDateTime</span><span class="sxs-lookup"><span data-stu-id="eec21-143">reviewHistoryPeriodEndDateTime</span></span>  | <span data-ttu-id="eec21-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eec21-144">DateTimeOffset</span></span>  | <span data-ttu-id="eec21-145">Timestamp, отзывы, начиная с этой даты или до этой даты, будут включены в извлеченные данные истории.</span><span class="sxs-lookup"><span data-stu-id="eec21-145">Timestamp, reviews starting on or before this date will be included in the fetched history data.</span></span> <span data-ttu-id="eec21-146">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eec21-146">Required.</span></span>  |
|<span data-ttu-id="eec21-147">scopes</span><span class="sxs-lookup"><span data-stu-id="eec21-147">scopes</span></span>|<span data-ttu-id="eec21-148">[accessReviewQueryScope](../resources/accessreviewqueryscope.md) collection</span><span class="sxs-lookup"><span data-stu-id="eec21-148">[accessReviewQueryScope](../resources/accessreviewqueryscope.md) collection</span></span>| <span data-ttu-id="eec21-149">Используется для фильтрации отзывов, включенных в извлеченные данные истории.</span><span class="sxs-lookup"><span data-stu-id="eec21-149">Used to filter which reviews are included in the fetched history data.</span></span> <span data-ttu-id="eec21-150">Извлекает отзывы, область которых совпадает с этой предоставленной областью.</span><span class="sxs-lookup"><span data-stu-id="eec21-150">Fetches reviews whose scope matches with this provided scope.</span></span> <span data-ttu-id="eec21-151">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="eec21-151">Required.</span></span> <br> <span data-ttu-id="eec21-152">Дополнительные возможности [см. в разделах Поддерживаемые запросы области для accessReviewHistoryDefinition.](#supported-scope-queries-for-accessreviewhistorydefinition)</span><span class="sxs-lookup"><span data-stu-id="eec21-152">For more, see [Supported scope queries for accessReviewHistoryDefinition](#supported-scope-queries-for-accessreviewhistorydefinition).</span></span> |

### <a name="supported-scope-queries-for-accessreviewhistorydefinition"></a><span data-ttu-id="eec21-153">Поддерживаемые запросы области для accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="eec21-153">Supported scope queries for accessReviewHistoryDefinition</span></span>

<span data-ttu-id="eec21-154">Свойство **областей** [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) основано на **accessReviewQueryScope**, ресурсе, который позволяет настраивать различные ресурсы в свойстве **запроса.**</span><span class="sxs-lookup"><span data-stu-id="eec21-154">The **scopes** property of [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) is based on **accessReviewQueryScope**, a resource that allows you to configure different resources in it's **query** property.</span></span> <span data-ttu-id="eec21-155">Эти ресурсы затем представляют область определения истории и диктуют тип данных истории отзывов, которые включаются в загружаемый CSV-файл, который создается при создания определения истории.</span><span class="sxs-lookup"><span data-stu-id="eec21-155">These resources then represent the scope of the history definition and dictate the type of review history data that is included in the downloadable CSV file which is generated when the history definition is created.</span></span>

<span data-ttu-id="eec21-156">Используйте следующий формат для свойства **запроса:**</span><span class="sxs-lookup"><span data-stu-id="eec21-156">Use the following format for the **query** property:</span></span>

```http
/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '{object}')
```

<span data-ttu-id="eec21-157">Значение является одним из ресурсов, которые `{object}` можно настроить в **accessReviewScheduleDefinition**.</span><span class="sxs-lookup"><span data-stu-id="eec21-157">The value of `{object}` is one of the resources that can be configured in an **accessReviewScheduleDefinition**.</span></span> <span data-ttu-id="eec21-158">Например, ниже приводится каждый результат проверки accessReviewScheduleDefinition для отдельных групп (и исключает определения, охватив все группы Microsoft 365 с гостевых пользователей).</span><span class="sxs-lookup"><span data-stu-id="eec21-158">For example, the following includes every accessReviewScheduleDefinition review result on individual groups (and excludes definitions scoped to all Microsoft 365 groups with guest users).</span></span>

```http
/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')
```

<span data-ttu-id="eec21-159">Дополнительные поддерживаемые значения см. в $filter [параметре запроса accessReviewScheduleDefinition.](accessreviewscheduledefinition-list.md#use-the-filter-query-parameter)</span><span class="sxs-lookup"><span data-stu-id="eec21-159">For more supported values, see Use the [$filter query parameter on accessReviewScheduleDefinition](accessreviewscheduledefinition-list.md#use-the-filter-query-parameter).</span></span>

## <a name="response"></a><span data-ttu-id="eec21-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="eec21-160">Response</span></span>

<span data-ttu-id="eec21-161">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="eec21-161">If successful, this method returns a `201 Created` response code and an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eec21-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="eec21-162">Examples</span></span>

<span data-ttu-id="eec21-163">В следующем примере показано, как создать определение истории доступа для доступа к отзывам по пакетам и группам доступа, которое будет работать между датой начала 01/01/2021 и датой окончания 04/05/2021.</span><span class="sxs-lookup"><span data-stu-id="eec21-163">The following example shows how to create an access review history definition scoped to access reviews on access packages and groups, running between the start date of 01/01/2021 and end date of 04/05/2021.</span></span>

### <a name="request"></a><span data-ttu-id="eec21-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="eec21-164">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="eec21-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="eec21-165">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="eec21-166">C#</span><span class="sxs-lookup"><span data-stu-id="eec21-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewhistorydefinition-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eec21-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eec21-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewhistorydefinition-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eec21-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eec21-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewhistorydefinition-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eec21-169">Java</span><span class="sxs-lookup"><span data-stu-id="eec21-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewhistorydefinition-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="eec21-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="eec21-170">Response</span></span>
><span data-ttu-id="eec21-171">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="eec21-171">**Note:** The response object shown here might be shortened for readability.</span></span>
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
