---
title: Управление спискамиRoleDefinitions
description: Получите коллекцию governanceRoleDefinitions на ресурсе.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 6e7d6876a9877a1bf8d146086e3aac3ec74ad60d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435814"
---
# <a name="list-governanceroledefinitions"></a><span data-ttu-id="63ad6-103">Управление спискамиRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="63ad6-103">List governanceRoleDefinitions</span></span>

<span data-ttu-id="63ad6-104">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="63ad6-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="63ad6-105">Получите коллекцию [governanceRoleDefinitions на](../resources/governanceroledefinition.md) ресурсе.</span><span class="sxs-lookup"><span data-stu-id="63ad6-105">Get a collection of [governanceRoleDefinitions](../resources/governanceroledefinition.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="63ad6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63ad6-106">Permissions</span></span>
<span data-ttu-id="63ad6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="63ad6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="63ad6-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="63ad6-109">Azure resources</span></span>

| <span data-ttu-id="63ad6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63ad6-110">Permission type</span></span> | <span data-ttu-id="63ad6-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63ad6-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="63ad6-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63ad6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="63ad6-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="63ad6-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="63ad6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63ad6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63ad6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63ad6-115">Not supported.</span></span> |
| <span data-ttu-id="63ad6-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="63ad6-116">Application</span></span> | <span data-ttu-id="63ad6-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="63ad6-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="63ad6-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="63ad6-118">Azure AD</span></span>

| <span data-ttu-id="63ad6-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63ad6-119">Permission type</span></span> | <span data-ttu-id="63ad6-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63ad6-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="63ad6-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63ad6-121">Delegated (work or school account)</span></span> | <span data-ttu-id="63ad6-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="63ad6-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="63ad6-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63ad6-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63ad6-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63ad6-124">Not supported.</span></span> |
| <span data-ttu-id="63ad6-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="63ad6-125">Application</span></span> | <span data-ttu-id="63ad6-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="63ad6-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="63ad6-127">Группы</span><span class="sxs-lookup"><span data-stu-id="63ad6-127">Groups</span></span>

|<span data-ttu-id="63ad6-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63ad6-128">Permission type</span></span> | <span data-ttu-id="63ad6-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63ad6-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="63ad6-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63ad6-130">Delegated (work or school account)</span></span> | <span data-ttu-id="63ad6-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="63ad6-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="63ad6-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63ad6-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63ad6-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63ad6-133">Not supported.</span></span> |
| <span data-ttu-id="63ad6-134">Приложение</span><span class="sxs-lookup"><span data-stu-id="63ad6-134">Application</span></span> | <span data-ttu-id="63ad6-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="63ad6-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="63ad6-136">Помимо области разрешений этот API требует, чтобы у запросителя было как минимум одно назначение ролей на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="63ad6-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="63ad6-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63ad6-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions
GET /privilegedAccess/azureResources/roleDefinitions?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="63ad6-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="63ad6-138">Optional query parameters</span></span>
<span data-ttu-id="63ad6-139">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="63ad6-139">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63ad6-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63ad6-140">Request headers</span></span>
| <span data-ttu-id="63ad6-141">Имя</span><span class="sxs-lookup"><span data-stu-id="63ad6-141">Name</span></span>      |<span data-ttu-id="63ad6-142">Описание</span><span class="sxs-lookup"><span data-stu-id="63ad6-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="63ad6-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63ad6-143">Authorization</span></span>  | <span data-ttu-id="63ad6-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="63ad6-144">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="63ad6-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63ad6-145">Request body</span></span>
<span data-ttu-id="63ad6-146">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="63ad6-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="63ad6-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="63ad6-147">Response</span></span>
<span data-ttu-id="63ad6-148">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` объектов [governanceRoleDefinition](../resources/governanceroledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="63ad6-148">If successful, this method returns a `200 OK` response code and collection of [governanceRoleDefinition](../resources/governanceroledefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="63ad6-149">Пример</span><span class="sxs-lookup"><span data-stu-id="63ad6-149">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinitions"
}-->
<span data-ttu-id="63ad6-150">В этом примере показано, как получить все определения ролей подписки Wingtip Toys - Prod.</span><span class="sxs-lookup"><span data-stu-id="63ad6-150">This example shows how to get all role definitions of the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="63ad6-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="63ad6-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions  
```
##### <a name="response"></a><span data-ttu-id="63ad6-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="63ad6-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleDefinition",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 21906

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleDefinitions",
    "value": [
        {
            "id": "00efc9e0-1b96-4e9a-99a3-a3df0735cf88",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/befefa01-2a29-4197-83a8-272ff33ce314",
            "templateId": "befefa01-2a29-4197-83a8-272ff33ce314",
            "displayName": "DNS Zone Contributor"
        },
        {
            "id": "051f7264-a992-429a-b345-90415af9f917",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/c12c1c16-33a1-487b-954d-41c89c60f349",
            "templateId": "c12c1c16-33a1-487b-954d-41c89c60f349",
            "displayName": "Reader and Data Access"
        },
        {
            "id": "0789c03d-445d-40ab-aed3-d110a98146c7",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/5d28c62d-5b37-4476-8438-e587778df237",
            "templateId": "5d28c62d-5b37-4476-8438-e587778df237",
            "displayName": "New Relic APM Account Contributor"
        },
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List governanceRoleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


