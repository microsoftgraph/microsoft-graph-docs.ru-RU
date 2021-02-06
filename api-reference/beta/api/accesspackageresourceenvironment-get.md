---
title: Get accessPackageResourceEnvironment
description: Чтение свойств и связей объекта accessPackageResourceEnvironment.
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8ec973b1f8d7b38b27e267d54b8cbcd424af23bc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137718"
---
# <a name="get-accesspackageresourceenvironment"></a><span data-ttu-id="393f3-103">Get accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="393f3-103">Get accessPackageResourceEnvironment</span></span>
<span data-ttu-id="393f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="393f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="393f3-105">Чтение свойств и связей объекта [accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)</span><span class="sxs-lookup"><span data-stu-id="393f3-105">Read the properties and relationships of an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="393f3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="393f3-106">Permissions</span></span>
<span data-ttu-id="393f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="393f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="393f3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="393f3-109">Permission type</span></span>|<span data-ttu-id="393f3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="393f3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="393f3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="393f3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="393f3-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="393f3-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="393f3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="393f3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="393f3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="393f3-114">Not supported.</span></span>|
|<span data-ttu-id="393f3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="393f3-115">Application</span></span>|<span data-ttu-id="393f3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="393f3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="393f3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="393f3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageResourceEnvironments/{accessPackageResourceEnvironmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="393f3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="393f3-118">Optional query parameters</span></span>
<span data-ttu-id="393f3-119">В настоящее время этот метод не поддерживает [параметры запросов OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="393f3-119">This method does not currently support [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="393f3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="393f3-120">Request headers</span></span>
|<span data-ttu-id="393f3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="393f3-121">Name</span></span>|<span data-ttu-id="393f3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="393f3-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="393f3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="393f3-123">Authorization</span></span>|<span data-ttu-id="393f3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="393f3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="393f3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="393f3-126">Request body</span></span>
<span data-ttu-id="393f3-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="393f3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="393f3-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="393f3-128">Response</span></span>

<span data-ttu-id="393f3-129">В случае успешного выполнения этот метод возвращает код отклика и объект `200 OK` [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="393f3-129">If successful, this method returns a `200 OK` response code and an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="393f3-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="393f3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="393f3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="393f3-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceenvironment"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceEnvironments/{accessPackageResourceEnvironmentId}
```


### <a name="response"></a><span data-ttu-id="393f3-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="393f3-132">Response</span></span>
<span data-ttu-id="393f3-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="393f3-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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

