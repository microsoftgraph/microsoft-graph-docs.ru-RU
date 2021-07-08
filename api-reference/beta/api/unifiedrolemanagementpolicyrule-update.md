---
title: Обновление unifiedRoleManagementPolicyRule
description: Обновление свойств единого объектаRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 4d70b105f3516547c851e8be21be18b15009439a
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334698"
---
# <a name="update-unifiedrolemanagementpolicyrule"></a><span data-ttu-id="85cb4-103">Обновление unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="85cb4-103">Update unifiedRoleManagementPolicyRule</span></span>
<span data-ttu-id="85cb4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85cb4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85cb4-105">Обновление свойств единого [объектаRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="85cb4-105">Update the properties of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="85cb4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85cb4-106">Permissions</span></span>
<span data-ttu-id="85cb4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85cb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85cb4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85cb4-109">Permission type</span></span>|<span data-ttu-id="85cb4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85cb4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85cb4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85cb4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="85cb4-112">RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="85cb4-112">RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="85cb4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85cb4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85cb4-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85cb4-114">Not supported</span></span>|
|<span data-ttu-id="85cb4-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="85cb4-115">Application</span></span>|<span data-ttu-id="85cb4-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85cb4-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="85cb4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85cb4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
PATCH /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/effectiveRules/{unifiedRoleManagementPolicyRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="85cb4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85cb4-118">Request headers</span></span>
|<span data-ttu-id="85cb4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="85cb4-119">Name</span></span>|<span data-ttu-id="85cb4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="85cb4-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="85cb4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85cb4-121">Authorization</span></span>|<span data-ttu-id="85cb4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85cb4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="85cb4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85cb4-124">Content-Type</span></span>|<span data-ttu-id="85cb4-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85cb4-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="85cb4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85cb4-127">Request body</span></span>
<span data-ttu-id="85cb4-128">В теле запроса поставляем представление JSON единого [объектаRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="85cb4-128">In the request body, supply a JSON representation of the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>

<span data-ttu-id="85cb4-129">В следующей таблице показаны свойства, необходимые при обновлении [единой системыRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="85cb4-129">The following table shows the properties that are required when you update the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

|<span data-ttu-id="85cb4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="85cb4-130">Property</span></span>|<span data-ttu-id="85cb4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="85cb4-131">Type</span></span>|<span data-ttu-id="85cb4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="85cb4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85cb4-133">id</span><span class="sxs-lookup"><span data-stu-id="85cb4-133">id</span></span>|<span data-ttu-id="85cb4-134">String</span><span class="sxs-lookup"><span data-stu-id="85cb4-134">String</span></span>|<span data-ttu-id="85cb4-135">Уникальный идентификатор для правила.</span><span class="sxs-lookup"><span data-stu-id="85cb4-135">Unique identifier for the rule.</span></span>|
|<span data-ttu-id="85cb4-136">target</span><span class="sxs-lookup"><span data-stu-id="85cb4-136">target</span></span>|[<span data-ttu-id="85cb4-137">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="85cb4-137">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="85cb4-138">Цель правила политики.</span><span class="sxs-lookup"><span data-stu-id="85cb4-138">The target for the policy rule.</span></span>|



## <a name="response"></a><span data-ttu-id="85cb4-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="85cb4-139">Response</span></span>

<span data-ttu-id="85cb4-140">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [унифицированный объектRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="85cb4-140">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="85cb4-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="85cb4-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="85cb4-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="85cb4-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="85cb4-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="85cb4-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedrolemanagementpolicyrule"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
Content-Type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyRule",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="85cb4-144">C#</span><span class="sxs-lookup"><span data-stu-id="85cb4-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedrolemanagementpolicyrule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85cb4-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85cb4-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedrolemanagementpolicyrule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85cb4-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85cb4-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedrolemanagementpolicyrule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85cb4-147">Java</span><span class="sxs-lookup"><span data-stu-id="85cb4-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedrolemanagementpolicyrule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="85cb4-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="85cb4-148">Response</span></span>
<span data-ttu-id="85cb4-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="85cb4-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
```http
HTTP/1.1 204 OK

```
<!--
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyRule",
  "id": "ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  }
}
```
-->
