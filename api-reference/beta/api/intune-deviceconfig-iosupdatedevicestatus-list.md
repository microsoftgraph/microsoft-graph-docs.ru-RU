---
title: Перечисление объектов iosUpdateDeviceStatus
description: Список свойств и связей объектов iosUpdateDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e31e88eec5cf2aa2b221e73d5527b1b9989ef171
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43438551"
---
# <a name="list-iosupdatedevicestatuses"></a><span data-ttu-id="4bda6-103">Перечисление объектов iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="4bda6-103">List iosUpdateDeviceStatuses</span></span>

<span data-ttu-id="4bda6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bda6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4bda6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bda6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bda6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4bda6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bda6-107">Список свойств и связей объектов [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="4bda6-107">List properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4bda6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4bda6-108">Prerequisites</span></span>
<span data-ttu-id="4bda6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bda6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bda6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bda6-111">Permission type</span></span>|<span data-ttu-id="4bda6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bda6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bda6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bda6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4bda6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bda6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4bda6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bda6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bda6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bda6-116">Not supported.</span></span>|
|<span data-ttu-id="4bda6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4bda6-117">Application</span></span>|<span data-ttu-id="4bda6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bda6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bda6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bda6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="4bda6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4bda6-120">Request headers</span></span>
|<span data-ttu-id="4bda6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4bda6-121">Header</span></span>|<span data-ttu-id="4bda6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4bda6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bda6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bda6-123">Authorization</span></span>|<span data-ttu-id="4bda6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bda6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bda6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4bda6-125">Accept</span></span>|<span data-ttu-id="4bda6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4bda6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bda6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4bda6-127">Request body</span></span>
<span data-ttu-id="4bda6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4bda6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bda6-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4bda6-129">Response</span></span>
<span data-ttu-id="4bda6-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4bda6-130">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bda6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4bda6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4bda6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bda6-132">Request</span></span>
<span data-ttu-id="4bda6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4bda6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses
```

### <a name="response"></a><span data-ttu-id="4bda6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bda6-134">Response</span></span>
<span data-ttu-id="4bda6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4bda6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 708

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
      "platform": 8,
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



