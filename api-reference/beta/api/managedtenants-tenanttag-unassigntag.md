---
title: 'tenantTag: unassignTag'
description: Un-assigns the tenant tag from the specified managed tenants.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 41a2cc35ea47374ef16131fd6190476bcac77847
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442789"
---
# <a name="tenanttag-unassigntag"></a><span data-ttu-id="ec2ea-103">tenantTag: unassignTag</span><span class="sxs-lookup"><span data-stu-id="ec2ea-103">tenantTag: unassignTag</span></span>
<span data-ttu-id="ec2ea-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="ec2ea-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec2ea-105">Un-assigns the tenant tag from the specified managed tenants.</span><span class="sxs-lookup"><span data-stu-id="ec2ea-105">Un-assigns the tenant tag from the specified managed tenants.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec2ea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec2ea-106">Permissions</span></span>
<span data-ttu-id="ec2ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec2ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec2ea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec2ea-109">Permission type</span></span>|<span data-ttu-id="ec2ea-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec2ea-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec2ea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec2ea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ec2ea-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="ec2ea-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="ec2ea-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec2ea-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec2ea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec2ea-114">Not supported.</span></span>|
|<span data-ttu-id="ec2ea-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec2ea-115">Application</span></span>|<span data-ttu-id="ec2ea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec2ea-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec2ea-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec2ea-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenantTags/{tenantTagId}/unassignTag
```

## <a name="request-headers"></a><span data-ttu-id="ec2ea-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec2ea-118">Request headers</span></span>
|<span data-ttu-id="ec2ea-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ec2ea-119">Name</span></span>|<span data-ttu-id="ec2ea-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ec2ea-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ec2ea-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec2ea-121">Authorization</span></span>|<span data-ttu-id="ec2ea-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec2ea-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ec2ea-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ec2ea-124">Content-Type</span></span>|<span data-ttu-id="ec2ea-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec2ea-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec2ea-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec2ea-127">Request body</span></span>
<span data-ttu-id="ec2ea-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec2ea-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ec2ea-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="ec2ea-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ec2ea-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="ec2ea-130">Parameter</span></span>|<span data-ttu-id="ec2ea-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ec2ea-131">Type</span></span>|<span data-ttu-id="ec2ea-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ec2ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec2ea-133">tenantIds</span><span class="sxs-lookup"><span data-stu-id="ec2ea-133">tenantIds</span></span>|<span data-ttu-id="ec2ea-134">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="ec2ea-134">String collection</span></span>|<span data-ttu-id="ec2ea-135">Коллекция идентификаторов Azure Active Directory для управляемых клиентов.</span><span class="sxs-lookup"><span data-stu-id="ec2ea-135">The collection of Azure Active Directory tenant identifiers for managed tenants.</span></span>|

## <a name="response"></a><span data-ttu-id="ec2ea-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec2ea-136">Response</span></span>

<span data-ttu-id="ec2ea-137">В случае успеха это действие возвращает код отклика и `200 OK` [tenantTag](../resources/managedtenants-tenanttag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ec2ea-137">If successful, this action returns a `200 OK` response code and a [tenantTag](../resources/managedtenants-tenanttag.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ec2ea-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="ec2ea-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ec2ea-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec2ea-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ec2ea-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec2ea-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tenanttag_unassigntag"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}/unassignTag
Content-Type: application/json
Content-length: 41

{
  "tenantIds": [
    "String"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="ec2ea-141">C#</span><span class="sxs-lookup"><span data-stu-id="ec2ea-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tenanttag-unassigntag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec2ea-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec2ea-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tenanttag-unassigntag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec2ea-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec2ea-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tenanttag-unassigntag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec2ea-144">Java</span><span class="sxs-lookup"><span data-stu-id="ec2ea-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tenanttag-unassigntag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ec2ea-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec2ea-145">Response</span></span>
><span data-ttu-id="ec2ea-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ec2ea-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantTags/$entity",
  "id": "2a66c69f-87ec-4fb3-a797-dd500cc3454d",
  "displayName": "Support",
  "description": "Tenants that has purcahsed support",
  "tenants": [],
  "isDeleted": null,
  "createdDateTime": "2021-06-26T13:51:23.3927236Z",
  "createdByUserId": "65ca7649-4ccb-4823-9c39-42bd75191bf8",
  "lastActionDateTime": "2021-07-11T19:57:56.4242898Z",
  "lastActionByUserId": "50bf7bd8-1b3a-4d1d-94c5-86d27e68857f"
}
```
