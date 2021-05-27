---
title: Get unifiedRoleManagementPolicyRule
description: Ознакомьтесь с свойствами и отношениями объекта unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 76fb785c11f9ccbd321a6a44e314b05a4e0169f5
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680236"
---
# <a name="get-unifiedrolemanagementpolicyrule"></a><span data-ttu-id="b2a55-103">Get unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="b2a55-103">Get unifiedRoleManagementPolicyRule</span></span>
<span data-ttu-id="b2a55-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2a55-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b2a55-105">Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="b2a55-105">Read the properties and relationships of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2a55-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2a55-106">Permissions</span></span>
<span data-ttu-id="b2a55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2a55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2a55-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2a55-109">Permission type</span></span>|<span data-ttu-id="b2a55-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2a55-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2a55-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2a55-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b2a55-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="b2a55-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="b2a55-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2a55-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2a55-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b2a55-114">Not supported</span></span>|
|<span data-ttu-id="b2a55-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b2a55-115">Application</span></span>|<span data-ttu-id="b2a55-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="b2a55-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2a55-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2a55-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/effectiveRules/{unifiedRoleManagementPolicyRuleId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b2a55-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b2a55-118">Optional query parameters</span></span>
<span data-ttu-id="b2a55-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b2a55-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b2a55-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b2a55-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b2a55-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2a55-121">Request headers</span></span>
|<span data-ttu-id="b2a55-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b2a55-122">Name</span></span>|<span data-ttu-id="b2a55-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b2a55-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b2a55-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2a55-124">Authorization</span></span>|<span data-ttu-id="b2a55-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2a55-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2a55-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2a55-127">Request body</span></span>
<span data-ttu-id="b2a55-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2a55-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2a55-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2a55-129">Response</span></span>

<span data-ttu-id="b2a55-130">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` объект [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b2a55-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b2a55-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="b2a55-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b2a55-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2a55-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b2a55-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2a55-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedrolemanagementpolicyrule"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
```
# <a name="c"></a>[<span data-ttu-id="b2a55-134">C#</span><span class="sxs-lookup"><span data-stu-id="b2a55-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedrolemanagementpolicyrule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2a55-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2a55-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedrolemanagementpolicyrule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2a55-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2a55-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedrolemanagementpolicyrule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2a55-137">Java</span><span class="sxs-lookup"><span data-stu-id="b2a55-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedrolemanagementpolicyrule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b2a55-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2a55-138">Response</span></span>
<span data-ttu-id="b2a55-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b2a55-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRule"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba",
    "target": {
      "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
    }
  }
}
```

