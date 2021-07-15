---
title: Get tenantTag
description: Ознакомьтесь с свойствами и отношениями объекта tenantTag.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 711adc2987df3b2707ea8a23e8a06c45f4cb398d
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441076"
---
# <a name="get-tenanttag"></a><span data-ttu-id="056b1-103">Get tenantTag</span><span class="sxs-lookup"><span data-stu-id="056b1-103">Get tenantTag</span></span>
<span data-ttu-id="056b1-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="056b1-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="056b1-105">Ознакомьтесь с свойствами и отношениями объекта [tenantTag.](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="056b1-105">Read the properties and relationships of a [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="056b1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="056b1-106">Permissions</span></span>
<span data-ttu-id="056b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="056b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="056b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="056b1-109">Permission type</span></span>|<span data-ttu-id="056b1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="056b1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="056b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="056b1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="056b1-112">ManagedTenants.Read.All, ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="056b1-112">ManagedTenants.Read.All, ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="056b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="056b1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="056b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="056b1-114">Not supported.</span></span>|
|<span data-ttu-id="056b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="056b1-115">Application</span></span>|<span data-ttu-id="056b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="056b1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="056b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="056b1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="056b1-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="056b1-118">Optional query parameters</span></span>
<span data-ttu-id="056b1-119">Этот метод поддерживает [параметры запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$count` , , , , , и `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="056b1-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="056b1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="056b1-120">Request headers</span></span>
|<span data-ttu-id="056b1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="056b1-121">Name</span></span>|<span data-ttu-id="056b1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="056b1-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="056b1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="056b1-123">Authorization</span></span>|<span data-ttu-id="056b1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="056b1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="056b1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="056b1-126">Request body</span></span>
<span data-ttu-id="056b1-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="056b1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="056b1-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="056b1-128">Response</span></span>

<span data-ttu-id="056b1-129">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект tenantTag](../resources/managedtenants-tenanttag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="056b1-129">If successful, this method returns a `200 OK` response code and a [tenantTag](../resources/managedtenants-tenanttag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="056b1-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="056b1-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="056b1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="056b1-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="056b1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="056b1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tenanttag"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```
# <a name="c"></a>[<span data-ttu-id="056b1-133">C#</span><span class="sxs-lookup"><span data-stu-id="056b1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tenanttag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="056b1-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="056b1-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tenanttag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="056b1-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="056b1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tenanttag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="056b1-136">Java</span><span class="sxs-lookup"><span data-stu-id="056b1-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tenanttag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="056b1-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="056b1-137">Response</span></span>
><span data-ttu-id="056b1-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="056b1-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/tenantTags/$entity",
    "id": "913391c0-5466-42b4-900d-0a7501399cb0",
    "displayName": "Onboarding",
    "description": "Tenants that we are currently onboarding",
    "tenantIds": [
        "38227791-a88b-4fcc-81c5-58cf77668320",
        "34298981-4fc8-4974-9486-c8909ed1521b",
        "4d262a25-c70a-430b-9e8e-46c31dec116b"
    ],
    "isDeleted": null,
    "createdDateTime": "2021-06-16T20:36:31.086644Z",
    "createdByUserId": "9bf6a5ad-aecb-4194-a16b-38e02702a602",
    "lastActionDateTime": "2021-06-28T20:46:09.0071888Z",
    "lastActionByUserId": "08ea0285-30cb-46cc-abc8-3d8422e21ecb",
    "tenants": [
        {
            "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320"
        },
        {
            "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b"
        },
        {
            "tenantId": "4d262a25-c70a-430b-9e8e-46c31dec116b"
        }
    ]
}
```
