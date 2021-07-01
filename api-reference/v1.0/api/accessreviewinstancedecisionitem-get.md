---
title: Get accessReviewInstanceDecisionItem
description: Ознакомьтесь с свойствами и отношениями объекта accessReviewInstanceDecisionItem.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2f72596f4f89fe71f6d7cee310e721dd230357ee
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209733"
---
# <a name="get-accessreviewinstancedecisionitem"></a><span data-ttu-id="f2569-103">Get accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="f2569-103">Get accessReviewInstanceDecisionItem</span></span>
<span data-ttu-id="f2569-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2569-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f2569-105">Ознакомьтесь с свойствами и отношениями [объекта accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="f2569-105">Read the properties and relationships of an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2569-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2569-106">Permissions</span></span>
<span data-ttu-id="f2569-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2569-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2569-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2569-109">Permission type</span></span>|<span data-ttu-id="f2569-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2569-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2569-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2569-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2569-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2569-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="f2569-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2569-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2569-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2569-114">Not supported.</span></span>|
|<span data-ttu-id="f2569-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f2569-115">Application</span></span>|<span data-ttu-id="f2569-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2569-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2569-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2569-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2569-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f2569-118">Optional query parameters</span></span>
<span data-ttu-id="f2569-119">Этот метод поддерживает `$select` параметр запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="f2569-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="f2569-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f2569-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2569-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2569-121">Request headers</span></span>
|<span data-ttu-id="f2569-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f2569-122">Name</span></span>|<span data-ttu-id="f2569-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f2569-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f2569-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2569-124">Authorization</span></span>|<span data-ttu-id="f2569-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2569-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2569-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2569-127">Request body</span></span>
<span data-ttu-id="f2569-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2569-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2569-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2569-129">Response</span></span>

<span data-ttu-id="f2569-130">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f2569-130">If successful, this method returns a `200 OK` response code and an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2569-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f2569-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2569-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2569-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f2569-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2569-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/instances/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/decisions/9550e25b-f315-4454-9d87-16b885c35de4
```
# <a name="c"></a>[<span data-ttu-id="f2569-134">C#</span><span class="sxs-lookup"><span data-stu-id="f2569-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2569-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2569-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2569-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2569-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2569-137">Java</span><span class="sxs-lookup"><span data-stu-id="f2569-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f2569-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2569-138">Response</span></span>
><span data-ttu-id="f2569-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f2569-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd')/instances('7070ea1c-8d12-457b-bd35-a37dc59e54e0')/decisions/$entity",
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
```
