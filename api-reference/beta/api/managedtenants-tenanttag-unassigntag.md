---
title: 'tenantTag: unassignTag'
description: Un-assigns the tenant tag from the specified managed tenants.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: c4cb34b12c075ee44df36baf57cdd14a6739f2d9
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403117"
---
# <a name="tenanttag-unassigntag"></a><span data-ttu-id="883ba-103">tenantTag: unassignTag</span><span class="sxs-lookup"><span data-stu-id="883ba-103">tenantTag: unassignTag</span></span>
<span data-ttu-id="883ba-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="883ba-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="883ba-105">Un-assigns the tenant tag from the specified managed tenants.</span><span class="sxs-lookup"><span data-stu-id="883ba-105">Un-assigns the tenant tag from the specified managed tenants.</span></span>

## <a name="permissions"></a><span data-ttu-id="883ba-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="883ba-106">Permissions</span></span>
<span data-ttu-id="883ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="883ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="883ba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="883ba-109">Permission type</span></span>|<span data-ttu-id="883ba-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="883ba-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="883ba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="883ba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="883ba-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="883ba-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="883ba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="883ba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="883ba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="883ba-114">Not supported.</span></span>|
|<span data-ttu-id="883ba-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="883ba-115">Application</span></span>|<span data-ttu-id="883ba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="883ba-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="883ba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="883ba-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenantTags/{tenantTagId}/unassignTag
```

## <a name="request-headers"></a><span data-ttu-id="883ba-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="883ba-118">Request headers</span></span>
|<span data-ttu-id="883ba-119">Имя</span><span class="sxs-lookup"><span data-stu-id="883ba-119">Name</span></span>|<span data-ttu-id="883ba-120">Описание</span><span class="sxs-lookup"><span data-stu-id="883ba-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="883ba-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="883ba-121">Authorization</span></span>|<span data-ttu-id="883ba-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="883ba-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="883ba-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="883ba-124">Content-Type</span></span>|<span data-ttu-id="883ba-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="883ba-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="883ba-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="883ba-127">Request body</span></span>
<span data-ttu-id="883ba-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="883ba-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="883ba-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="883ba-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="883ba-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="883ba-130">Parameter</span></span>|<span data-ttu-id="883ba-131">Тип</span><span class="sxs-lookup"><span data-stu-id="883ba-131">Type</span></span>|<span data-ttu-id="883ba-132">Описание</span><span class="sxs-lookup"><span data-stu-id="883ba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="883ba-133">tenantIds</span><span class="sxs-lookup"><span data-stu-id="883ba-133">tenantIds</span></span>|<span data-ttu-id="883ba-134">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="883ba-134">String collection</span></span>|<span data-ttu-id="883ba-135">Коллекция идентификаторов Azure Active Directory для управляемых клиентов.</span><span class="sxs-lookup"><span data-stu-id="883ba-135">The collection of Azure Active Directory tenant identifiers for managed tenants.</span></span>|

## <a name="response"></a><span data-ttu-id="883ba-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="883ba-136">Response</span></span>

<span data-ttu-id="883ba-137">В случае успеха это действие возвращает код отклика и `200 OK` [tenantTag](../resources/managedtenants-tenanttag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="883ba-137">If successful, this action returns a `200 OK` response code and a [tenantTag](../resources/managedtenants-tenanttag.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="883ba-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="883ba-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="883ba-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="883ba-139">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="883ba-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="883ba-140">Response</span></span>
><span data-ttu-id="883ba-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="883ba-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
