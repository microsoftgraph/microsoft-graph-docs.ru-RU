---
title: Список cloudPcOverviews
description: Получите список объектов cloudPcOverview и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 5550c1bf9bccf00552d5251b7bf173a4022d1cd3
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402430"
---
# <a name="list-cloudpcoverviews"></a><span data-ttu-id="9a0a2-103">Список cloudPcOverviews</span><span class="sxs-lookup"><span data-stu-id="9a0a2-103">List cloudPcOverviews</span></span>
<span data-ttu-id="9a0a2-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="9a0a2-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a0a2-105">Получите список объектов [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="9a0a2-105">Get a list of the [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a0a2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a0a2-106">Permissions</span></span>
<span data-ttu-id="9a0a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a0a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a0a2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a0a2-109">Permission type</span></span>|<span data-ttu-id="9a0a2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a0a2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a0a2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a0a2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9a0a2-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a0a2-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="9a0a2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a0a2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a0a2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a0a2-114">Not supported.</span></span>|
|<span data-ttu-id="9a0a2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a0a2-115">Application</span></span>|<span data-ttu-id="9a0a2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a0a2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a0a2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a0a2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcsOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9a0a2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9a0a2-118">Optional query parameters</span></span>
<span data-ttu-id="9a0a2-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="9a0a2-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a0a2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a0a2-120">Request headers</span></span>
|<span data-ttu-id="9a0a2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9a0a2-121">Name</span></span>|<span data-ttu-id="9a0a2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9a0a2-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9a0a2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a0a2-123">Authorization</span></span>|<span data-ttu-id="9a0a2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a0a2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a0a2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a0a2-126">Request body</span></span>
<span data-ttu-id="9a0a2-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a0a2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a0a2-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a0a2-128">Response</span></span>

<span data-ttu-id="9a0a2-129">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9a0a2-129">If successful, this method returns a `200 OK` response code and a collection of [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a0a2-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="9a0a2-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9a0a2-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a0a2-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_cloudpcoverview"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcsOverview
```


### <a name="response"></a><span data-ttu-id="9a0a2-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a0a2-132">Response</span></span>
><span data-ttu-id="9a0a2-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9a0a2-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.cloudPcOverview)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedTenants.cloudPcOverview",
      "id": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee",
      "totalCloudPcStatus": 18,
      "numberOfCloudPcStatusNotProvisioned": 4,
      "numberOfCloudPcStatusProvisioning": 0,
      "numberOfCloudPcStatusProvisioned": 14,
      "numberOfCloudPcStatusUpgrading": 0,
      "numberOfCloudPcStatusInGracePeriod": 0,
      "numberOfCloudPcStatusDeprovisioning": 0,
      "numberOfCloudPcStatusFailed": 0,
      "numberOfCloudPcStatusUnknown": 0,
      "totalCloudPcConnectionStatus": 25,
      "numberOfCloudPcConnectionStatusPending": 0,
      "numberOfCloudPcConnectionStatusRunning": 0,
      "numberOfCloudPcConnectionStatusPassed": 17,
      "numberOfCloudPcConnectionStatusFailed": 6,
      "numberOfCloudPcConnectionStatusUnkownFutureValue": 0,
      "lastRefreshedDateTime": "2021-07-11T17:18:46.4830816Z"
    }
  ]
}
```
