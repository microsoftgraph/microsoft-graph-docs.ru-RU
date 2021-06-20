---
title: List accessReviewInstanceDecisionItems
description: Получите список объектов accessReviewInstanceDecisionItem и их свойств.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1ffc4738de0cbef15aa9c440f9e1f80045df01bc
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031286"
---
# <a name="list-accessreviewinstancedecisionitems"></a><span data-ttu-id="474cd-103">List accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="474cd-103">List accessReviewInstanceDecisionItems</span></span>
<span data-ttu-id="474cd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="474cd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="474cd-105">Получите список объектов [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="474cd-105">Get a list of the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects and their properties.</span></span>

>[!NOTE]
><span data-ttu-id="474cd-106">Размер страницы по умолчанию для этого API — 100 объектов accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="474cd-106">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="474cd-107">Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов.</span><span class="sxs-lookup"><span data-stu-id="474cd-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="474cd-108">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="474cd-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="474cd-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="474cd-109">Permissions</span></span>
<span data-ttu-id="474cd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="474cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="474cd-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="474cd-112">Permission type</span></span>|<span data-ttu-id="474cd-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="474cd-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="474cd-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="474cd-114">Delegated (work or school account)</span></span>|<span data-ttu-id="474cd-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="474cd-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="474cd-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="474cd-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="474cd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="474cd-117">Not supported.</span></span>|
|<span data-ttu-id="474cd-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="474cd-118">Application</span></span>|<span data-ttu-id="474cd-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="474cd-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="474cd-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="474cd-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="474cd-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="474cd-121">Optional query parameters</span></span>
<span data-ttu-id="474cd-122">Этот метод поддерживает `$select` `$filter` параметры запроса `$orderBy` `$skip` `$top` OData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="474cd-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="474cd-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="474cd-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="474cd-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="474cd-124">Request headers</span></span>
|<span data-ttu-id="474cd-125">Имя</span><span class="sxs-lookup"><span data-stu-id="474cd-125">Name</span></span>|<span data-ttu-id="474cd-126">Описание</span><span class="sxs-lookup"><span data-stu-id="474cd-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="474cd-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="474cd-127">Authorization</span></span>|<span data-ttu-id="474cd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="474cd-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="474cd-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="474cd-130">Request body</span></span>
<span data-ttu-id="474cd-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="474cd-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="474cd-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="474cd-132">Response</span></span>

<span data-ttu-id="474cd-133">В случае успеха этот метод возвращает код отклика и коллекцию `200 OK` [объектов accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="474cd-133">If successful, this method returns a `200 OK` response code and a collection of [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="474cd-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="474cd-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="474cd-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="474cd-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/instances/7070ea1c-8d12-457b-bd35-a37dc59e54e0/decisions
```


### <a name="response"></a><span data-ttu-id="474cd-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="474cd-136">Response</span></span>
><span data-ttu-id="474cd-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="474cd-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewInstanceDecisionItem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd')/instances('7070ea1c-8d12-457b-bd35-a37dc59e54e0')/decisions",
    "@odata.count": 1,
    "value": [
        {
            "id": "9550e25b-f315-4454-9d87-16b885c35de4",
            "accessReviewId": "7070ea1c-8d12-457b-bd35-a37dc59e54e0",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "principalLink": "https://graph.microsoft.com/v1.0/users/1800bb2c-955d-4205-8471-3a6c3116435d",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "1800bb2c-955d-4205-8471-3a6c3116435d",
                "userDisplayName": "guest example",
                "userPrincipalName": "guest@guest.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "1800bb2c-955d-4205-8471-3a6c3116435d",
                "displayName": "guest example",
                "userPrincipalName": "guest@guest.com"
            }
        }
    ]
}
```
