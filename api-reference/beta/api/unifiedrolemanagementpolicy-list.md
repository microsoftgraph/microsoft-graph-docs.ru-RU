---
title: Список унифицированныхRoleManagementPolicies
description: Получите список объектов unifiedRoleManagementPolicy и их свойств.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 809e947965f180fca2bdc0078ff69a64c00960cc
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299581"
---
# <a name="list-unifiedrolemanagementpolicies"></a><span data-ttu-id="daee9-103">Список унифицированныхRoleManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="daee9-103">List unifiedRoleManagementPolicies</span></span>
<span data-ttu-id="daee9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daee9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daee9-105">Получите список объектов [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="daee9-105">Get a list of the [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="daee9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="daee9-106">Permissions</span></span>
<span data-ttu-id="daee9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="daee9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daee9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="daee9-109">Permission type</span></span>|<span data-ttu-id="daee9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="daee9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="daee9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="daee9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="daee9-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="daee9-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="daee9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="daee9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="daee9-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="daee9-114">Not supported</span></span>|
|<span data-ttu-id="daee9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="daee9-115">Application</span></span>|<span data-ttu-id="daee9-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="daee9-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="daee9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="daee9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="daee9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="daee9-118">Optional query parameters</span></span>
<span data-ttu-id="daee9-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="daee9-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="daee9-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="daee9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="daee9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="daee9-121">Request headers</span></span>
|<span data-ttu-id="daee9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="daee9-122">Name</span></span>|<span data-ttu-id="daee9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="daee9-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="daee9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="daee9-124">Authorization</span></span>|<span data-ttu-id="daee9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="daee9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="daee9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="daee9-127">Request body</span></span>
<span data-ttu-id="daee9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="daee9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="daee9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="daee9-129">Response</span></span>

<span data-ttu-id="daee9-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="daee9-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="daee9-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="daee9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="daee9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="daee9-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies
```


### <a name="response"></a><span data-ttu-id="daee9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="daee9-133">Response</span></span>
<span data-ttu-id="daee9-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="daee9-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "f93a5c37-5c37-f93a-375c-3af9375c3af9",
      "displayName": "Policy1",
      "description": "Policy for all privileged admins",
      "isOrganizationDefault": false,
      "scopeId": "f93a5c37-5c37-f93a-375c-3af9375c3af9",
      "scopeType": "subscription",
      "lastModifiedDateTime": "2020-09-09T21:35:27.91Z",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identity"
      }
    }
  ]
}
```

