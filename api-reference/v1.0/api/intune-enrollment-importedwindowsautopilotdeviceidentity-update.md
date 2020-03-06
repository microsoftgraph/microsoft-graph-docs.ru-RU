---
title: Обновление importedWindowsAutopilotDeviceIdentity
description: Обновляет свойства объекта importedWindowsAutopilotDeviceIdentity.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6a28e13eae11af95a8fe5d259298331f97c69148
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513401"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="d5d28-103">Обновление importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="d5d28-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="d5d28-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5d28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5d28-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5d28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5d28-106">Обновляет свойства объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="d5d28-106">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5d28-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d5d28-107">Prerequisites</span></span>
<span data-ttu-id="d5d28-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5d28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5d28-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5d28-110">Permission type</span></span>|<span data-ttu-id="d5d28-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5d28-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5d28-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5d28-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d5d28-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5d28-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d5d28-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5d28-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5d28-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5d28-115">Not supported.</span></span>|
|<span data-ttu-id="d5d28-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5d28-116">Application</span></span>|<span data-ttu-id="d5d28-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5d28-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5d28-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5d28-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="d5d28-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d5d28-119">Request headers</span></span>
|<span data-ttu-id="d5d28-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5d28-120">Header</span></span>|<span data-ttu-id="d5d28-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d5d28-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5d28-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5d28-122">Authorization</span></span>|<span data-ttu-id="d5d28-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5d28-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5d28-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d5d28-124">Accept</span></span>|<span data-ttu-id="d5d28-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d5d28-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5d28-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5d28-126">Request body</span></span>
<span data-ttu-id="d5d28-127">В теле запроса добавьте представление объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5d28-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="d5d28-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="d5d28-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="d5d28-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5d28-129">Property</span></span>|<span data-ttu-id="d5d28-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d5d28-130">Type</span></span>|<span data-ttu-id="d5d28-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d5d28-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5d28-132">id</span><span class="sxs-lookup"><span data-stu-id="d5d28-132">id</span></span>|<span data-ttu-id="d5d28-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d5d28-133">String</span></span>|<span data-ttu-id="d5d28-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="d5d28-134">The GUID for the object</span></span>|
|<span data-ttu-id="d5d28-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="d5d28-135">orderIdentifier</span></span>|<span data-ttu-id="d5d28-136">Строка</span><span class="sxs-lookup"><span data-stu-id="d5d28-136">String</span></span>|<span data-ttu-id="d5d28-137">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="d5d28-137">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d5d28-138">serialNumber</span><span class="sxs-lookup"><span data-stu-id="d5d28-138">serialNumber</span></span>|<span data-ttu-id="d5d28-139">String</span><span class="sxs-lookup"><span data-stu-id="d5d28-139">String</span></span>|<span data-ttu-id="d5d28-140">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="d5d28-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d5d28-141">productKey</span><span class="sxs-lookup"><span data-stu-id="d5d28-141">productKey</span></span>|<span data-ttu-id="d5d28-142">Строка</span><span class="sxs-lookup"><span data-stu-id="d5d28-142">String</span></span>|<span data-ttu-id="d5d28-143">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="d5d28-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d5d28-144">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="d5d28-144">hardwareIdentifier</span></span>|<span data-ttu-id="d5d28-145">Двоичный</span><span class="sxs-lookup"><span data-stu-id="d5d28-145">Binary</span></span>|<span data-ttu-id="d5d28-146">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="d5d28-146">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="d5d28-147">state</span><span class="sxs-lookup"><span data-stu-id="d5d28-147">state</span></span>|[<span data-ttu-id="d5d28-148">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="d5d28-148">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="d5d28-149">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="d5d28-149">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="d5d28-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="d5d28-150">Response</span></span>
<span data-ttu-id="d5d28-151">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d5d28-151">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5d28-152">Пример</span><span class="sxs-lookup"><span data-stu-id="d5d28-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5d28-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5d28-153">Request</span></span>
<span data-ttu-id="d5d28-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5d28-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 541

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
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
```

### <a name="response"></a><span data-ttu-id="d5d28-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5d28-155">Response</span></span>
<span data-ttu-id="d5d28-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5d28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

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
```




