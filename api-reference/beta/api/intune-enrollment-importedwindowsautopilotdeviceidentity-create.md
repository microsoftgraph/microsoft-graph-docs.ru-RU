---
title: Создать importedWindowsAutopilotDeviceIdentity
description: Создать новый объект importedWindowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f7a35693408b214d028af90945e0d3179af83395
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532725"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="93e60-103">Создать importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="93e60-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="93e60-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93e60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93e60-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93e60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93e60-106">Создать новый объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="93e60-106">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93e60-107">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="93e60-107">Prerequisites</span></span>
<span data-ttu-id="93e60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93e60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93e60-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93e60-110">Permission type</span></span>|<span data-ttu-id="93e60-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="93e60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93e60-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93e60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="93e60-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93e60-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="93e60-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93e60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93e60-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93e60-115">Not supported.</span></span>|
|<span data-ttu-id="93e60-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93e60-116">Application</span></span>|<span data-ttu-id="93e60-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93e60-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93e60-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93e60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="93e60-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93e60-119">Request headers</span></span>
|<span data-ttu-id="93e60-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93e60-120">Header</span></span>|<span data-ttu-id="93e60-121">Значение</span><span class="sxs-lookup"><span data-stu-id="93e60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93e60-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93e60-122">Authorization</span></span>|<span data-ttu-id="93e60-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93e60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93e60-124">Accept</span><span class="sxs-lookup"><span data-stu-id="93e60-124">Accept</span></span>|<span data-ttu-id="93e60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="93e60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93e60-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93e60-126">Request body</span></span>
<span data-ttu-id="93e60-127">В тексте запроса добавьте представление объекта importedWindowsAutopilotDeviceIdentity в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93e60-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="93e60-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="93e60-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="93e60-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="93e60-129">Property</span></span>|<span data-ttu-id="93e60-130">Тип</span><span class="sxs-lookup"><span data-stu-id="93e60-130">Type</span></span>|<span data-ttu-id="93e60-131">Описание</span><span class="sxs-lookup"><span data-stu-id="93e60-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93e60-132">id</span><span class="sxs-lookup"><span data-stu-id="93e60-132">id</span></span>|<span data-ttu-id="93e60-133">String</span><span class="sxs-lookup"><span data-stu-id="93e60-133">String</span></span>|<span data-ttu-id="93e60-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="93e60-134">The GUID for the object</span></span>|
|<span data-ttu-id="93e60-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="93e60-135">orderIdentifier</span></span>|<span data-ttu-id="93e60-136">String</span><span class="sxs-lookup"><span data-stu-id="93e60-136">String</span></span>|<span data-ttu-id="93e60-137">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="93e60-137">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="93e60-138">serialNumber</span><span class="sxs-lookup"><span data-stu-id="93e60-138">serialNumber</span></span>|<span data-ttu-id="93e60-139">String</span><span class="sxs-lookup"><span data-stu-id="93e60-139">String</span></span>|<span data-ttu-id="93e60-140">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="93e60-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="93e60-141">productKey</span><span class="sxs-lookup"><span data-stu-id="93e60-141">productKey</span></span>|<span data-ttu-id="93e60-142">Строка</span><span class="sxs-lookup"><span data-stu-id="93e60-142">String</span></span>|<span data-ttu-id="93e60-143">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="93e60-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="93e60-144">Импортид</span><span class="sxs-lookup"><span data-stu-id="93e60-144">importId</span></span>|<span data-ttu-id="93e60-145">String</span><span class="sxs-lookup"><span data-stu-id="93e60-145">String</span></span>|<span data-ttu-id="93e60-146">Идентификатор импорта для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="93e60-146">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="93e60-147">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="93e60-147">hardwareIdentifier</span></span>|<span data-ttu-id="93e60-148">Двоичный</span><span class="sxs-lookup"><span data-stu-id="93e60-148">Binary</span></span>|<span data-ttu-id="93e60-149">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="93e60-149">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="93e60-150">state</span><span class="sxs-lookup"><span data-stu-id="93e60-150">state</span></span>|[<span data-ttu-id="93e60-151">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="93e60-151">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="93e60-152">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="93e60-152">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="93e60-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="93e60-153">Response</span></span>
<span data-ttu-id="93e60-154">В случае успешного выполнения данный метод возвращает код отклика `201 Created` и объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="93e60-154">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93e60-155">Пример</span><span class="sxs-lookup"><span data-stu-id="93e60-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="93e60-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="93e60-156">Request</span></span>
<span data-ttu-id="93e60-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93e60-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 575

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
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
```

### <a name="response"></a><span data-ttu-id="93e60-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="93e60-158">Response</span></span>
<span data-ttu-id="93e60-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93e60-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 624

{
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
```





