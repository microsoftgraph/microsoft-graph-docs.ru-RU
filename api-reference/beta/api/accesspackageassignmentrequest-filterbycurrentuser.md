---
title: 'accessPackageAssignmentRequest: filterByCurrentUser'
description: Извлечение списка объектов accesspackageassignmentrequest, фильтруемых на входе пользователя.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f65ca1c94f2702245b1765e904bb3c559cab6685
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473968"
---
# <a name="accesspackageassignmentrequest-filterbycurrentuser"></a><span data-ttu-id="ef3d0-103">accessPackageAssignmentRequest: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="ef3d0-103">accessPackageAssignmentRequest: filterByCurrentUser</span></span>
<span data-ttu-id="ef3d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef3d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef3d0-105">В [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md)вы можете получить список объектов [accessPackageAssignmentRequest,](../resources/accesspackageassignmentrequest.md) фильтруемых для пользователя, входив в него.</span><span class="sxs-lookup"><span data-stu-id="ef3d0-105">In [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects filtered on the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef3d0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef3d0-106">Permissions</span></span>
<span data-ttu-id="ef3d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef3d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef3d0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef3d0-109">Permission type</span></span>|<span data-ttu-id="ef3d0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef3d0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef3d0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef3d0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ef3d0-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef3d0-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="ef3d0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef3d0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef3d0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef3d0-114">Not supported.</span></span>|
|<span data-ttu-id="ef3d0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef3d0-115">Application</span></span>|<span data-ttu-id="ef3d0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef3d0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef3d0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef3d0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/filterByCurrentUser
```

## <a name="function-parameters"></a><span data-ttu-id="ef3d0-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="ef3d0-118">Function parameters</span></span>
<span data-ttu-id="ef3d0-119">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="ef3d0-119">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ef3d0-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="ef3d0-120">Parameter</span></span>|<span data-ttu-id="ef3d0-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ef3d0-121">Type</span></span>|<span data-ttu-id="ef3d0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ef3d0-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef3d0-123">on</span><span class="sxs-lookup"><span data-stu-id="ef3d0-123">on</span></span>|[<span data-ttu-id="ef3d0-124">accessPackageAssignmentRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="ef3d0-124">accessPackageAssignmentRequestFilterByCurrentUserOptions</span></span>](../resources/accesspackageassignmentrequest-accesspackageassignmentrequestfilterbycurrentuseroptions.md)|<span data-ttu-id="ef3d0-125">Список текущих пользовательских параметров, которые можно использовать для фильтрации в списке запросов на назначение пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="ef3d0-125">The list of current user options that can be used to filter on the access package assignment requests list.</span></span>|

- <span data-ttu-id="ef3d0-126">`target` используется для получения объектов, в которых целевым объектом является пользователь, заявив `accessPackageAssignmentRequest` о подписании.</span><span class="sxs-lookup"><span data-stu-id="ef3d0-126">`target` is used to get the `accessPackageAssignmentRequest` objects where the signed-in user is the target.</span></span> <span data-ttu-id="ef3d0-127">В итоговом списке содержатся все запросы назначения, текущие и просроченные, которые запрашивались вызываемой или вызываемой, во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="ef3d0-127">The resulting list includes all the assignment requests, current and expired, that were requested by the caller or for the caller, across all catalogs and access packages.</span></span>

- <span data-ttu-id="ef3d0-128">`createdBy` используется для получения `accessPackageAssignmentRequest` объектов, созданных подписанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="ef3d0-128">`createdBy` is used to get the `accessPackageAssignmentRequest` objects created by the signed-in user.</span></span> <span data-ttu-id="ef3d0-129">В итоговом списке содержатся все запросы на назначение, созданные вызываемой для себя или от имени других лиц, например в случае прямого назначения администратора во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="ef3d0-129">The resulting list includes all of the assignment requests that the caller has created for themselves or on behalf of others, such as in case of admin direct assignment, across all catalogs and access packages.</span></span>

- <span data-ttu-id="ef3d0-130">`approver` используется для получения объектов, в которых пользователь, заявив, что является разрешенным одобритель в любом из `accessPackageAssignmentRequest` `accessPackageAssignment/accessPackageAssignmentPolicy/requestApprovalSettings/approvalStages` содержащихся `primaryApprovers` `escalationApprovers` (или).</span><span class="sxs-lookup"><span data-stu-id="ef3d0-130">`approver` is used to get the `accessPackageAssignmentRequest` objects where the signed-in user is an allowed approver in any contained `accessPackageAssignment/accessPackageAssignmentPolicy/requestApprovalSettings/approvalStages` (`primaryApprovers` or `escalationApprovers`).</span></span> <span data-ttu-id="ef3d0-131">В итоговом списке содержатся  запросы на назначение в ожидаемом состоянии, во всех каталогах и пакетах доступа, которые требуют решения от вызываемого.</span><span class="sxs-lookup"><span data-stu-id="ef3d0-131">The resulting list includes the assignment requests in *pending* state, across all catalogs and access packages and that need a decision from the caller.</span></span> <span data-ttu-id="ef3d0-132">В итоговом списке содержатся запросы на назначение в состоянии, во всех каталогах и пакетах доступа, которые требуют решения от `pending` вызываемого.</span><span class="sxs-lookup"><span data-stu-id="ef3d0-132">The resulting list includes the assignment requests in a `pending` state, across all catalogs and access packages and that need a decision from the caller.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef3d0-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef3d0-133">Request headers</span></span>
|<span data-ttu-id="ef3d0-134">Имя</span><span class="sxs-lookup"><span data-stu-id="ef3d0-134">Name</span></span>|<span data-ttu-id="ef3d0-135">Описание</span><span class="sxs-lookup"><span data-stu-id="ef3d0-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ef3d0-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef3d0-136">Authorization</span></span>|<span data-ttu-id="ef3d0-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef3d0-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef3d0-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef3d0-139">Request body</span></span>
<span data-ttu-id="ef3d0-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef3d0-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef3d0-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef3d0-141">Response</span></span>

<span data-ttu-id="ef3d0-142">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [коллекцию accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ef3d0-142">If successful, this method returns a `200 OK` response code and an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ef3d0-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="ef3d0-143">Examples</span></span>

<span data-ttu-id="ef3d0-144">В следующем примере получается состояние запросов назначения пакетов доступа, целевых для подписанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ef3d0-144">The following example gets the status of access package assignment requests targeted for the signed-in user.</span></span>

### <a name="request"></a><span data-ttu-id="ef3d0-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef3d0-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ef3d0-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef3d0-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/filterByCurrentUser(on='target')
```
# <a name="c"></a>[<span data-ttu-id="ef3d0-147">C#</span><span class="sxs-lookup"><span data-stu-id="ef3d0-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accesspackageassignmentrequest-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef3d0-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef3d0-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackageassignmentrequest-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef3d0-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef3d0-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackageassignmentrequest-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef3d0-150">Java</span><span class="sxs-lookup"><span data-stu-id="ef3d0-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accesspackageassignmentrequest-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ef3d0-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef3d0-151">Response</span></span>
> <span data-ttu-id="ef3d0-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ef3d0-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignmentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
            "createdDateTime": "2021-01-19T20:02:23.907Z",
            "completedDate": "2021-01-19T20:02:40.97Z",
            "id": "46c1410d-ef96-44c5-ae9c-a577d014fe0e",
            "requestType": "AdminAdd",
            "requestState": "Delivered",
            "requestStatus": "Fulfilled",
            "isValidationOnly": false,
            "expirationDateTime": null,
            "justification": null,
            "answers": [],
            "schedule": {
                "startDateTime": "2021-01-19T20:01:57.643Z",
                "recurrence": null,
                "expiration": {
                    "endDateTime": null,
                    "duration": null,
                    "type": "noExpiration"
                }
            }
        }
    ]
}
```

