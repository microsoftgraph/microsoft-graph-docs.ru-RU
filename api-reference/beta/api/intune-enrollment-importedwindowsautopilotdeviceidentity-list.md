---
title: Список importedWindowsAutopilotDeviceIdentities
description: Список свойств и связей между объектамиimportedWindowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df41f60fe66622b8caadf706025a8f11507faa6d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701951"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="32a5a-103">Список importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="32a5a-103">List importedWindowsAutopilotDeviceIdentities</span></span>

<span data-ttu-id="32a5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32a5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32a5a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32a5a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32a5a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32a5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32a5a-107">Список свойств и связей между объектами[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="32a5a-107">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32a5a-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="32a5a-108">Prerequisites</span></span>
<span data-ttu-id="32a5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32a5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32a5a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32a5a-111">Permission type</span></span>|<span data-ttu-id="32a5a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32a5a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32a5a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32a5a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32a5a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="32a5a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="32a5a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32a5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32a5a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32a5a-116">Not supported.</span></span>|
|<span data-ttu-id="32a5a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32a5a-117">Application</span></span>|<span data-ttu-id="32a5a-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="32a5a-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32a5a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32a5a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="32a5a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="32a5a-120">Request headers</span></span>
|<span data-ttu-id="32a5a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32a5a-121">Header</span></span>|<span data-ttu-id="32a5a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="32a5a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32a5a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32a5a-123">Authorization</span></span>|<span data-ttu-id="32a5a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32a5a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32a5a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="32a5a-125">Accept</span></span>|<span data-ttu-id="32a5a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32a5a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32a5a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="32a5a-127">Request body</span></span>
<span data-ttu-id="32a5a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="32a5a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32a5a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="32a5a-129">Response</span></span>
<span data-ttu-id="32a5a-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="32a5a-130">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32a5a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="32a5a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="32a5a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="32a5a-132">Request</span></span>
<span data-ttu-id="32a5a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32a5a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="32a5a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="32a5a-134">Response</span></span>
<span data-ttu-id="32a5a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32a5a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 825

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
      "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
      "orderIdentifier": "Order Identifier value",
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





