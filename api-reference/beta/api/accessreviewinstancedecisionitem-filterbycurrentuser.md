---
title: 'accessReviewInstanceDecisionItem: filterByCurrentUser'
description: Извлекает все объекты accessReviewInstanceDecisionItem в accessReviewInstance, для которых вызываемая пользователь является рецензентом.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f4f045ac67e1b98179f64a5a09102c975a2f0374
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031498"
---
# <a name="accessreviewinstancedecisionitem-filterbycurrentuser"></a><span data-ttu-id="f2c70-103">accessReviewInstanceDecisionItem: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="f2c70-103">accessReviewInstanceDecisionItem: filterByCurrentUser</span></span>
<span data-ttu-id="f2c70-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2c70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2c70-105">Извлекает все [объекты accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) на заданном [accessReviewInstance,](../resources/accessreviewinstance.md) для которого вызываемая пользователь является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="f2c70-105">Retrieves all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects on a given [accessReviewInstance](../resources/accessreviewinstance.md) for which the calling user is the reviewer.</span></span>

>[!NOTE]
><span data-ttu-id="f2c70-106">Размер страницы по умолчанию для этого API — 100 объектов accessReviewInstanceDecisionItem.</span><span class="sxs-lookup"><span data-stu-id="f2c70-106">The default page size for this API is 100 accessReviewInstanceDecisionItem objects.</span></span> <span data-ttu-id="f2c70-107">Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов.</span><span class="sxs-lookup"><span data-stu-id="f2c70-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="f2c70-108">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="f2c70-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="f2c70-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2c70-109">Permissions</span></span>
<span data-ttu-id="f2c70-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2c70-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2c70-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2c70-112">Permission type</span></span>|<span data-ttu-id="f2c70-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2c70-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2c70-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2c70-114">Delegated (work or school account)</span></span>|<span data-ttu-id="f2c70-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2c70-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="f2c70-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2c70-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2c70-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2c70-117">Not supported.</span></span>|
|<span data-ttu-id="f2c70-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="f2c70-118">Application</span></span>|<span data-ttu-id="f2c70-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2c70-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2c70-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2c70-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/filterByCurrentUser(on='reviewer')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2c70-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f2c70-121">Optional query parameters</span></span>
<span data-ttu-id="f2c70-122">Этот метод поддерживает `$select` `$filter` параметры запроса `$orderBy` `$skip` `$top` OData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f2c70-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="f2c70-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f2c70-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2c70-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2c70-124">Request headers</span></span>
|<span data-ttu-id="f2c70-125">Имя</span><span class="sxs-lookup"><span data-stu-id="f2c70-125">Name</span></span>|<span data-ttu-id="f2c70-126">Описание</span><span class="sxs-lookup"><span data-stu-id="f2c70-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f2c70-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2c70-127">Authorization</span></span>|<span data-ttu-id="f2c70-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2c70-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2c70-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2c70-130">Request body</span></span>
<span data-ttu-id="f2c70-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2c70-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2c70-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2c70-132">Response</span></span>

<span data-ttu-id="f2c70-133">В случае успешной работы эта функция возвращает код ответа и `200 OK` [коллекцию accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f2c70-133">If successful, this function returns a `200 OK` response code and a [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2c70-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="f2c70-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2c70-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2c70-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstancedecisionitem_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/0185aab8-9a7e-44b5-ae36-41b923c3bf87/instances/1234aab8-9a7e-5678-ae36-41b923c3bf87/decisions/filterByCurrentUser(on='reviewer')
```


### <a name="response"></a><span data-ttu-id="f2c70-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2c70-136">Response</span></span>
><span data-ttu-id="f2c70-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f2c70-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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
            "id": "139166ec-d214-4835-95aa-3c1d89581e51",
            "accessReviewId": "8d035c9d-798d-47fa-beb4-f986a4b8126f",
            "reviewedDateTime": "2021-05-03T19:28:25.02Z",
            "decision": "Approve",
            "justification": "Kathleen still needs access to the Marketing group as she works in the Marketing organization.",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "principalLink": "https://graph.microsoft.com/v1.0/users/1800bb2c-955d-4205-8471-3a6c3116435d",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "36c4c56e-fce3-4e2d-b28e-4ac0c7d2fa10",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
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
                "userPrincipalName": "guest@contoso.com"
            }
        }
    ]
}
```
