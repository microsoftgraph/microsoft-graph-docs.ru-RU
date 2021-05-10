---
title: Перечисление правил
description: Получите ресурсы unifiedRoleManagementPolicyRule из свойства навигации правил.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c4a9f37cc806f3afec446e826e43f90a43d626b8
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299587"
---
# <a name="list-rules"></a><span data-ttu-id="ad015-103">Перечисление правил</span><span class="sxs-lookup"><span data-stu-id="ad015-103">List rules</span></span>
<span data-ttu-id="ad015-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad015-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad015-105">Получите ресурсы unifiedRoleManagementPolicyRule из свойства навигации правил.</span><span class="sxs-lookup"><span data-stu-id="ad015-105">Get the unifiedRoleManagementPolicyRule resources from the rules navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad015-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad015-106">Permissions</span></span>
<span data-ttu-id="ad015-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad015-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad015-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad015-109">Permission type</span></span>|<span data-ttu-id="ad015-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad015-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad015-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad015-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ad015-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="ad015-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="ad015-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad015-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad015-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ad015-114">Not supported</span></span>|
|<span data-ttu-id="ad015-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad015-115">Application</span></span>|<span data-ttu-id="ad015-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="ad015-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad015-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad015-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad015-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ad015-118">Optional query parameters</span></span>
<span data-ttu-id="ad015-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="ad015-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ad015-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ad015-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad015-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad015-121">Request headers</span></span>
|<span data-ttu-id="ad015-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ad015-122">Name</span></span>|<span data-ttu-id="ad015-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ad015-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ad015-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad015-124">Authorization</span></span>|<span data-ttu-id="ad015-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad015-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad015-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad015-127">Request body</span></span>
<span data-ttu-id="ad015-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad015-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad015-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad015-129">Response</span></span>

<span data-ttu-id="ad015-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ad015-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ad015-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ad015-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ad015-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad015-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicyrule"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies/ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba/rules
```


### <a name="response"></a><span data-ttu-id="ad015-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad015-133">Response</span></span>
<span data-ttu-id="ad015-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ad015-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

