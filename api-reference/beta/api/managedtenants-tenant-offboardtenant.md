---
title: 'клиент: offboardTenant'
description: Выполняет соответствующие процедуры по удалению управляемого клиента с платформы управления с несколькими арендаторами. Никакие отношения, такие как торговля и административные привилегии делегирования, не будут влиять. Единственным изменением, которое было внося это действие, является отсутствование клиента с платформы управления с несколькими клиентами.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: d6d4d07c7af19299e679275354206bc55da3ffdb
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442549"
---
# <a name="tenant-offboardtenant"></a><span data-ttu-id="e840f-105">клиент: offboardTenant</span><span class="sxs-lookup"><span data-stu-id="e840f-105">tenant: offboardTenant</span></span>
<span data-ttu-id="e840f-106">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="e840f-106">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e840f-107">Выполняет соответствующие процедуры по удалению управляемого клиента с платформы управления с несколькими арендаторами.</span><span class="sxs-lookup"><span data-stu-id="e840f-107">Carries out the appropriate procedures to remove a managed tenant from the multi-tenant management platform.</span></span> <span data-ttu-id="e840f-108">Никакие отношения, такие как торговля и административные привилегии делегирования, не будут влиять.</span><span class="sxs-lookup"><span data-stu-id="e840f-108">No relationships, such as commerce and delegate administrative privileges, will be impacted.</span></span> <span data-ttu-id="e840f-109">Единственным изменением, которое было внося это действие, является отсутствование клиента с платформы управления с несколькими клиентами.</span><span class="sxs-lookup"><span data-stu-id="e840f-109">The only change made by invoking this action is the tenant will be deprovisioned from the multi-tenant management platform.</span></span>

## <a name="permissions"></a><span data-ttu-id="e840f-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e840f-110">Permissions</span></span>
<span data-ttu-id="e840f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e840f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e840f-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e840f-113">Permission type</span></span>|<span data-ttu-id="e840f-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e840f-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e840f-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e840f-115">Delegated (work or school account)</span></span>|<span data-ttu-id="e840f-116">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e840f-116">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="e840f-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e840f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e840f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e840f-118">Not supported.</span></span>|
|<span data-ttu-id="e840f-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e840f-119">Application</span></span>|<span data-ttu-id="e840f-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e840f-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e840f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e840f-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenants/{tenantId}/offboardTenant
```

## <a name="request-headers"></a><span data-ttu-id="e840f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e840f-122">Request headers</span></span>
|<span data-ttu-id="e840f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e840f-123">Name</span></span>|<span data-ttu-id="e840f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e840f-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e840f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e840f-125">Authorization</span></span>|<span data-ttu-id="e840f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e840f-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e840f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e840f-128">Request body</span></span>
<span data-ttu-id="e840f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e840f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e840f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e840f-130">Response</span></span>

<span data-ttu-id="e840f-131">В случае успешного действия возвращается код ответа и `200 OK` [клиент в](../resources/managedtenants-tenant.md) тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e840f-131">If successful, this action returns a `200 OK` response code and a [tenant](../resources/managedtenants-tenant.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e840f-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="e840f-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e840f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e840f-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e840f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e840f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tenant_offboardtenant"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenants/{tenantId}/offboardTenant
```
# <a name="c"></a>[<span data-ttu-id="e840f-135">C#</span><span class="sxs-lookup"><span data-stu-id="e840f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tenant-offboardtenant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e840f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e840f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tenant-offboardtenant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e840f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e840f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tenant-offboardtenant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e840f-138">Java</span><span class="sxs-lookup"><span data-stu-id="e840f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tenant-offboardtenant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e840f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e840f-139">Response</span></span>
><span data-ttu-id="e840f-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e840f-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenant"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.managedTenants.tenant",
    "id": "String (identifier)",
    "tenantId": "String",
    "displayName": "String",
    "contract": {
      "@odata.type": "microsoft.graph.managedTenants.tenantContract"
    },
    "tenantStatusInformation": {
      "@odata.type": "microsoft.graph.managedTenants.tenantStatusInformation"
    },
    "lastUpdatedDateTime": "String (timestamp)",
    "createdDateTime": "String (timestamp)"
  }
}
```
