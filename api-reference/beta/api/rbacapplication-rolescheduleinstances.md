---
title: 'rbacApplication: roleScheduleInstances'
description: Извлечение обеих ролейAssignmentScheduleInstances и roleEligibilityScheduleInstances.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 497b29892bb510aec9763cab21ce8f06518a2eee
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679675"
---
# <a name="rbacapplication-rolescheduleinstances"></a><span data-ttu-id="ca2e1-103">rbacApplication: roleScheduleInstances</span><span class="sxs-lookup"><span data-stu-id="ca2e1-103">rbacApplication: roleScheduleInstances</span></span>
<span data-ttu-id="ca2e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca2e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca2e1-105">Извлечение обеих ролейAssignmentScheduleInstances и roleEligibilityScheduleInstances.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-105">Retrieve both roleAssignmentScheduleInstances and roleEligibilityScheduleInstances.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca2e1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca2e1-106">Permissions</span></span>
<span data-ttu-id="ca2e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca2e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca2e1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca2e1-109">Permission type</span></span>|<span data-ttu-id="ca2e1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca2e1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca2e1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca2e1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ca2e1-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="ca2e1-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="ca2e1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca2e1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca2e1-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ca2e1-114">Not supported</span></span>|
|<span data-ttu-id="ca2e1-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ca2e1-115">Application</span></span>|<span data-ttu-id="ca2e1-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="ca2e1-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca2e1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca2e1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleScheduleInstances
```

## <a name="query-parameters"></a><span data-ttu-id="ca2e1-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="ca2e1-118">Query parameters</span></span>
<span data-ttu-id="ca2e1-119">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ca2e1-120">В следующей таблице показаны параметры запроса, которые можно использовать с помощью этого метода.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-120">The following table shows the query parameters that can be used with this method.</span></span>

|<span data-ttu-id="ca2e1-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="ca2e1-121">Parameter</span></span>|<span data-ttu-id="ca2e1-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ca2e1-122">Type</span></span>|<span data-ttu-id="ca2e1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ca2e1-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca2e1-124">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="ca2e1-124">directoryScopeId</span></span>|<span data-ttu-id="ca2e1-125">String</span><span class="sxs-lookup"><span data-stu-id="ca2e1-125">String</span></span>|<span data-ttu-id="ca2e1-126">Id объекта каталога, который представляет область назначения.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-126">Id of the directory object that represents the scope of the assignment.</span></span> <span data-ttu-id="ca2e1-127">Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-127">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="ca2e1-128">Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-128">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="ca2e1-129">Области приложений — это области, которые определяются и понимаются только этим приложением.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-129">App scopes are scopes that are defined and understood by this application only.</span></span> |
|<span data-ttu-id="ca2e1-130">appScopeId</span><span class="sxs-lookup"><span data-stu-id="ca2e1-130">appScopeId</span></span>|<span data-ttu-id="ca2e1-131">String</span><span class="sxs-lookup"><span data-stu-id="ca2e1-131">String</span></span>|<span data-ttu-id="ca2e1-132">Id конкретной области приложения.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-132">Id of the app specific scope.</span></span> <span data-ttu-id="ca2e1-133">Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-133">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="ca2e1-134">Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-134">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="ca2e1-135">Используйте "/" для области для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-135">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="ca2e1-136">Области приложений — это области, которые определяются и понимаются только этим приложением.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-136">App scopes are scopes that are defined and understood by this application only.</span></span> |
|<span data-ttu-id="ca2e1-137">principalId</span><span class="sxs-lookup"><span data-stu-id="ca2e1-137">principalId</span></span>|<span data-ttu-id="ca2e1-138">String</span><span class="sxs-lookup"><span data-stu-id="ca2e1-138">String</span></span>|<span data-ttu-id="ca2e1-139">Objectid основного, к которому относятся графики.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-139">Objectid of the principal to which the schedules belong.</span></span> |
|<span data-ttu-id="ca2e1-140">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="ca2e1-140">roleDefinitionId</span></span>|<span data-ttu-id="ca2e1-141">String</span><span class="sxs-lookup"><span data-stu-id="ca2e1-141">String</span></span>|<span data-ttu-id="ca2e1-142">ID единогоRoleDefinition для назначения.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-142">ID of the unifiedRoleDefinition for the assignment.</span></span> <span data-ttu-id="ca2e1-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-143">Read only.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="ca2e1-144">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca2e1-144">Request headers</span></span>
|<span data-ttu-id="ca2e1-145">Имя</span><span class="sxs-lookup"><span data-stu-id="ca2e1-145">Name</span></span>|<span data-ttu-id="ca2e1-146">Описание</span><span class="sxs-lookup"><span data-stu-id="ca2e1-146">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ca2e1-147">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca2e1-147">Authorization</span></span>|<span data-ttu-id="ca2e1-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca2e1-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca2e1-150">Request body</span></span>
<span data-ttu-id="ca2e1-151">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca2e1-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca2e1-152">Response</span></span>

<span data-ttu-id="ca2e1-153">В случае успешной работы этот метод возвращает код ответа и `200 OK` [унифицированную коллекциюRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-153">If successful, this method returns a `200 OK` response code and a [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ca2e1-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="ca2e1-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ca2e1-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca2e1-155">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ca2e1-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca2e1-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rbacapplication_rolescheduleinstances"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleScheduleInstances(directoryScopeId='parameterValue',appScopeId='parameterValue',principalId='parameterValue',roleDefinitionId='parameterValue')
```
# <a name="c"></a>[<span data-ttu-id="ca2e1-157">C#</span><span class="sxs-lookup"><span data-stu-id="ca2e1-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rbacapplication-rolescheduleinstances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca2e1-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca2e1-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rbacapplication-rolescheduleinstances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca2e1-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca2e1-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rbacapplication-rolescheduleinstances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca2e1-160">Java</span><span class="sxs-lookup"><span data-stu-id="ca2e1-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rbacapplication-rolescheduleinstances-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ca2e1-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca2e1-161">Response</span></span>
<span data-ttu-id="ca2e1-162">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ca2e1-162">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleScheduleInstanceBase)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.Identity.Governance.Common.Data.ExternalModels.V1.unifiedRoleScheduleInstanceBase",
      "id": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "principalId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "roleDefinitionId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "directoryScopeId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "appScopeId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea"
    }
  ]
}
```
