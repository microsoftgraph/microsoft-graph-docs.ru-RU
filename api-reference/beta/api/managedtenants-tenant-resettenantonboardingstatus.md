---
title: 'клиент: resetTenantOnboardingStatus'
description: Выполняет соответствующие процедуры для сброса состояния onboarding для управляемого клиента, который был удален с платформы управления с несколькими арендаторами с помощью действия offboardTenant. Путем ссылки на это действие платформа будет пытаться установить на борт управляемого клиента для управления.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: e7d584343475f5f1698b4bccde13a0f1115abf43
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440439"
---
# <a name="tenant-resettenantonboardingstatus"></a><span data-ttu-id="0d21e-104">клиент: resetTenantOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="0d21e-104">tenant: resetTenantOnboardingStatus</span></span>
<span data-ttu-id="0d21e-105">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="0d21e-105">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d21e-106">Выполняет соответствующие процедуры для сброса состояния onboarding для управляемого клиента, который был удален с платформы управления с несколькими арендаторами с помощью [действия offboardTenant.](../api/managedtenants-tenant-offboardtenant.md)</span><span class="sxs-lookup"><span data-stu-id="0d21e-106">Carries out the appropriate procedures to reset the onboarding status for the managed tenant that was removed from the multi-tenant management platform using the [offboardTenant](../api/managedtenants-tenant-offboardtenant.md) action.</span></span> <span data-ttu-id="0d21e-107">Путем ссылки на это действие платформа будет пытаться установить на борт управляемого клиента для управления.</span><span class="sxs-lookup"><span data-stu-id="0d21e-107">By invoking this action the platform will attempt to onboard the managed tenant for management.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d21e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d21e-108">Permissions</span></span>
<span data-ttu-id="0d21e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d21e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d21e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d21e-111">Permission type</span></span>|<span data-ttu-id="0d21e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d21e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d21e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d21e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d21e-114">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d21e-114">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="0d21e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d21e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d21e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d21e-116">Not supported.</span></span>|
|<span data-ttu-id="0d21e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d21e-117">Application</span></span>|<span data-ttu-id="0d21e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d21e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d21e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d21e-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenants/{tenantId}/resetTenantOnboardingStatus
```

## <a name="request-headers"></a><span data-ttu-id="0d21e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d21e-120">Request headers</span></span>
|<span data-ttu-id="0d21e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0d21e-121">Name</span></span>|<span data-ttu-id="0d21e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0d21e-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0d21e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d21e-123">Authorization</span></span>|<span data-ttu-id="0d21e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d21e-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d21e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d21e-126">Request body</span></span>
<span data-ttu-id="0d21e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d21e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d21e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d21e-128">Response</span></span>

<span data-ttu-id="0d21e-129">В случае успешного действия возвращается код ответа и `200 OK` [клиент в](../resources/managedtenants-tenant.md) тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0d21e-129">If successful, this action returns a `200 OK` response code and a [tenant](../resources/managedtenants-tenant.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d21e-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="0d21e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0d21e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d21e-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0d21e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d21e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tenant_resettenantonboardingstatus"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenants/{tenantId}/resetTenantOnboardingStatus
```
# <a name="c"></a>[<span data-ttu-id="0d21e-133">C#</span><span class="sxs-lookup"><span data-stu-id="0d21e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tenant-resettenantonboardingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d21e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d21e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tenant-resettenantonboardingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d21e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d21e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tenant-resettenantonboardingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d21e-136">Java</span><span class="sxs-lookup"><span data-stu-id="0d21e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tenant-resettenantonboardingstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0d21e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d21e-137">Response</span></span>
><span data-ttu-id="0d21e-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0d21e-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.type": "#microsoft.graph.managedTenants.tenant",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b",
  "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
  "contract": {
    "displayName": "Fourth Coffee",
    "defaultDomainName": "fourthcoffe001.onmicrosoft.com",
    "contractType": 2
  },
  "tenantStatusInformation": {
    "onboardingStatus": "inactive",
    "onboardingDateTime": "2012-02-20T00:00:00Z",
    "onboardedByUserId": "",
    "offboardedDateTime": "2012-02-20T00:00:00Z",
    "offboardedBy": "",
    "delegatedPrivilegeStatus": "delegatedAdminPrivileges",
    "workloadStatuses": []
  },
  "createdDateTime": "2012-02-20T00:00:00Z",
  "lastUpdatedDatetime": "2021-02-20T00:00:00Z"
}
```
