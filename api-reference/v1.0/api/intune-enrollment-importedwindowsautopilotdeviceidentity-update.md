---
title: Обновление importedWindowsAutopilotDeviceIdentity
description: Обновляет свойства объекта importedWindowsAutopilotDeviceIdentity.
ms.openlocfilehash: ec784e6f0032e0167c9b9339d65568d923ee3c74
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028105"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="74051-103">Обновление importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="74051-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="74051-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="74051-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74051-105">Обновляет свойства объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="74051-105">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="74051-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="74051-106">Prerequisites</span></span>
<span data-ttu-id="74051-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74051-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74051-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74051-109">Permission type</span></span>|<span data-ttu-id="74051-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="74051-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74051-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74051-111">Delegated (work or school account)</span></span>|<span data-ttu-id="74051-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74051-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="74051-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74051-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74051-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74051-114">Not supported.</span></span>|
|<span data-ttu-id="74051-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74051-115">Application</span></span>|<span data-ttu-id="74051-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74051-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74051-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74051-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="74051-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74051-118">Request headers</span></span>
|<span data-ttu-id="74051-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74051-119">Header</span></span>|<span data-ttu-id="74051-120">Значение</span><span class="sxs-lookup"><span data-stu-id="74051-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74051-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="74051-121">Authorization</span></span>|<span data-ttu-id="74051-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="74051-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74051-123">Accept</span><span class="sxs-lookup"><span data-stu-id="74051-123">Accept</span></span>|<span data-ttu-id="74051-124">application/json</span><span class="sxs-lookup"><span data-stu-id="74051-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74051-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="74051-125">Request body</span></span>
<span data-ttu-id="74051-126">В теле запроса добавьте представление объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74051-126">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="74051-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="74051-127">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="74051-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="74051-128">Property</span></span>|<span data-ttu-id="74051-129">Тип</span><span class="sxs-lookup"><span data-stu-id="74051-129">Type</span></span>|<span data-ttu-id="74051-130">Описание</span><span class="sxs-lookup"><span data-stu-id="74051-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74051-131">id</span><span class="sxs-lookup"><span data-stu-id="74051-131">id</span></span>|<span data-ttu-id="74051-132">Строка</span><span class="sxs-lookup"><span data-stu-id="74051-132">String</span></span>|<span data-ttu-id="74051-133">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="74051-133">The GUID for the object</span></span>|
|<span data-ttu-id="74051-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="74051-134">orderIdentifier</span></span>|<span data-ttu-id="74051-135">Строка</span><span class="sxs-lookup"><span data-stu-id="74051-135">String</span></span>|<span data-ttu-id="74051-136">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="74051-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="74051-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="74051-137">serialNumber</span></span>|<span data-ttu-id="74051-138">Строка</span><span class="sxs-lookup"><span data-stu-id="74051-138">String</span></span>|<span data-ttu-id="74051-139">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="74051-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="74051-140">productKey</span><span class="sxs-lookup"><span data-stu-id="74051-140">productKey</span></span>|<span data-ttu-id="74051-141">Строка</span><span class="sxs-lookup"><span data-stu-id="74051-141">String</span></span>|<span data-ttu-id="74051-142">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="74051-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="74051-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="74051-143">hardwareIdentifier</span></span>|<span data-ttu-id="74051-144">Двоичный</span><span class="sxs-lookup"><span data-stu-id="74051-144">Binary</span></span>|<span data-ttu-id="74051-145">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="74051-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="74051-146">state</span><span class="sxs-lookup"><span data-stu-id="74051-146">state</span></span>|[<span data-ttu-id="74051-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="74051-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="74051-148">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="74051-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="74051-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="74051-149">Response</span></span>
<span data-ttu-id="74051-150">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="74051-150">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74051-151">Пример</span><span class="sxs-lookup"><span data-stu-id="74051-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="74051-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="74051-152">Request</span></span>
<span data-ttu-id="74051-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74051-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="74051-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="74051-154">Response</span></span>
<span data-ttu-id="74051-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="74051-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



