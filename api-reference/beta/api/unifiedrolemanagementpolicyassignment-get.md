---
title: Get unifiedRoleManagementPolicyAssignment
description: Ознакомьтесь с свойствами и отношениями единого объектаRoleManagementPolicyAssignment.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 45c74509b4530981d0417874f1490c3596d88898
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299574"
---
# <a name="get-unifiedrolemanagementpolicyassignment"></a><span data-ttu-id="3ea3e-103">Get unifiedRoleManagementPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="3ea3e-103">Get unifiedRoleManagementPolicyAssignment</span></span>
<span data-ttu-id="3ea3e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ea3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ea3e-105">Ознакомьтесь с свойствами и отношениями единого [объектаRoleManagementPolicyAssignment.](../resources/unifiedrolemanagementpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3ea3e-105">Read the properties and relationships of an [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ea3e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ea3e-106">Permissions</span></span>
<span data-ttu-id="3ea3e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ea3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ea3e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ea3e-109">Permission type</span></span>|<span data-ttu-id="3ea3e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ea3e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ea3e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ea3e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3ea3e-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="3ea3e-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="3ea3e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ea3e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ea3e-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3ea3e-114">Not supported</span></span>|
|<span data-ttu-id="3ea3e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ea3e-115">Application</span></span>|<span data-ttu-id="3ea3e-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="3ea3e-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ea3e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ea3e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicyAssignments/{unifiedRoleManagementPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3ea3e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3ea3e-118">Optional query parameters</span></span>
<span data-ttu-id="3ea3e-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="3ea3e-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3ea3e-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3ea3e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ea3e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ea3e-121">Request headers</span></span>
|<span data-ttu-id="3ea3e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3ea3e-122">Name</span></span>|<span data-ttu-id="3ea3e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3ea3e-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3ea3e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ea3e-124">Authorization</span></span>|<span data-ttu-id="3ea3e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ea3e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ea3e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ea3e-127">Request body</span></span>
<span data-ttu-id="3ea3e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ea3e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ea3e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ea3e-129">Response</span></span>

<span data-ttu-id="3ea3e-130">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [унифицированный объектRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3ea3e-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3ea3e-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="3ea3e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3ea3e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ea3e-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedrolemanagementpolicyassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicyAssignments/d6e4112f-112f-d6e4-2f11-e4d62f11e4d6
```


### <a name="response"></a><span data-ttu-id="3ea3e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ea3e-133">Response</span></span>
<span data-ttu-id="3ea3e-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3ea3e-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAssignment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
    "policyId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
    "scopeId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
    "scopeType": "subscription",
    "roleDefinitionId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6"
  }
}
```

