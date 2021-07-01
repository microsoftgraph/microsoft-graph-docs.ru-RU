---
title: 'accessReviewInstance: filterByCurrentUser'
description: Извлечение всех объектов accessReviewInstance для данного рецензента.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6d32cf12ed95c34cc82dd40a05e928f4069c1f51
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209852"
---
# <a name="accessreviewinstance-filterbycurrentuser"></a><span data-ttu-id="fb1b5-103">accessReviewInstance: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="fb1b5-103">accessReviewInstance: filterByCurrentUser</span></span>
<span data-ttu-id="fb1b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb1b5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fb1b5-105">Извлекайте все объекты [accessReviewInstance](../resources/accessreviewinstance.md) в заданном [accessReviewScheduleDefinition,](../resources/accessreviewscheduledefinition.md) где пользователь вызовов является рецензентом на одном или более [объектах accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="fb1b5-105">Retrieve all [accessReviewInstance](../resources/accessreviewinstance.md) objects on a given [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) where the calling user is a reviewer on one or more [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects.</span></span>

>[!NOTE]
><span data-ttu-id="fb1b5-106">Размер страницы по умолчанию для этого API — 100 объектов accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="fb1b5-106">The default page size for this API is 100 accessReviewInstance objects.</span></span> <span data-ttu-id="fb1b5-107">Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов.</span><span class="sxs-lookup"><span data-stu-id="fb1b5-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="fb1b5-108">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="fb1b5-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="fb1b5-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb1b5-109">Permissions</span></span>
<span data-ttu-id="fb1b5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb1b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb1b5-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb1b5-112">Permission type</span></span>|<span data-ttu-id="fb1b5-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb1b5-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb1b5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb1b5-114">Delegated (work or school account)</span></span>|<span data-ttu-id="fb1b5-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb1b5-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="fb1b5-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb1b5-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb1b5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb1b5-117">Not supported.</span></span>|
|<span data-ttu-id="fb1b5-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="fb1b5-118">Application</span></span>|<span data-ttu-id="fb1b5-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb1b5-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb1b5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb1b5-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/filterByCurrentUser(on='reviewer')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb1b5-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fb1b5-121">Optional query parameters</span></span>
<span data-ttu-id="fb1b5-122">Этот метод поддерживает `$select` `$filter` параметры запроса `$orderBy` `$skip` `$top` OData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fb1b5-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="fb1b5-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fb1b5-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb1b5-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb1b5-124">Request headers</span></span>
|<span data-ttu-id="fb1b5-125">Имя</span><span class="sxs-lookup"><span data-stu-id="fb1b5-125">Name</span></span>|<span data-ttu-id="fb1b5-126">Описание</span><span class="sxs-lookup"><span data-stu-id="fb1b5-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fb1b5-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb1b5-127">Authorization</span></span>|<span data-ttu-id="fb1b5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb1b5-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb1b5-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb1b5-130">Request body</span></span>
<span data-ttu-id="fb1b5-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb1b5-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb1b5-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb1b5-132">Response</span></span>

<span data-ttu-id="fb1b5-133">В случае успешной работы эта функция возвращает код отклика и `200 OK` [коллекцию accessReviewInstance](../resources/accessreviewinstance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fb1b5-133">If successful, this function returns a `200 OK` response code and a [accessReviewInstance](../resources/accessreviewinstance.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fb1b5-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="fb1b5-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fb1b5-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb1b5-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fb1b5-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb1b5-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/filterByCurrentUser(on='reviewer')
```
# <a name="c"></a>[<span data-ttu-id="fb1b5-137">C#</span><span class="sxs-lookup"><span data-stu-id="fb1b5-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb1b5-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb1b5-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb1b5-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb1b5-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb1b5-140">Java</span><span class="sxs-lookup"><span data-stu-id="fb1b5-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="fb1b5-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb1b5-141">Response</span></span>
><span data-ttu-id="fb1b5-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fb1b5-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewInstance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(accessReviewInstance)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInstance",
            "id": "7ca879f0-77ea-4386-b110-776dec898935",
            "startDateTime": "2021-04-20T00:45:51.627Z",
            "endDateTime": "2021-04-23T00:45:51.627Z",
            "status": "Applied",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/6b7b9930-38a0-4f93-a107-3bc9904c83d7/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        }
    ]
}
```
