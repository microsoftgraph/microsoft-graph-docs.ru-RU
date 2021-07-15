---
title: Список credentialUserRegistrationsSummaries
description: Получите список объектов credentialUserRegistrationsSummary и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 0b6df505752378f35f1594fac7d59239bb9d0dfd
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442980"
---
# <a name="list-credentialuserregistrationssummaries"></a><span data-ttu-id="20338-103">Список credentialUserRegistrationsSummaries</span><span class="sxs-lookup"><span data-stu-id="20338-103">List credentialUserRegistrationsSummaries</span></span>
<span data-ttu-id="20338-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="20338-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20338-105">Получите список объектов [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="20338-105">Get a list of the [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="20338-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="20338-106">Permissions</span></span>
<span data-ttu-id="20338-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20338-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20338-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20338-109">Permission type</span></span>|<span data-ttu-id="20338-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20338-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20338-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20338-111">Delegated (work or school account)</span></span>|<span data-ttu-id="20338-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="20338-112">Reports.Read.All</span></span>|
|<span data-ttu-id="20338-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20338-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20338-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20338-114">Not supported.</span></span>|
|<span data-ttu-id="20338-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20338-115">Application</span></span>|<span data-ttu-id="20338-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20338-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20338-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20338-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/credentialUserRegistrationsSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20338-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="20338-118">Optional query parameters</span></span>
<span data-ttu-id="20338-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="20338-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20338-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20338-120">Request headers</span></span>
|<span data-ttu-id="20338-121">Имя</span><span class="sxs-lookup"><span data-stu-id="20338-121">Name</span></span>|<span data-ttu-id="20338-122">Описание</span><span class="sxs-lookup"><span data-stu-id="20338-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="20338-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20338-123">Authorization</span></span>|<span data-ttu-id="20338-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20338-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20338-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20338-126">Request body</span></span>
<span data-ttu-id="20338-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="20338-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20338-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="20338-128">Response</span></span>

<span data-ttu-id="20338-129">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="20338-129">If successful, this method returns a `200 OK` response code and a collection of [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20338-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="20338-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="20338-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="20338-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="20338-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="20338-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_credentialuserregistrationssummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/credentialUserRegistrationsSummaries
```
# <a name="c"></a>[<span data-ttu-id="20338-133">C#</span><span class="sxs-lookup"><span data-stu-id="20338-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-credentialuserregistrationssummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20338-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20338-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-credentialuserregistrationssummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20338-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20338-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-credentialuserregistrationssummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20338-136">Java</span><span class="sxs-lookup"><span data-stu-id="20338-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-credentialuserregistrationssummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="20338-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="20338-137">Response</span></span>
><span data-ttu-id="20338-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="20338-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.credentialUserRegistrationsSummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#credentialUserRegistrationsSummaries",
  "value": [
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320",
      "mfaAndSsprCapableUserCount": 2,
      "ssprEnabledUserCount": 9,
      "mfaRegisteredUserCount": 3,
      "ssprRegisteredUserCount": 2,
      "totalUserCount": 9,
      "securityDefaultsEnabled": false,
      "mfaConditionalAccessPolicyState": "enabled",
      "lastRefreshedDateTime": "2021-07-11T09:58:11.5730661Z",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantDisplayName": "Consolidated Messenger"
    },
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b",
      "mfaAndSsprCapableUserCount": 0,
      "ssprEnabledUserCount": 1,
      "mfaRegisteredUserCount": 0,
      "ssprRegisteredUserCount": 0,
      "totalUserCount": 7,
      "securityDefaultsEnabled": false,
      "mfaConditionalAccessPolicyState": "enabledForReportingButNotEnforced",
      "lastRefreshedDateTime": "2021-07-11T11:15:52.9375367Z",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee"
    }
  ]
}
```
