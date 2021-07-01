---
title: 'accessReviewScheduleDefinition: filterByCurrentUser'
description: Возвращает объекты accessReviewScheduleDefinition, в которых вызываемая пользователь является рецензентом.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2185e064dcd39049e90063dbcbe1100f9da36344
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209605"
---
# <a name="accessreviewscheduledefinition-filterbycurrentuser"></a><span data-ttu-id="64b06-103">accessReviewScheduleDefinition: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="64b06-103">accessReviewScheduleDefinition: filterByCurrentUser</span></span>
<span data-ttu-id="64b06-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64b06-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64b06-105">Возвращает [объекты accessReviewScheduleDefinition,](../resources/accessreviewscheduledefinition.md) в которых вызываемая пользователь является рецензентом на одном или более [объектах accessReviewInstance.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="64b06-105">Returns [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects where the calling user is a reviewer on one or more [accessReviewInstance](../resources/accessreviewinstance.md) objects.</span></span>

>[!NOTE]
><span data-ttu-id="64b06-106">Размер страницы по умолчанию для этого API — 100 объектов accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="64b06-106">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="64b06-107">Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов.</span><span class="sxs-lookup"><span data-stu-id="64b06-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="64b06-108">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="64b06-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="64b06-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64b06-109">Permissions</span></span>
<span data-ttu-id="64b06-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64b06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64b06-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64b06-112">Permission type</span></span>|<span data-ttu-id="64b06-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64b06-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64b06-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64b06-114">Delegated (work or school account)</span></span>|<span data-ttu-id="64b06-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64b06-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="64b06-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64b06-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64b06-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64b06-117">Not supported.</span></span>|
|<span data-ttu-id="64b06-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="64b06-118">Application</span></span>|<span data-ttu-id="64b06-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64b06-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64b06-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64b06-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/filterByCurrentUser(on='reviewer')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64b06-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="64b06-121">Optional query parameters</span></span>
<span data-ttu-id="64b06-122">Этот метод поддерживает `$select` `$filter` параметры запроса `$orderBy` `$skip` `$top` OData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="64b06-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="64b06-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="64b06-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="64b06-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64b06-124">Request headers</span></span>
|<span data-ttu-id="64b06-125">Имя</span><span class="sxs-lookup"><span data-stu-id="64b06-125">Name</span></span>|<span data-ttu-id="64b06-126">Описание</span><span class="sxs-lookup"><span data-stu-id="64b06-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="64b06-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64b06-127">Authorization</span></span>|<span data-ttu-id="64b06-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64b06-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64b06-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64b06-130">Request body</span></span>
<span data-ttu-id="64b06-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64b06-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64b06-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="64b06-132">Response</span></span>

<span data-ttu-id="64b06-133">В случае успешной работы эта функция возвращает код отклика и `200 OK` [коллекцию accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="64b06-133">If successful, this function returns a `200 OK` response code and a [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64b06-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="64b06-134">Examples</span></span>
<span data-ttu-id="64b06-135">Возвращает все определения обзора, в которых вызываемая пользователь является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="64b06-135">Returns all review definitions where the calling user is a reviewer.</span></span>

### <a name="request"></a><span data-ttu-id="64b06-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="64b06-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="64b06-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="64b06-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewscheduledefinition_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/filterByCurrentUser(on='reviewer')
```
# <a name="c"></a>[<span data-ttu-id="64b06-138">C#</span><span class="sxs-lookup"><span data-stu-id="64b06-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewscheduledefinition-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64b06-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64b06-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewscheduledefinition-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64b06-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64b06-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewscheduledefinition-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64b06-141">Java</span><span class="sxs-lookup"><span data-stu-id="64b06-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewscheduledefinition-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="64b06-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="64b06-142">Response</span></span>
><span data-ttu-id="64b06-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="64b06-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewScheduleDefinition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(accessReviewScheduleDefinition)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewScheduleDefinition",
            "id": "66666337-b075-4a92-9d71-255cc4b5d12a",
            "displayName": "All groups review",
            "createdDateTime": "2021-03-09T00:45:51.6272836Z",
            "lastModifiedDateTime": "2021-03-09T00:46:11.2041753Z",
            "status": "InProgress",
            "descriptionForAdmins": "All groups review",
            "descriptionForReviewers": "",
            "createdBy": {
                "id": "cae33dff-88e8-4e02-8a52-de021295997e",
                "displayName": "Example user",
                "userPrincipalName": "exampleuser@contoso.com"
            },
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            },
            "instanceEnumerationScope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            },
            "reviewers": [
                {
                    "query": "./owners",
                    "queryType": "MicrosoftGraph",
                    "queryRoot": null
                }
            ],
            "fallbackReviewers": [],
            "settings": {
                "mailNotificationsEnabled": true,
                "reminderNotificationsEnabled": true,
                "justificationRequiredOnApproval": true,
                "defaultDecisionEnabled": false,
                "defaultDecision": "None",
                "instanceDurationInDays": 3,
                "autoApplyDecisionsEnabled": true,
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
                        "startDate": "2021-03-09",
                        "endDate": "9999-12-31"
                    }
                },
                "applyActions": [
                    {
                        "@odata.type": "#microsoft.graph.removeAccessApplyAction"
                    }
                ]
            },
            "instances": []
        }
    ]
}
```
