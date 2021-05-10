---
title: Get unifiedRoleManagementPolicy
description: Ознакомьтесь с свойствами и отношениями объекта unifiedRoleManagementPolicy.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c88442960327de7d89d17e32549bc6eefb874db1
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299646"
---
# <a name="get-unifiedrolemanagementpolicy"></a><span data-ttu-id="86120-103">Get unifiedRoleManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="86120-103">Get unifiedRoleManagementPolicy</span></span>
<span data-ttu-id="86120-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86120-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86120-105">Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleManagementPolicy.](../resources/unifiedrolemanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="86120-105">Read the properties and relationships of an [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="86120-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86120-106">Permissions</span></span>
<span data-ttu-id="86120-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86120-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86120-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86120-109">Permission type</span></span>|<span data-ttu-id="86120-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86120-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86120-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86120-111">Delegated (work or school account)</span></span>|<span data-ttu-id="86120-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="86120-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="86120-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86120-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86120-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="86120-114">Not supported</span></span>|
|<span data-ttu-id="86120-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86120-115">Application</span></span>|<span data-ttu-id="86120-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="86120-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="86120-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86120-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="86120-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="86120-118">Optional query parameters</span></span>
<span data-ttu-id="86120-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="86120-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="86120-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="86120-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="86120-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86120-121">Request headers</span></span>
|<span data-ttu-id="86120-122">Имя</span><span class="sxs-lookup"><span data-stu-id="86120-122">Name</span></span>|<span data-ttu-id="86120-123">Описание</span><span class="sxs-lookup"><span data-stu-id="86120-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="86120-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86120-124">Authorization</span></span>|<span data-ttu-id="86120-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86120-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86120-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86120-127">Request body</span></span>
<span data-ttu-id="86120-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="86120-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86120-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="86120-129">Response</span></span>

<span data-ttu-id="86120-130">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` объект [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="86120-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="86120-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="86120-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86120-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="86120-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedrolemanagementpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies/f93a5c37-5c37-f93a-375c-3af9375c3af9
```


### <a name="response"></a><span data-ttu-id="86120-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="86120-133">Response</span></span>
<span data-ttu-id="86120-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="86120-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "f93a5c37-5c37-f93a-375c-3af9375c3af9",
    "displayName": "Policy1",
    "description": "Policy for privileged admins",
    "isOrganizationDefault": true,
    "scopeId": "f93a5c37-5c37-f93a-375c-3af9375c3af9",
    "scopeType": "subscription",
    "lastModifiedDateTime": "2020-09-09T21:35:27.91Z",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identity"
    }
  }
}
```

