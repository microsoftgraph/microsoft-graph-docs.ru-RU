---
title: 'managementActionTenantDeploymentStatus: changeDeploymentStatus'
description: Изменение состояния развертывания уровня клиента для действия управления. Эти сведения используются для получения сведений о том, какие действия управления находятся в определенном состоянии. В качестве примера может быть план применения многофакторной проверки подлинности для администраторов, поэтому было бы идеально изменить состояние на запланированное, чтобы отразить соответствующий статус.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 572ee7f6c6769ec500c47edee5d35dd18fe75d3f
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440922"
---
# <a name="managementactiontenantdeploymentstatus-changedeploymentstatus"></a><span data-ttu-id="8ecf6-105">managementActionTenantDeploymentStatus: changeDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="8ecf6-105">managementActionTenantDeploymentStatus: changeDeploymentStatus</span></span>
<span data-ttu-id="8ecf6-106">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="8ecf6-106">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ecf6-107">Изменение состояния развертывания уровня клиента для действия управления.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-107">Changes the tenant level deployment status for the management action.</span></span> <span data-ttu-id="8ecf6-108">Эти сведения используются для получения сведений о том, какие действия управления находятся в определенном состоянии.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-108">This information is used to provide insights into what management actions are in a specific state.</span></span> <span data-ttu-id="8ecf6-109">В качестве примера может быть план применения многофакторной проверки подлинности для администраторов, поэтому было бы идеально изменить состояние на запланированное, чтобы отразить соответствующий статус.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-109">As example there might be a plan to apply the require multi-factor authentication for admins, so it would be ideal to change the status to planned to reflect the appropriate status.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ecf6-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ecf6-110">Permissions</span></span>
<span data-ttu-id="8ecf6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ecf6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ecf6-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ecf6-113">Permission type</span></span>|<span data-ttu-id="8ecf6-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ecf6-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ecf6-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ecf6-115">Delegated (work or school account)</span></span>|<span data-ttu-id="8ecf6-116">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ecf6-116">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="8ecf6-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ecf6-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ecf6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-118">Not supported.</span></span>|
|<span data-ttu-id="8ecf6-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ecf6-119">Application</span></span>|<span data-ttu-id="8ecf6-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ecf6-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ecf6-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/changeDeploymentStatus
```

## <a name="request-headers"></a><span data-ttu-id="8ecf6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ecf6-122">Request headers</span></span>
|<span data-ttu-id="8ecf6-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8ecf6-123">Name</span></span>|<span data-ttu-id="8ecf6-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8ecf6-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8ecf6-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ecf6-125">Authorization</span></span>|<span data-ttu-id="8ecf6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8ecf6-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ecf6-128">Content-Type</span></span>|<span data-ttu-id="8ecf6-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ecf6-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ecf6-131">Request body</span></span>
<span data-ttu-id="8ecf6-132">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8ecf6-133">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8ecf6-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="8ecf6-134">Parameter</span></span>|<span data-ttu-id="8ecf6-135">Тип</span><span class="sxs-lookup"><span data-stu-id="8ecf6-135">Type</span></span>|<span data-ttu-id="8ecf6-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8ecf6-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ecf6-137">tenantGroupId</span><span class="sxs-lookup"><span data-stu-id="8ecf6-137">tenantGroupId</span></span>|<span data-ttu-id="8ecf6-138">String</span><span class="sxs-lookup"><span data-stu-id="8ecf6-138">String</span></span>|<span data-ttu-id="8ecf6-139">Идентификатор группы клиента.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-139">The identifier for the tenant group.</span></span>|
|<span data-ttu-id="8ecf6-140">tenantId</span><span class="sxs-lookup"><span data-stu-id="8ecf6-140">tenantId</span></span>|<span data-ttu-id="8ecf6-141">String</span><span class="sxs-lookup"><span data-stu-id="8ecf6-141">String</span></span>|<span data-ttu-id="8ecf6-142">Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="8ecf6-142">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|
|<span data-ttu-id="8ecf6-143">managementActionId</span><span class="sxs-lookup"><span data-stu-id="8ecf6-143">managementActionId</span></span>|<span data-ttu-id="8ecf6-144">String</span><span class="sxs-lookup"><span data-stu-id="8ecf6-144">String</span></span>|<span data-ttu-id="8ecf6-145">Идентификатор для действия [управления](../resources/managedtenants-managementaction.md).</span><span class="sxs-lookup"><span data-stu-id="8ecf6-145">The identifier for the [management action](../resources/managedtenants-managementaction.md).</span></span>|
|<span data-ttu-id="8ecf6-146">managementTemplateId</span><span class="sxs-lookup"><span data-stu-id="8ecf6-146">managementTemplateId</span></span>|<span data-ttu-id="8ecf6-147">String</span><span class="sxs-lookup"><span data-stu-id="8ecf6-147">String</span></span>|<span data-ttu-id="8ecf6-148">Идентификатор шаблона [управления.](../resources/managedtenants-managementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="8ecf6-148">The identifier for the [management template](../resources/managedtenants-managementtemplate.md).</span></span>|
|<span data-ttu-id="8ecf6-149">status</span><span class="sxs-lookup"><span data-stu-id="8ecf6-149">status</span></span>|<span data-ttu-id="8ecf6-150">String</span><span class="sxs-lookup"><span data-stu-id="8ecf6-150">String</span></span>|<span data-ttu-id="8ecf6-151">Новый статус развертывания клиента [действия](../resources/managedtenants-managementaction.md) управления.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-151">The new status for the [management action](../resources/managedtenants-managementaction.md) tenant deployment.</span></span>|

## <a name="response"></a><span data-ttu-id="8ecf6-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ecf6-152">Response</span></span>

<span data-ttu-id="8ecf6-153">В случае успешного выполнения это действие возвращает код ответа и `200 OK` [управлениеActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-153">If successful, this action returns a `200 OK` response code and a [managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8ecf6-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="8ecf6-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8ecf6-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ecf6-155">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8ecf6-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ecf6-156">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8ecf6-157">C#</span><span class="sxs-lookup"><span data-stu-id="8ecf6-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/managementactiontenantdeploymentstatus-changedeploymentstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ecf6-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ecf6-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/managementactiontenantdeploymentstatus-changedeploymentstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ecf6-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ecf6-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/managementactiontenantdeploymentstatus-changedeploymentstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8ecf6-160">Java</span><span class="sxs-lookup"><span data-stu-id="8ecf6-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/managementactiontenantdeploymentstatus-changedeploymentstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8ecf6-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ecf6-161">Response</span></span>
><span data-ttu-id="8ecf6-162">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-162">**Note:** The response object shown here might be shortened for readability.</span></span>
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
