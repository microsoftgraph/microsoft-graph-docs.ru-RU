---
title: Управление спискамиActions
description: Получите список объектов managementAction и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 03aedec0464908bf25deb004e6cbe4bdb5027acb
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402435"
---
# <a name="list-managementactions"></a><span data-ttu-id="e3b19-103">Управление спискамиActions</span><span class="sxs-lookup"><span data-stu-id="e3b19-103">List managementActions</span></span>
<span data-ttu-id="e3b19-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="e3b19-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3b19-105">Получите список объектов [managementAction](../resources/managedtenants-managementaction.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="e3b19-105">Get a list of the [managementAction](../resources/managedtenants-managementaction.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3b19-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3b19-106">Permissions</span></span>
<span data-ttu-id="e3b19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3b19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3b19-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3b19-109">Permission type</span></span>|<span data-ttu-id="e3b19-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3b19-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3b19-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3b19-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3b19-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3b19-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="e3b19-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3b19-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3b19-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3b19-114">Not supported.</span></span>|
|<span data-ttu-id="e3b19-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3b19-115">Application</span></span>|<span data-ttu-id="e3b19-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3b19-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3b19-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3b19-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementActions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3b19-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e3b19-118">Optional query parameters</span></span>
<span data-ttu-id="e3b19-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="e3b19-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3b19-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3b19-120">Request headers</span></span>
|<span data-ttu-id="e3b19-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e3b19-121">Name</span></span>|<span data-ttu-id="e3b19-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e3b19-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e3b19-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3b19-123">Authorization</span></span>|<span data-ttu-id="e3b19-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3b19-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3b19-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3b19-126">Request body</span></span>
<span data-ttu-id="e3b19-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3b19-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3b19-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3b19-128">Response</span></span>

<span data-ttu-id="e3b19-129">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов managementAction](../resources/managedtenants-managementaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e3b19-129">If successful, this method returns a `200 OK` response code and a collection of [managementAction](../resources/managedtenants-managementaction.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3b19-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="e3b19-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e3b19-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3b19-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_managementaction"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActions
```


### <a name="response"></a><span data-ttu-id="e3b19-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3b19-132">Response</span></span>
><span data-ttu-id="e3b19-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e3b19-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.managementAction)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementActions",
    "value": [
        {
            "id": "4274db74-99c4-40be-bbeb-da4351136be2",
            "referenceTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
            "displayName": "Baseline - Require MFA for end users",
            "description": null,
            "category": "identity",
            "workloadActions": [
                {
                    "actionId": "fcb7ace7-3ea6-4474-912a-00ee78554445",
                    "category": "automated",
                    "displayName": "ConditionalAccessPolicy",
                    "description": null,
                    "service": "AAD",
                    "settings": [
                        {
                            "valueType": "string",
                            "displayName": "DisplayName",
                            "overwriteAllowed": false,
                            "jsonValue": "\"Baseline - Require MFA for end users\""
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
                            "jsonValue": "[\"All\"]"
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
                            "jsonValue": "[\"mfa\"]"
                        }
                    ]
                }
            ]
        }
    ]
}
```
