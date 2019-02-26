---
title: Создать importedWindowsAutopilotDeviceIdentity
description: Создание нового объекта importedWindowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b7aa20bae6db2d3e93178439836ea8abded8563b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251708"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="87a7c-103">Создать importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="87a7c-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="87a7c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87a7c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87a7c-105">Создать новый объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="87a7c-105">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87a7c-106">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="87a7c-106">Prerequisites</span></span>
<span data-ttu-id="87a7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="87a7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="87a7c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87a7c-109">Permission type</span></span>|<span data-ttu-id="87a7c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="87a7c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87a7c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87a7c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="87a7c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87a7c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="87a7c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87a7c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87a7c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87a7c-114">Not supported.</span></span>|
|<span data-ttu-id="87a7c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87a7c-115">Application</span></span>|<span data-ttu-id="87a7c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87a7c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87a7c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87a7c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="87a7c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87a7c-118">Request headers</span></span>
|<span data-ttu-id="87a7c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87a7c-119">Header</span></span>|<span data-ttu-id="87a7c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="87a7c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87a7c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="87a7c-121">Authorization</span></span>|<span data-ttu-id="87a7c-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="87a7c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87a7c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="87a7c-123">Accept</span></span>|<span data-ttu-id="87a7c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="87a7c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87a7c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87a7c-125">Request body</span></span>
<span data-ttu-id="87a7c-126">В тексте запроса добавьте представление объекта importedWindowsAutopilotDeviceIdentity в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87a7c-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="87a7c-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="87a7c-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="87a7c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="87a7c-128">Property</span></span>|<span data-ttu-id="87a7c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="87a7c-129">Type</span></span>|<span data-ttu-id="87a7c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="87a7c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87a7c-131">id</span><span class="sxs-lookup"><span data-stu-id="87a7c-131">id</span></span>|<span data-ttu-id="87a7c-132">String</span><span class="sxs-lookup"><span data-stu-id="87a7c-132">String</span></span>|<span data-ttu-id="87a7c-133">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="87a7c-133">The GUID for the object</span></span>|
|<span data-ttu-id="87a7c-134">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="87a7c-134">orderIdentifier</span></span>|<span data-ttu-id="87a7c-135">String</span><span class="sxs-lookup"><span data-stu-id="87a7c-135">String</span></span>|<span data-ttu-id="87a7c-136">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="87a7c-136">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="87a7c-137">serialNumber</span><span class="sxs-lookup"><span data-stu-id="87a7c-137">serialNumber</span></span>|<span data-ttu-id="87a7c-138">String</span><span class="sxs-lookup"><span data-stu-id="87a7c-138">String</span></span>|<span data-ttu-id="87a7c-139">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="87a7c-139">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="87a7c-140">productKey</span><span class="sxs-lookup"><span data-stu-id="87a7c-140">productKey</span></span>|<span data-ttu-id="87a7c-141">Строка</span><span class="sxs-lookup"><span data-stu-id="87a7c-141">String</span></span>|<span data-ttu-id="87a7c-142">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="87a7c-142">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="87a7c-143">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="87a7c-143">hardwareIdentifier</span></span>|<span data-ttu-id="87a7c-144">Двоичный</span><span class="sxs-lookup"><span data-stu-id="87a7c-144">Binary</span></span>|<span data-ttu-id="87a7c-145">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="87a7c-145">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="87a7c-146">state</span><span class="sxs-lookup"><span data-stu-id="87a7c-146">state</span></span>|[<span data-ttu-id="87a7c-147">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="87a7c-147">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="87a7c-148">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="87a7c-148">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="87a7c-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="87a7c-149">Response</span></span>
<span data-ttu-id="87a7c-150">В случае успешного выполнения данный метод возвращает код отклика `201 Created` и объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="87a7c-150">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87a7c-151">Пример</span><span class="sxs-lookup"><span data-stu-id="87a7c-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="87a7c-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="87a7c-152">Request</span></span>
<span data-ttu-id="87a7c-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87a7c-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="87a7c-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="87a7c-154">Response</span></span>
<span data-ttu-id="87a7c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="87a7c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



