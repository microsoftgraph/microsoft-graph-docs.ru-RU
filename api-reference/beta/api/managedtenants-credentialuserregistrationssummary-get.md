---
title: Получите credentialUserRegistrationsSummary
description: Ознакомьтесь с свойствами и отношениями объекта credentialUserRegistrationsSummary.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 1b79d187f54898e1acb78defdead34edf821c965
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440040"
---
# <a name="get-credentialuserregistrationssummary"></a><span data-ttu-id="2b760-103">Получите credentialUserRegistrationsSummary</span><span class="sxs-lookup"><span data-stu-id="2b760-103">Get credentialUserRegistrationsSummary</span></span>
<span data-ttu-id="2b760-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="2b760-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b760-105">Ознакомьтесь с свойствами и отношениями объекта [credentialUserRegistrationsSummary.](../resources/managedtenants-credentialuserregistrationssummary.md)</span><span class="sxs-lookup"><span data-stu-id="2b760-105">Read the properties and relationships of a [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b760-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b760-106">Permissions</span></span>
<span data-ttu-id="2b760-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b760-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b760-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b760-109">Permission type</span></span>|<span data-ttu-id="2b760-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b760-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b760-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b760-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2b760-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b760-112">Reports.Read.All</span></span>|
|<span data-ttu-id="2b760-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b760-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b760-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b760-114">Not supported.</span></span>|
|<span data-ttu-id="2b760-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b760-115">Application</span></span>|<span data-ttu-id="2b760-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b760-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b760-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b760-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/credentialUserRegistrationsSummaries/{credentialUserRegistrationsSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b760-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2b760-118">Optional query parameters</span></span>
<span data-ttu-id="2b760-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="2b760-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b760-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b760-120">Request headers</span></span>
|<span data-ttu-id="2b760-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2b760-121">Name</span></span>|<span data-ttu-id="2b760-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2b760-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2b760-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b760-123">Authorization</span></span>|<span data-ttu-id="2b760-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b760-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b760-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b760-126">Request body</span></span>
<span data-ttu-id="2b760-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b760-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b760-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b760-128">Response</span></span>

<span data-ttu-id="2b760-129">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2b760-129">If successful, this method returns a `200 OK` response code and a [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2b760-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="2b760-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2b760-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b760-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2b760-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b760-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationssummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/credentialUserRegistrationsSummaries/{credentialUserRegistrationsSummaryId}
```
# <a name="c"></a>[<span data-ttu-id="2b760-133">C#</span><span class="sxs-lookup"><span data-stu-id="2b760-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-credentialuserregistrationssummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b760-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b760-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-credentialuserregistrationssummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b760-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b760-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-credentialuserregistrationssummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b760-136">Java</span><span class="sxs-lookup"><span data-stu-id="2b760-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-credentialuserregistrationssummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2b760-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b760-137">Response</span></span>
><span data-ttu-id="2b760-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2b760-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.credentialUserRegistrationsSummary"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.credentialUserRegistrationsSummary",
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
```
