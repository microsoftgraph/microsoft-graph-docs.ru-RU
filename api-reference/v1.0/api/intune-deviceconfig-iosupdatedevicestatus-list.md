---
title: Перечисление объектов iosUpdateDeviceStatus
description: Список свойств и связей объектов iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 681495495892e6d00f692bc8aa6c9afca0706e15
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970620"
---
# <a name="list-iosupdatedevicestatuses"></a><span data-ttu-id="8b0a6-103">Перечисление объектов iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="8b0a6-103">List iosUpdateDeviceStatuses</span></span>

> <span data-ttu-id="8b0a6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b0a6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b0a6-105">Список свойств и связей объектов [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8b0a6-105">List properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b0a6-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8b0a6-106">Prerequisites</span></span>
<span data-ttu-id="8b0a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b0a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b0a6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b0a6-109">Permission type</span></span>|<span data-ttu-id="8b0a6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b0a6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b0a6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b0a6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8b0a6-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b0a6-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8b0a6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b0a6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b0a6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b0a6-114">Not supported.</span></span>|
|<span data-ttu-id="8b0a6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b0a6-115">Application</span></span>|<span data-ttu-id="8b0a6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b0a6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b0a6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b0a6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="8b0a6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b0a6-118">Request headers</span></span>
|<span data-ttu-id="8b0a6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b0a6-119">Header</span></span>|<span data-ttu-id="8b0a6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8b0a6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b0a6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b0a6-121">Authorization</span></span>|<span data-ttu-id="8b0a6-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b0a6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b0a6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8b0a6-123">Accept</span></span>|<span data-ttu-id="8b0a6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8b0a6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b0a6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b0a6-125">Request body</span></span>
<span data-ttu-id="8b0a6-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b0a6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b0a6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b0a6-127">Response</span></span>
<span data-ttu-id="8b0a6-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b0a6-128">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b0a6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8b0a6-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b0a6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b0a6-130">Request</span></span>
<span data-ttu-id="8b0a6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b0a6-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses
```

### <a name="response"></a><span data-ttu-id="8b0a6-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b0a6-132">Response</span></span>
<span data-ttu-id="8b0a6-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b0a6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



