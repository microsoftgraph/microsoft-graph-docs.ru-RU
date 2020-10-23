---
title: Обновление importedWindowsAutopilotDeviceIdentity
description: Обновляет свойства объекта importedWindowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8cf2210df9398a283ade5c0f3a3656c6a352178d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736431"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="0312f-103">Обновление importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="0312f-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="0312f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0312f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0312f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0312f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0312f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0312f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0312f-107">Обновляет свойства объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="0312f-107">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0312f-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0312f-108">Prerequisites</span></span>
<span data-ttu-id="0312f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0312f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0312f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0312f-111">Permission type</span></span>|<span data-ttu-id="0312f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0312f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0312f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0312f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0312f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0312f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0312f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0312f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0312f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0312f-116">Not supported.</span></span>|
|<span data-ttu-id="0312f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0312f-117">Application</span></span>|<span data-ttu-id="0312f-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0312f-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0312f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0312f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="0312f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0312f-120">Request headers</span></span>
|<span data-ttu-id="0312f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0312f-121">Header</span></span>|<span data-ttu-id="0312f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0312f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0312f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0312f-123">Authorization</span></span>|<span data-ttu-id="0312f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0312f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0312f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0312f-125">Accept</span></span>|<span data-ttu-id="0312f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0312f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0312f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0312f-127">Request body</span></span>
<span data-ttu-id="0312f-128">В теле запроса добавьте представление объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0312f-128">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="0312f-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="0312f-129">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="0312f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0312f-130">Property</span></span>|<span data-ttu-id="0312f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0312f-131">Type</span></span>|<span data-ttu-id="0312f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0312f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0312f-133">id</span><span class="sxs-lookup"><span data-stu-id="0312f-133">id</span></span>|<span data-ttu-id="0312f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0312f-134">String</span></span>|<span data-ttu-id="0312f-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="0312f-135">The GUID for the object</span></span>|
|<span data-ttu-id="0312f-136">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="0312f-136">orderIdentifier</span></span>|<span data-ttu-id="0312f-137">Строка</span><span class="sxs-lookup"><span data-stu-id="0312f-137">String</span></span>|<span data-ttu-id="0312f-138">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="0312f-138">Order Id of the Windows autopilot device.</span></span> <span data-ttu-id="0312f-139">— Устаревшее</span><span class="sxs-lookup"><span data-stu-id="0312f-139">- Deprecate</span></span>|
|<span data-ttu-id="0312f-140">грауптаг</span><span class="sxs-lookup"><span data-stu-id="0312f-140">groupTag</span></span>|<span data-ttu-id="0312f-141">Строка</span><span class="sxs-lookup"><span data-stu-id="0312f-141">String</span></span>|<span data-ttu-id="0312f-142">Тег Group для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="0312f-142">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0312f-143">serialNumber</span><span class="sxs-lookup"><span data-stu-id="0312f-143">serialNumber</span></span>|<span data-ttu-id="0312f-144">Строка</span><span class="sxs-lookup"><span data-stu-id="0312f-144">String</span></span>|<span data-ttu-id="0312f-145">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="0312f-145">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0312f-146">productKey</span><span class="sxs-lookup"><span data-stu-id="0312f-146">productKey</span></span>|<span data-ttu-id="0312f-147">Строка</span><span class="sxs-lookup"><span data-stu-id="0312f-147">String</span></span>|<span data-ttu-id="0312f-148">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="0312f-148">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0312f-149">импортид</span><span class="sxs-lookup"><span data-stu-id="0312f-149">importId</span></span>|<span data-ttu-id="0312f-150">Строка</span><span class="sxs-lookup"><span data-stu-id="0312f-150">String</span></span>|<span data-ttu-id="0312f-151">Идентификатор импорта для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="0312f-151">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0312f-152">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="0312f-152">hardwareIdentifier</span></span>|<span data-ttu-id="0312f-153">Двоичный</span><span class="sxs-lookup"><span data-stu-id="0312f-153">Binary</span></span>|<span data-ttu-id="0312f-154">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="0312f-154">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="0312f-155">state</span><span class="sxs-lookup"><span data-stu-id="0312f-155">state</span></span>|[<span data-ttu-id="0312f-156">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="0312f-156">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="0312f-157">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="0312f-157">Current state of the imported device.</span></span>|
|<span data-ttu-id="0312f-158">ассигнедусерпринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="0312f-158">assignedUserPrincipalName</span></span>|<span data-ttu-id="0312f-159">Строка</span><span class="sxs-lookup"><span data-stu-id="0312f-159">String</span></span>|<span data-ttu-id="0312f-160">Имя участника-пользователя для пользователя, которому будет назначено устройство</span><span class="sxs-lookup"><span data-stu-id="0312f-160">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="0312f-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="0312f-161">Response</span></span>
<span data-ttu-id="0312f-162">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0312f-162">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0312f-163">Пример</span><span class="sxs-lookup"><span data-stu-id="0312f-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="0312f-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="0312f-164">Request</span></span>
<span data-ttu-id="0312f-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0312f-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 679

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "orderIdentifier": "Order Identifier value",
  "groupTag": "Group Tag value",
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

### <a name="response"></a><span data-ttu-id="0312f-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="0312f-166">Response</span></span>
<span data-ttu-id="0312f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0312f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 728

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
  "orderIdentifier": "Order Identifier value",
  "groupTag": "Group Tag value",
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





