---
title: Получение importedWindowsAutopilotDeviceIdentity
description: Чтение свойств и связей между объектамиimportedWindowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 786533d0c65b623c00e9326336f9993339033fb2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805308"
---
# <a name="get-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="7233e-103">Получение importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="7233e-103">Get importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="7233e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7233e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7233e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7233e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7233e-106">Чтение свойств и связей между объектами[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="7233e-106">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7233e-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7233e-107">Prerequisites</span></span>
<span data-ttu-id="7233e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7233e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7233e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7233e-110">Permission type</span></span>|<span data-ttu-id="7233e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7233e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7233e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7233e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7233e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7233e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="7233e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7233e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7233e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7233e-115">Not supported.</span></span>|
|<span data-ttu-id="7233e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7233e-116">Application</span></span>|<span data-ttu-id="7233e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7233e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7233e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7233e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7233e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7233e-119">Optional query parameters</span></span>
<span data-ttu-id="7233e-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7233e-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7233e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7233e-121">Request headers</span></span>
|<span data-ttu-id="7233e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7233e-122">Header</span></span>|<span data-ttu-id="7233e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7233e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7233e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7233e-124">Authorization</span></span>|<span data-ttu-id="7233e-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7233e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7233e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="7233e-126">Accept</span></span>|<span data-ttu-id="7233e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7233e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7233e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7233e-128">Request body</span></span>
<span data-ttu-id="7233e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7233e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7233e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7233e-130">Response</span></span>
<span data-ttu-id="7233e-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7233e-131">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7233e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7233e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7233e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7233e-133">Request</span></span>
<span data-ttu-id="7233e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7233e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="7233e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7233e-135">Response</span></span>
<span data-ttu-id="7233e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7233e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 671

{
  "value": {
    "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
    "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
    "orderIdentifier": "Order Identifier value",
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
    }
  }
}
```





