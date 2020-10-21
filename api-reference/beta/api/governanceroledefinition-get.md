---
title: Получение Говернанцероледефинитион
description: Получение свойств и связей объекта Говернанцероледефинитион.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 1e9a2f52ea264f7bbcf3353e68deb9f51378efd1
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634981"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="ca18e-103">Получение Говернанцероледефинитион</span><span class="sxs-lookup"><span data-stu-id="ca18e-103">Get governanceRoleDefinition</span></span>

<span data-ttu-id="ca18e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca18e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca18e-105">Получение свойств и связей объекта [говернанцероледефинитион](../resources/governanceroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ca18e-105">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca18e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca18e-106">Permissions</span></span>
<span data-ttu-id="ca18e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="ca18e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="ca18e-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="ca18e-109">Azure resources</span></span>

| <span data-ttu-id="ca18e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca18e-110">Permission type</span></span> | <span data-ttu-id="ca18e-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca18e-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="ca18e-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca18e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ca18e-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="ca18e-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="ca18e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca18e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca18e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca18e-115">Not supported.</span></span> |
| <span data-ttu-id="ca18e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ca18e-116">Application</span></span> | <span data-ttu-id="ca18e-117">Привилежедакцесс. Read. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="ca18e-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="ca18e-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="ca18e-118">Azure AD</span></span>

| <span data-ttu-id="ca18e-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca18e-119">Permission type</span></span> | <span data-ttu-id="ca18e-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca18e-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="ca18e-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca18e-121">Delegated (work or school account)</span></span> | <span data-ttu-id="ca18e-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="ca18e-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="ca18e-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca18e-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca18e-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca18e-124">Not supported.</span></span> |
| <span data-ttu-id="ca18e-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="ca18e-125">Application</span></span> | <span data-ttu-id="ca18e-126">Привилежедакцесс. Read. AzureAD</span><span class="sxs-lookup"><span data-stu-id="ca18e-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="ca18e-127">Группы</span><span class="sxs-lookup"><span data-stu-id="ca18e-127">Groups</span></span>

|<span data-ttu-id="ca18e-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca18e-128">Permission type</span></span> | <span data-ttu-id="ca18e-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca18e-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="ca18e-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca18e-130">Delegated (work or school account)</span></span> | <span data-ttu-id="ca18e-131">Привилежедакцесс. ReadWrite. Азуреадграупс</span><span class="sxs-lookup"><span data-stu-id="ca18e-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="ca18e-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca18e-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca18e-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca18e-133">Not supported.</span></span> |
| <span data-ttu-id="ca18e-134">Приложение</span><span class="sxs-lookup"><span data-stu-id="ca18e-134">Application</span></span> | <span data-ttu-id="ca18e-135">Привилежедакцесс. Read. Азуреадграупс</span><span class="sxs-lookup"><span data-stu-id="ca18e-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="ca18e-136">Кроме области разрешений, этот API требует, чтобы запрашивающий был иметь по крайней мере одно назначение роли для ресурса, к которому относится [говернанцероледефинитион](../resources/governanceroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="ca18e-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="ca18e-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca18e-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ca18e-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ca18e-138">Optional query parameters</span></span>
<span data-ttu-id="ca18e-139">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ca18e-139">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca18e-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca18e-140">Request headers</span></span>
| <span data-ttu-id="ca18e-141">Имя</span><span class="sxs-lookup"><span data-stu-id="ca18e-141">Name</span></span>      |<span data-ttu-id="ca18e-142">Описание</span><span class="sxs-lookup"><span data-stu-id="ca18e-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ca18e-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca18e-143">Authorization</span></span>  | <span data-ttu-id="ca18e-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ca18e-144">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="ca18e-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca18e-145">Request body</span></span>
<span data-ttu-id="ca18e-146">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ca18e-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ca18e-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca18e-147">Response</span></span>
<span data-ttu-id="ca18e-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [говернанцероледефинитион](../resources/governanceroledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca18e-148">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ca18e-149">Пример</span><span class="sxs-lookup"><span data-stu-id="ca18e-149">Example</span></span>
<span data-ttu-id="ca18e-150">В этом примере показано, как получить сведения об участниках определения роли DNS в подписке Wingtip Toys-произ.</span><span class="sxs-lookup"><span data-stu-id="ca18e-150">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="ca18e-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca18e-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="ca18e-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca18e-152">Response</span></span>
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


