---
title: Список importedWindowsAutopilotDeviceIdentities
description: Список свойств и связей между объектамиimportedWindowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4a2da69d891998d643b94f9033560dddefd60d54
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875469"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="ab709-103">Список importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="ab709-103">List importedWindowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="ab709-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ab709-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab709-105">Список свойств и связей между объектами[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="ab709-105">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab709-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ab709-106">Prerequisites</span></span>
<span data-ttu-id="ab709-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab709-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab709-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab709-109">Permission type</span></span>|<span data-ttu-id="ab709-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab709-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab709-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab709-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ab709-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab709-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ab709-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab709-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab709-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab709-114">Not supported.</span></span>|
|<span data-ttu-id="ab709-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab709-115">Application</span></span>|<span data-ttu-id="ab709-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab709-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab709-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab709-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="ab709-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab709-118">Request headers</span></span>
|<span data-ttu-id="ab709-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab709-119">Header</span></span>|<span data-ttu-id="ab709-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ab709-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab709-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab709-121">Authorization</span></span>|<span data-ttu-id="ab709-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ab709-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab709-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ab709-123">Accept</span></span>|<span data-ttu-id="ab709-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ab709-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab709-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ab709-125">Request body</span></span>
<span data-ttu-id="ab709-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab709-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab709-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab709-127">Response</span></span>
<span data-ttu-id="ab709-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ab709-128">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab709-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ab709-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab709-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab709-130">Request</span></span>
<span data-ttu-id="ab709-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab709-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="ab709-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab709-132">Response</span></span>
<span data-ttu-id="ab709-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ab709-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
      "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
      "orderIdentifier": "Order Identifier value",
      "serialNumber": "Serial Number value",
      "productKey": "Product Key value",
      "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
      "state": {
        "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
        "deviceImportStatus": "pending",
        "deviceRegistrationId": "Device Registration Id value",
        "deviceErrorCode": 15,
        "deviceErrorName": "Device Error Name value"
      }
    }
  ]
}
```



