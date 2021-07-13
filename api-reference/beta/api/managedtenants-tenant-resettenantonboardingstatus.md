---
title: 'клиент: resetTenantOnboardingStatus'
description: Выполняет соответствующие процедуры для сброса состояния onboarding для управляемого клиента, который был удален с платформы управления с несколькими арендаторами с помощью действия offboardTenant. Путем ссылки на это действие платформа будет пытаться установить на борт управляемого клиента для управления.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: dadbf614e74da6d139e2a07e98a528ae2955cd8a
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403048"
---
# <a name="tenant-resettenantonboardingstatus"></a><span data-ttu-id="63798-104">клиент: resetTenantOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="63798-104">tenant: resetTenantOnboardingStatus</span></span>
<span data-ttu-id="63798-105">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="63798-105">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63798-106">Выполняет соответствующие процедуры для сброса состояния onboarding для управляемого клиента, который был удален с платформы управления с несколькими арендаторами с помощью [действия offboardTenant.](../api/managedtenants-tenant-offboardtenant.md)</span><span class="sxs-lookup"><span data-stu-id="63798-106">Carries out the appropriate procedures to reset the onboarding status for the managed tenant that was removed from the multi-tenant management platform using the [offboardTenant](../api/managedtenants-tenant-offboardtenant.md) action.</span></span> <span data-ttu-id="63798-107">Путем ссылки на это действие платформа будет пытаться установить на борт управляемого клиента для управления.</span><span class="sxs-lookup"><span data-stu-id="63798-107">By invoking this action the platform will attempt to onboard the managed tenant for management.</span></span>

## <a name="permissions"></a><span data-ttu-id="63798-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63798-108">Permissions</span></span>
<span data-ttu-id="63798-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63798-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63798-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63798-111">Permission type</span></span>|<span data-ttu-id="63798-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63798-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63798-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63798-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63798-114">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63798-114">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="63798-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63798-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63798-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63798-116">Not supported.</span></span>|
|<span data-ttu-id="63798-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63798-117">Application</span></span>|<span data-ttu-id="63798-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63798-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63798-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63798-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenants/{tenantId}/resetTenantOnboardingStatus
```

## <a name="request-headers"></a><span data-ttu-id="63798-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63798-120">Request headers</span></span>
|<span data-ttu-id="63798-121">Имя</span><span class="sxs-lookup"><span data-stu-id="63798-121">Name</span></span>|<span data-ttu-id="63798-122">Описание</span><span class="sxs-lookup"><span data-stu-id="63798-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="63798-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63798-123">Authorization</span></span>|<span data-ttu-id="63798-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63798-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="63798-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63798-126">Request body</span></span>
<span data-ttu-id="63798-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="63798-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63798-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="63798-128">Response</span></span>

<span data-ttu-id="63798-129">В случае успешного действия возвращается код ответа и `200 OK` [клиент в](../resources/managedtenants-tenant.md) тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="63798-129">If successful, this action returns a `200 OK` response code and a [tenant](../resources/managedtenants-tenant.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63798-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="63798-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="63798-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="63798-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "tenant_resettenantonboardingstatus"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenants/{tenantId}/resetTenantOnboardingStatus
```

### <a name="response"></a><span data-ttu-id="63798-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="63798-132">Response</span></span>
><span data-ttu-id="63798-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="63798-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
