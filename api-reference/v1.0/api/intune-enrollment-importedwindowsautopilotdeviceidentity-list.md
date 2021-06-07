---
title: Список importedWindowsAutopilotDeviceIdentities
description: Список свойств и связей между объектамиimportedWindowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 65f0b42d7aae5932443460250e82ad18951eeaab
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753402"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="9f6ff-103">Список importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="9f6ff-103">List importedWindowsAutopilotDeviceIdentities</span></span>

<span data-ttu-id="9f6ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f6ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f6ff-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f6ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f6ff-106">Список свойств и связей между объектами[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="9f6ff-106">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f6ff-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9f6ff-107">Prerequisites</span></span>
<span data-ttu-id="9f6ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f6ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f6ff-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f6ff-110">Permission type</span></span>|<span data-ttu-id="9f6ff-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f6ff-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f6ff-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f6ff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f6ff-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f6ff-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9f6ff-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f6ff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f6ff-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f6ff-115">Not supported.</span></span>|
|<span data-ttu-id="9f6ff-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9f6ff-116">Application</span></span>|<span data-ttu-id="9f6ff-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f6ff-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f6ff-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f6ff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="9f6ff-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9f6ff-119">Request headers</span></span>
|<span data-ttu-id="9f6ff-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f6ff-120">Header</span></span>|<span data-ttu-id="9f6ff-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9f6ff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f6ff-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f6ff-122">Authorization</span></span>|<span data-ttu-id="9f6ff-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f6ff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f6ff-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9f6ff-124">Accept</span></span>|<span data-ttu-id="9f6ff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f6ff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f6ff-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f6ff-126">Request body</span></span>
<span data-ttu-id="9f6ff-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f6ff-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f6ff-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f6ff-128">Response</span></span>
<span data-ttu-id="9f6ff-129">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9f6ff-129">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f6ff-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9f6ff-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f6ff-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f6ff-131">Request</span></span>
<span data-ttu-id="9f6ff-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f6ff-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="9f6ff-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f6ff-133">Response</span></span>
<span data-ttu-id="9f6ff-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f6ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 773

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
      "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
      "groupTag": "Group Tag value",
      "serialNumber": "Serial Number value",
      "productKey": "Product Key value",
      "importId": "Import Id value",
      "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
      "state": {
        "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
        "deviceImportStatus": "pending",
        "deviceRegistrationId": "Device Registration Id value",
        "deviceErrorCode": 15,
        "deviceErrorName": "Device Error Name value"
      },
      "assignedUserPrincipalName": "Assigned User Principal Name value"
    }
  ]
}
```




