---
title: Get governanceRoleDefinition
description: Извлечение свойств и связей управленияRoleDefinition.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 97d3ed248d5a808cf57edf5f18cc37cc07e44bf7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435842"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="1f4ab-103">Get governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1f4ab-103">Get governanceRoleDefinition</span></span>

<span data-ttu-id="1f4ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f4ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f4ab-105">Извлечение свойств и связей [управленияRoleDefinition](../resources/governanceroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="1f4ab-105">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1f4ab-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f4ab-106">Permissions</span></span>
<span data-ttu-id="1f4ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="1f4ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="1f4ab-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="1f4ab-109">Azure resources</span></span>

| <span data-ttu-id="1f4ab-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f4ab-110">Permission type</span></span> | <span data-ttu-id="1f4ab-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f4ab-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="1f4ab-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f4ab-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1f4ab-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="1f4ab-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="1f4ab-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f4ab-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f4ab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f4ab-115">Not supported.</span></span> |
| <span data-ttu-id="1f4ab-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="1f4ab-116">Application</span></span> | <span data-ttu-id="1f4ab-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="1f4ab-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="1f4ab-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="1f4ab-118">Azure AD</span></span>

| <span data-ttu-id="1f4ab-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f4ab-119">Permission type</span></span> | <span data-ttu-id="1f4ab-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f4ab-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="1f4ab-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f4ab-121">Delegated (work or school account)</span></span> | <span data-ttu-id="1f4ab-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="1f4ab-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="1f4ab-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f4ab-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f4ab-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f4ab-124">Not supported.</span></span> |
| <span data-ttu-id="1f4ab-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="1f4ab-125">Application</span></span> | <span data-ttu-id="1f4ab-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="1f4ab-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="1f4ab-127">Группы</span><span class="sxs-lookup"><span data-stu-id="1f4ab-127">Groups</span></span>

|<span data-ttu-id="1f4ab-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f4ab-128">Permission type</span></span> | <span data-ttu-id="1f4ab-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f4ab-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="1f4ab-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f4ab-130">Delegated (work or school account)</span></span> | <span data-ttu-id="1f4ab-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="1f4ab-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="1f4ab-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f4ab-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f4ab-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f4ab-133">Not supported.</span></span> |
| <span data-ttu-id="1f4ab-134">Приложение</span><span class="sxs-lookup"><span data-stu-id="1f4ab-134">Application</span></span> | <span data-ttu-id="1f4ab-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="1f4ab-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="1f4ab-136">Помимо области разрешений, этот API требует, чтобы у запросителя было по крайней мере одно назначение ролей на ресурсе, которому принадлежит [governanceRoleDefinition.](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f4ab-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="1f4ab-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f4ab-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1f4ab-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1f4ab-138">Optional query parameters</span></span>
<span data-ttu-id="1f4ab-139">Этот метод **не поддерживает** [параметры запроса OData для](/graph/query-parameters) настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1f4ab-139">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f4ab-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f4ab-140">Request headers</span></span>
| <span data-ttu-id="1f4ab-141">Имя</span><span class="sxs-lookup"><span data-stu-id="1f4ab-141">Name</span></span>      |<span data-ttu-id="1f4ab-142">Описание</span><span class="sxs-lookup"><span data-stu-id="1f4ab-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1f4ab-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f4ab-143">Authorization</span></span>  | <span data-ttu-id="1f4ab-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1f4ab-144">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="1f4ab-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f4ab-145">Request body</span></span>
<span data-ttu-id="1f4ab-146">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f4ab-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1f4ab-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f4ab-147">Response</span></span>
<span data-ttu-id="1f4ab-148">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект governanceRoleDefinition](../resources/governanceroledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1f4ab-148">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f4ab-149">Пример</span><span class="sxs-lookup"><span data-stu-id="1f4ab-149">Example</span></span>
<span data-ttu-id="1f4ab-150">В этом примере показано, как получить сведения об определении роли DNS Zone Contributor в подписке Wingtip Toys - Prod.</span><span class="sxs-lookup"><span data-stu-id="1f4ab-150">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="1f4ab-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f4ab-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="1f4ab-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f4ab-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 174

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleDefinitions/$entity",
    "id": "00efc9e0-1b96-4e9a-99a3-a3df0735cf88",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/befefa01-2a29-4197-83a8-272ff33ce314",
    "templateId": "befefa01-2a29-4197-83a8-272ff33ce314",
    "displayName": "DNS Zone Contributor"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


