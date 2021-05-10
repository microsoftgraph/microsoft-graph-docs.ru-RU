---
title: Get unifiedRoleManagementPolicyRule
description: Ознакомьтесь с свойствами и отношениями объекта unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8640e539623d179b88f1b7279469bbfcf5b00adc
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299557"
---
# <a name="get-unifiedrolemanagementpolicyrule"></a><span data-ttu-id="ef9d6-103">Get unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="ef9d6-103">Get unifiedRoleManagementPolicyRule</span></span>
<span data-ttu-id="ef9d6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef9d6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ef9d6-105">Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="ef9d6-105">Read the properties and relationships of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef9d6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef9d6-106">Permissions</span></span>
<span data-ttu-id="ef9d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef9d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef9d6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef9d6-109">Permission type</span></span>|<span data-ttu-id="ef9d6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef9d6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef9d6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef9d6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ef9d6-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="ef9d6-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="ef9d6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef9d6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef9d6-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ef9d6-114">Not supported</span></span>|
|<span data-ttu-id="ef9d6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef9d6-115">Application</span></span>|<span data-ttu-id="ef9d6-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="ef9d6-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef9d6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef9d6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/effectiveRules/{unifiedRoleManagementPolicyRuleId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ef9d6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ef9d6-118">Optional query parameters</span></span>
<span data-ttu-id="ef9d6-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ef9d6-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ef9d6-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ef9d6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef9d6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef9d6-121">Request headers</span></span>
|<span data-ttu-id="ef9d6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ef9d6-122">Name</span></span>|<span data-ttu-id="ef9d6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ef9d6-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ef9d6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef9d6-124">Authorization</span></span>|<span data-ttu-id="ef9d6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef9d6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef9d6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef9d6-127">Request body</span></span>
<span data-ttu-id="ef9d6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef9d6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef9d6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef9d6-129">Response</span></span>

<span data-ttu-id="ef9d6-130">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` объект [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ef9d6-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ef9d6-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ef9d6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ef9d6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef9d6-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedrolemanagementpolicyrule"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
```


### <a name="response"></a><span data-ttu-id="ef9d6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef9d6-133">Response</span></span>
<span data-ttu-id="ef9d6-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ef9d6-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

