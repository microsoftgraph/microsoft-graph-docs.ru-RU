---
title: Список решений
description: Получите ресурсы accessReviewInstanceDecisionItem из свойства навигации решений.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 74de88c1e14e9983580a80c1c1698842eaddc8f9
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031504"
---
# <a name="list-decisions"></a><span data-ttu-id="146e4-103">Список решений</span><span class="sxs-lookup"><span data-stu-id="146e4-103">List decisions</span></span>
<span data-ttu-id="146e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="146e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="146e4-105">Получите [объекты accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) из решений [по accessReviewInstance.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="146e4-105">Get the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects from the decisions on an [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

>[!NOTE]
><span data-ttu-id="146e4-106">Размер страницы по умолчанию для этого API — 100 объектов accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="146e4-106">The default page size for this API is 100 accessReviewInstance objects.</span></span> <span data-ttu-id="146e4-107">Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов.</span><span class="sxs-lookup"><span data-stu-id="146e4-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="146e4-108">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="146e4-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="146e4-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="146e4-109">Permissions</span></span>
<span data-ttu-id="146e4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="146e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="146e4-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="146e4-112">Permission type</span></span>|<span data-ttu-id="146e4-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="146e4-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="146e4-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="146e4-114">Delegated (work or school account)</span></span>|<span data-ttu-id="146e4-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="146e4-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="146e4-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="146e4-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="146e4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="146e4-117">Not supported.</span></span>|
|<span data-ttu-id="146e4-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="146e4-118">Application</span></span>|<span data-ttu-id="146e4-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="146e4-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="146e4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="146e4-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="146e4-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="146e4-121">Optional query parameters</span></span>
<span data-ttu-id="146e4-122">Этот метод поддерживает `$select` `$filter` параметры запроса `$orderBy` `$skip` `$top` OData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="146e4-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="146e4-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="146e4-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="146e4-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="146e4-124">Request headers</span></span>
|<span data-ttu-id="146e4-125">Имя</span><span class="sxs-lookup"><span data-stu-id="146e4-125">Name</span></span>|<span data-ttu-id="146e4-126">Описание</span><span class="sxs-lookup"><span data-stu-id="146e4-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="146e4-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="146e4-127">Authorization</span></span>|<span data-ttu-id="146e4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="146e4-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="146e4-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="146e4-130">Request body</span></span>
<span data-ttu-id="146e4-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="146e4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="146e4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="146e4-132">Response</span></span>

<span data-ttu-id="146e4-133">В случае успеха этот метод возвращает код отклика и коллекцию `200 OK` [объектов accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="146e4-133">If successful, this method returns a `200 OK` response code and a collection of [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="146e4-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="146e4-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="146e4-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="146e4-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/16d424f6-0100-4bf1-9ebc-fe009c5e5006/instances/bb14c722-51b8-4962-9bd2-1d96ba773d80/decisions
```


### <a name="response"></a><span data-ttu-id="146e4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="146e4-136">Response</span></span>
><span data-ttu-id="146e4-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="146e4-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('16d424f6-0100-4bf1-9ebc-fe009c5e5006')/instances('bb14c722-51b8-4962-9bd2-1d96ba773d80')/decisions",
    "@odata.count": 1,
    "value": [
        {
            "id": "bfbd4d74-275c-4368-aaa1-06c93838d0d5",
            "accessReviewId": "bb14c722-51b8-4962-9bd2-1d96ba773d80",
            "reviewedDateTime": "2021-05-05T16:48:28.79Z",
            "decision": "Deny",
            "justification": "bye alexxxxx",
            "appliedDateTime": "2021-05-05T16:50:30.9Z",
            "applyResult": "AppliedSuccessfully",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/540da31b-4d25-4934-b7f7-98bc230eb15a",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "ff15bedb-22de-49ad-b2d7-59656607484d",
                "displayName": "group owner",
                "userPrincipalName": "group owner"
            },
            "appliedBy": {
                "id": "8798d204-fa3c-4d7b-977d-bc939b8a0848",
                "displayName": "Access Reviews",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "540da31b-4d25-4934-b7f7-98bc230eb15a",
                "userDisplayName": "Alex Wilber",
                "userPrincipalName": "AlexW@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "540da31b-4d25-4934-b7f7-98bc230eb15a",
                "displayName": "Alex Wilber",
                "userPrincipalName": "AlexW@contoso.com"
            }
        }
    ]
}
```
