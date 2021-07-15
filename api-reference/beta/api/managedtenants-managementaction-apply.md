---
title: 'managementAction: применить'
description: Применяет действие управления к определенному управляемому клиенту. При выполнении этой операции будут созданы соответствующие конфигурации и созданы политики. В качестве примера при применении требуемой многофакторной проверки подлинности для действий управления администраторами создается политика условного доступа Azure Active Directory, которая требует многофакторной проверки подлинности для всех пользователей, на которых назначена роль административного каталога.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 801a4e66338dfb53f74d454c4ac6d2eba2c58505
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442194"
---
# <a name="managementaction-apply"></a><span data-ttu-id="45e72-105">managementAction: применить</span><span class="sxs-lookup"><span data-stu-id="45e72-105">managementAction: apply</span></span>
<span data-ttu-id="45e72-106">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="45e72-106">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45e72-107">Применяет действие управления к определенному управляемому клиенту.</span><span class="sxs-lookup"><span data-stu-id="45e72-107">Applies a management action against a specific managed tenant.</span></span> <span data-ttu-id="45e72-108">При выполнении этой операции будут созданы соответствующие конфигурации и созданы политики.</span><span class="sxs-lookup"><span data-stu-id="45e72-108">By performing this operation the appropriate configurations will be made and policies created.</span></span> <span data-ttu-id="45e72-109">В качестве примера при применении требуемой многофакторной проверки подлинности для действий управления администраторами создается политика условного доступа Azure Active Directory, которая требует многофакторной проверки подлинности для всех пользователей, на которых назначена роль административного каталога.</span><span class="sxs-lookup"><span data-stu-id="45e72-109">As example when applying the require multi-factor authentication for admins management action will create an Azure Active Directory conditional access policy that requires multi-factor authentication for all users that have been assigned an administrative directory role.</span></span>

## <a name="permissions"></a><span data-ttu-id="45e72-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45e72-110">Permissions</span></span>
<span data-ttu-id="45e72-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45e72-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45e72-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45e72-113">Permission type</span></span>|<span data-ttu-id="45e72-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45e72-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45e72-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45e72-115">Delegated (work or school account)</span></span>|<span data-ttu-id="45e72-116">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45e72-116">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="45e72-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45e72-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45e72-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45e72-118">Not supported.</span></span>|
|<span data-ttu-id="45e72-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45e72-119">Application</span></span>|<span data-ttu-id="45e72-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45e72-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45e72-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45e72-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/managementActions/{managementActionId}/apply
```

## <a name="request-headers"></a><span data-ttu-id="45e72-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45e72-122">Request headers</span></span>
|<span data-ttu-id="45e72-123">Имя</span><span class="sxs-lookup"><span data-stu-id="45e72-123">Name</span></span>|<span data-ttu-id="45e72-124">Описание</span><span class="sxs-lookup"><span data-stu-id="45e72-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="45e72-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45e72-125">Authorization</span></span>|<span data-ttu-id="45e72-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45e72-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="45e72-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="45e72-128">Content-Type</span></span>|<span data-ttu-id="45e72-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45e72-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45e72-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45e72-131">Request body</span></span>
<span data-ttu-id="45e72-132">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45e72-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="45e72-133">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="45e72-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="45e72-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="45e72-134">Parameter</span></span>|<span data-ttu-id="45e72-135">Тип</span><span class="sxs-lookup"><span data-stu-id="45e72-135">Type</span></span>|<span data-ttu-id="45e72-136">Описание</span><span class="sxs-lookup"><span data-stu-id="45e72-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45e72-137">tenantId</span><span class="sxs-lookup"><span data-stu-id="45e72-137">tenantId</span></span>|<span data-ttu-id="45e72-138">String</span><span class="sxs-lookup"><span data-stu-id="45e72-138">String</span></span>|<span data-ttu-id="45e72-139">Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="45e72-139">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|
|<span data-ttu-id="45e72-140">tenantGroupId</span><span class="sxs-lookup"><span data-stu-id="45e72-140">tenantGroupId</span></span>|<span data-ttu-id="45e72-141">String</span><span class="sxs-lookup"><span data-stu-id="45e72-141">String</span></span>|<span data-ttu-id="45e72-142">Идентификатор группы клиента.</span><span class="sxs-lookup"><span data-stu-id="45e72-142">The identifier of the tenant group.</span></span>|
|<span data-ttu-id="45e72-143">managementTemplateId</span><span class="sxs-lookup"><span data-stu-id="45e72-143">managementTemplateId</span></span>|<span data-ttu-id="45e72-144">String</span><span class="sxs-lookup"><span data-stu-id="45e72-144">String</span></span>|<span data-ttu-id="45e72-145">Идентификатор шаблона [управления](../resources/managedtenants-managementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="45e72-145">The identifier of the [management template](../resources/managedtenants-managementtemplate.md).</span></span>|

## <a name="response"></a><span data-ttu-id="45e72-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="45e72-146">Response</span></span>

<span data-ttu-id="45e72-147">В случае успешного выполнения это действие возвращает код ответа и `200 OK` [управлениеActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="45e72-147">If successful, this action returns a `200 OK` response code and a [managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45e72-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="45e72-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="45e72-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="45e72-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="45e72-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="45e72-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="45e72-151">C#</span><span class="sxs-lookup"><span data-stu-id="45e72-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/managementaction-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45e72-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45e72-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/managementaction-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45e72-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45e72-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/managementaction-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45e72-154">Java</span><span class="sxs-lookup"><span data-stu-id="45e72-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/managementaction-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="45e72-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="45e72-155">Response</span></span>
><span data-ttu-id="45e72-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="45e72-156">**Note:** The response object shown here might be shortened for readability.</span></span>
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
