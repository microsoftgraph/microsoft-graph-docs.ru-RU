---
title: 'tenantTag: assignTag'
description: Назначьте тег клиента указанным управляемым арендаторам.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 867f252eca5fc84f5f77e916c38d50bd564b7e9a
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441765"
---
# <a name="tenanttag-assigntag"></a><span data-ttu-id="10018-103">tenantTag: assignTag</span><span class="sxs-lookup"><span data-stu-id="10018-103">tenantTag: assignTag</span></span>
<span data-ttu-id="10018-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="10018-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10018-105">Назначьте тег клиента указанным управляемым арендаторам.</span><span class="sxs-lookup"><span data-stu-id="10018-105">Assign the tenant tag to the specified managed tenants.</span></span>

## <a name="permissions"></a><span data-ttu-id="10018-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10018-106">Permissions</span></span>
<span data-ttu-id="10018-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10018-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10018-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10018-109">Permission type</span></span>|<span data-ttu-id="10018-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10018-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10018-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10018-111">Delegated (work or school account)</span></span>|<span data-ttu-id="10018-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="10018-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="10018-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10018-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10018-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10018-114">Not supported.</span></span>|
|<span data-ttu-id="10018-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10018-115">Application</span></span>|<span data-ttu-id="10018-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10018-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10018-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10018-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenantTags/{tenantTagId}/assignTag
```

## <a name="request-headers"></a><span data-ttu-id="10018-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10018-118">Request headers</span></span>
|<span data-ttu-id="10018-119">Имя</span><span class="sxs-lookup"><span data-stu-id="10018-119">Name</span></span>|<span data-ttu-id="10018-120">Описание</span><span class="sxs-lookup"><span data-stu-id="10018-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="10018-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10018-121">Authorization</span></span>|<span data-ttu-id="10018-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10018-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="10018-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10018-124">Content-Type</span></span>|<span data-ttu-id="10018-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10018-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="10018-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10018-127">Request body</span></span>
<span data-ttu-id="10018-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10018-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="10018-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="10018-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="10018-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="10018-130">Parameter</span></span>|<span data-ttu-id="10018-131">Тип</span><span class="sxs-lookup"><span data-stu-id="10018-131">Type</span></span>|<span data-ttu-id="10018-132">Описание</span><span class="sxs-lookup"><span data-stu-id="10018-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10018-133">tenantIds</span><span class="sxs-lookup"><span data-stu-id="10018-133">tenantIds</span></span>|<span data-ttu-id="10018-134">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="10018-134">String collection</span></span>|<span data-ttu-id="10018-135">Коллекция идентификаторов Azure Active Directory, на которые должен быть назначен тег клиента.</span><span class="sxs-lookup"><span data-stu-id="10018-135">The collection of Azure Active Directory tenant identifiers where the tenant tag should be assigned.</span></span>|

## <a name="response"></a><span data-ttu-id="10018-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="10018-136">Response</span></span>

<span data-ttu-id="10018-137">В случае успеха это действие возвращает код отклика и `200 OK` [tenantTag](../resources/managedtenants-tenanttag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="10018-137">If successful, this action returns a `200 OK` response code and a [tenantTag](../resources/managedtenants-tenanttag.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10018-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="10018-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="10018-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="10018-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="10018-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="10018-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tenanttag_assigntag"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}/assignTag
Content-Type: application/json
Content-length: 41

{
  "tenantIds": [
    "String"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="10018-141">C#</span><span class="sxs-lookup"><span data-stu-id="10018-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tenanttag-assigntag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10018-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10018-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tenanttag-assigntag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10018-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10018-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tenanttag-assigntag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10018-144">Java</span><span class="sxs-lookup"><span data-stu-id="10018-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tenanttag-assigntag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="10018-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="10018-145">Response</span></span>
><span data-ttu-id="10018-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="10018-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantTags/$entity",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b",
  "displayName": "Support",
  "description": "Tenants that have purchased support",
  "tenants": [
    {
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b"
    }
  ],
  "isDeleted": null,
  "createdDateTime": "2021-06-26T13:51:23.3927236Z",
  "createdByUserId": "65ca7649-4ccb-4823-9c39-42bd75191bf8",
  "lastActionDateTime": "2021-07-11T19:55:19.7230386Z",
  "lastActionByUserId": "50bf7bd8-1b3a-4d1d-94c5-86d27e68857f"
}
```
