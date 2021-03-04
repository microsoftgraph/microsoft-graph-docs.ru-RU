---
title: Get governanceResource
description: Извлечение свойств и связей объекта governanceResource.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 83e41655dd08307f50b0f21f05d9c3b9975de0b2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435992"
---
# <a name="get-governanceresource"></a><span data-ttu-id="29ec7-103">Get governanceResource</span><span class="sxs-lookup"><span data-stu-id="29ec7-103">Get governanceResource</span></span>

<span data-ttu-id="29ec7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29ec7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29ec7-105">Извлечение свойств и связей объекта [governanceResource.](../resources/governanceresource.md)</span><span class="sxs-lookup"><span data-stu-id="29ec7-105">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="29ec7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29ec7-106">Permissions</span></span>
<span data-ttu-id="29ec7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="29ec7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="29ec7-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="29ec7-109">Azure resources</span></span>

| <span data-ttu-id="29ec7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29ec7-110">Permission type</span></span> | <span data-ttu-id="29ec7-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29ec7-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="29ec7-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29ec7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="29ec7-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="29ec7-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="29ec7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29ec7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29ec7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29ec7-115">Not supported.</span></span> |
| <span data-ttu-id="29ec7-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="29ec7-116">Application</span></span> | <span data-ttu-id="29ec7-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="29ec7-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="29ec7-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="29ec7-118">Azure AD</span></span>

| <span data-ttu-id="29ec7-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29ec7-119">Permission type</span></span> | <span data-ttu-id="29ec7-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29ec7-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="29ec7-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29ec7-121">Delegated (work or school account)</span></span> | <span data-ttu-id="29ec7-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="29ec7-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="29ec7-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29ec7-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29ec7-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29ec7-124">Not supported.</span></span> |
| <span data-ttu-id="29ec7-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="29ec7-125">Application</span></span> | <span data-ttu-id="29ec7-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="29ec7-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="29ec7-127">Группы</span><span class="sxs-lookup"><span data-stu-id="29ec7-127">Groups</span></span>

|<span data-ttu-id="29ec7-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29ec7-128">Permission type</span></span> | <span data-ttu-id="29ec7-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29ec7-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="29ec7-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29ec7-130">Delegated (work or school account)</span></span> | <span data-ttu-id="29ec7-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="29ec7-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="29ec7-132">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29ec7-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29ec7-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29ec7-133">Not supported.</span></span> |
| <span data-ttu-id="29ec7-134">Приложение</span><span class="sxs-lookup"><span data-stu-id="29ec7-134">Application</span></span> | <span data-ttu-id="29ec7-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="29ec7-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="29ec7-136">Помимо области разрешений этот API требует, чтобы у запросителя было как минимум одно назначение ролей на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="29ec7-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="29ec7-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29ec7-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="29ec7-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="29ec7-138">Optional query parameters</span></span>
<span data-ttu-id="29ec7-139">Этот метод **поддерживает** только  `$select` `$expand` [параметры запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="29ec7-139">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29ec7-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29ec7-140">Request headers</span></span>
| <span data-ttu-id="29ec7-141">Имя</span><span class="sxs-lookup"><span data-stu-id="29ec7-141">Name</span></span>      |<span data-ttu-id="29ec7-142">Описание</span><span class="sxs-lookup"><span data-stu-id="29ec7-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="29ec7-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="29ec7-143">Authorization</span></span>  | <span data-ttu-id="29ec7-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="29ec7-144">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="29ec7-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29ec7-145">Request body</span></span>
<span data-ttu-id="29ec7-146">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="29ec7-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="29ec7-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="29ec7-147">Response</span></span>
<span data-ttu-id="29ec7-148">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект governanceResource](../resources/governanceresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="29ec7-148">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29ec7-149">Пример</span><span class="sxs-lookup"><span data-stu-id="29ec7-149">Example</span></span>
<span data-ttu-id="29ec7-150">В этом примере показано, как получить сведения о подписке Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span><span class="sxs-lookup"><span data-stu-id="29ec7-150">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="29ec7-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="29ec7-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="29ec7-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="29ec7-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 459

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceResources/$entity",
    "id": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",
    "type": "subscription",
    "displayName": "Wingtip Toys - Prod",
    "status": "Active",
    "registeredDateTime": "2018-04-05T22:30:37.13Z",
    "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


