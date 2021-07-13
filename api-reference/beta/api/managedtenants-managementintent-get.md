---
title: Get managementIntent
description: Ознакомьтесь с свойствами и отношениями объекта managementIntent.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 2e4c5cd374638c5e147cc95043cf846f0323d1e6
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402628"
---
# <a name="get-managementintent"></a><span data-ttu-id="5f1fe-103">Get managementIntent</span><span class="sxs-lookup"><span data-stu-id="5f1fe-103">Get managementIntent</span></span>
<span data-ttu-id="5f1fe-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="5f1fe-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f1fe-105">Ознакомьтесь с свойствами и отношениями объекта [managementIntent.](../resources/managedtenants-managementintent.md)</span><span class="sxs-lookup"><span data-stu-id="5f1fe-105">Read the properties and relationships of a [managementIntent](../resources/managedtenants-managementintent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f1fe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f1fe-106">Permissions</span></span>
<span data-ttu-id="5f1fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f1fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f1fe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f1fe-109">Permission type</span></span>|<span data-ttu-id="5f1fe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f1fe-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f1fe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f1fe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5f1fe-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f1fe-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="5f1fe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f1fe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f1fe-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f1fe-114">Not supported.</span></span>|
|<span data-ttu-id="5f1fe-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f1fe-115">Application</span></span>|<span data-ttu-id="5f1fe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f1fe-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f1fe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f1fe-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementIntents/{managementIntentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f1fe-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5f1fe-118">Optional query parameters</span></span>
<span data-ttu-id="5f1fe-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="5f1fe-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f1fe-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f1fe-120">Request headers</span></span>
|<span data-ttu-id="5f1fe-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5f1fe-121">Name</span></span>|<span data-ttu-id="5f1fe-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5f1fe-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5f1fe-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f1fe-123">Authorization</span></span>|<span data-ttu-id="5f1fe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f1fe-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f1fe-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f1fe-126">Request body</span></span>
<span data-ttu-id="5f1fe-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5f1fe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f1fe-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f1fe-128">Response</span></span>

<span data-ttu-id="5f1fe-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект managementIntent](../resources/managedtenants-managementintent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5f1fe-129">If successful, this method returns a `200 OK` response code and a [managementIntent](../resources/managedtenants-managementintent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f1fe-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="5f1fe-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5f1fe-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f1fe-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_managementintent"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementIntents/{managementIntentId}
```

### <a name="response"></a><span data-ttu-id="5f1fe-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f1fe-132">Response</span></span>
><span data-ttu-id="5f1fe-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5f1fe-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementIntent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementIntents/$entity",
    "id": "586895ab-8a59-4b79-be25-b06949a819bb",
    "displayName": "Default Baseline",
    "isGlobal": true,
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
```
