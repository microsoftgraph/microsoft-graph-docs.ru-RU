---
title: Get riskyUser
description: Ознакомьтесь с свойствами и отношениями объекта riskyUser.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 523e5c3abe471ac2951615411c232517895dce64
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441411"
---
# <a name="get-riskyuser"></a><span data-ttu-id="a6d8e-103">Get riskyUser</span><span class="sxs-lookup"><span data-stu-id="a6d8e-103">Get riskyUser</span></span>
<span data-ttu-id="a6d8e-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="a6d8e-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6d8e-105">Ознакомьтесь с свойствами и отношениями объекта [riskyUser.](../resources/managedtenants-riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="a6d8e-105">Read the properties and relationships of a [riskyUser](../resources/managedtenants-riskyuser.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6d8e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6d8e-106">Permissions</span></span>
<span data-ttu-id="a6d8e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6d8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6d8e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6d8e-109">Permission type</span></span>|<span data-ttu-id="a6d8e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6d8e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6d8e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6d8e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a6d8e-112">IdentityRiskyUser.Read.All, IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6d8e-112">IdentityRiskyUser.Read.All, IdentityRiskyUser.ReadWrite.All</span></span>|
|<span data-ttu-id="a6d8e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6d8e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6d8e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6d8e-114">Not supported.</span></span>|
|<span data-ttu-id="a6d8e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6d8e-115">Application</span></span>|<span data-ttu-id="a6d8e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6d8e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6d8e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6d8e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/riskyUsers/{riskyUserId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6d8e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a6d8e-118">Optional query parameters</span></span>
<span data-ttu-id="a6d8e-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="a6d8e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6d8e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6d8e-120">Request headers</span></span>
|<span data-ttu-id="a6d8e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a6d8e-121">Name</span></span>|<span data-ttu-id="a6d8e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a6d8e-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a6d8e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6d8e-123">Authorization</span></span>|<span data-ttu-id="a6d8e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6d8e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6d8e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6d8e-126">Request body</span></span>
<span data-ttu-id="a6d8e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a6d8e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6d8e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6d8e-128">Response</span></span>

<span data-ttu-id="a6d8e-129">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [riskyUser](../resources/managedtenants-riskyuser.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a6d8e-129">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/managedtenants-riskyuser.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a6d8e-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="a6d8e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a6d8e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6d8e-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a6d8e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6d8e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/riskyUsers/{riskyUserId}
```
# <a name="c"></a>[<span data-ttu-id="a6d8e-133">C#</span><span class="sxs-lookup"><span data-stu-id="a6d8e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6d8e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6d8e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6d8e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6d8e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6d8e-136">Java</span><span class="sxs-lookup"><span data-stu-id="a6d8e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a6d8e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6d8e-137">Response</span></span>
><span data-ttu-id="a6d8e-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a6d8e-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.riskyUser"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.riskyUser",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b_ae8d3a3f-be95-429c-8063-635ccc16e899",
  "userId": "ae8d3a3f-be95-429c-8063-635ccc16e899",
  "userDisplayName": "Cynthia Becker",
  "userPrincipalName": "cynthia@fourthcoffee002.onmicrosoft.com",
  "riskState": "atRisk",
  "riskLevel": "hidden",
  "riskDetail": "hidden",
  "isDeleted": false,
  "riskLastUpdatedDateTime": "2021-06-10T13:58:34.5171907Z",
  "lastRefreshedDateTime": "2021-07-11T11:32:55.2168558Z",
  "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
  "tenantDisplayName": "Fourth Coffee"
}
```
