---
title: Список accessPackageResourceEnvironments
description: Получить список объектов accessPackageResourceEnvironment.
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cf7116ef1512dca40cae66d92030b032d3aefa23
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137724"
---
# <a name="list-accesspackageresourceenvironments"></a><span data-ttu-id="71fa8-103">Список accessPackageResourceEnvironments</span><span class="sxs-lookup"><span data-stu-id="71fa8-103">List accessPackageResourceEnvironments</span></span>
<span data-ttu-id="71fa8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71fa8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="71fa8-105">Получить список объектов [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="71fa8-105">Retrieve a list of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="71fa8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71fa8-106">Permissions</span></span>
<span data-ttu-id="71fa8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71fa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71fa8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71fa8-109">Permission type</span></span>|<span data-ttu-id="71fa8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71fa8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71fa8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71fa8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="71fa8-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71fa8-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="71fa8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71fa8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71fa8-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="71fa8-114">Not supported</span></span>|
|<span data-ttu-id="71fa8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71fa8-115">Application</span></span>|<span data-ttu-id="71fa8-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="71fa8-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="71fa8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71fa8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71fa8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="71fa8-118">Optional query parameters</span></span>
<span data-ttu-id="71fa8-119">Для этого метода требуется параметр `$filter` [запроса OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="71fa8-119">This method requires the `$filter` [OData query parameter](/graph/query-parameters).</span></span> <span data-ttu-id="71fa8-120">Необходимо подать `$filter` заявку на **originSystem с установленным** для ( `eq` ) `SharePointOnline` .</span><span class="sxs-lookup"><span data-stu-id="71fa8-120">You must apply `$filter` for an **originSystem** set to (`eq`) `SharePointOnline`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71fa8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71fa8-121">Request headers</span></span>
|<span data-ttu-id="71fa8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="71fa8-122">Name</span></span>|<span data-ttu-id="71fa8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="71fa8-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="71fa8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71fa8-124">Authorization</span></span>|<span data-ttu-id="71fa8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71fa8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71fa8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71fa8-127">Request body</span></span>
<span data-ttu-id="71fa8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71fa8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71fa8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="71fa8-129">Response</span></span>

<span data-ttu-id="71fa8-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="71fa8-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="71fa8-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="71fa8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="71fa8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="71fa8-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_accesspackageresourceenvironment"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceEnvironments?$filter=originSystem eq 'SharePointOnline'
```


### <a name="response"></a><span data-ttu-id="71fa8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="71fa8-133">Response</span></span>
<span data-ttu-id="71fa8-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="71fa8-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

