---
title: 'клиент: offboardTenant'
description: Выполняет соответствующие процедуры по удалению управляемого клиента с платформы управления с несколькими арендаторами. Никакие отношения, такие как торговля и административные привилегии делегирования, не будут влиять. Единственным изменением, которое было внося это действие, является отсутствование клиента с платформы управления с несколькими клиентами.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: fc7a21323b7f1cd0abfe171eb80cead469d7816b
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403124"
---
# <a name="tenant-offboardtenant"></a><span data-ttu-id="f927a-105">клиент: offboardTenant</span><span class="sxs-lookup"><span data-stu-id="f927a-105">tenant: offboardTenant</span></span>
<span data-ttu-id="f927a-106">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="f927a-106">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f927a-107">Выполняет соответствующие процедуры по удалению управляемого клиента с платформы управления с несколькими арендаторами.</span><span class="sxs-lookup"><span data-stu-id="f927a-107">Carries out the appropriate procedures to remove a managed tenant from the multi-tenant management platform.</span></span> <span data-ttu-id="f927a-108">Никакие отношения, такие как торговля и административные привилегии делегирования, не будут влиять.</span><span class="sxs-lookup"><span data-stu-id="f927a-108">No relationships, such as commerce and delegate administrative privileges, will be impacted.</span></span> <span data-ttu-id="f927a-109">Единственным изменением, которое было внося это действие, является отсутствование клиента с платформы управления с несколькими клиентами.</span><span class="sxs-lookup"><span data-stu-id="f927a-109">The only change made by invoking this action is the tenant will be deprovisioned from the multi-tenant management platform.</span></span>

## <a name="permissions"></a><span data-ttu-id="f927a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f927a-110">Permissions</span></span>
<span data-ttu-id="f927a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f927a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f927a-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f927a-113">Permission type</span></span>|<span data-ttu-id="f927a-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f927a-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f927a-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f927a-115">Delegated (work or school account)</span></span>|<span data-ttu-id="f927a-116">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f927a-116">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="f927a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f927a-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f927a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f927a-118">Not supported.</span></span>|
|<span data-ttu-id="f927a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f927a-119">Application</span></span>|<span data-ttu-id="f927a-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f927a-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f927a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f927a-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenants/{tenantId}/offboardTenant
```

## <a name="request-headers"></a><span data-ttu-id="f927a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f927a-122">Request headers</span></span>
|<span data-ttu-id="f927a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="f927a-123">Name</span></span>|<span data-ttu-id="f927a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f927a-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f927a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f927a-125">Authorization</span></span>|<span data-ttu-id="f927a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f927a-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f927a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f927a-128">Request body</span></span>
<span data-ttu-id="f927a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f927a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f927a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f927a-130">Response</span></span>

<span data-ttu-id="f927a-131">В случае успешного действия возвращается код ответа и `200 OK` [клиент в](../resources/managedtenants-tenant.md) тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f927a-131">If successful, this action returns a `200 OK` response code and a [tenant](../resources/managedtenants-tenant.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f927a-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="f927a-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f927a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f927a-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "tenant_offboardtenant"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenants/{tenantId}/offboardTenant
```

### <a name="response"></a><span data-ttu-id="f927a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f927a-134">Response</span></span>
><span data-ttu-id="f927a-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f927a-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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
