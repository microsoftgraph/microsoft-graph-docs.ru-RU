---
title: Обновление importedWindowsAutopilotDeviceIdentity
description: Обновляет свойства объекта importedWindowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a81e7b8291bab7698869c60d5403fd07be08cb5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261336"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="5b15e-103">Обновление importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="5b15e-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="5b15e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b15e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b15e-105">Обновляет свойства объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="5b15e-105">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b15e-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5b15e-106">Prerequisites</span></span>
<span data-ttu-id="5b15e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5b15e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5b15e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b15e-109">Permission type</span></span>|<span data-ttu-id="5b15e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b15e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b15e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b15e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5b15e-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b15e-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5b15e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b15e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b15e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b15e-114">Not supported.</span></span>|
|<span data-ttu-id="5b15e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b15e-115">Application</span></span>|<span data-ttu-id="5b15e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b15e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b15e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b15e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="5b15e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b15e-118">Request headers</span></span>
|<span data-ttu-id="5b15e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b15e-119">Header</span></span>|<span data-ttu-id="5b15e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5b15e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b15e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b15e-121">Authorization</span></span>|<span data-ttu-id="5b15e-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5b15e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b15e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5b15e-123">Accept</span></span>|<span data-ttu-id="5b15e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5b15e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b15e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5b15e-125">Request body</span></span>
<span data-ttu-id="5b15e-126">В теле запроса добавьте представление объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b15e-126">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="5b15e-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="5b15e-127">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="5b15e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b15e-128">Property</span></span>|<span data-ttu-id="5b15e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="5b15e-129">Type</span></span>|<span data-ttu-id="5b15e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5b15e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b15e-131">id</span><span class="sxs-lookup"><span data-stu-id="5b15e-131">id</span></span>|<span data-ttu-id="5b15e-132">String</span><span class="sxs-lookup"><span data-stu-id="5b15e-132">String</span></span>|<span data-ttu-id="5b15e-133">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="5b15e-133">The GUID for the object</span></span>|
|<span data-ttu-id="5b15e-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="5b15e-134">orderIdentifier</span></span>|<span data-ttu-id="5b15e-135">String</span><span class="sxs-lookup"><span data-stu-id="5b15e-135">String</span></span>|<span data-ttu-id="5b15e-136">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="5b15e-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5b15e-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="5b15e-137">serialNumber</span></span>|<span data-ttu-id="5b15e-138">String</span><span class="sxs-lookup"><span data-stu-id="5b15e-138">String</span></span>|<span data-ttu-id="5b15e-139">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="5b15e-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5b15e-140">productKey</span><span class="sxs-lookup"><span data-stu-id="5b15e-140">productKey</span></span>|<span data-ttu-id="5b15e-141">Строка</span><span class="sxs-lookup"><span data-stu-id="5b15e-141">String</span></span>|<span data-ttu-id="5b15e-142">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="5b15e-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5b15e-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="5b15e-143">hardwareIdentifier</span></span>|<span data-ttu-id="5b15e-144">Двоичный</span><span class="sxs-lookup"><span data-stu-id="5b15e-144">Binary</span></span>|<span data-ttu-id="5b15e-145">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="5b15e-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5b15e-146">state</span><span class="sxs-lookup"><span data-stu-id="5b15e-146">state</span></span>|[<span data-ttu-id="5b15e-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="5b15e-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="5b15e-148">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="5b15e-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="5b15e-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b15e-149">Response</span></span>
<span data-ttu-id="5b15e-150">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5b15e-150">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b15e-151">Пример</span><span class="sxs-lookup"><span data-stu-id="5b15e-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b15e-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b15e-152">Request</span></span>
<span data-ttu-id="5b15e-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b15e-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b15e-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b15e-154">Response</span></span>
<span data-ttu-id="5b15e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5b15e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



