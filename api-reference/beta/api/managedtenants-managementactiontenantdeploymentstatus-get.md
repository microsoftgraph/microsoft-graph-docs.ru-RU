---
title: Get managementActionTenantDeploymentStatus
description: Ознакомьтесь с свойствами и отношениями объекта managementActionTenantDeploymentStatus.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: ac7da25234fd72abf979a7c8304a3a53d3554661
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442622"
---
# <a name="get-managementactiontenantdeploymentstatus"></a><span data-ttu-id="1968d-103">Get managementActionTenantDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="1968d-103">Get managementActionTenantDeploymentStatus</span></span>
<span data-ttu-id="1968d-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="1968d-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1968d-105">Ознакомьтесь с свойствами и отношениями объекта [managementActionTenantDeploymentStatus.](../resources/managedtenants-managementactiontenantdeploymentstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1968d-105">Read the properties and relationships of a [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1968d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1968d-106">Permissions</span></span>
<span data-ttu-id="1968d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1968d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1968d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1968d-109">Permission type</span></span>|<span data-ttu-id="1968d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1968d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1968d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1968d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1968d-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1968d-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="1968d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1968d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1968d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1968d-114">Not supported.</span></span>|
|<span data-ttu-id="1968d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1968d-115">Application</span></span>|<span data-ttu-id="1968d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1968d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1968d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1968d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/{managementActionTenantDeploymentStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1968d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1968d-118">Optional query parameters</span></span>
<span data-ttu-id="1968d-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="1968d-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1968d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1968d-120">Request headers</span></span>
|<span data-ttu-id="1968d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1968d-121">Name</span></span>|<span data-ttu-id="1968d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1968d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1968d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1968d-123">Authorization</span></span>|<span data-ttu-id="1968d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1968d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1968d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1968d-126">Request body</span></span>
<span data-ttu-id="1968d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1968d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1968d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1968d-128">Response</span></span>

<span data-ttu-id="1968d-129">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [объект managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1968d-129">If successful, this method returns a `200 OK` response code and a [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1968d-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="1968d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1968d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1968d-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1968d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1968d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_managementactiontenantdeploymentstatus"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/{managementActionTenantDeploymentStatusId}
```
# <a name="c"></a>[<span data-ttu-id="1968d-133">C#</span><span class="sxs-lookup"><span data-stu-id="1968d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-managementactiontenantdeploymentstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1968d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1968d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-managementactiontenantdeploymentstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1968d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1968d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-managementactiontenantdeploymentstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1968d-136">Java</span><span class="sxs-lookup"><span data-stu-id="1968d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-managementactiontenantdeploymentstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1968d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1968d-137">Response</span></span>
><span data-ttu-id="1968d-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1968d-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementActionTenantDeploymentStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/$entity",
    "id": "df7aed9c-c05a-4fc9-b958-64fafaed911d_34298981-4fc8-4974-9486-c8909ed1521b",
    "tenantGroupId": "df7aed9c-c05a-4fc9-b958-64fafaed911d",
    "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
    "statuses": [
        {
            "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
            "managementActionId": "4274db74-99c4-40be-bbeb-da4351136be2",
            "status": "completed",
            "workloadActionDeploymentStatuses": [
                {
                    "actionId": "fcb7ace7-3ea6-4474-912a-00ee78554445",
                    "status": "completed",
                    "deployedPolicyId": "949e8893-68fb-4c9d-b8a0-13c229a7e397",
                    "lastDeploymentDateTime": "2021-06-22T04:09:20.3054223Z",
                    "error": null
                }
            ]
        },
        {
            "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
            "managementActionId": "f104bb7f-4854-4209-ba09-c3788f9894c5",
            "status": "completed",
            "workloadActionDeploymentStatuses": [
                {
                    "actionId": "00a9a585-f51c-4b68-b4f5-f0c3165df8ac",
                    "status": "completed",
                    "deployedPolicyId": "19a8d6a6-d87e-4059-85b3-c73bfc5cea15",
                    "lastDeploymentDateTime": "2021-06-22T17:01:44.851214Z",
                    "error": null
                }
            ]
        }
    ]
}
```
