---
title: 'managementAction: применить'
description: Применяет действие управления к определенному управляемому клиенту. При выполнении этой операции будут созданы соответствующие конфигурации и созданы политики. В качестве примера при применении требуемой многофакторной проверки подлинности для действий управления администраторами создается политика условного доступа Azure Active Directory, которая требует многофакторной проверки подлинности для всех пользователей, на которых назначена роль административного каталога.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: c5ba45154faf95e85a3f7f7878c18a4bb4981d16
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403053"
---
# <a name="managementaction-apply"></a><span data-ttu-id="ecd75-105">managementAction: применить</span><span class="sxs-lookup"><span data-stu-id="ecd75-105">managementAction: apply</span></span>
<span data-ttu-id="ecd75-106">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="ecd75-106">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecd75-107">Применяет действие управления к определенному управляемому клиенту.</span><span class="sxs-lookup"><span data-stu-id="ecd75-107">Applies a management action against a specific managed tenant.</span></span> <span data-ttu-id="ecd75-108">При выполнении этой операции будут созданы соответствующие конфигурации и созданы политики.</span><span class="sxs-lookup"><span data-stu-id="ecd75-108">By performing this operation the appropriate configurations will be made and policies created.</span></span> <span data-ttu-id="ecd75-109">В качестве примера при применении требуемой многофакторной проверки подлинности для действий управления администраторами создается политика условного доступа Azure Active Directory, которая требует многофакторной проверки подлинности для всех пользователей, на которых назначена роль административного каталога.</span><span class="sxs-lookup"><span data-stu-id="ecd75-109">As example when applying the require multi-factor authentication for admins management action will create an Azure Active Directory conditional access policy that requires multi-factor authentication for all users that have been assigned an administrative directory role.</span></span>

## <a name="permissions"></a><span data-ttu-id="ecd75-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ecd75-110">Permissions</span></span>
<span data-ttu-id="ecd75-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecd75-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecd75-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ecd75-113">Permission type</span></span>|<span data-ttu-id="ecd75-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ecd75-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecd75-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ecd75-115">Delegated (work or school account)</span></span>|<span data-ttu-id="ecd75-116">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecd75-116">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="ecd75-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ecd75-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecd75-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecd75-118">Not supported.</span></span>|
|<span data-ttu-id="ecd75-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ecd75-119">Application</span></span>|<span data-ttu-id="ecd75-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecd75-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecd75-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ecd75-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/managementActions/{managementActionId}/apply
```

## <a name="request-headers"></a><span data-ttu-id="ecd75-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ecd75-122">Request headers</span></span>
|<span data-ttu-id="ecd75-123">Имя</span><span class="sxs-lookup"><span data-stu-id="ecd75-123">Name</span></span>|<span data-ttu-id="ecd75-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ecd75-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ecd75-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ecd75-125">Authorization</span></span>|<span data-ttu-id="ecd75-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecd75-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ecd75-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ecd75-128">Content-Type</span></span>|<span data-ttu-id="ecd75-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecd75-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecd75-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ecd75-131">Request body</span></span>
<span data-ttu-id="ecd75-132">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ecd75-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ecd75-133">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="ecd75-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ecd75-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="ecd75-134">Parameter</span></span>|<span data-ttu-id="ecd75-135">Тип</span><span class="sxs-lookup"><span data-stu-id="ecd75-135">Type</span></span>|<span data-ttu-id="ecd75-136">Описание</span><span class="sxs-lookup"><span data-stu-id="ecd75-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecd75-137">tenantId</span><span class="sxs-lookup"><span data-stu-id="ecd75-137">tenantId</span></span>|<span data-ttu-id="ecd75-138">String</span><span class="sxs-lookup"><span data-stu-id="ecd75-138">String</span></span>|<span data-ttu-id="ecd75-139">Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="ecd75-139">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|
|<span data-ttu-id="ecd75-140">tenantGroupId</span><span class="sxs-lookup"><span data-stu-id="ecd75-140">tenantGroupId</span></span>|<span data-ttu-id="ecd75-141">String</span><span class="sxs-lookup"><span data-stu-id="ecd75-141">String</span></span>|<span data-ttu-id="ecd75-142">Идентификатор группы клиента.</span><span class="sxs-lookup"><span data-stu-id="ecd75-142">The identifier of the tenant group.</span></span>|
|<span data-ttu-id="ecd75-143">managementTemplateId</span><span class="sxs-lookup"><span data-stu-id="ecd75-143">managementTemplateId</span></span>|<span data-ttu-id="ecd75-144">String</span><span class="sxs-lookup"><span data-stu-id="ecd75-144">String</span></span>|<span data-ttu-id="ecd75-145">Идентификатор шаблона [управления](../resources/managedtenants-managementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="ecd75-145">The identifier of the [management template](../resources/managedtenants-managementtemplate.md).</span></span>|

## <a name="response"></a><span data-ttu-id="ecd75-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecd75-146">Response</span></span>

<span data-ttu-id="ecd75-147">В случае успешного выполнения это действие возвращает код ответа и `200 OK` [управлениеActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ecd75-147">If successful, this action returns a `200 OK` response code and a [managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ecd75-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="ecd75-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ecd75-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecd75-149">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "managementaction_apply"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActions/{managementActionId}/apply
Content-Type: application/json
Content-length: 95

{
  "tenantId": "String",
  "tenantGroupId": "String",
  "managementTemplateId": "String"
}
```

### <a name="response"></a><span data-ttu-id="ecd75-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecd75-150">Response</span></span>
><span data-ttu-id="ecd75-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ecd75-151">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "managementTemplateId": "e2cadc41-a08f-45e7-8eb1-942d224dfb9a",
  "managementActionId": "b22a4713-8428-4952-8cac-d48962ecbdc9",
  "status": "completed",
  "workloadActionDeploymentStatuses": [
    {
      "actionId": "46b80b42-06c7-45b4-b6fb-aa0aecace87b",
      "status": "completed",
      "deployedPolicyId": null,
      "lastDeploymentDateTime": "2021-07-11T19:35:10.4463799Z",
      "error": null
    }
  ]
}
```
