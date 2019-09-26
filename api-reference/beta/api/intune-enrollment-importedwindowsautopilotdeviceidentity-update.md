---
title: Обновление importedWindowsAutopilotDeviceIdentity
description: Обновляет свойства объекта importedWindowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 437ba567bbb0d3e4338f05ccbd90a76bb5588cf2
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37184855"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="14f43-103">Обновление importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="14f43-103">Update importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="14f43-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14f43-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14f43-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14f43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14f43-106">Обновляет свойства объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="14f43-106">Update the properties of a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14f43-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="14f43-107">Prerequisites</span></span>
<span data-ttu-id="14f43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14f43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14f43-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14f43-110">Permission type</span></span>|<span data-ttu-id="14f43-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="14f43-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14f43-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14f43-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14f43-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14f43-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="14f43-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14f43-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14f43-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14f43-115">Not supported.</span></span>|
|<span data-ttu-id="14f43-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14f43-116">Application</span></span>|<span data-ttu-id="14f43-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14f43-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14f43-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14f43-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="14f43-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14f43-119">Request headers</span></span>
|<span data-ttu-id="14f43-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14f43-120">Header</span></span>|<span data-ttu-id="14f43-121">Значение</span><span class="sxs-lookup"><span data-stu-id="14f43-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14f43-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14f43-122">Authorization</span></span>|<span data-ttu-id="14f43-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14f43-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14f43-124">Accept</span><span class="sxs-lookup"><span data-stu-id="14f43-124">Accept</span></span>|<span data-ttu-id="14f43-125">application/json</span><span class="sxs-lookup"><span data-stu-id="14f43-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14f43-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="14f43-126">Request body</span></span>
<span data-ttu-id="14f43-127">В теле запроса добавьте представление объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14f43-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="14f43-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="14f43-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="14f43-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="14f43-129">Property</span></span>|<span data-ttu-id="14f43-130">Тип</span><span class="sxs-lookup"><span data-stu-id="14f43-130">Type</span></span>|<span data-ttu-id="14f43-131">Описание</span><span class="sxs-lookup"><span data-stu-id="14f43-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14f43-132">id</span><span class="sxs-lookup"><span data-stu-id="14f43-132">id</span></span>|<span data-ttu-id="14f43-133">String</span><span class="sxs-lookup"><span data-stu-id="14f43-133">String</span></span>|<span data-ttu-id="14f43-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="14f43-134">The GUID for the object</span></span>|
|<span data-ttu-id="14f43-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="14f43-135">orderIdentifier</span></span>|<span data-ttu-id="14f43-136">String.</span><span class="sxs-lookup"><span data-stu-id="14f43-136">String</span></span>|<span data-ttu-id="14f43-137">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="14f43-137">Order Id of the Windows autopilot device.</span></span> <span data-ttu-id="14f43-138">— Устаревшее</span><span class="sxs-lookup"><span data-stu-id="14f43-138">- Deprecate</span></span>|
|<span data-ttu-id="14f43-139">грауптаг</span><span class="sxs-lookup"><span data-stu-id="14f43-139">groupTag</span></span>|<span data-ttu-id="14f43-140">String.</span><span class="sxs-lookup"><span data-stu-id="14f43-140">String</span></span>|<span data-ttu-id="14f43-141">Тег Group для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="14f43-141">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="14f43-142">serialNumber</span><span class="sxs-lookup"><span data-stu-id="14f43-142">serialNumber</span></span>|<span data-ttu-id="14f43-143">String</span><span class="sxs-lookup"><span data-stu-id="14f43-143">String</span></span>|<span data-ttu-id="14f43-144">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="14f43-144">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="14f43-145">productKey</span><span class="sxs-lookup"><span data-stu-id="14f43-145">productKey</span></span>|<span data-ttu-id="14f43-146">Строка</span><span class="sxs-lookup"><span data-stu-id="14f43-146">String</span></span>|<span data-ttu-id="14f43-147">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="14f43-147">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="14f43-148">импортид</span><span class="sxs-lookup"><span data-stu-id="14f43-148">importId</span></span>|<span data-ttu-id="14f43-149">String.</span><span class="sxs-lookup"><span data-stu-id="14f43-149">String</span></span>|<span data-ttu-id="14f43-150">Идентификатор импорта для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="14f43-150">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="14f43-151">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="14f43-151">hardwareIdentifier</span></span>|<span data-ttu-id="14f43-152">Двоичный</span><span class="sxs-lookup"><span data-stu-id="14f43-152">Binary</span></span>|<span data-ttu-id="14f43-153">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="14f43-153">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="14f43-154">state</span><span class="sxs-lookup"><span data-stu-id="14f43-154">state</span></span>|[<span data-ttu-id="14f43-155">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="14f43-155">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="14f43-156">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="14f43-156">Current state of the imported device.</span></span>|
|<span data-ttu-id="14f43-157">ассигнедусерпринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="14f43-157">assignedUserPrincipalName</span></span>|<span data-ttu-id="14f43-158">String.</span><span class="sxs-lookup"><span data-stu-id="14f43-158">String</span></span>|<span data-ttu-id="14f43-159">Имя участника-пользователя для пользователя, которому будет назначено устройство</span><span class="sxs-lookup"><span data-stu-id="14f43-159">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="14f43-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="14f43-160">Response</span></span>
<span data-ttu-id="14f43-161">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="14f43-161">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14f43-162">Пример</span><span class="sxs-lookup"><span data-stu-id="14f43-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="14f43-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="14f43-163">Request</span></span>
<span data-ttu-id="14f43-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14f43-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="14f43-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="14f43-165">Response</span></span>
<span data-ttu-id="14f43-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14f43-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




