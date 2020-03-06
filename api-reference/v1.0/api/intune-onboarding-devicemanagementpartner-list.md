---
title: Список объектов deviceManagementPartner
description: Список свойств и связей объектов deviceManagementPartner.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 465ac4b2718fcc8e689c816dbb1cd4d8efa8654c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512519"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="588d5-103">Список объектов deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="588d5-103">List deviceManagementPartners</span></span>

<span data-ttu-id="588d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="588d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="588d5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="588d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="588d5-106">Список свойств и связей объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="588d5-106">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="588d5-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="588d5-107">Prerequisites</span></span>
<span data-ttu-id="588d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="588d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="588d5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="588d5-110">Permission type</span></span>|<span data-ttu-id="588d5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="588d5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="588d5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="588d5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="588d5-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="588d5-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="588d5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="588d5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="588d5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="588d5-115">Not supported.</span></span>|
|<span data-ttu-id="588d5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="588d5-116">Application</span></span>|<span data-ttu-id="588d5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="588d5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="588d5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="588d5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="588d5-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="588d5-119">Request headers</span></span>
|<span data-ttu-id="588d5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="588d5-120">Header</span></span>|<span data-ttu-id="588d5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="588d5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="588d5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="588d5-122">Authorization</span></span>|<span data-ttu-id="588d5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="588d5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="588d5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="588d5-124">Accept</span></span>|<span data-ttu-id="588d5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="588d5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="588d5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="588d5-126">Request body</span></span>
<span data-ttu-id="588d5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="588d5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="588d5-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="588d5-128">Response</span></span>
<span data-ttu-id="588d5-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="588d5-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="588d5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="588d5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="588d5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="588d5-131">Request</span></span>
<span data-ttu-id="588d5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="588d5-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="588d5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="588d5-133">Response</span></span>
<span data-ttu-id="588d5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="588d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 624

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementPartner",
      "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "unavailable",
      "partnerAppType": "singleTenantApp",
      "singleTenantAppId": "Single Tenant App Id value",
      "displayName": "Display Name value",
      "isConfigured": true,
      "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
      "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
    }
  ]
}
```




