---
title: 'accessReviewInstanceDecisionItem: filterByCurrentUser'
description: Извлекает все объекты accessReviewInstanceDecisionItem в accessReviewInstance, для которых вызываемая пользователь является рецензентом.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 63c77f98082169def1758bc73ec20dbec3377855
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031346"
---
# <a name="accessreviewinstancedecisionitem-filterbycurrentuser"></a><span data-ttu-id="35169-103">accessReviewInstanceDecisionItem: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="35169-103">accessReviewInstanceDecisionItem: filterByCurrentUser</span></span>
<span data-ttu-id="35169-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35169-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35169-105">Извлекает все [объекты accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) на заданном [accessReviewInstance,](../resources/accessreviewinstance.md) для которого вызываемая пользователь является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="35169-105">Retrieves all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects on a given [accessReviewInstance](../resources/accessreviewinstance.md) for which the calling user is the reviewer.</span></span>

>[!NOTE]
><span data-ttu-id="35169-106">Размер страницы по умолчанию для этого API — 100 объектов accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="35169-106">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="35169-107">Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов.</span><span class="sxs-lookup"><span data-stu-id="35169-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="35169-108">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="35169-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="35169-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35169-109">Permissions</span></span>
<span data-ttu-id="35169-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35169-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35169-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35169-112">Permission type</span></span>|<span data-ttu-id="35169-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35169-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35169-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35169-114">Delegated (work or school account)</span></span>|<span data-ttu-id="35169-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35169-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="35169-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35169-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35169-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35169-117">Not supported.</span></span>|
|<span data-ttu-id="35169-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35169-118">Application</span></span>|<span data-ttu-id="35169-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35169-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35169-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35169-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/filterByCurrentUser(on='reviewer')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="35169-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="35169-121">Optional query parameters</span></span>
<span data-ttu-id="35169-122">Этот метод поддерживает `$select` `$filter` параметры запроса `$orderBy` `$skip` `$top` OData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="35169-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="35169-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="35169-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="35169-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35169-124">Request headers</span></span>
|<span data-ttu-id="35169-125">Имя</span><span class="sxs-lookup"><span data-stu-id="35169-125">Name</span></span>|<span data-ttu-id="35169-126">Описание</span><span class="sxs-lookup"><span data-stu-id="35169-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="35169-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35169-127">Authorization</span></span>|<span data-ttu-id="35169-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35169-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="35169-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35169-130">Request body</span></span>
<span data-ttu-id="35169-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35169-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35169-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="35169-132">Response</span></span>

<span data-ttu-id="35169-133">В случае успешной работы эта функция возвращает код ответа и `200 OK` [коллекцию accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="35169-133">If successful, this function returns a `200 OK` response code and a [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="35169-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="35169-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="35169-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="35169-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstancedecisionitem_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/1234ea1c-8d12-457b-1234-a37dc59e54e0/instances/7070ea1c-8d12-457b-bd35-a37dc59e54e0/decisions/filterByCurrentUser(on='reviewer')
```


### <a name="response"></a><span data-ttu-id="35169-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="35169-136">Response</span></span>
><span data-ttu-id="35169-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="35169-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(accessReviewInstanceDecisionItem)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItem",
            "id": "9550e25b-f315-4454-9d87-16b885c35de4",
            "accessReviewId": "7070ea1c-8d12-457b-bd35-a37dc59e54e0",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "principalLink": "https://graph.microsoft.com/v1.0/users/55555b2c-955d-4205-8471-3a6c3116435d",
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
