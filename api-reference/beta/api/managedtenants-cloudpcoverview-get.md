---
title: Get cloudPcOverview
description: Ознакомьтесь с свойствами и отношениями объекта cloudPcOverview.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: f6874205f1a5fc37c135c152a16b0491821c2613
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402501"
---
# <a name="get-cloudpcoverview"></a><span data-ttu-id="7c5f5-103">Get cloudPcOverview</span><span class="sxs-lookup"><span data-stu-id="7c5f5-103">Get cloudPcOverview</span></span>
<span data-ttu-id="7c5f5-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="7c5f5-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c5f5-105">Ознакомьтесь с свойствами и отношениями объекта [cloudPcOverview.](../resources/managedtenants-cloudpcoverview.md)</span><span class="sxs-lookup"><span data-stu-id="7c5f5-105">Read the properties and relationships of a [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c5f5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c5f5-106">Permissions</span></span>
<span data-ttu-id="7c5f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c5f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c5f5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c5f5-109">Permission type</span></span>|<span data-ttu-id="7c5f5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c5f5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c5f5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c5f5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7c5f5-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c5f5-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="7c5f5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c5f5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c5f5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c5f5-114">Not supported.</span></span>|
|<span data-ttu-id="7c5f5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c5f5-115">Application</span></span>|<span data-ttu-id="7c5f5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c5f5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c5f5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c5f5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcsOverview/{cloudPcOverviewId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7c5f5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7c5f5-118">Optional query parameters</span></span>
<span data-ttu-id="7c5f5-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="7c5f5-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c5f5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c5f5-120">Request headers</span></span>
|<span data-ttu-id="7c5f5-121">Имя</span><span class="sxs-lookup"><span data-stu-id="7c5f5-121">Name</span></span>|<span data-ttu-id="7c5f5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7c5f5-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7c5f5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c5f5-123">Authorization</span></span>|<span data-ttu-id="7c5f5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c5f5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c5f5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c5f5-126">Request body</span></span>
<span data-ttu-id="7c5f5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7c5f5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c5f5-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c5f5-128">Response</span></span>

<span data-ttu-id="7c5f5-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7c5f5-129">If successful, this method returns a `200 OK` response code and a [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7c5f5-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="7c5f5-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7c5f5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c5f5-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_cloudpcoverview"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcsOverview/{cloudPcOverviewId}
```


### <a name="response"></a><span data-ttu-id="7c5f5-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c5f5-132">Response</span></span>
><span data-ttu-id="7c5f5-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7c5f5-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.cloudPcOverview"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

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
```
