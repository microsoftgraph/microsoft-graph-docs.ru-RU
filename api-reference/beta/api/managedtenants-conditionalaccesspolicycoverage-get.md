---
title: Get conditionalAccessPolicyCoverage
description: Ознакомьтесь с свойствами и отношениями объекта conditionalAccessPolicyCoverage.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 1c3dffaea58476a30c28d05ea3aceeba750741e5
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440145"
---
# <a name="get-conditionalaccesspolicycoverage"></a><span data-ttu-id="b0053-103">Get conditionalAccessPolicyCoverage</span><span class="sxs-lookup"><span data-stu-id="b0053-103">Get conditionalAccessPolicyCoverage</span></span>
<span data-ttu-id="b0053-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="b0053-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0053-105">Ознакомьтесь с свойствами и отношениями объекта [conditionalAccessPolicyCoverage.](../resources/managedtenants-conditionalaccesspolicycoverage.md)</span><span class="sxs-lookup"><span data-stu-id="b0053-105">Read the properties and relationships of a [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0053-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0053-106">Permissions</span></span>
<span data-ttu-id="b0053-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0053-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0053-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0053-109">Permission type</span></span>|<span data-ttu-id="b0053-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0053-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0053-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0053-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b0053-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess и Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0053-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess, and Application.Read.All</span></span>|
|<span data-ttu-id="b0053-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0053-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0053-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0053-114">Not supported.</span></span>|
|<span data-ttu-id="b0053-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0053-115">Application</span></span>|<span data-ttu-id="b0053-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0053-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0053-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0053-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/conditionalAccessPolicyCoverages/{conditionalAccessPolicyCoverageId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0053-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b0053-118">Optional query parameters</span></span>
<span data-ttu-id="b0053-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="b0053-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0053-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0053-120">Request headers</span></span>
|<span data-ttu-id="b0053-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b0053-121">Name</span></span>|<span data-ttu-id="b0053-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b0053-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b0053-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0053-123">Authorization</span></span>|<span data-ttu-id="b0053-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0053-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0053-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0053-126">Request body</span></span>
<span data-ttu-id="b0053-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0053-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0053-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0053-128">Response</span></span>

<span data-ttu-id="b0053-129">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b0053-129">If successful, this method returns a `200 OK` response code and a [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b0053-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="b0053-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b0053-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0053-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b0053-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0053-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conditionalaccesspolicycoverage"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/conditionalAccessPolicyCoverages/{conditionalAccessPolicyCoverageId}
```
# <a name="c"></a>[<span data-ttu-id="b0053-133">C#</span><span class="sxs-lookup"><span data-stu-id="b0053-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conditionalaccesspolicycoverage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0053-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0053-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conditionalaccesspolicycoverage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0053-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0053-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conditionalaccesspolicycoverage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b0053-136">Java</span><span class="sxs-lookup"><span data-stu-id="b0053-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conditionalaccesspolicycoverage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b0053-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0053-137">Response</span></span>
><span data-ttu-id="b0053-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b0053-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.conditionalAccessPolicyCoverage"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
  "id": "38227791-a88b-4fcc-81c5-58cf77668320",
  "conditionalAccessPolicyState": "enabled",
  "requiresDeviceCompliance": false,
  "latestPolicyModifiedDateTime": "2021-07-11T14:56:13.598304Z",
  "tenantDisplayName": "Consolidated Messenger"
}
```
