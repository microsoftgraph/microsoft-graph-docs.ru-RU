---
title: Создать importedWindowsAutopilotDeviceIdentity
description: Создать новый объект importedWindowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2ed8ed1af797e68998318f5ef7dea3836343cff4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968933"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="a1950-103">Создать importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="a1950-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="a1950-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1950-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1950-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1950-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1950-106">Создать новый объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="a1950-106">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1950-107">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="a1950-107">Prerequisites</span></span>
<span data-ttu-id="a1950-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1950-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1950-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1950-110">Permission type</span></span>|<span data-ttu-id="a1950-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1950-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1950-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1950-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1950-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1950-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a1950-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1950-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1950-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1950-115">Not supported.</span></span>|
|<span data-ttu-id="a1950-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1950-116">Application</span></span>|<span data-ttu-id="a1950-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1950-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1950-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1950-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="a1950-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1950-119">Request headers</span></span>
|<span data-ttu-id="a1950-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1950-120">Header</span></span>|<span data-ttu-id="a1950-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a1950-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1950-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1950-122">Authorization</span></span>|<span data-ttu-id="a1950-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1950-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1950-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a1950-124">Accept</span></span>|<span data-ttu-id="a1950-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1950-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1950-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1950-126">Request body</span></span>
<span data-ttu-id="a1950-127">В тексте запроса добавьте представление объекта importedWindowsAutopilotDeviceIdentity в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1950-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="a1950-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="a1950-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="a1950-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1950-129">Property</span></span>|<span data-ttu-id="a1950-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a1950-130">Type</span></span>|<span data-ttu-id="a1950-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a1950-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1950-132">id</span><span class="sxs-lookup"><span data-stu-id="a1950-132">id</span></span>|<span data-ttu-id="a1950-133">String</span><span class="sxs-lookup"><span data-stu-id="a1950-133">String</span></span>|<span data-ttu-id="a1950-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="a1950-134">The GUID for the object</span></span>|
|<span data-ttu-id="a1950-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="a1950-135">orderIdentifier</span></span>|<span data-ttu-id="a1950-136">String</span><span class="sxs-lookup"><span data-stu-id="a1950-136">String</span></span>|<span data-ttu-id="a1950-137">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="a1950-137">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a1950-138">serialNumber</span><span class="sxs-lookup"><span data-stu-id="a1950-138">serialNumber</span></span>|<span data-ttu-id="a1950-139">String</span><span class="sxs-lookup"><span data-stu-id="a1950-139">String</span></span>|<span data-ttu-id="a1950-140">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="a1950-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a1950-141">productKey</span><span class="sxs-lookup"><span data-stu-id="a1950-141">productKey</span></span>|<span data-ttu-id="a1950-142">Строка</span><span class="sxs-lookup"><span data-stu-id="a1950-142">String</span></span>|<span data-ttu-id="a1950-143">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="a1950-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a1950-144">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="a1950-144">hardwareIdentifier</span></span>|<span data-ttu-id="a1950-145">Двоичный</span><span class="sxs-lookup"><span data-stu-id="a1950-145">Binary</span></span>|<span data-ttu-id="a1950-146">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="a1950-146">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a1950-147">state</span><span class="sxs-lookup"><span data-stu-id="a1950-147">state</span></span>|[<span data-ttu-id="a1950-148">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="a1950-148">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="a1950-149">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="a1950-149">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="a1950-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1950-150">Response</span></span>
<span data-ttu-id="a1950-151">В случае успешного выполнения данный метод возвращает код отклика `201 Created` и объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="a1950-151">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1950-152">Пример</span><span class="sxs-lookup"><span data-stu-id="a1950-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1950-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1950-153">Request</span></span>
<span data-ttu-id="a1950-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1950-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="a1950-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1950-155">Response</span></span>
<span data-ttu-id="a1950-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1950-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




