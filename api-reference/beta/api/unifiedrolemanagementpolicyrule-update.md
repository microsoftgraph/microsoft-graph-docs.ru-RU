---
title: Обновление unifiedRoleManagementPolicyRule
description: Обновление свойств единого объектаRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 5c5e8fe49f4d88d07c5627b55db6fd0f5e3839e8
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682287"
---
# <a name="update-unifiedrolemanagementpolicyrule"></a><span data-ttu-id="7bffb-103">Обновление unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="7bffb-103">Update unifiedRoleManagementPolicyRule</span></span>
<span data-ttu-id="7bffb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bffb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7bffb-105">Обновление свойств единого [объектаRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="7bffb-105">Update the properties of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bffb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7bffb-106">Permissions</span></span>
<span data-ttu-id="7bffb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bffb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bffb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bffb-109">Permission type</span></span>|<span data-ttu-id="7bffb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bffb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bffb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bffb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7bffb-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="7bffb-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="7bffb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bffb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bffb-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7bffb-114">Not supported</span></span>|
|<span data-ttu-id="7bffb-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="7bffb-115">Application</span></span>|<span data-ttu-id="7bffb-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7bffb-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bffb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bffb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
PATCH /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/effectiveRules/{unifiedRoleManagementPolicyRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="7bffb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bffb-118">Request headers</span></span>
|<span data-ttu-id="7bffb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7bffb-119">Name</span></span>|<span data-ttu-id="7bffb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7bffb-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7bffb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7bffb-121">Authorization</span></span>|<span data-ttu-id="7bffb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7bffb-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7bffb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7bffb-124">Content-Type</span></span>|<span data-ttu-id="7bffb-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7bffb-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bffb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7bffb-127">Request body</span></span>
<span data-ttu-id="7bffb-128">В теле запроса поставляем представление JSON единого [объектаRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="7bffb-128">In the request body, supply a JSON representation of the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>

<span data-ttu-id="7bffb-129">В следующей таблице показаны свойства, необходимые при обновлении [единой системыRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="7bffb-129">The following table shows the properties that are required when you update the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

|<span data-ttu-id="7bffb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bffb-130">Property</span></span>|<span data-ttu-id="7bffb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7bffb-131">Type</span></span>|<span data-ttu-id="7bffb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7bffb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bffb-133">id</span><span class="sxs-lookup"><span data-stu-id="7bffb-133">id</span></span>|<span data-ttu-id="7bffb-134">String</span><span class="sxs-lookup"><span data-stu-id="7bffb-134">String</span></span>|<span data-ttu-id="7bffb-135">Уникальный идентификатор для правила.</span><span class="sxs-lookup"><span data-stu-id="7bffb-135">Unique identifier for the rule.</span></span>|
|<span data-ttu-id="7bffb-136">target</span><span class="sxs-lookup"><span data-stu-id="7bffb-136">target</span></span>|[<span data-ttu-id="7bffb-137">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="7bffb-137">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="7bffb-138">Цель правила политики.</span><span class="sxs-lookup"><span data-stu-id="7bffb-138">The target for the policy rule.</span></span>|



## <a name="response"></a><span data-ttu-id="7bffb-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bffb-139">Response</span></span>

<span data-ttu-id="7bffb-140">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [унифицированный объектRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7bffb-140">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7bffb-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="7bffb-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7bffb-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bffb-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7bffb-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bffb-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7bffb-144">C#</span><span class="sxs-lookup"><span data-stu-id="7bffb-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedrolemanagementpolicyrule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7bffb-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7bffb-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedrolemanagementpolicyrule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7bffb-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7bffb-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedrolemanagementpolicyrule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7bffb-147">Java</span><span class="sxs-lookup"><span data-stu-id="7bffb-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedrolemanagementpolicyrule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7bffb-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bffb-148">Response</span></span>
<span data-ttu-id="7bffb-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7bffb-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRule"
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
