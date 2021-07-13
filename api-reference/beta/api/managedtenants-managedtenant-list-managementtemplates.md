---
title: Управление спискамиTemplates
description: Получите список объектов managementTemplate и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 0a133a0340d8bfb52da24400a8760b34735d765d
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402634"
---
# <a name="list-managementtemplates"></a><span data-ttu-id="5ae77-103">Управление спискамиTemplates</span><span class="sxs-lookup"><span data-stu-id="5ae77-103">List managementTemplates</span></span>
<span data-ttu-id="5ae77-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="5ae77-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ae77-105">Получите список объектов [managementTemplate](../resources/managedtenants-managementtemplate.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="5ae77-105">Get a list of the [managementTemplate](../resources/managedtenants-managementtemplate.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ae77-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ae77-106">Permissions</span></span>
<span data-ttu-id="5ae77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ae77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ae77-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ae77-109">Permission type</span></span>|<span data-ttu-id="5ae77-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ae77-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ae77-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ae77-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5ae77-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ae77-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="5ae77-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ae77-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ae77-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ae77-114">Not supported.</span></span>|
|<span data-ttu-id="5ae77-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ae77-115">Application</span></span>|<span data-ttu-id="5ae77-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ae77-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ae77-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ae77-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ae77-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5ae77-118">Optional query parameters</span></span>
<span data-ttu-id="5ae77-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="5ae77-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ae77-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ae77-120">Request headers</span></span>
|<span data-ttu-id="5ae77-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5ae77-121">Name</span></span>|<span data-ttu-id="5ae77-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5ae77-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5ae77-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ae77-123">Authorization</span></span>|<span data-ttu-id="5ae77-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ae77-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ae77-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ae77-126">Request body</span></span>
<span data-ttu-id="5ae77-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5ae77-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ae77-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ae77-128">Response</span></span>

<span data-ttu-id="5ae77-129">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов managementTemplate](../resources/managedtenants-managementtemplate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5ae77-129">If successful, this method returns a `200 OK` response code and a collection of [managementTemplate](../resources/managedtenants-managementtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5ae77-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="5ae77-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5ae77-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ae77-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_managementtemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementTemplates
```


### <a name="response"></a><span data-ttu-id="5ae77-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ae77-132">Response</span></span>
><span data-ttu-id="5ae77-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5ae77-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.managementTemplate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementTemplates",
  "value": [
    {
      "id": "e5834405-43d2-4815-867d-3dd600308d1c_1",
      "displayName": "Baseline - Block Legacy Authentication",
      "description": null,
      "category": "identity",
      "parameters": [
        {
          "valueType": "string",
          "displayName": "DisplayName",
          "description": null,
          "jsonDefaultValue": "\"Baseline - Block Legacy Authentication\"",
          "jsonAllowedValues": "null"
        },
        {
          "valueType": "string",
          "displayName": "State",
          "description": null,
          "jsonDefaultValue": "\"enabledForReportingButNotEnforced\"",
          "jsonAllowedValues": "[\"enabled\",\"disabled\",\"enabledForReportingButNotEnforced\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "ClientAppTypes",
          "description": null,
          "jsonDefaultValue": "[\"exchangeActiveSync\",\"other\"]",
          "jsonAllowedValues": "[\"exchangeActiveSync\",\"other\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "IncludeApplications",
          "description": null,
          "jsonDefaultValue": "[\"All\"]",
          "jsonAllowedValues": "[\"All\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "IncludeUsers",
          "description": null,
          "jsonDefaultValue": "[\"None\"]",
          "jsonAllowedValues": "[\"All\",\"None\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "IncludeLocations",
          "description": null,
          "jsonDefaultValue": "[\"All\"]",
          "jsonAllowedValues": "[\"All\",\"AllTrusted\"]"
        },
        {
          "valueType": "string",
          "displayName": "GrantControls.Operator",
          "description": null,
          "jsonDefaultValue": "\"OR\"",
          "jsonAllowedValues": "[\"OR\",\"AND\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "GrantControls.BuiltInControls",
          "description": null,
          "jsonDefaultValue": "[\"block\"]",
          "jsonAllowedValues": "[\"block\"]"
        }
      ],
      "workloadActions": [
        {
          "actionId": "6a3ad0bc-5d7e-4a49-a105-c559aa4633e1",
          "category": "automated",
          "displayName": "ConditionalAccessPolicy",
          "description": null,
          "service": "AAD",
          "settings": [
            {
              "valueType": "string",
              "displayName": "DisplayName",
              "overwriteAllowed": false,
              "jsonValue": "\"Baseline - Block Legacy Authentication\""
            },
            {
              "valueType": "string",
              "displayName": "State",
              "overwriteAllowed": false,
              "jsonValue": "\"enabledForReportingButNotEnforced\""
            },
            {
              "valueType": "stringCollection",
              "displayName": "ClientAppTypes",
              "overwriteAllowed": false,
              "jsonValue": "[\"exchangeActiveSync\",\"other\"]"
            },
            {
              "valueType": "stringCollection",
              "displayName": "IncludeApplications",
              "overwriteAllowed": false,
              "jsonValue": "[\"All\"]"
            },
            {
              "valueType": "stringCollection",
              "displayName": "IncludeUsers",
              "overwriteAllowed": false,
              "jsonValue": "[\"None\"]"
            },
            {
              "valueType": "stringCollection",
              "displayName": "IncludeLocations",
              "overwriteAllowed": false,
              "jsonValue": "[\"All\"]"
            },
            {
              "valueType": "string",
              "displayName": "GrantControls.Operator",
              "overwriteAllowed": false,
              "jsonValue": "\"OR\""
            },
            {
              "valueType": "stringCollection",
              "displayName": "GrantControls.BuiltInControls",
              "overwriteAllowed": false,
              "jsonValue": "[\"block\"]"
            }
          ]
        }
      ]
    }
  ]
}
```
