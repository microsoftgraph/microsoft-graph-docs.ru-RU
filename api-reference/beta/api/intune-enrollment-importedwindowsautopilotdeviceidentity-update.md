---
title: Обновление importedWindowsAutopilotDeviceIdentity
description: Обновляет свойства объекта importedWindowsAutopilotDeviceIdentity.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5fa7434a5ee9e5218e6bfd40bad6b6497b5f4b47
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404787"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="50f35-103">Обновление importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="50f35-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="50f35-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="50f35-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="50f35-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50f35-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50f35-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50f35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50f35-107">Обновляет свойства объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="50f35-107">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50f35-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="50f35-108">Prerequisites</span></span>
<span data-ttu-id="50f35-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="50f35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="50f35-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50f35-111">Permission type</span></span>|<span data-ttu-id="50f35-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="50f35-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50f35-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50f35-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50f35-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50f35-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="50f35-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50f35-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50f35-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50f35-116">Not supported.</span></span>|
|<span data-ttu-id="50f35-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50f35-117">Application</span></span>|<span data-ttu-id="50f35-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50f35-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50f35-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50f35-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="50f35-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50f35-120">Request headers</span></span>
|<span data-ttu-id="50f35-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50f35-121">Header</span></span>|<span data-ttu-id="50f35-122">Значение</span><span class="sxs-lookup"><span data-stu-id="50f35-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50f35-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50f35-123">Authorization</span></span>|<span data-ttu-id="50f35-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="50f35-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50f35-125">Accept</span><span class="sxs-lookup"><span data-stu-id="50f35-125">Accept</span></span>|<span data-ttu-id="50f35-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50f35-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50f35-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="50f35-127">Request body</span></span>
<span data-ttu-id="50f35-128">В теле запроса добавьте представление объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50f35-128">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="50f35-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="50f35-129">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="50f35-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="50f35-130">Property</span></span>|<span data-ttu-id="50f35-131">Тип</span><span class="sxs-lookup"><span data-stu-id="50f35-131">Type</span></span>|<span data-ttu-id="50f35-132">Описание</span><span class="sxs-lookup"><span data-stu-id="50f35-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50f35-133">id</span><span class="sxs-lookup"><span data-stu-id="50f35-133">id</span></span>|<span data-ttu-id="50f35-134">Строка</span><span class="sxs-lookup"><span data-stu-id="50f35-134">String</span></span>|<span data-ttu-id="50f35-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="50f35-135">The GUID for the object</span></span>|
|<span data-ttu-id="50f35-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="50f35-136">orderIdentifier</span></span>|<span data-ttu-id="50f35-137">Строка</span><span class="sxs-lookup"><span data-stu-id="50f35-137">String</span></span>|<span data-ttu-id="50f35-138">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="50f35-138">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="50f35-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="50f35-139">serialNumber</span></span>|<span data-ttu-id="50f35-140">Строка</span><span class="sxs-lookup"><span data-stu-id="50f35-140">String</span></span>|<span data-ttu-id="50f35-141">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="50f35-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="50f35-142">productKey</span><span class="sxs-lookup"><span data-stu-id="50f35-142">productKey</span></span>|<span data-ttu-id="50f35-143">Строка</span><span class="sxs-lookup"><span data-stu-id="50f35-143">String</span></span>|<span data-ttu-id="50f35-144">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="50f35-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="50f35-145">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="50f35-145">hardwareIdentifier</span></span>|<span data-ttu-id="50f35-146">Двоичный</span><span class="sxs-lookup"><span data-stu-id="50f35-146">Binary</span></span>|<span data-ttu-id="50f35-147">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="50f35-147">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="50f35-148">state</span><span class="sxs-lookup"><span data-stu-id="50f35-148">state</span></span>|[<span data-ttu-id="50f35-149">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="50f35-149">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="50f35-150">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="50f35-150">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="50f35-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="50f35-151">Response</span></span>
<span data-ttu-id="50f35-152">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="50f35-152">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50f35-153">Пример</span><span class="sxs-lookup"><span data-stu-id="50f35-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="50f35-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="50f35-154">Request</span></span>
<span data-ttu-id="50f35-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50f35-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="50f35-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="50f35-156">Response</span></span>
<span data-ttu-id="50f35-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="50f35-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




