---
title: Get managementActionTenantDeploymentStatus
description: Ознакомьтесь с свойствами и отношениями объекта managementActionTenantDeploymentStatus.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 9efb91eed729ed88d7f95554d752d85e1510480b
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402633"
---
# <a name="get-managementactiontenantdeploymentstatus"></a><span data-ttu-id="68da4-103">Get managementActionTenantDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="68da4-103">Get managementActionTenantDeploymentStatus</span></span>
<span data-ttu-id="68da4-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="68da4-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68da4-105">Ознакомьтесь с свойствами и отношениями объекта [managementActionTenantDeploymentStatus.](../resources/managedtenants-managementactiontenantdeploymentstatus.md)</span><span class="sxs-lookup"><span data-stu-id="68da4-105">Read the properties and relationships of a [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="68da4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68da4-106">Permissions</span></span>
<span data-ttu-id="68da4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68da4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68da4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68da4-109">Permission type</span></span>|<span data-ttu-id="68da4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68da4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68da4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68da4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="68da4-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68da4-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="68da4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68da4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68da4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68da4-114">Not supported.</span></span>|
|<span data-ttu-id="68da4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68da4-115">Application</span></span>|<span data-ttu-id="68da4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68da4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68da4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68da4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/{managementActionTenantDeploymentStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68da4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="68da4-118">Optional query parameters</span></span>
<span data-ttu-id="68da4-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="68da4-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="68da4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68da4-120">Request headers</span></span>
|<span data-ttu-id="68da4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="68da4-121">Name</span></span>|<span data-ttu-id="68da4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="68da4-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="68da4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68da4-123">Authorization</span></span>|<span data-ttu-id="68da4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68da4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="68da4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68da4-126">Request body</span></span>
<span data-ttu-id="68da4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68da4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68da4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="68da4-128">Response</span></span>

<span data-ttu-id="68da4-129">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [объект managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="68da4-129">If successful, this method returns a `200 OK` response code and a [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="68da4-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="68da4-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="68da4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="68da4-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_managementactiontenantdeploymentstatus"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/{managementActionTenantDeploymentStatusId}
```

### <a name="response"></a><span data-ttu-id="68da4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="68da4-132">Response</span></span>
><span data-ttu-id="68da4-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="68da4-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
