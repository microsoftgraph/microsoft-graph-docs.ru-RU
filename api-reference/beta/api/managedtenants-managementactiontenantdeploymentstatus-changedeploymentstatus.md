---
title: 'managementActionTenantDeploymentStatus: changeDeploymentStatus'
description: Изменение состояния развертывания уровня клиента для действия управления. Эти сведения используются для получения сведений о том, какие действия управления находятся в определенном состоянии. В качестве примера может быть план применения многофакторной проверки подлинности для администраторов, поэтому было бы идеально изменить состояние на запланированное, чтобы отразить соответствующий статус.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 4d8c5acacee4eb31e8d014820466eae69534232f
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403049"
---
# <a name="managementactiontenantdeploymentstatus-changedeploymentstatus"></a><span data-ttu-id="3726a-105">managementActionTenantDeploymentStatus: changeDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="3726a-105">managementActionTenantDeploymentStatus: changeDeploymentStatus</span></span>
<span data-ttu-id="3726a-106">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="3726a-106">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3726a-107">Изменение состояния развертывания уровня клиента для действия управления.</span><span class="sxs-lookup"><span data-stu-id="3726a-107">Changes the tenant level deployment status for the management action.</span></span> <span data-ttu-id="3726a-108">Эти сведения используются для получения сведений о том, какие действия управления находятся в определенном состоянии.</span><span class="sxs-lookup"><span data-stu-id="3726a-108">This information is used to provide insights into what management actions are in a specific state.</span></span> <span data-ttu-id="3726a-109">В качестве примера может быть план применения многофакторной проверки подлинности для администраторов, поэтому было бы идеально изменить состояние на запланированное, чтобы отразить соответствующий статус.</span><span class="sxs-lookup"><span data-stu-id="3726a-109">As example there might be a plan to apply the require multi-factor authentication for admins, so it would be ideal to change the status to planned to reflect the appropriate status.</span></span>

## <a name="permissions"></a><span data-ttu-id="3726a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3726a-110">Permissions</span></span>
<span data-ttu-id="3726a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3726a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3726a-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3726a-113">Permission type</span></span>|<span data-ttu-id="3726a-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3726a-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3726a-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3726a-115">Delegated (work or school account)</span></span>|<span data-ttu-id="3726a-116">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3726a-116">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="3726a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3726a-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3726a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3726a-118">Not supported.</span></span>|
|<span data-ttu-id="3726a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3726a-119">Application</span></span>|<span data-ttu-id="3726a-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3726a-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3726a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3726a-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/changeDeploymentStatus
```

## <a name="request-headers"></a><span data-ttu-id="3726a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3726a-122">Request headers</span></span>
|<span data-ttu-id="3726a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="3726a-123">Name</span></span>|<span data-ttu-id="3726a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3726a-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3726a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3726a-125">Authorization</span></span>|<span data-ttu-id="3726a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3726a-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3726a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3726a-128">Content-Type</span></span>|<span data-ttu-id="3726a-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3726a-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3726a-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3726a-131">Request body</span></span>
<span data-ttu-id="3726a-132">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3726a-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3726a-133">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="3726a-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3726a-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="3726a-134">Parameter</span></span>|<span data-ttu-id="3726a-135">Тип</span><span class="sxs-lookup"><span data-stu-id="3726a-135">Type</span></span>|<span data-ttu-id="3726a-136">Описание</span><span class="sxs-lookup"><span data-stu-id="3726a-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3726a-137">tenantGroupId</span><span class="sxs-lookup"><span data-stu-id="3726a-137">tenantGroupId</span></span>|<span data-ttu-id="3726a-138">String</span><span class="sxs-lookup"><span data-stu-id="3726a-138">String</span></span>|<span data-ttu-id="3726a-139">Идентификатор группы клиента.</span><span class="sxs-lookup"><span data-stu-id="3726a-139">The identifier for the tenant group.</span></span>|
|<span data-ttu-id="3726a-140">tenantId</span><span class="sxs-lookup"><span data-stu-id="3726a-140">tenantId</span></span>|<span data-ttu-id="3726a-141">String</span><span class="sxs-lookup"><span data-stu-id="3726a-141">String</span></span>|<span data-ttu-id="3726a-142">Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="3726a-142">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|
|<span data-ttu-id="3726a-143">managementActionId</span><span class="sxs-lookup"><span data-stu-id="3726a-143">managementActionId</span></span>|<span data-ttu-id="3726a-144">String</span><span class="sxs-lookup"><span data-stu-id="3726a-144">String</span></span>|<span data-ttu-id="3726a-145">Идентификатор для действия [управления](../resources/managedtenants-managementaction.md).</span><span class="sxs-lookup"><span data-stu-id="3726a-145">The identifier for the [management action](../resources/managedtenants-managementaction.md).</span></span>|
|<span data-ttu-id="3726a-146">managementTemplateId</span><span class="sxs-lookup"><span data-stu-id="3726a-146">managementTemplateId</span></span>|<span data-ttu-id="3726a-147">String</span><span class="sxs-lookup"><span data-stu-id="3726a-147">String</span></span>|<span data-ttu-id="3726a-148">Идентификатор шаблона [управления.](../resources/managedtenants-managementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="3726a-148">The identifier for the [management template](../resources/managedtenants-managementtemplate.md).</span></span>|
|<span data-ttu-id="3726a-149">status</span><span class="sxs-lookup"><span data-stu-id="3726a-149">status</span></span>|<span data-ttu-id="3726a-150">String</span><span class="sxs-lookup"><span data-stu-id="3726a-150">String</span></span>|<span data-ttu-id="3726a-151">Новый статус развертывания клиента [действия](../resources/managedtenants-managementaction.md) управления.</span><span class="sxs-lookup"><span data-stu-id="3726a-151">The new status for the [management action](../resources/managedtenants-managementaction.md) tenant deployment.</span></span>|

## <a name="response"></a><span data-ttu-id="3726a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="3726a-152">Response</span></span>

<span data-ttu-id="3726a-153">В случае успешного выполнения это действие возвращает код ответа и `200 OK` [управлениеActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3726a-153">If successful, this action returns a `200 OK` response code and a [managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3726a-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="3726a-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3726a-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="3726a-155">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "managementactiontenantdeploymentstatus_changedeploymentstatus"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/changeDeploymentStatus
Content-Type: application/json
Content-length: 153

{
  "tenantGroupId": "String",
  "tenantId": "String",
  "managementActionId": "String",
  "managementTemplateId": "String",
  "status": "String"
}
```

### <a name="response"></a><span data-ttu-id="3726a-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="3726a-156">Response</span></span>
><span data-ttu-id="3726a-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3726a-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.managedTenants.ManagementActionDeploymentStatus",
  "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
  "managementActionId": "e96a8cdb-0435-4808-9956-cf6b8ae77aa6",
  "status": "planned",
  "workloadActionDeploymentStatuses": []
}
```
