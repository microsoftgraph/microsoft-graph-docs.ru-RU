---
title: Get managementAction
description: Ознакомьтесь с свойствами и отношениями объекта managementAction.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 1e576eba2d7b5d77433596701d331422f48d5d9d
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442218"
---
# <a name="get-managementaction"></a><span data-ttu-id="e21c3-103">Get managementAction</span><span class="sxs-lookup"><span data-stu-id="e21c3-103">Get managementAction</span></span>
<span data-ttu-id="e21c3-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="e21c3-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e21c3-105">Ознакомьтесь с свойствами и отношениями объекта [managementAction.](../resources/managedtenants-managementaction.md)</span><span class="sxs-lookup"><span data-stu-id="e21c3-105">Read the properties and relationships of a [managementAction](../resources/managedtenants-managementaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e21c3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e21c3-106">Permissions</span></span>
<span data-ttu-id="e21c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e21c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e21c3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e21c3-109">Permission type</span></span>|<span data-ttu-id="e21c3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e21c3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e21c3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e21c3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e21c3-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21c3-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="e21c3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e21c3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e21c3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e21c3-114">Not supported.</span></span>|
|<span data-ttu-id="e21c3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e21c3-115">Application</span></span>|<span data-ttu-id="e21c3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e21c3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e21c3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e21c3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementActions/{managementActionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e21c3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e21c3-118">Optional query parameters</span></span>
<span data-ttu-id="e21c3-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="e21c3-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e21c3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e21c3-120">Request headers</span></span>
|<span data-ttu-id="e21c3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e21c3-121">Name</span></span>|<span data-ttu-id="e21c3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e21c3-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e21c3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e21c3-123">Authorization</span></span>|<span data-ttu-id="e21c3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e21c3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e21c3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e21c3-126">Request body</span></span>
<span data-ttu-id="e21c3-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e21c3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e21c3-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e21c3-128">Response</span></span>

<span data-ttu-id="e21c3-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект managementAction](../resources/managedtenants-managementaction.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e21c3-129">If successful, this method returns a `200 OK` response code and a [managementAction](../resources/managedtenants-managementaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e21c3-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="e21c3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e21c3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e21c3-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e21c3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e21c3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_managementaction"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActions/{managementActionId}
```
# <a name="c"></a>[<span data-ttu-id="e21c3-133">C#</span><span class="sxs-lookup"><span data-stu-id="e21c3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-managementaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e21c3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e21c3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-managementaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e21c3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e21c3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-managementaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e21c3-136">Java</span><span class="sxs-lookup"><span data-stu-id="e21c3-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-managementaction-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e21c3-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e21c3-137">Response</span></span>
><span data-ttu-id="e21c3-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e21c3-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementAction"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementActions/$entity",
    "id": "4274db74-99c4-40be-bbeb-da4351136be2",
    "referenceTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
    "displayName": "Baseline - Require MFA for end users",
    "description": null,
    "category": "identity",
    "workloadActions": [
        {
            "actionId": "fcb7ace7-3ea6-4474-912a-00ee78554445",
            "category": "automated",
            "displayName": "ConditionalAccessPolicy",
            "description": null,
            "service": "AAD",
            "settings": [
                {
                    "valueType": "string",
                    "displayName": "DisplayName",
                    "overwriteAllowed": false,
                    "jsonValue": "\"Baseline - Require MFA for end users\""
                },
                {
                    "valueType": "string",
                    "displayName": "State",
                    "overwriteAllowed": false,
                    "jsonValue": "\"enabledForReportingButNotEnforced\""
                },
                {
                    "valueType": "stringCollection",
                    "displayName": "ClientAppTypes",
                    "overwriteAllowed": false,
                    "jsonValue": "[\"All\"]"
                },
                {
                    "valueType": "stringCollection",
                    "displayName": "IncludeApplications",
                    "overwriteAllowed": false,
                    "jsonValue": "[\"All\"]"
                },
                {
                    "valueType": "stringCollection",
                    "displayName": "IncludeUsers",
                    "overwriteAllowed": false,
                    "jsonValue": "[\"None\"]"
                },
                {
                    "valueType": "stringCollection",
                    "displayName": "IncludeLocations",
                    "overwriteAllowed": false,
                    "jsonValue": "[\"All\"]"
                },
                {
                    "valueType": "string",
                    "displayName": "GrantControls.Operator",
                    "overwriteAllowed": false,
                    "jsonValue": "\"OR\""
                },
                {
                    "valueType": "stringCollection",
                    "displayName": "GrantControls.BuiltInControls",
                    "overwriteAllowed": false,
                    "jsonValue": "[\"mfa\"]"
                }
            ]
        }
    ]
}
```
