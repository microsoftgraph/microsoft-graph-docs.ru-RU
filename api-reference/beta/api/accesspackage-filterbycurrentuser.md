---
title: 'accessPackage: filterByCurrentUser'
description: Извлечение списка объектов accesspackage, фильтруемых на входе пользователя.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a4212c06606c6363a31e64dee7da820d93ea13fa
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299551"
---
# <a name="accesspackage-filterbycurrentuser"></a><span data-ttu-id="49007-103">accessPackage: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="49007-103">accessPackage: filterByCurrentUser</span></span>
<span data-ttu-id="49007-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49007-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49007-105">В [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md)извлекайте список объектов [accessPackage,](../resources/accesspackage.md) фильтруемых на входе пользователя.</span><span class="sxs-lookup"><span data-stu-id="49007-105">In [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackage](../resources/accesspackage.md) objects filtered on the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="49007-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49007-106">Permissions</span></span>
<span data-ttu-id="49007-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49007-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49007-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49007-109">Permission type</span></span>|<span data-ttu-id="49007-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49007-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49007-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49007-111">Delegated (work or school account)</span></span>|<span data-ttu-id="49007-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49007-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="49007-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49007-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49007-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49007-114">Not supported.</span></span>|
|<span data-ttu-id="49007-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49007-115">Application</span></span>|<span data-ttu-id="49007-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49007-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49007-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49007-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackages/filterByCurrentUser
```

## <a name="function-parameters"></a><span data-ttu-id="49007-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="49007-118">Function parameters</span></span>
<span data-ttu-id="49007-119">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="49007-119">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="49007-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="49007-120">Parameter</span></span>|<span data-ttu-id="49007-121">Тип</span><span class="sxs-lookup"><span data-stu-id="49007-121">Type</span></span>|<span data-ttu-id="49007-122">Описание</span><span class="sxs-lookup"><span data-stu-id="49007-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49007-123">on</span><span class="sxs-lookup"><span data-stu-id="49007-123">on</span></span>|[<span data-ttu-id="49007-124">accessPackageFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="49007-124">accessPackageFilterByCurrentUserOptions</span></span>](../resources/accesspackage-accesspackagefilterbycurrentuseroptions.md)|<span data-ttu-id="49007-125">Список текущих пользовательских параметров, которые можно использовать для фильтрации в списке пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="49007-125">The list of current user options that can be used to filter on the access packages list.</span></span>|

- <span data-ttu-id="49007-126">`allowedRequestor` используется для получения объектов, для которых входя в нее пользователь может `accessPackage` отправлять запросы доступа.</span><span class="sxs-lookup"><span data-stu-id="49007-126">`allowedRequestor` is used to get the `accessPackage` objects for which the signed-in user is allowed to submit access requests.</span></span> <span data-ttu-id="49007-127">В итоговом списке содержатся все пакеты доступа, которые могут запрашиваться вызываемой по всем каталогам.</span><span class="sxs-lookup"><span data-stu-id="49007-127">The resulting list includes all access packages that can be requested by the caller across all catalogs.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49007-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49007-128">Request headers</span></span>
|<span data-ttu-id="49007-129">Имя</span><span class="sxs-lookup"><span data-stu-id="49007-129">Name</span></span>|<span data-ttu-id="49007-130">Описание</span><span class="sxs-lookup"><span data-stu-id="49007-130">Description</span></span>|
|:---|:---|
|<span data-ttu-id="49007-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49007-131">Authorization</span></span>|<span data-ttu-id="49007-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49007-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49007-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49007-134">Request body</span></span>
<span data-ttu-id="49007-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49007-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49007-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="49007-136">Response</span></span>

<span data-ttu-id="49007-137">В случае успешной работы этот метод возвращает код отклика и `200 OK` [коллекцию accessPackage](../resources/accesspackage.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="49007-137">If successful, this method returns a `200 OK` response code and an [accessPackage](../resources/accesspackage.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49007-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="49007-138">Examples</span></span>
<span data-ttu-id="49007-139">В следующем примере получаются пакеты доступа, которые могут запрашиваться пользователем, входив в него.</span><span class="sxs-lookup"><span data-stu-id="49007-139">The following example gets the access packages that can be requested by the signed-in user.</span></span>

### <a name="request"></a><span data-ttu-id="49007-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="49007-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentrequest_filterByCurrentUser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/filterByCurrentUser(on='allowedRequestor')
```


### <a name="response"></a><span data-ttu-id="49007-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="49007-141">Response</span></span>
> <span data-ttu-id="49007-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="49007-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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

