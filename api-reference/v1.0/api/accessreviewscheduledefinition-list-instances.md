---
title: Список экземпляров
description: Получите ресурсы accessReviewInstance из свойства навигации экземпляров.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 99c26cb5c6066ca0bc74587a9e2ad24ed6beedb7
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030307"
---
# <a name="list-instances"></a><span data-ttu-id="76f1c-103">экземпляры списков;</span><span class="sxs-lookup"><span data-stu-id="76f1c-103">List instances</span></span>
<span data-ttu-id="76f1c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76f1c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="76f1c-105">Получите [ресурсы accessReviewInstance](../resources/accessreviewinstance.md) из свойства навигации экземпляров в [accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="76f1c-105">Get the [accessReviewInstance](../resources/accessreviewinstance.md) resources from the instances navigation property on an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span>

>[!NOTE]
><span data-ttu-id="76f1c-106">Размер страницы по умолчанию для этого API — 100 объектов accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="76f1c-106">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="76f1c-107">Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов.</span><span class="sxs-lookup"><span data-stu-id="76f1c-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="76f1c-108">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="76f1c-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="76f1c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76f1c-109">Permissions</span></span>
<span data-ttu-id="76f1c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76f1c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76f1c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76f1c-112">Permission type</span></span>|<span data-ttu-id="76f1c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76f1c-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76f1c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76f1c-114">Delegated (work or school account)</span></span>|<span data-ttu-id="76f1c-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76f1c-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="76f1c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76f1c-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76f1c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76f1c-117">Not supported.</span></span>|
|<span data-ttu-id="76f1c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76f1c-118">Application</span></span>|<span data-ttu-id="76f1c-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76f1c-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76f1c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76f1c-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="76f1c-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="76f1c-121">Optional query parameters</span></span>
<span data-ttu-id="76f1c-122">Этот метод поддерживает `$select` `$filter` параметры запроса `$orderBy` `$skip` `$top` OData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="76f1c-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="76f1c-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="76f1c-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="76f1c-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76f1c-124">Request headers</span></span>
|<span data-ttu-id="76f1c-125">Имя</span><span class="sxs-lookup"><span data-stu-id="76f1c-125">Name</span></span>|<span data-ttu-id="76f1c-126">Описание</span><span class="sxs-lookup"><span data-stu-id="76f1c-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="76f1c-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76f1c-127">Authorization</span></span>|<span data-ttu-id="76f1c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76f1c-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="76f1c-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76f1c-130">Request body</span></span>
<span data-ttu-id="76f1c-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="76f1c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76f1c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="76f1c-132">Response</span></span>

<span data-ttu-id="76f1c-133">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов accessReviewInstance](../resources/accessreviewinstance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="76f1c-133">If successful, this method returns a `200 OK` response code and a collection of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="76f1c-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="76f1c-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="76f1c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="76f1c-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_accessreviewinstance"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2dca8959-b716-4b4c-a93d-a535c01eb6e0/instances
```


### <a name="response"></a><span data-ttu-id="76f1c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="76f1c-136">Response</span></span>
><span data-ttu-id="76f1c-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="76f1c-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('2dca8959-b716-4b4c-a93d-a535c01eb6e0')/instances",
    "@odata.count": 1,
    "value": [
        {
            "id": "8d035c9d-798d-47fa-beb4-f986a4b8126f",
            "startDateTime": "2021-05-01T07:00:00Z",
            "endDateTime": "2021-05-15T07:00:00Z",
            "status": "InProgress",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/0914d821-ca3b-45cc-98ee-54c00a04deef/transitiveMembers",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        }
    ]
}
```
