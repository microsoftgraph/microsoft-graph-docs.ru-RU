---
title: Обновление importedWindowsAutopilotDeviceIdentity
description: Обновляет свойства объекта importedWindowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e073cabe69b9415aae67deaa8b3d482efd12b3cb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908352"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="7c8fc-103">Обновление importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="7c8fc-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="7c8fc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c8fc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c8fc-106">Обновляет свойства объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="7c8fc-106">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c8fc-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7c8fc-107">Prerequisites</span></span>
<span data-ttu-id="7c8fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c8fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c8fc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c8fc-110">Permission type</span></span>|<span data-ttu-id="7c8fc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c8fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c8fc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c8fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c8fc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c8fc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7c8fc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c8fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c8fc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-115">Not supported.</span></span>|
|<span data-ttu-id="7c8fc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c8fc-116">Application</span></span>|<span data-ttu-id="7c8fc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c8fc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c8fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="7c8fc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c8fc-119">Request headers</span></span>
|<span data-ttu-id="7c8fc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c8fc-120">Header</span></span>|<span data-ttu-id="7c8fc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7c8fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c8fc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c8fc-122">Authorization</span></span>|<span data-ttu-id="7c8fc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c8fc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7c8fc-124">Accept</span></span>|<span data-ttu-id="7c8fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c8fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c8fc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c8fc-126">Request body</span></span>
<span data-ttu-id="7c8fc-127">В теле запроса добавьте представление объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="7c8fc-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="7c8fc-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="7c8fc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c8fc-129">Property</span></span>|<span data-ttu-id="7c8fc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7c8fc-130">Type</span></span>|<span data-ttu-id="7c8fc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7c8fc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c8fc-132">id</span><span class="sxs-lookup"><span data-stu-id="7c8fc-132">id</span></span>|<span data-ttu-id="7c8fc-133">Строка</span><span class="sxs-lookup"><span data-stu-id="7c8fc-133">String</span></span>|<span data-ttu-id="7c8fc-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="7c8fc-134">The GUID for the object</span></span>|
|<span data-ttu-id="7c8fc-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="7c8fc-135">orderIdentifier</span></span>|<span data-ttu-id="7c8fc-136">Строка</span><span class="sxs-lookup"><span data-stu-id="7c8fc-136">String</span></span>|<span data-ttu-id="7c8fc-137">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-137">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7c8fc-138">serialNumber</span><span class="sxs-lookup"><span data-stu-id="7c8fc-138">serialNumber</span></span>|<span data-ttu-id="7c8fc-139">String</span><span class="sxs-lookup"><span data-stu-id="7c8fc-139">String</span></span>|<span data-ttu-id="7c8fc-140">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7c8fc-141">productKey</span><span class="sxs-lookup"><span data-stu-id="7c8fc-141">productKey</span></span>|<span data-ttu-id="7c8fc-142">Строка</span><span class="sxs-lookup"><span data-stu-id="7c8fc-142">String</span></span>|<span data-ttu-id="7c8fc-143">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7c8fc-144">Импортид</span><span class="sxs-lookup"><span data-stu-id="7c8fc-144">importId</span></span>|<span data-ttu-id="7c8fc-145">Строка</span><span class="sxs-lookup"><span data-stu-id="7c8fc-145">String</span></span>|<span data-ttu-id="7c8fc-146">Идентификатор импорта для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-146">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7c8fc-147">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="7c8fc-147">hardwareIdentifier</span></span>|<span data-ttu-id="7c8fc-148">Двоичный</span><span class="sxs-lookup"><span data-stu-id="7c8fc-148">Binary</span></span>|<span data-ttu-id="7c8fc-149">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-149">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7c8fc-150">state</span><span class="sxs-lookup"><span data-stu-id="7c8fc-150">state</span></span>|[<span data-ttu-id="7c8fc-151">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="7c8fc-151">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="7c8fc-152">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-152">Current state of the imported device.</span></span>|
|<span data-ttu-id="7c8fc-153">АссигнедусерпринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="7c8fc-153">assignedUserPrincipalName</span></span>|<span data-ttu-id="7c8fc-154">Строка</span><span class="sxs-lookup"><span data-stu-id="7c8fc-154">String</span></span>|<span data-ttu-id="7c8fc-155">ИМЯ участника-пользователя для пользователя, которому будет назначено устройство</span><span class="sxs-lookup"><span data-stu-id="7c8fc-155">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="7c8fc-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c8fc-156">Response</span></span>
<span data-ttu-id="7c8fc-157">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-157">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c8fc-158">Пример</span><span class="sxs-lookup"><span data-stu-id="7c8fc-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c8fc-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c8fc-159">Request</span></span>
<span data-ttu-id="7c8fc-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 645

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
  },
  "assignedUserPrincipalName": "Assigned User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="7c8fc-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c8fc-161">Response</span></span>
<span data-ttu-id="7c8fc-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c8fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 694

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
  },
  "assignedUserPrincipalName": "Assigned User Principal Name value"
}
```




