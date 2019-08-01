---
title: Обновление importedWindowsAutopilotDeviceIdentity
description: Обновляет свойства объекта importedWindowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4ac55088b70b31057b026e16263995c9c37b858f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020866"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="b0678-103">Обновление importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="b0678-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="b0678-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0678-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0678-105">Обновляет свойства объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="b0678-105">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0678-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b0678-106">Prerequisites</span></span>
<span data-ttu-id="b0678-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0678-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0678-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0678-109">Permission type</span></span>|<span data-ttu-id="b0678-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0678-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0678-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0678-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b0678-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0678-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b0678-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0678-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0678-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0678-114">Not supported.</span></span>|
|<span data-ttu-id="b0678-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0678-115">Application</span></span>|<span data-ttu-id="b0678-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0678-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0678-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0678-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="b0678-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0678-118">Request headers</span></span>
|<span data-ttu-id="b0678-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0678-119">Header</span></span>|<span data-ttu-id="b0678-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b0678-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0678-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0678-121">Authorization</span></span>|<span data-ttu-id="b0678-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0678-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0678-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b0678-123">Accept</span></span>|<span data-ttu-id="b0678-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b0678-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0678-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b0678-125">Request body</span></span>
<span data-ttu-id="b0678-126">В теле запроса добавьте представление объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0678-126">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="b0678-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="b0678-127">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="b0678-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0678-128">Property</span></span>|<span data-ttu-id="b0678-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b0678-129">Type</span></span>|<span data-ttu-id="b0678-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b0678-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0678-131">id</span><span class="sxs-lookup"><span data-stu-id="b0678-131">id</span></span>|<span data-ttu-id="b0678-132">String</span><span class="sxs-lookup"><span data-stu-id="b0678-132">String</span></span>|<span data-ttu-id="b0678-133">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="b0678-133">The GUID for the object</span></span>|
|<span data-ttu-id="b0678-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="b0678-134">orderIdentifier</span></span>|<span data-ttu-id="b0678-135">String</span><span class="sxs-lookup"><span data-stu-id="b0678-135">String</span></span>|<span data-ttu-id="b0678-136">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="b0678-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b0678-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="b0678-137">serialNumber</span></span>|<span data-ttu-id="b0678-138">String</span><span class="sxs-lookup"><span data-stu-id="b0678-138">String</span></span>|<span data-ttu-id="b0678-139">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="b0678-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b0678-140">productKey</span><span class="sxs-lookup"><span data-stu-id="b0678-140">productKey</span></span>|<span data-ttu-id="b0678-141">Строка</span><span class="sxs-lookup"><span data-stu-id="b0678-141">String</span></span>|<span data-ttu-id="b0678-142">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="b0678-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b0678-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="b0678-143">hardwareIdentifier</span></span>|<span data-ttu-id="b0678-144">Двоичный</span><span class="sxs-lookup"><span data-stu-id="b0678-144">Binary</span></span>|<span data-ttu-id="b0678-145">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="b0678-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b0678-146">state</span><span class="sxs-lookup"><span data-stu-id="b0678-146">state</span></span>|[<span data-ttu-id="b0678-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="b0678-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="b0678-148">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="b0678-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="b0678-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0678-149">Response</span></span>
<span data-ttu-id="b0678-150">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b0678-150">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0678-151">Пример</span><span class="sxs-lookup"><span data-stu-id="b0678-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0678-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0678-152">Request</span></span>
<span data-ttu-id="b0678-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0678-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b0678-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0678-154">Response</span></span>
<span data-ttu-id="b0678-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0678-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



