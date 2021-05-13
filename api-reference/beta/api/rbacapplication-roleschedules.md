---
title: 'rbacApplication: roleSchedules'
description: Извлечение обеих ролейAssignmentSchedules и roleEligibilitySchedules.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d8bd07d0d029182c163322d2b93ea25a38d94cfd
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474698"
---
# <a name="rbacapplication-roleschedules"></a><span data-ttu-id="6fb9a-103">rbacApplication: roleSchedules</span><span class="sxs-lookup"><span data-stu-id="6fb9a-103">rbacApplication: roleSchedules</span></span>
<span data-ttu-id="6fb9a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fb9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fb9a-105">Извлечение обеих ролейAssignmentSchedules и roleEligibilitySchedules.</span><span class="sxs-lookup"><span data-stu-id="6fb9a-105">Retrieve both roleAssignmentSchedules and roleEligibilitySchedules.</span></span>

## <a name="permissions"></a><span data-ttu-id="6fb9a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6fb9a-106">Permissions</span></span>
<span data-ttu-id="6fb9a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fb9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fb9a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6fb9a-109">Permission type</span></span>|<span data-ttu-id="6fb9a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6fb9a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fb9a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6fb9a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6fb9a-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="6fb9a-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="6fb9a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6fb9a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fb9a-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6fb9a-114">Not supported</span></span>|
|<span data-ttu-id="6fb9a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6fb9a-115">Application</span></span>|<span data-ttu-id="6fb9a-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="6fb9a-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fb9a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6fb9a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleSchedules
```

## <a name="function-parameters"></a><span data-ttu-id="6fb9a-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="6fb9a-118">Function parameters</span></span>
<span data-ttu-id="6fb9a-119">В следующей таблице показаны параметры запроса, которые можно использовать с помощью этого метода.</span><span class="sxs-lookup"><span data-stu-id="6fb9a-119">The following table shows the query parameters that can be used with this method.</span></span>

|<span data-ttu-id="6fb9a-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="6fb9a-120">Parameter</span></span>|<span data-ttu-id="6fb9a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6fb9a-121">Type</span></span>|<span data-ttu-id="6fb9a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6fb9a-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fb9a-123">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="6fb9a-123">directoryScopeId</span></span>|<span data-ttu-id="6fb9a-124">String</span><span class="sxs-lookup"><span data-stu-id="6fb9a-124">String</span></span>|<span data-ttu-id="6fb9a-125">Id объекта каталога, который представляет область назначения.</span><span class="sxs-lookup"><span data-stu-id="6fb9a-125">Id of the directory object that represents the scope of the assignment.</span></span> <span data-ttu-id="6fb9a-126">Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="6fb9a-126">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="6fb9a-127">Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям.</span><span class="sxs-lookup"><span data-stu-id="6fb9a-127">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="6fb9a-128">Области приложений — это области, которые определяются и понимаются только этим приложением.</span><span class="sxs-lookup"><span data-stu-id="6fb9a-128">App scopes are scopes that are defined and understood by this application only.</span></span> |
|<span data-ttu-id="6fb9a-129">appScopeId</span><span class="sxs-lookup"><span data-stu-id="6fb9a-129">appScopeId</span></span>|<span data-ttu-id="6fb9a-130">String</span><span class="sxs-lookup"><span data-stu-id="6fb9a-130">String</span></span>|<span data-ttu-id="6fb9a-131">Id конкретной области приложения.</span><span class="sxs-lookup"><span data-stu-id="6fb9a-131">Id of the app specific scope.</span></span> <span data-ttu-id="6fb9a-132">Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="6fb9a-132">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="6fb9a-133">Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям.</span><span class="sxs-lookup"><span data-stu-id="6fb9a-133">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="6fb9a-134">Используйте "/" для области для клиента.</span><span class="sxs-lookup"><span data-stu-id="6fb9a-134">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="6fb9a-135">Области приложений — это области, которые определяются и понимаются только этим приложением.</span><span class="sxs-lookup"><span data-stu-id="6fb9a-135">App scopes are scopes that are defined and understood by this application only.</span></span> |
|<span data-ttu-id="6fb9a-136">principalId</span><span class="sxs-lookup"><span data-stu-id="6fb9a-136">principalId</span></span>|<span data-ttu-id="6fb9a-137">String</span><span class="sxs-lookup"><span data-stu-id="6fb9a-137">String</span></span>|<span data-ttu-id="6fb9a-138">Objectid основного, к которому относятся графики.</span><span class="sxs-lookup"><span data-stu-id="6fb9a-138">Objectid of the principal to which the schedules belong.</span></span> |
|<span data-ttu-id="6fb9a-139">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="6fb9a-139">roleDefinitionId</span></span>|<span data-ttu-id="6fb9a-140">String</span><span class="sxs-lookup"><span data-stu-id="6fb9a-140">String</span></span>|<span data-ttu-id="6fb9a-141">ID единогоRoleDefinition для назначения.</span><span class="sxs-lookup"><span data-stu-id="6fb9a-141">ID of the unifiedRoleDefinition for the assignment.</span></span> <span data-ttu-id="6fb9a-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6fb9a-142">Read only.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="6fb9a-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6fb9a-143">Request headers</span></span>
|<span data-ttu-id="6fb9a-144">Имя</span><span class="sxs-lookup"><span data-stu-id="6fb9a-144">Name</span></span>|<span data-ttu-id="6fb9a-145">Описание</span><span class="sxs-lookup"><span data-stu-id="6fb9a-145">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6fb9a-146">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6fb9a-146">Authorization</span></span>|<span data-ttu-id="6fb9a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6fb9a-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fb9a-149">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6fb9a-149">Request body</span></span>
<span data-ttu-id="6fb9a-150">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6fb9a-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fb9a-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fb9a-151">Response</span></span>

<span data-ttu-id="6fb9a-152">В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6fb9a-152">If successful, this method returns a `200 OK` response code and a [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6fb9a-153">Примеры</span><span class="sxs-lookup"><span data-stu-id="6fb9a-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6fb9a-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="6fb9a-154">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6fb9a-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fb9a-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rbacapplication_roleschedules"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleSchedules(directoryScopeId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',appScopeId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',principalId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',roleDefinitionId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea')
```
# <a name="c"></a>[<span data-ttu-id="6fb9a-156">C#</span><span class="sxs-lookup"><span data-stu-id="6fb9a-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rbacapplication-roleschedules-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6fb9a-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fb9a-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rbacapplication-roleschedules-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6fb9a-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fb9a-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rbacapplication-roleschedules-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6fb9a-159">Java</span><span class="sxs-lookup"><span data-stu-id="6fb9a-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rbacapplication-roleschedules-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6fb9a-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fb9a-160">Response</span></span>
<span data-ttu-id="6fb9a-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6fb9a-161">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleScheduleBase)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.Identity.Governance.Common.Data.ExternalModels.V1.unifiedRoleScheduleBase",
      "id": "String (identifier)",
      "principalId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "roleDefinitionId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "directoryScopeId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "appScopeId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "createdUsing": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "createdDateTime": "2020-09-09T21:32:27.91Z",
      "modifiedDateTime": "2020-09-09T21:32:27.91Z",
      "status": "Provisioned"
    }
  ]
}
```
