---
title: Создать importedWindowsAutopilotDeviceIdentity
description: Создание нового объекта importedWindowsAutopilotDeviceIdentity.
ms.openlocfilehash: 3fe1661aa4281753aa79584bfa08c28024d01297
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079172"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="fcc13-103">Создать importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="fcc13-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="fcc13-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fcc13-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fcc13-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcc13-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fcc13-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fcc13-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fcc13-107">Создать новый объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="fcc13-107">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fcc13-108">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="fcc13-108">Prerequisites</span></span>
<span data-ttu-id="fcc13-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcc13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcc13-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcc13-111">Permission type</span></span>|<span data-ttu-id="fcc13-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcc13-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcc13-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcc13-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fcc13-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcc13-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fcc13-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcc13-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcc13-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcc13-116">Not supported.</span></span>|
|<span data-ttu-id="fcc13-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcc13-117">Application</span></span>|<span data-ttu-id="fcc13-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcc13-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcc13-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcc13-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="fcc13-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcc13-120">Request headers</span></span>
|<span data-ttu-id="fcc13-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fcc13-121">Header</span></span>|<span data-ttu-id="fcc13-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fcc13-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcc13-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcc13-123">Authorization</span></span>|<span data-ttu-id="fcc13-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fcc13-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcc13-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fcc13-125">Accept</span></span>|<span data-ttu-id="fcc13-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fcc13-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcc13-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcc13-127">Request body</span></span>
<span data-ttu-id="fcc13-128">В тексте запроса добавьте представление объекта importedWindowsAutopilotDeviceIdentity в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcc13-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="fcc13-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="fcc13-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="fcc13-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcc13-130">Property</span></span>|<span data-ttu-id="fcc13-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fcc13-131">Type</span></span>|<span data-ttu-id="fcc13-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fcc13-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcc13-133">id</span><span class="sxs-lookup"><span data-stu-id="fcc13-133">id</span></span>|<span data-ttu-id="fcc13-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fcc13-134">String</span></span>|<span data-ttu-id="fcc13-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="fcc13-135">The GUID for the object</span></span>|
|<span data-ttu-id="fcc13-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="fcc13-136">orderIdentifier</span></span>|<span data-ttu-id="fcc13-137">Строка</span><span class="sxs-lookup"><span data-stu-id="fcc13-137">String</span></span>|<span data-ttu-id="fcc13-138">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="fcc13-138">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="fcc13-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="fcc13-139">serialNumber</span></span>|<span data-ttu-id="fcc13-140">Строка</span><span class="sxs-lookup"><span data-stu-id="fcc13-140">String</span></span>|<span data-ttu-id="fcc13-141">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="fcc13-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="fcc13-142">productKey</span><span class="sxs-lookup"><span data-stu-id="fcc13-142">productKey</span></span>|<span data-ttu-id="fcc13-143">Строка</span><span class="sxs-lookup"><span data-stu-id="fcc13-143">String</span></span>|<span data-ttu-id="fcc13-144">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="fcc13-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="fcc13-145">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="fcc13-145">hardwareIdentifier</span></span>|<span data-ttu-id="fcc13-146">Двоичный</span><span class="sxs-lookup"><span data-stu-id="fcc13-146">Binary</span></span>|<span data-ttu-id="fcc13-147">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="fcc13-147">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="fcc13-148">state</span><span class="sxs-lookup"><span data-stu-id="fcc13-148">state</span></span>|[<span data-ttu-id="fcc13-149">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="fcc13-149">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="fcc13-150">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="fcc13-150">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="fcc13-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="fcc13-151">Response</span></span>
<span data-ttu-id="fcc13-152">В случае успешного выполнения данный метод возвращает код отклика `201 Created` и объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="fcc13-152">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcc13-153">Пример</span><span class="sxs-lookup"><span data-stu-id="fcc13-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="fcc13-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcc13-154">Request</span></span>
<span data-ttu-id="fcc13-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcc13-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fcc13-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="fcc13-156">Response</span></span>
<span data-ttu-id="fcc13-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="fcc13-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





