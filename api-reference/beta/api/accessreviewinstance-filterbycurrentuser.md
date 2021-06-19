---
title: 'accessReviewInstance: filterByCurrentUser'
description: Возвращает все объекты accessReviewInstance для данного рецензента.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: db6de64071645fe97d5fffa4e3968ea63db5578e
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031507"
---
# <a name="accessreviewinstance-filterbycurrentuser"></a><span data-ttu-id="c9faf-103">accessReviewInstance: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="c9faf-103">accessReviewInstance: filterByCurrentUser</span></span>
<span data-ttu-id="c9faf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9faf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9faf-105">Возвращает все объекты [accessReviewInstance](../resources/accessreviewinstance.md) в заданном [accessReviewScheduleDefinition,](../resources/accessreviewscheduledefinition.md) где пользователь вызовов является рецензентом на одном или более [объектах accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="c9faf-105">Returns all [accessReviewInstance](../resources/accessreviewinstance.md) objects on a given [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) where the calling user is a reviewer on one or more [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects.</span></span>

>[!NOTE]
><span data-ttu-id="c9faf-106">Размер страницы по умолчанию для этого API — 100 объектов accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="c9faf-106">The default page size for this API is 100 accessReviewInstance objects.</span></span> <span data-ttu-id="c9faf-107">Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов.</span><span class="sxs-lookup"><span data-stu-id="c9faf-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="c9faf-108">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="c9faf-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="c9faf-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9faf-109">Permissions</span></span>
<span data-ttu-id="c9faf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9faf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9faf-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9faf-112">Permission type</span></span>|<span data-ttu-id="c9faf-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9faf-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9faf-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9faf-114">Delegated (work or school account)</span></span>|<span data-ttu-id="c9faf-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9faf-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="c9faf-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9faf-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9faf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9faf-117">Not supported.</span></span>|
|<span data-ttu-id="c9faf-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="c9faf-118">Application</span></span>|<span data-ttu-id="c9faf-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9faf-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9faf-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9faf-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/filterByCurrentUser(on='reviewer')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9faf-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c9faf-121">Optional query parameters</span></span>
<span data-ttu-id="c9faf-122">Этот метод поддерживает `$select` параметры `$filter` запроса `$orderBy` `$skip` OData и для настройки `$top` ответа.</span><span class="sxs-lookup"><span data-stu-id="c9faf-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="c9faf-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c9faf-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9faf-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9faf-124">Request headers</span></span>
|<span data-ttu-id="c9faf-125">Имя</span><span class="sxs-lookup"><span data-stu-id="c9faf-125">Name</span></span>|<span data-ttu-id="c9faf-126">Описание</span><span class="sxs-lookup"><span data-stu-id="c9faf-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c9faf-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9faf-127">Authorization</span></span>|<span data-ttu-id="c9faf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9faf-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9faf-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9faf-130">Request body</span></span>
<span data-ttu-id="c9faf-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9faf-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9faf-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9faf-132">Response</span></span>

<span data-ttu-id="c9faf-133">В случае успешной работы эта функция возвращает код отклика и `200 OK` [коллекцию accessReviewInstance](../resources/accessreviewinstance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c9faf-133">If successful, this function returns a `200 OK` response code and a [accessReviewInstance](../resources/accessreviewinstance.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c9faf-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="c9faf-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c9faf-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9faf-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/08531375-eff6-4e21-b1a8-de0eb37ec913/instances/filterByCurrentUser(on='reviewer')
```

### <a name="response"></a><span data-ttu-id="c9faf-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9faf-136">Response</span></span>
><span data-ttu-id="c9faf-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c9faf-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(accessReviewInstance)",
    "@odata.count": 2,
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
        },
        {
            "@odata.type": "#microsoft.graph.accessReviewInstance",
            "id": "00ef5dba-4a32-48b3-b18a-57b244c0c4ba",
            "startDateTime": "2021-04-13T00:45:51.627Z",
            "endDateTime": "2021-04-16T00:45:51.627Z",
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
