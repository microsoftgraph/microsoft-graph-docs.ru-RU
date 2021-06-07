---
title: Создать importedWindowsAutopilotDeviceIdentity
description: Создать новый объект importedWindowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d0478e84f3bf0679588fbc9f962b3471dec90f1d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753418"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="af7a8-103">Создать importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="af7a8-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="af7a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af7a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af7a8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af7a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af7a8-106">Создать новый объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="af7a8-106">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af7a8-107">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="af7a8-107">Prerequisites</span></span>
<span data-ttu-id="af7a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af7a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af7a8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af7a8-110">Permission type</span></span>|<span data-ttu-id="af7a8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="af7a8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af7a8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af7a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="af7a8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af7a8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="af7a8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af7a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af7a8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af7a8-115">Not supported.</span></span>|
|<span data-ttu-id="af7a8-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="af7a8-116">Application</span></span>|<span data-ttu-id="af7a8-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af7a8-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af7a8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af7a8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="af7a8-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="af7a8-119">Request headers</span></span>
|<span data-ttu-id="af7a8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af7a8-120">Header</span></span>|<span data-ttu-id="af7a8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="af7a8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af7a8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="af7a8-122">Authorization</span></span>|<span data-ttu-id="af7a8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af7a8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af7a8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="af7a8-124">Accept</span></span>|<span data-ttu-id="af7a8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="af7a8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af7a8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af7a8-126">Request body</span></span>
<span data-ttu-id="af7a8-127">В тексте запроса добавьте представление объекта importedWindowsAutopilotDeviceIdentity в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af7a8-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="af7a8-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="af7a8-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="af7a8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="af7a8-129">Property</span></span>|<span data-ttu-id="af7a8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="af7a8-130">Type</span></span>|<span data-ttu-id="af7a8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="af7a8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af7a8-132">id</span><span class="sxs-lookup"><span data-stu-id="af7a8-132">id</span></span>|<span data-ttu-id="af7a8-133">String</span><span class="sxs-lookup"><span data-stu-id="af7a8-133">String</span></span>|<span data-ttu-id="af7a8-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="af7a8-134">The GUID for the object</span></span>|
|<span data-ttu-id="af7a8-135">groupTag</span><span class="sxs-lookup"><span data-stu-id="af7a8-135">groupTag</span></span>|<span data-ttu-id="af7a8-136">String</span><span class="sxs-lookup"><span data-stu-id="af7a8-136">String</span></span>|<span data-ttu-id="af7a8-137">Тег группы устройства Windows автопилота.</span><span class="sxs-lookup"><span data-stu-id="af7a8-137">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="af7a8-138">serialNumber</span><span class="sxs-lookup"><span data-stu-id="af7a8-138">serialNumber</span></span>|<span data-ttu-id="af7a8-139">Строка</span><span class="sxs-lookup"><span data-stu-id="af7a8-139">String</span></span>|<span data-ttu-id="af7a8-140">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="af7a8-140">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="af7a8-141">productKey</span><span class="sxs-lookup"><span data-stu-id="af7a8-141">productKey</span></span>|<span data-ttu-id="af7a8-142">Строка</span><span class="sxs-lookup"><span data-stu-id="af7a8-142">String</span></span>|<span data-ttu-id="af7a8-143">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="af7a8-143">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="af7a8-144">importId</span><span class="sxs-lookup"><span data-stu-id="af7a8-144">importId</span></span>|<span data-ttu-id="af7a8-145">String</span><span class="sxs-lookup"><span data-stu-id="af7a8-145">String</span></span>|<span data-ttu-id="af7a8-146">Импорт Id устройства Windows автопилота.</span><span class="sxs-lookup"><span data-stu-id="af7a8-146">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="af7a8-147">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="af7a8-147">hardwareIdentifier</span></span>|<span data-ttu-id="af7a8-148">Двоичный</span><span class="sxs-lookup"><span data-stu-id="af7a8-148">Binary</span></span>|<span data-ttu-id="af7a8-149">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="af7a8-149">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="af7a8-150">state</span><span class="sxs-lookup"><span data-stu-id="af7a8-150">state</span></span>|[<span data-ttu-id="af7a8-151">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="af7a8-151">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="af7a8-152">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="af7a8-152">Current state of the imported device.</span></span>|
|<span data-ttu-id="af7a8-153">assignedUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="af7a8-153">assignedUserPrincipalName</span></span>|<span data-ttu-id="af7a8-154">String</span><span class="sxs-lookup"><span data-stu-id="af7a8-154">String</span></span>|<span data-ttu-id="af7a8-155">UPN пользователя, на которое будет назначено устройство</span><span class="sxs-lookup"><span data-stu-id="af7a8-155">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="af7a8-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="af7a8-156">Response</span></span>
<span data-ttu-id="af7a8-157">В случае успешного выполнения данный метод возвращает код отклика `201 Created` и объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="af7a8-157">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af7a8-158">Пример</span><span class="sxs-lookup"><span data-stu-id="af7a8-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="af7a8-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="af7a8-159">Request</span></span>
<span data-ttu-id="af7a8-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af7a8-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 631

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
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

### <a name="response"></a><span data-ttu-id="af7a8-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="af7a8-161">Response</span></span>
<span data-ttu-id="af7a8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af7a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 680

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
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




