---
title: Создать importedWindowsAutopilotDeviceIdentity
description: Создать новый объект importedWindowsAutopilotDeviceIdentity.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 74a1c84c9a7d88f83e7cf3dcaf64b05b13eeb55d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364174"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="70a31-103">Создать importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="70a31-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="70a31-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70a31-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70a31-105">Создать новый объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="70a31-105">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70a31-106">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="70a31-106">Prerequisites</span></span>
<span data-ttu-id="70a31-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70a31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70a31-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70a31-109">Permission type</span></span>|<span data-ttu-id="70a31-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="70a31-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70a31-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70a31-111">Delegated (work or school account)</span></span>|<span data-ttu-id="70a31-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70a31-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="70a31-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70a31-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70a31-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70a31-114">Not supported.</span></span>|
|<span data-ttu-id="70a31-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70a31-115">Application</span></span>|<span data-ttu-id="70a31-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70a31-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70a31-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70a31-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="70a31-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70a31-118">Request headers</span></span>
|<span data-ttu-id="70a31-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70a31-119">Header</span></span>|<span data-ttu-id="70a31-120">Значение</span><span class="sxs-lookup"><span data-stu-id="70a31-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70a31-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70a31-121">Authorization</span></span>|<span data-ttu-id="70a31-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70a31-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70a31-123">Accept</span><span class="sxs-lookup"><span data-stu-id="70a31-123">Accept</span></span>|<span data-ttu-id="70a31-124">application/json</span><span class="sxs-lookup"><span data-stu-id="70a31-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70a31-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70a31-125">Request body</span></span>
<span data-ttu-id="70a31-126">В тексте запроса добавьте представление объекта importedWindowsAutopilotDeviceIdentity в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70a31-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="70a31-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="70a31-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="70a31-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="70a31-128">Property</span></span>|<span data-ttu-id="70a31-129">Тип</span><span class="sxs-lookup"><span data-stu-id="70a31-129">Type</span></span>|<span data-ttu-id="70a31-130">Описание</span><span class="sxs-lookup"><span data-stu-id="70a31-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70a31-131">id</span><span class="sxs-lookup"><span data-stu-id="70a31-131">id</span></span>|<span data-ttu-id="70a31-132">String</span><span class="sxs-lookup"><span data-stu-id="70a31-132">String</span></span>|<span data-ttu-id="70a31-133">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="70a31-133">The GUID for the object</span></span>|
|<span data-ttu-id="70a31-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="70a31-134">orderIdentifier</span></span>|<span data-ttu-id="70a31-135">String</span><span class="sxs-lookup"><span data-stu-id="70a31-135">String</span></span>|<span data-ttu-id="70a31-136">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="70a31-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="70a31-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="70a31-137">serialNumber</span></span>|<span data-ttu-id="70a31-138">String</span><span class="sxs-lookup"><span data-stu-id="70a31-138">String</span></span>|<span data-ttu-id="70a31-139">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="70a31-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="70a31-140">productKey</span><span class="sxs-lookup"><span data-stu-id="70a31-140">productKey</span></span>|<span data-ttu-id="70a31-141">Строка</span><span class="sxs-lookup"><span data-stu-id="70a31-141">String</span></span>|<span data-ttu-id="70a31-142">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="70a31-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="70a31-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="70a31-143">hardwareIdentifier</span></span>|<span data-ttu-id="70a31-144">Двоичный</span><span class="sxs-lookup"><span data-stu-id="70a31-144">Binary</span></span>|<span data-ttu-id="70a31-145">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="70a31-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="70a31-146">state</span><span class="sxs-lookup"><span data-stu-id="70a31-146">state</span></span>|[<span data-ttu-id="70a31-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="70a31-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="70a31-148">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="70a31-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="70a31-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="70a31-149">Response</span></span>
<span data-ttu-id="70a31-150">В случае успешного выполнения данный метод возвращает код отклика `201 Created` и объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="70a31-150">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70a31-151">Пример</span><span class="sxs-lookup"><span data-stu-id="70a31-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="70a31-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="70a31-152">Request</span></span>
<span data-ttu-id="70a31-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70a31-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="70a31-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="70a31-154">Response</span></span>
<span data-ttu-id="70a31-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70a31-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




