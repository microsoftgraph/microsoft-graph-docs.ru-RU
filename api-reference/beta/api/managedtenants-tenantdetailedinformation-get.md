---
title: Get tenantDetailedInformation
description: Ознакомьтесь с свойствами и отношениями объекта tenantDetailedInformation.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: a9e771d5391989dd884d77240091ffba4f523353
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441874"
---
# <a name="get-tenantdetailedinformation"></a><span data-ttu-id="60b1b-103">Get tenantDetailedInformation</span><span class="sxs-lookup"><span data-stu-id="60b1b-103">Get tenantDetailedInformation</span></span>
<span data-ttu-id="60b1b-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="60b1b-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60b1b-105">Ознакомьтесь с свойствами и отношениями объекта [tenantDetailedInformation.](../resources/managedtenants-tenantdetailedinformation.md)</span><span class="sxs-lookup"><span data-stu-id="60b1b-105">Read the properties and relationships of a [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="60b1b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60b1b-106">Permissions</span></span>
<span data-ttu-id="60b1b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60b1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60b1b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60b1b-109">Permission type</span></span>|<span data-ttu-id="60b1b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60b1b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60b1b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60b1b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="60b1b-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60b1b-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="60b1b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60b1b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60b1b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60b1b-114">Not supported.</span></span>|
|<span data-ttu-id="60b1b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60b1b-115">Application</span></span>|<span data-ttu-id="60b1b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60b1b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60b1b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60b1b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantsDetailedInformation/{tenantDetailedInformationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="60b1b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="60b1b-118">Optional query parameters</span></span>
<span data-ttu-id="60b1b-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="60b1b-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="60b1b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60b1b-120">Request headers</span></span>
|<span data-ttu-id="60b1b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="60b1b-121">Name</span></span>|<span data-ttu-id="60b1b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="60b1b-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="60b1b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60b1b-123">Authorization</span></span>|<span data-ttu-id="60b1b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60b1b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60b1b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60b1b-126">Request body</span></span>
<span data-ttu-id="60b1b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60b1b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60b1b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="60b1b-128">Response</span></span>

<span data-ttu-id="60b1b-129">В случае успеха этот метод возвращает код отклика и `200 OK` [объект tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="60b1b-129">If successful, this method returns a `200 OK` response code and a [tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60b1b-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="60b1b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="60b1b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="60b1b-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="60b1b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="60b1b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tenantdetailedinformation"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantsDetailedInformation/{tenantDetailedInformationId}
```
# <a name="c"></a>[<span data-ttu-id="60b1b-133">C#</span><span class="sxs-lookup"><span data-stu-id="60b1b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tenantdetailedinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60b1b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60b1b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tenantdetailedinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60b1b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60b1b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tenantdetailedinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="60b1b-136">Java</span><span class="sxs-lookup"><span data-stu-id="60b1b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tenantdetailedinformation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="60b1b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="60b1b-137">Response</span></span>
><span data-ttu-id="60b1b-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="60b1b-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantDetailedInformation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.tenantDetailedInformation",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b",
  "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
  "companyName": "Fourth Coffee",
  "defaultDomainName": "fourthcoffee001.onmicrosoft.com",
  "countryName": "United States",
  "countryCode": "US",
  "city": "Redmond",
  "region": "NA",
  "verticalName": "Software",
  "industryName": "Computer",
  "segmentName": "Service"
}
```
