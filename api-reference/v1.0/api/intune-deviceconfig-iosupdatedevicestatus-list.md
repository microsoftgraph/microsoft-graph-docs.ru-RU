---
title: Перечисление объектов iosUpdateDeviceStatus
description: Список свойств и связей объектов iosUpdateDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1b5641cd31396b958b318123a4c705d87854430b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756304"
---
# <a name="list-iosupdatedevicestatuses"></a><span data-ttu-id="31197-103">Перечисление объектов iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="31197-103">List iosUpdateDeviceStatuses</span></span>

<span data-ttu-id="31197-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31197-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31197-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31197-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31197-106">Список свойств и связей объектов [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="31197-106">List properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31197-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="31197-107">Prerequisites</span></span>
<span data-ttu-id="31197-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31197-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31197-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31197-110">Permission type</span></span>|<span data-ttu-id="31197-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31197-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31197-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31197-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31197-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31197-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="31197-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31197-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31197-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31197-115">Not supported.</span></span>|
|<span data-ttu-id="31197-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="31197-116">Application</span></span>|<span data-ttu-id="31197-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31197-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31197-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31197-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="31197-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="31197-119">Request headers</span></span>
|<span data-ttu-id="31197-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="31197-120">Header</span></span>|<span data-ttu-id="31197-121">Значение</span><span class="sxs-lookup"><span data-stu-id="31197-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31197-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="31197-122">Authorization</span></span>|<span data-ttu-id="31197-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31197-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31197-124">Accept</span><span class="sxs-lookup"><span data-stu-id="31197-124">Accept</span></span>|<span data-ttu-id="31197-125">application/json</span><span class="sxs-lookup"><span data-stu-id="31197-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31197-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31197-126">Request body</span></span>
<span data-ttu-id="31197-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="31197-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31197-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="31197-128">Response</span></span>
<span data-ttu-id="31197-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="31197-129">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31197-130">Пример</span><span class="sxs-lookup"><span data-stu-id="31197-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="31197-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="31197-131">Request</span></span>
<span data-ttu-id="31197-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31197-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses
```

### <a name="response"></a><span data-ttu-id="31197-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="31197-133">Response</span></span>
<span data-ttu-id="31197-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31197-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 686

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
      "id": "63a79499-9499-63a7-9994-a7639994a763",
      "installStatus": "available",
      "osVersion": "Os Version value",
      "deviceId": "Device Id value",
      "userId": "User Id value",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




