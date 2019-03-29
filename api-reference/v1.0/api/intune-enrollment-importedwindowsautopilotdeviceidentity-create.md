---
title: Создать importedWindowsAutopilotDeviceIdentity
description: Создать новый объект importedWindowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 664b0d52eea5d61918e234c9fa582fa57f50d8b5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980098"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="28034-103">Создать importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="28034-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="28034-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28034-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28034-105">Создать новый объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="28034-105">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28034-106">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="28034-106">Prerequisites</span></span>
<span data-ttu-id="28034-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28034-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28034-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28034-109">Permission type</span></span>|<span data-ttu-id="28034-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="28034-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28034-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28034-111">Delegated (work or school account)</span></span>|<span data-ttu-id="28034-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28034-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="28034-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28034-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28034-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28034-114">Not supported.</span></span>|
|<span data-ttu-id="28034-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28034-115">Application</span></span>|<span data-ttu-id="28034-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28034-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28034-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28034-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="28034-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28034-118">Request headers</span></span>
|<span data-ttu-id="28034-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28034-119">Header</span></span>|<span data-ttu-id="28034-120">Значение</span><span class="sxs-lookup"><span data-stu-id="28034-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28034-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28034-121">Authorization</span></span>|<span data-ttu-id="28034-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28034-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28034-123">Accept</span><span class="sxs-lookup"><span data-stu-id="28034-123">Accept</span></span>|<span data-ttu-id="28034-124">application/json</span><span class="sxs-lookup"><span data-stu-id="28034-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28034-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28034-125">Request body</span></span>
<span data-ttu-id="28034-126">В тексте запроса добавьте представление объекта importedWindowsAutopilotDeviceIdentity в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28034-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="28034-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="28034-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="28034-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="28034-128">Property</span></span>|<span data-ttu-id="28034-129">Тип</span><span class="sxs-lookup"><span data-stu-id="28034-129">Type</span></span>|<span data-ttu-id="28034-130">Описание</span><span class="sxs-lookup"><span data-stu-id="28034-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28034-131">id</span><span class="sxs-lookup"><span data-stu-id="28034-131">id</span></span>|<span data-ttu-id="28034-132">String</span><span class="sxs-lookup"><span data-stu-id="28034-132">String</span></span>|<span data-ttu-id="28034-133">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="28034-133">The GUID for the object</span></span>|
|<span data-ttu-id="28034-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="28034-134">orderIdentifier</span></span>|<span data-ttu-id="28034-135">String</span><span class="sxs-lookup"><span data-stu-id="28034-135">String</span></span>|<span data-ttu-id="28034-136">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="28034-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="28034-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="28034-137">serialNumber</span></span>|<span data-ttu-id="28034-138">String</span><span class="sxs-lookup"><span data-stu-id="28034-138">String</span></span>|<span data-ttu-id="28034-139">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="28034-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="28034-140">productKey</span><span class="sxs-lookup"><span data-stu-id="28034-140">productKey</span></span>|<span data-ttu-id="28034-141">Строка</span><span class="sxs-lookup"><span data-stu-id="28034-141">String</span></span>|<span data-ttu-id="28034-142">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="28034-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="28034-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="28034-143">hardwareIdentifier</span></span>|<span data-ttu-id="28034-144">Двоичный</span><span class="sxs-lookup"><span data-stu-id="28034-144">Binary</span></span>|<span data-ttu-id="28034-145">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="28034-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="28034-146">state</span><span class="sxs-lookup"><span data-stu-id="28034-146">state</span></span>|[<span data-ttu-id="28034-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="28034-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="28034-148">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="28034-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="28034-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="28034-149">Response</span></span>
<span data-ttu-id="28034-150">В случае успешного выполнения данный метод возвращает код отклика `201 Created` и объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="28034-150">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28034-151">Пример</span><span class="sxs-lookup"><span data-stu-id="28034-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="28034-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="28034-152">Request</span></span>
<span data-ttu-id="28034-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28034-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="28034-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="28034-154">Response</span></span>
<span data-ttu-id="28034-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28034-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



