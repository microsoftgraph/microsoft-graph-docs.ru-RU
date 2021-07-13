---
title: Список tenantGroups
description: Получите список объектов tenantGroup и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 11bb89e594308fad86f61c2d9d1d422e684c48ee
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403089"
---
# <a name="list-tenantgroups"></a><span data-ttu-id="99366-103">Список tenantGroups</span><span class="sxs-lookup"><span data-stu-id="99366-103">List tenantGroups</span></span>
<span data-ttu-id="99366-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="99366-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99366-105">Получите список объектов [tenantGroup](../resources/managedtenants-tenantgroup.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="99366-105">Get a list of the [tenantGroup](../resources/managedtenants-tenantgroup.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="99366-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99366-106">Permissions</span></span>
<span data-ttu-id="99366-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99366-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99366-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99366-109">Permission type</span></span>|<span data-ttu-id="99366-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99366-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99366-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99366-111">Delegated (work or school account)</span></span>|<span data-ttu-id="99366-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99366-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="99366-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99366-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99366-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99366-114">Not supported.</span></span>|
|<span data-ttu-id="99366-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99366-115">Application</span></span>|<span data-ttu-id="99366-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99366-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99366-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99366-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="99366-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="99366-118">Optional query parameters</span></span>
<span data-ttu-id="99366-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="99366-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="99366-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99366-120">Request headers</span></span>
|<span data-ttu-id="99366-121">Имя</span><span class="sxs-lookup"><span data-stu-id="99366-121">Name</span></span>|<span data-ttu-id="99366-122">Описание</span><span class="sxs-lookup"><span data-stu-id="99366-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="99366-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99366-123">Authorization</span></span>|<span data-ttu-id="99366-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99366-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="99366-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99366-126">Request body</span></span>
<span data-ttu-id="99366-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="99366-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99366-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="99366-128">Response</span></span>

<span data-ttu-id="99366-129">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [tenantGroup](../resources/managedtenants-tenantgroup.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="99366-129">If successful, this method returns a `200 OK` response code and a collection of [tenantGroup](../resources/managedtenants-tenantgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="99366-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="99366-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="99366-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="99366-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_tenantgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantGroups
```


### <a name="response"></a><span data-ttu-id="99366-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="99366-132">Response</span></span>
><span data-ttu-id="99366-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="99366-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.tenantGroup)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/tenantGroups",
    "value": [
        {
            "id": "df7aed9c-c05a-4fc9-b958-64fafaed911d",
            "displayName": "Default",
            "allTenantsIncluded": true,
            "tenantIds": [],
            "managementIntents": [
                {
                    "managementIntentId": "586895ab-8a59-4b79-be25-b06949a819bb",
                    "managementIntentDisplayName": "Default Baseline",
                    "managementTemplates": [
                        {
                            "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
                            "displayName": "Baseline - Block Legacy Authentication",
                            "category": "identity"
                        },
                        {
                            "managementTemplateId": "12524106-036f-457f-b7a6-b003509d29c8",
                            "displayName": "Baseline - Require MFA for Admins",
                            "category": "identity"
                        },
                        {
                            "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
                            "displayName": "Baseline - Require MFA for end users",
                            "category": "identity"
                        },
                        {
                            "managementTemplateId": "e2cadc41-a08f-45e7-8eb1-942d224dfb9a",
                            "displayName": "Baseline - Enroll devices in MEM",
                            "category": "devices"
                        },
                        {
                            "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
                            "displayName": "Baseline - Setup Compliance Policy for Windows 10 devices",
                            "category": "devices"
                        },
                        {
                            "managementTemplateId": "b2d6d189-ea31-4cf8-b75e-41210c583127",
                            "displayName": "Baseline - Setup Microsoft Defender Antivirus Policy for Windows 10 devices",
                            "category": "devices"
                        }
                    ]
                }
            ],
            "managementActions": [
                {
                    "managementTemplateId": "12524106-036f-457f-b7a6-b003509d29c8",
                    "managementActionId": "eac82706-9f32-4274-ba5b-cf1f8ecf042b"
                },
                {
                    "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
                    "managementActionId": "f104bb7f-4854-4209-ba09-c3788f9894c5"
                },
                {
                    "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
                    "managementActionId": "4274db74-99c4-40be-bbeb-da4351136be2"
                },
                {
                    "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
                    "managementActionId": "e96a8cdb-0435-4808-9956-cf6b8ae77aa6"
                },
                {
                    "managementTemplateId": "b2d6d189-ea31-4cf8-b75e-41210c583127",
                    "managementActionId": "55f8da1a-4eec-4fb2-9c58-4c4b3cdf7222"
                },
                {
                    "managementTemplateId": "e2cadc41-a08f-45e7-8eb1-942d224dfb9a",
                    "managementActionId": "b22a4713-8428-4952-8cac-d48962ecbdc9"
                }
            ]
        }
    ]
}
```
