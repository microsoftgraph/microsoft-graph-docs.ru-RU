---
title: Список accessPackageResourceEnvironments
description: Получить список объектов accessPackageResourceEnvironment.
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2843300c166cf064c3cd79c79551ae6c7b764ecf
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176245"
---
# <a name="list-accesspackageresourceenvironments"></a><span data-ttu-id="6adf8-103">Список accessPackageResourceEnvironments</span><span class="sxs-lookup"><span data-stu-id="6adf8-103">List accessPackageResourceEnvironments</span></span>
<span data-ttu-id="6adf8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6adf8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6adf8-105">Получить список объектов [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="6adf8-105">Retrieve a list of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="6adf8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6adf8-106">Permissions</span></span>
<span data-ttu-id="6adf8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6adf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6adf8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6adf8-109">Permission type</span></span>|<span data-ttu-id="6adf8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6adf8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6adf8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6adf8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6adf8-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6adf8-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="6adf8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6adf8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6adf8-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6adf8-114">Not supported</span></span>|
|<span data-ttu-id="6adf8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6adf8-115">Application</span></span>|<span data-ttu-id="6adf8-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6adf8-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="6adf8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6adf8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6adf8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6adf8-118">Optional query parameters</span></span>
<span data-ttu-id="6adf8-119">Для этого метода требуется параметр `$filter` [запроса OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="6adf8-119">This method requires the `$filter` [OData query parameter](/graph/query-parameters).</span></span> <span data-ttu-id="6adf8-120">Необходимо подать `$filter` заявку на **originSystem с установленным** для ( `eq` ) `SharePointOnline` .</span><span class="sxs-lookup"><span data-stu-id="6adf8-120">You must apply `$filter` for an **originSystem** set to (`eq`) `SharePointOnline`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6adf8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6adf8-121">Request headers</span></span>
|<span data-ttu-id="6adf8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6adf8-122">Name</span></span>|<span data-ttu-id="6adf8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6adf8-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6adf8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6adf8-124">Authorization</span></span>|<span data-ttu-id="6adf8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6adf8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6adf8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6adf8-127">Request body</span></span>
<span data-ttu-id="6adf8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6adf8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6adf8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6adf8-129">Response</span></span>

<span data-ttu-id="6adf8-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6adf8-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6adf8-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="6adf8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6adf8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6adf8-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6adf8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6adf8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accesspackageresourceenvironment"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```
# <a name="c"></a>[<span data-ttu-id="6adf8-134">C#</span><span class="sxs-lookup"><span data-stu-id="6adf8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accesspackageresourceenvironment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6adf8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6adf8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accesspackageresourceenvironment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6adf8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6adf8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accesspackageresourceenvironment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6adf8-137">Java</span><span class="sxs-lookup"><span data-stu-id="6adf8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accesspackageresourceenvironment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6adf8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6adf8-138">Response</span></span>
<span data-ttu-id="6adf8-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6adf8-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageResourceEnvironment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceEnvironments",
  "value": [
    {
      "id": "615f2218-678f-471f-a60a-02c2f4f80c57",
      "displayName": "https://contoso.sharepoint.com/",
      "description": "https://contoso.sharepoint.com/",
      "originSystem": "SharePointOnline",
      "originId": "https://contoso-admin.sharepoint.com/",
      "isDefaultEnvironment": false,
      "connectionInfo": {
        "url": "https://contoso-admin.sharepoint.com/"
      }
    }
  ]
}
```

