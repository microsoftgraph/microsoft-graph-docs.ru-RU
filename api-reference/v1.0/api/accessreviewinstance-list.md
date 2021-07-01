---
title: Список accessReviewInstances
description: Получите список объектов accessReviewInstance и их свойств.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 60b5ba7e35acfb72f033f90cd37d4fd32c8a3d8b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210579"
---
# <a name="list-accessreviewinstances"></a><span data-ttu-id="8e223-103">Список accessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="8e223-103">List accessReviewInstances</span></span>
<span data-ttu-id="8e223-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e223-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e223-105">Получите список объектов [accessReviewInstance](../resources/accessreviewinstance.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="8e223-105">Get a list of the [accessReviewInstance](../resources/accessreviewinstance.md) objects and their properties.</span></span>

>[!NOTE]
><span data-ttu-id="8e223-106">Размер страницы по умолчанию для этого API — 100 объектов accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="8e223-106">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="8e223-107">Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов.</span><span class="sxs-lookup"><span data-stu-id="8e223-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="8e223-108">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="8e223-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="8e223-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e223-109">Permissions</span></span>
<span data-ttu-id="8e223-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e223-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e223-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e223-112">Permission type</span></span>|<span data-ttu-id="8e223-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e223-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e223-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e223-114">Delegated (work or school account)</span></span>|<span data-ttu-id="8e223-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e223-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="8e223-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e223-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e223-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e223-117">Not supported.</span></span>|
|<span data-ttu-id="8e223-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="8e223-118">Application</span></span>|<span data-ttu-id="8e223-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e223-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e223-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e223-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e223-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8e223-121">Optional query parameters</span></span>
<span data-ttu-id="8e223-122">Этот метод поддерживает `$select` `$filter` параметры запроса `$orderBy` `$skip` `$top` OData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8e223-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="8e223-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8e223-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e223-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e223-124">Request headers</span></span>
|<span data-ttu-id="8e223-125">Имя</span><span class="sxs-lookup"><span data-stu-id="8e223-125">Name</span></span>|<span data-ttu-id="8e223-126">Описание</span><span class="sxs-lookup"><span data-stu-id="8e223-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8e223-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e223-127">Authorization</span></span>|<span data-ttu-id="8e223-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e223-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e223-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e223-130">Request body</span></span>
<span data-ttu-id="8e223-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e223-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e223-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e223-132">Response</span></span>

<span data-ttu-id="8e223-133">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов accessReviewInstance](../resources/accessreviewinstance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8e223-133">If successful, this method returns a `200 OK` response code and a collection of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8e223-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="8e223-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8e223-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e223-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8e223-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e223-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessreviewinstance"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances
```
# <a name="c"></a>[<span data-ttu-id="8e223-137">C#</span><span class="sxs-lookup"><span data-stu-id="8e223-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e223-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e223-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e223-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e223-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e223-140">Java</span><span class="sxs-lookup"><span data-stu-id="8e223-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8e223-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e223-141">Response</span></span>
><span data-ttu-id="8e223-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8e223-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('8564a649-4f67-4e09-88e7-55def6530e88')/instances",
    "@odata.count": 2,
    "value": [
        {
            "id": "7bc18cf4-3d70-4009-bc8e-a7c5adb30849",
            "startDateTime": "2021-03-09T23:10:28.83Z",
            "endDateTime": "2021-03-09T23:10:28.83Z",
            "status": "Applied",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/f661fdd0-f0f7-42c0-8281-e89c6527ac63/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        }
    ]
}
```
