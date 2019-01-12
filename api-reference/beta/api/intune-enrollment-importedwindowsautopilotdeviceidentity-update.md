---
title: Обновление importedWindowsAutopilotDeviceIdentity
description: Обновляет свойства объекта importedWindowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8e2f5385729233d975b35fb7bd78e51931bdab34
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959470"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="e0313-103">Обновление importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="e0313-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="e0313-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e0313-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0313-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0313-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0313-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e0313-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0313-107">Обновляет свойства объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="e0313-107">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0313-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e0313-108">Prerequisites</span></span>
<span data-ttu-id="e0313-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0313-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0313-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0313-111">Permission type</span></span>|<span data-ttu-id="e0313-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0313-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0313-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0313-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0313-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0313-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e0313-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0313-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0313-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0313-116">Not supported.</span></span>|
|<span data-ttu-id="e0313-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0313-117">Application</span></span>|<span data-ttu-id="e0313-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0313-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0313-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0313-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="e0313-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0313-120">Request headers</span></span>
|<span data-ttu-id="e0313-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0313-121">Header</span></span>|<span data-ttu-id="e0313-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e0313-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0313-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0313-123">Authorization</span></span>|<span data-ttu-id="e0313-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e0313-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0313-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e0313-125">Accept</span></span>|<span data-ttu-id="e0313-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0313-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0313-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e0313-127">Request body</span></span>
<span data-ttu-id="e0313-128">В теле запроса добавьте представление объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0313-128">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="e0313-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="e0313-129">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="e0313-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0313-130">Property</span></span>|<span data-ttu-id="e0313-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e0313-131">Type</span></span>|<span data-ttu-id="e0313-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e0313-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0313-133">id</span><span class="sxs-lookup"><span data-stu-id="e0313-133">id</span></span>|<span data-ttu-id="e0313-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e0313-134">String</span></span>|<span data-ttu-id="e0313-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="e0313-135">The GUID for the object</span></span>|
|<span data-ttu-id="e0313-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="e0313-136">orderIdentifier</span></span>|<span data-ttu-id="e0313-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e0313-137">String</span></span>|<span data-ttu-id="e0313-138">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="e0313-138">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e0313-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="e0313-139">serialNumber</span></span>|<span data-ttu-id="e0313-140">Строка</span><span class="sxs-lookup"><span data-stu-id="e0313-140">String</span></span>|<span data-ttu-id="e0313-141">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="e0313-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e0313-142">productKey</span><span class="sxs-lookup"><span data-stu-id="e0313-142">productKey</span></span>|<span data-ttu-id="e0313-143">Строка</span><span class="sxs-lookup"><span data-stu-id="e0313-143">String</span></span>|<span data-ttu-id="e0313-144">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="e0313-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e0313-145">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="e0313-145">hardwareIdentifier</span></span>|<span data-ttu-id="e0313-146">Двоичный</span><span class="sxs-lookup"><span data-stu-id="e0313-146">Binary</span></span>|<span data-ttu-id="e0313-147">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="e0313-147">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e0313-148">state</span><span class="sxs-lookup"><span data-stu-id="e0313-148">state</span></span>|[<span data-ttu-id="e0313-149">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="e0313-149">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="e0313-150">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="e0313-150">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="e0313-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0313-151">Response</span></span>
<span data-ttu-id="e0313-152">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e0313-152">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0313-153">Пример</span><span class="sxs-lookup"><span data-stu-id="e0313-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0313-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0313-154">Request</span></span>
<span data-ttu-id="e0313-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0313-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 464

{
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

### <a name="response"></a><span data-ttu-id="e0313-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0313-156">Response</span></span>
<span data-ttu-id="e0313-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e0313-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





