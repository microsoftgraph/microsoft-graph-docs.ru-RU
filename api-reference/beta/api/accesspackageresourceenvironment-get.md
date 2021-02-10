---
title: Get accessPackageResourceEnvironment
description: Чтение свойств и связей объекта accessPackageResourceEnvironment.
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0169ad18a24ff27392c5679f91dfaecd43d76567
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176301"
---
# <a name="get-accesspackageresourceenvironment"></a><span data-ttu-id="5969d-103">Get accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="5969d-103">Get accessPackageResourceEnvironment</span></span>
<span data-ttu-id="5969d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5969d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5969d-105">Чтение свойств и связей объекта [accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)</span><span class="sxs-lookup"><span data-stu-id="5969d-105">Read the properties and relationships of an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5969d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5969d-106">Permissions</span></span>
<span data-ttu-id="5969d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5969d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5969d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5969d-109">Permission type</span></span>|<span data-ttu-id="5969d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5969d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5969d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5969d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5969d-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5969d-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="5969d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5969d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5969d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5969d-114">Not supported.</span></span>|
|<span data-ttu-id="5969d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5969d-115">Application</span></span>|<span data-ttu-id="5969d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5969d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5969d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5969d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageResourceEnvironments/{accessPackageResourceEnvironmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5969d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5969d-118">Optional query parameters</span></span>
<span data-ttu-id="5969d-119">В настоящее время этот метод не поддерживает [параметры запросов OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="5969d-119">This method does not currently support [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5969d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5969d-120">Request headers</span></span>
|<span data-ttu-id="5969d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5969d-121">Name</span></span>|<span data-ttu-id="5969d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5969d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5969d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5969d-123">Authorization</span></span>|<span data-ttu-id="5969d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5969d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5969d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5969d-126">Request body</span></span>
<span data-ttu-id="5969d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5969d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5969d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5969d-128">Response</span></span>

<span data-ttu-id="5969d-129">В случае успешного выполнения этот метод возвращает код отклика и объект `200 OK` [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5969d-129">If successful, this method returns a `200 OK` response code and an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5969d-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="5969d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5969d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5969d-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5969d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5969d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceenvironment"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceEnvironments/{accessPackageResourceEnvironmentId}
```
# <a name="c"></a>[<span data-ttu-id="5969d-133">C#</span><span class="sxs-lookup"><span data-stu-id="5969d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5969d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5969d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5969d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5969d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5969d-136">Java</span><span class="sxs-lookup"><span data-stu-id="5969d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5969d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5969d-137">Response</span></span>
<span data-ttu-id="5969d-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5969d-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceEnvironment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceEnvironments/$entity",
    "id": "615f2218-678f-471f-a60a-02c2f4f80c57",
    "displayName": "https://contoso.sharepoint.com/",
    "description": "GeoLocation: , RootSiteUrl: https://contoso.sharepoint.com/, TenantAdminUrl: https://contoso-admin.sharepoint.com/",
    "originSystem": "SharePointOnline",
    "originId": "https://contoso-admin.sharepoint.com/",
    "isDefaultEnvironment": false,
    "connectionInfo": {
        "url": "https://contoso-admin.sharepoint.com/"
    }
}
```

