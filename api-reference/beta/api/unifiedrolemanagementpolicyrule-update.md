---
title: Обновление unifiedRoleManagementPolicyRule
description: Обновление свойств единого объектаRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 05db197ef2fd4b54ea2036e42c06adc026f7746d
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299766"
---
# <a name="update-unifiedrolemanagementpolicyrule"></a><span data-ttu-id="b1a0e-103">Обновление unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="b1a0e-103">Update unifiedRoleManagementPolicyRule</span></span>
<span data-ttu-id="b1a0e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1a0e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b1a0e-105">Обновление свойств единого [объектаRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="b1a0e-105">Update the properties of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1a0e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1a0e-106">Permissions</span></span>
<span data-ttu-id="b1a0e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1a0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1a0e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1a0e-109">Permission type</span></span>|<span data-ttu-id="b1a0e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1a0e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1a0e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1a0e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b1a0e-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="b1a0e-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="b1a0e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1a0e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1a0e-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b1a0e-114">Not supported</span></span>|
|<span data-ttu-id="b1a0e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1a0e-115">Application</span></span>|<span data-ttu-id="b1a0e-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b1a0e-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1a0e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1a0e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
PATCH /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/effectiveRules/{unifiedRoleManagementPolicyRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="b1a0e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1a0e-118">Request headers</span></span>
|<span data-ttu-id="b1a0e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b1a0e-119">Name</span></span>|<span data-ttu-id="b1a0e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b1a0e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b1a0e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1a0e-121">Authorization</span></span>|<span data-ttu-id="b1a0e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1a0e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b1a0e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b1a0e-124">Content-Type</span></span>|<span data-ttu-id="b1a0e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1a0e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1a0e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1a0e-127">Request body</span></span>
<span data-ttu-id="b1a0e-128">В теле запроса поставляем представление JSON единого [объектаRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="b1a0e-128">In the request body, supply a JSON representation of the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>

<span data-ttu-id="b1a0e-129">В следующей таблице показаны свойства, необходимые при обновлении [единой системыRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="b1a0e-129">The following table shows the properties that are required when you update the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

|<span data-ttu-id="b1a0e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1a0e-130">Property</span></span>|<span data-ttu-id="b1a0e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b1a0e-131">Type</span></span>|<span data-ttu-id="b1a0e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b1a0e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1a0e-133">id</span><span class="sxs-lookup"><span data-stu-id="b1a0e-133">id</span></span>|<span data-ttu-id="b1a0e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b1a0e-134">String</span></span>|<span data-ttu-id="b1a0e-135">Уникальный идентификатор для правила.</span><span class="sxs-lookup"><span data-stu-id="b1a0e-135">Unique identifier for the rule.</span></span>|
|<span data-ttu-id="b1a0e-136">target</span><span class="sxs-lookup"><span data-stu-id="b1a0e-136">target</span></span>|[<span data-ttu-id="b1a0e-137">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="b1a0e-137">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="b1a0e-138">Цель правила политики.</span><span class="sxs-lookup"><span data-stu-id="b1a0e-138">The target for the policy rule.</span></span>|



## <a name="response"></a><span data-ttu-id="b1a0e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1a0e-139">Response</span></span>

<span data-ttu-id="b1a0e-140">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [унифицированный объектRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b1a0e-140">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b1a0e-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="b1a0e-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b1a0e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1a0e-142">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="b1a0e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1a0e-143">Response</span></span>
<span data-ttu-id="b1a0e-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b1a0e-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
