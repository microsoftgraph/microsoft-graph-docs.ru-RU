---
title: Получите accessPackageResourceEnvironment
description: Ознакомьтесь с свойствами и отношениями объекта accessPackageResourceEnvironment.
author: hanki-microsoft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6ba500b5f20dfb9dbf29054d0015ebe372e3753d
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298371"
---
# <a name="get-accesspackageresourceenvironment"></a><span data-ttu-id="e26ed-103">Получите accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="e26ed-103">Get accessPackageResourceEnvironment</span></span>
<span data-ttu-id="e26ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e26ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e26ed-105">Ознакомьтесь с свойствами и отношениями объекта [accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)</span><span class="sxs-lookup"><span data-stu-id="e26ed-105">Read the properties and relationships of an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e26ed-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e26ed-106">Permissions</span></span>
<span data-ttu-id="e26ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e26ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e26ed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e26ed-109">Permission type</span></span>|<span data-ttu-id="e26ed-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e26ed-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e26ed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e26ed-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e26ed-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e26ed-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="e26ed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e26ed-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e26ed-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e26ed-114">Not supported.</span></span>|
|<span data-ttu-id="e26ed-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e26ed-115">Application</span></span>|<span data-ttu-id="e26ed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e26ed-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e26ed-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e26ed-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageResourceEnvironments/{accessPackageResourceEnvironmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e26ed-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e26ed-118">Optional query parameters</span></span>
<span data-ttu-id="e26ed-119">Этот метод в настоящее время не поддерживает [параметры запроса OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="e26ed-119">This method does not currently support [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e26ed-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e26ed-120">Request headers</span></span>
|<span data-ttu-id="e26ed-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e26ed-121">Name</span></span>|<span data-ttu-id="e26ed-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e26ed-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e26ed-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e26ed-123">Authorization</span></span>|<span data-ttu-id="e26ed-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e26ed-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e26ed-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e26ed-126">Request body</span></span>
<span data-ttu-id="e26ed-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e26ed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e26ed-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e26ed-128">Response</span></span>

<span data-ttu-id="e26ed-129">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [объект accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e26ed-129">If successful, this method returns a `200 OK` response code and an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e26ed-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="e26ed-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e26ed-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e26ed-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e26ed-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e26ed-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceenvironment"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceEnvironments/{accessPackageResourceEnvironmentId}
```
# <a name="c"></a>[<span data-ttu-id="e26ed-133">C#</span><span class="sxs-lookup"><span data-stu-id="e26ed-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e26ed-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e26ed-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e26ed-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e26ed-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e26ed-136">Java</span><span class="sxs-lookup"><span data-stu-id="e26ed-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e26ed-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e26ed-137">Response</span></span>
> <span data-ttu-id="e26ed-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e26ed-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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

