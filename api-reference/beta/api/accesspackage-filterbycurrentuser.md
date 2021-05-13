---
title: 'accessPackage: filterByCurrentUser'
description: Извлечение списка объектов accesspackage, фильтруемых на входе пользователя.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9dbc8275bceceff6fb6beb90e3bfcf5acb476baa
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474038"
---
# <a name="accesspackage-filterbycurrentuser"></a><span data-ttu-id="26880-103">accessPackage: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="26880-103">accessPackage: filterByCurrentUser</span></span>
<span data-ttu-id="26880-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26880-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26880-105">В [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md)извлекайте список объектов [accessPackage,](../resources/accesspackage.md) фильтруемых на входе пользователя.</span><span class="sxs-lookup"><span data-stu-id="26880-105">In [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackage](../resources/accesspackage.md) objects filtered on the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="26880-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26880-106">Permissions</span></span>
<span data-ttu-id="26880-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26880-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26880-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26880-109">Permission type</span></span>|<span data-ttu-id="26880-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26880-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26880-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26880-111">Delegated (work or school account)</span></span>|<span data-ttu-id="26880-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26880-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="26880-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26880-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26880-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26880-114">Not supported.</span></span>|
|<span data-ttu-id="26880-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26880-115">Application</span></span>|<span data-ttu-id="26880-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26880-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26880-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26880-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackages/filterByCurrentUser
```

## <a name="function-parameters"></a><span data-ttu-id="26880-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="26880-118">Function parameters</span></span>
<span data-ttu-id="26880-119">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="26880-119">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="26880-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="26880-120">Parameter</span></span>|<span data-ttu-id="26880-121">Тип</span><span class="sxs-lookup"><span data-stu-id="26880-121">Type</span></span>|<span data-ttu-id="26880-122">Описание</span><span class="sxs-lookup"><span data-stu-id="26880-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26880-123">on</span><span class="sxs-lookup"><span data-stu-id="26880-123">on</span></span>|[<span data-ttu-id="26880-124">accessPackageFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="26880-124">accessPackageFilterByCurrentUserOptions</span></span>](../resources/accesspackage-accesspackagefilterbycurrentuseroptions.md)|<span data-ttu-id="26880-125">Список текущих пользовательских параметров, которые можно использовать для фильтрации в списке пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="26880-125">The list of current user options that can be used to filter on the access packages list.</span></span>|

- <span data-ttu-id="26880-126">`allowedRequestor` используется для получения объектов, для которых входя в нее пользователь может `accessPackage` отправлять запросы доступа.</span><span class="sxs-lookup"><span data-stu-id="26880-126">`allowedRequestor` is used to get the `accessPackage` objects for which the signed-in user is allowed to submit access requests.</span></span> <span data-ttu-id="26880-127">В итоговом списке содержатся все пакеты доступа, которые могут запрашиваться вызываемой по всем каталогам.</span><span class="sxs-lookup"><span data-stu-id="26880-127">The resulting list includes all access packages that can be requested by the caller across all catalogs.</span></span>

## <a name="request-headers"></a><span data-ttu-id="26880-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26880-128">Request headers</span></span>
|<span data-ttu-id="26880-129">Имя</span><span class="sxs-lookup"><span data-stu-id="26880-129">Name</span></span>|<span data-ttu-id="26880-130">Описание</span><span class="sxs-lookup"><span data-stu-id="26880-130">Description</span></span>|
|:---|:---|
|<span data-ttu-id="26880-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26880-131">Authorization</span></span>|<span data-ttu-id="26880-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26880-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="26880-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26880-134">Request body</span></span>
<span data-ttu-id="26880-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26880-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26880-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="26880-136">Response</span></span>

<span data-ttu-id="26880-137">В случае успешной работы этот метод возвращает код отклика и `200 OK` [коллекцию accessPackage](../resources/accesspackage.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="26880-137">If successful, this method returns a `200 OK` response code and an [accessPackage](../resources/accesspackage.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26880-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="26880-138">Examples</span></span>
<span data-ttu-id="26880-139">В следующем примере получаются пакеты доступа, которые могут запрашиваться пользователем, входив в него.</span><span class="sxs-lookup"><span data-stu-id="26880-139">The following example gets the access packages that can be requested by the signed-in user.</span></span>

### <a name="request"></a><span data-ttu-id="26880-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="26880-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="26880-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="26880-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentrequest_filterByCurrentUser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/filterByCurrentUser(on='allowedRequestor')
```
# <a name="c"></a>[<span data-ttu-id="26880-142">C#</span><span class="sxs-lookup"><span data-stu-id="26880-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accesspackageassignmentrequest-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26880-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26880-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackageassignmentrequest-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26880-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26880-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackageassignmentrequest-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26880-145">Java</span><span class="sxs-lookup"><span data-stu-id="26880-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accesspackageassignmentrequest-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="26880-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="26880-146">Response</span></span>
> <span data-ttu-id="26880-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="26880-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignmentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessPackage",
            "id": "d378b3b7-b42a-445a-8780-2841194f777e",
            "catalogId": "eb0f5e12-484d-4545-8ae1-fb1dfc28ab3c",
            "displayName": "Sales resources",
            "description": "Resources needed by the Sales department.",
            "isHidden": false,
            "isRoleScopesVisible": false,
            "createdBy": "TestGA@example.com",
            "createdDateTime": "2021-01-26T22:30:57.37Z",
            "modifiedBy": "TestGA@example.com",
            "modifiedDateTime": "2021-01-26T22:30:57.37Z"
        }
    ]
}
```

