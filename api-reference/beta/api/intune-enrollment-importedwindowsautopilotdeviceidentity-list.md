---
title: Список importedWindowsAutopilotDeviceIdentities
description: Список свойств и связей между объектамиimportedWindowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a3e41dddd5c5fd1dd46f6df67376b5215f563e3a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159027"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="b53f6-103">Список importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="b53f6-103">List importedWindowsAutopilotDeviceIdentities</span></span>

<span data-ttu-id="b53f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b53f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b53f6-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b53f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b53f6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b53f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b53f6-107">Список свойств и связей между объектами[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="b53f6-107">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b53f6-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b53f6-108">Prerequisites</span></span>
<span data-ttu-id="b53f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b53f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b53f6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b53f6-111">Permission type</span></span>|<span data-ttu-id="b53f6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b53f6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b53f6-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b53f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b53f6-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b53f6-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b53f6-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b53f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b53f6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b53f6-116">Not supported.</span></span>|
|<span data-ttu-id="b53f6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b53f6-117">Application</span></span>|<span data-ttu-id="b53f6-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b53f6-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b53f6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b53f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="b53f6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b53f6-120">Request headers</span></span>
|<span data-ttu-id="b53f6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b53f6-121">Header</span></span>|<span data-ttu-id="b53f6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b53f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b53f6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b53f6-123">Authorization</span></span>|<span data-ttu-id="b53f6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b53f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b53f6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b53f6-125">Accept</span></span>|<span data-ttu-id="b53f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b53f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b53f6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b53f6-127">Request body</span></span>
<span data-ttu-id="b53f6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b53f6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b53f6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b53f6-129">Response</span></span>
<span data-ttu-id="b53f6-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b53f6-130">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b53f6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b53f6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b53f6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b53f6-132">Request</span></span>
<span data-ttu-id="b53f6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b53f6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="b53f6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b53f6-134">Response</span></span>
<span data-ttu-id="b53f6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b53f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




