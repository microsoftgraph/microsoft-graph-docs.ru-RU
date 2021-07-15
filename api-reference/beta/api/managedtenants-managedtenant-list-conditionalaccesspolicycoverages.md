---
title: Список conditionalAccessPolicyCoverages
description: Получите список объектов conditionalAccessPolicyCoverage и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: a35b7032b4b1fb19b73ff4110a4b43af3c388487
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442664"
---
# <a name="list-conditionalaccesspolicycoverages"></a><span data-ttu-id="ef5c4-103">Список conditionalAccessPolicyCoverages</span><span class="sxs-lookup"><span data-stu-id="ef5c4-103">List conditionalAccessPolicyCoverages</span></span>
<span data-ttu-id="ef5c4-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="ef5c4-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef5c4-105">Получите список объектов [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="ef5c4-105">Get a list of the [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) objects and their properties.</span></span> <span data-ttu-id="ef5c4-106">Используйте эту операцию для списка Azure Active Directory политики условного доступа для всех клиентов, управляемых платформой управления с несколькими клиентами.</span><span class="sxs-lookup"><span data-stu-id="ef5c4-106">Use this operation to list of Azure Active Directory conditional access policy coverage across all tenants that are being managed by the multi-tenant management platform.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef5c4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef5c4-107">Permissions</span></span>
<span data-ttu-id="ef5c4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef5c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef5c4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef5c4-110">Permission type</span></span>|<span data-ttu-id="ef5c4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef5c4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef5c4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef5c4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef5c4-113">Policy.Read.All, Policy.ReadWrite.ConditionalAccess и Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef5c4-113">Policy.Read.All, Policy.ReadWrite.ConditionalAccess, and Application.Read.All</span></span>|
|<span data-ttu-id="ef5c4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef5c4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef5c4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef5c4-115">Not supported.</span></span>|
|<span data-ttu-id="ef5c4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef5c4-116">Application</span></span>|<span data-ttu-id="ef5c4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef5c4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef5c4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef5c4-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/conditionalAccessPolicyCoverages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ef5c4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ef5c4-119">Optional query parameters</span></span>
<span data-ttu-id="ef5c4-120">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="ef5c4-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef5c4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef5c4-121">Request headers</span></span>
|<span data-ttu-id="ef5c4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ef5c4-122">Name</span></span>|<span data-ttu-id="ef5c4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ef5c4-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ef5c4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef5c4-124">Authorization</span></span>|<span data-ttu-id="ef5c4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef5c4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef5c4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef5c4-127">Request body</span></span>
<span data-ttu-id="ef5c4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef5c4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef5c4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef5c4-129">Response</span></span>

<span data-ttu-id="ef5c4-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ef5c4-130">If successful, this method returns a `200 OK` response code and a collection of [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ef5c4-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ef5c4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ef5c4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef5c4-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ef5c4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef5c4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_conditionalaccesspolicycoverage"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/conditionalAccessPolicyCoverages
```
# <a name="c"></a>[<span data-ttu-id="ef5c4-134">C#</span><span class="sxs-lookup"><span data-stu-id="ef5c4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-conditionalaccesspolicycoverage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef5c4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef5c4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-conditionalaccesspolicycoverage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef5c4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef5c4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-conditionalaccesspolicycoverage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef5c4-137">Java</span><span class="sxs-lookup"><span data-stu-id="ef5c4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-conditionalaccesspolicycoverage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ef5c4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef5c4-138">Response</span></span>
><span data-ttu-id="ef5c4-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ef5c4-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.conditionalAccessPolicyCoverage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
      "id": "38227791-a88b-4fcc-81c5-58cf77668320",
      "conditionalAccessPolicyState": "enabled",
      "requiresDeviceCompliance": false,
      "latestPolicyModifiedDateTime": "2021-07-11T14:56:13.598304Z",
      "tenantDisplayName": "Consolidated Messenger"
    }
  ]
}
```
