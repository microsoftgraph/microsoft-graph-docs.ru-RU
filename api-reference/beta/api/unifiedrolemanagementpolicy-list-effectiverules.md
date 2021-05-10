---
title: Список effectiveRules
description: Получите ресурсы unifiedRoleManagementPolicyRule из свойства эффективной навигацииRules.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7ce8a5889cb395c18f5995746f406507ade5e4d7
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299592"
---
# <a name="list-effectiverules"></a><span data-ttu-id="819df-103">Список effectiveRules</span><span class="sxs-lookup"><span data-stu-id="819df-103">List effectiveRules</span></span>
<span data-ttu-id="819df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="819df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="819df-105">Получите ресурсы unifiedRoleManagementPolicyRule из свойства эффективной навигацииRules.</span><span class="sxs-lookup"><span data-stu-id="819df-105">Get the unifiedRoleManagementPolicyRule resources from the effectiveRules navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="819df-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="819df-106">Permissions</span></span>
<span data-ttu-id="819df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="819df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="819df-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="819df-109">Permission type</span></span>|<span data-ttu-id="819df-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="819df-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="819df-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="819df-111">Delegated (work or school account)</span></span>|<span data-ttu-id="819df-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="819df-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="819df-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="819df-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="819df-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="819df-114">Not supported</span></span>|
|<span data-ttu-id="819df-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="819df-115">Application</span></span>|<span data-ttu-id="819df-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="819df-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="819df-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="819df-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/effectiveRules
```

## <a name="optional-query-parameters"></a><span data-ttu-id="819df-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="819df-118">Optional query parameters</span></span>
<span data-ttu-id="819df-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="819df-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="819df-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="819df-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="819df-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="819df-121">Request headers</span></span>
|<span data-ttu-id="819df-122">Имя</span><span class="sxs-lookup"><span data-stu-id="819df-122">Name</span></span>|<span data-ttu-id="819df-123">Описание</span><span class="sxs-lookup"><span data-stu-id="819df-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="819df-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="819df-124">Authorization</span></span>|<span data-ttu-id="819df-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="819df-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="819df-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="819df-127">Request body</span></span>
<span data-ttu-id="819df-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="819df-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="819df-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="819df-129">Response</span></span>

<span data-ttu-id="819df-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="819df-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="819df-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="819df-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="819df-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="819df-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicyrule"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies/ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba/effectiveRules
```


### <a name="response"></a><span data-ttu-id="819df-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="819df-133">Response</span></span>
<span data-ttu-id="819df-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="819df-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicyRule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba",
      "target": {
        "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
      }
    }
  ]
}
```

