---
title: Список importedWindowsAutopilotDeviceIdentities
description: Список свойств и связей между объектамиimportedWindowsAutopilotDeviceIdentity.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a7b077021809dbd0927a48c8c940b29498792222
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364132"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="53862-103">Список importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="53862-103">List importedWindowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="53862-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53862-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53862-105">Список свойств и связей между объектами[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="53862-105">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53862-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="53862-106">Prerequisites</span></span>
<span data-ttu-id="53862-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53862-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53862-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53862-109">Permission type</span></span>|<span data-ttu-id="53862-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="53862-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53862-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53862-111">Delegated (work or school account)</span></span>|<span data-ttu-id="53862-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="53862-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="53862-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53862-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53862-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53862-114">Not supported.</span></span>|
|<span data-ttu-id="53862-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53862-115">Application</span></span>|<span data-ttu-id="53862-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53862-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53862-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53862-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="53862-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53862-118">Request headers</span></span>
|<span data-ttu-id="53862-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53862-119">Header</span></span>|<span data-ttu-id="53862-120">Значение</span><span class="sxs-lookup"><span data-stu-id="53862-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53862-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53862-121">Authorization</span></span>|<span data-ttu-id="53862-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53862-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53862-123">Accept</span><span class="sxs-lookup"><span data-stu-id="53862-123">Accept</span></span>|<span data-ttu-id="53862-124">application/json</span><span class="sxs-lookup"><span data-stu-id="53862-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53862-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53862-125">Request body</span></span>
<span data-ttu-id="53862-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53862-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53862-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="53862-127">Response</span></span>
<span data-ttu-id="53862-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="53862-128">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53862-129">Пример</span><span class="sxs-lookup"><span data-stu-id="53862-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="53862-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="53862-130">Request</span></span>
<span data-ttu-id="53862-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53862-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="53862-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="53862-132">Response</span></span>
<span data-ttu-id="53862-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53862-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




