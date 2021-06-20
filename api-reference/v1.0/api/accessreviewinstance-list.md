---
title: Список accessReviewInstances
description: Получите список объектов accessReviewInstance и их свойств.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 01a52e1b597971d887b763076913e8db0c70abc7
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031315"
---
# <a name="list-accessreviewinstances"></a><span data-ttu-id="dadb9-103">Список accessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="dadb9-103">List accessReviewInstances</span></span>
<span data-ttu-id="dadb9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dadb9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dadb9-105">Получите список объектов [accessReviewInstance](../resources/accessreviewinstance.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="dadb9-105">Get a list of the [accessReviewInstance](../resources/accessreviewinstance.md) objects and their properties.</span></span>

>[!NOTE]
><span data-ttu-id="dadb9-106">Размер страницы по умолчанию для этого API — 100 объектов accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="dadb9-106">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="dadb9-107">Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов.</span><span class="sxs-lookup"><span data-stu-id="dadb9-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="dadb9-108">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="dadb9-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="dadb9-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dadb9-109">Permissions</span></span>
<span data-ttu-id="dadb9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dadb9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dadb9-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dadb9-112">Permission type</span></span>|<span data-ttu-id="dadb9-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dadb9-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dadb9-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dadb9-114">Delegated (work or school account)</span></span>|<span data-ttu-id="dadb9-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dadb9-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="dadb9-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dadb9-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dadb9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dadb9-117">Not supported.</span></span>|
|<span data-ttu-id="dadb9-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dadb9-118">Application</span></span>|<span data-ttu-id="dadb9-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dadb9-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dadb9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dadb9-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dadb9-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dadb9-121">Optional query parameters</span></span>
<span data-ttu-id="dadb9-122">Этот метод поддерживает `$select` `$filter` параметры запроса `$orderBy` `$skip` `$top` OData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dadb9-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="dadb9-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="dadb9-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="dadb9-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dadb9-124">Request headers</span></span>
|<span data-ttu-id="dadb9-125">Имя</span><span class="sxs-lookup"><span data-stu-id="dadb9-125">Name</span></span>|<span data-ttu-id="dadb9-126">Описание</span><span class="sxs-lookup"><span data-stu-id="dadb9-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dadb9-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dadb9-127">Authorization</span></span>|<span data-ttu-id="dadb9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dadb9-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dadb9-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dadb9-130">Request body</span></span>
<span data-ttu-id="dadb9-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dadb9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dadb9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="dadb9-132">Response</span></span>

<span data-ttu-id="dadb9-133">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов accessReviewInstance](../resources/accessreviewinstance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dadb9-133">If successful, this method returns a `200 OK` response code and a collection of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dadb9-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="dadb9-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dadb9-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="dadb9-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_accessreviewinstance"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances
```


### <a name="response"></a><span data-ttu-id="dadb9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="dadb9-136">Response</span></span>
><span data-ttu-id="dadb9-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dadb9-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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
