---
title: Создать importedWindowsAutopilotDeviceIdentity
description: Создать новый объект importedWindowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2c39fed44dd8d4d7f0516f2215534ed861e13ec4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149865"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="28c5a-103">Создать importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="28c5a-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="28c5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28c5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28c5a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28c5a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28c5a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28c5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28c5a-107">Создать новый объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="28c5a-107">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28c5a-108">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="28c5a-108">Prerequisites</span></span>
<span data-ttu-id="28c5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28c5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28c5a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28c5a-111">Permission type</span></span>|<span data-ttu-id="28c5a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28c5a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28c5a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28c5a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28c5a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28c5a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="28c5a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28c5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28c5a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28c5a-116">Not supported.</span></span>|
|<span data-ttu-id="28c5a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="28c5a-117">Application</span></span>|<span data-ttu-id="28c5a-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28c5a-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28c5a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28c5a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="28c5a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="28c5a-120">Request headers</span></span>
|<span data-ttu-id="28c5a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28c5a-121">Header</span></span>|<span data-ttu-id="28c5a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="28c5a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28c5a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="28c5a-123">Authorization</span></span>|<span data-ttu-id="28c5a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28c5a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28c5a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="28c5a-125">Accept</span></span>|<span data-ttu-id="28c5a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28c5a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28c5a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28c5a-127">Request body</span></span>
<span data-ttu-id="28c5a-128">В тексте запроса добавьте представление объекта importedWindowsAutopilotDeviceIdentity в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28c5a-128">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="28c5a-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="28c5a-129">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="28c5a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="28c5a-130">Property</span></span>|<span data-ttu-id="28c5a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="28c5a-131">Type</span></span>|<span data-ttu-id="28c5a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="28c5a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28c5a-133">id</span><span class="sxs-lookup"><span data-stu-id="28c5a-133">id</span></span>|<span data-ttu-id="28c5a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="28c5a-134">String</span></span>|<span data-ttu-id="28c5a-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="28c5a-135">The GUID for the object</span></span>|
|<span data-ttu-id="28c5a-136">groupTag</span><span class="sxs-lookup"><span data-stu-id="28c5a-136">groupTag</span></span>|<span data-ttu-id="28c5a-137">Строка</span><span class="sxs-lookup"><span data-stu-id="28c5a-137">String</span></span>|<span data-ttu-id="28c5a-138">Групповой тег устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="28c5a-138">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="28c5a-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="28c5a-139">serialNumber</span></span>|<span data-ttu-id="28c5a-140">Строка</span><span class="sxs-lookup"><span data-stu-id="28c5a-140">String</span></span>|<span data-ttu-id="28c5a-141">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="28c5a-141">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="28c5a-142">productKey</span><span class="sxs-lookup"><span data-stu-id="28c5a-142">productKey</span></span>|<span data-ttu-id="28c5a-143">Строка</span><span class="sxs-lookup"><span data-stu-id="28c5a-143">String</span></span>|<span data-ttu-id="28c5a-144">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="28c5a-144">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="28c5a-145">importId</span><span class="sxs-lookup"><span data-stu-id="28c5a-145">importId</span></span>|<span data-ttu-id="28c5a-146">Строка</span><span class="sxs-lookup"><span data-stu-id="28c5a-146">String</span></span>|<span data-ttu-id="28c5a-147">Импорт Id устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="28c5a-147">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="28c5a-148">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="28c5a-148">hardwareIdentifier</span></span>|<span data-ttu-id="28c5a-149">Двоичный</span><span class="sxs-lookup"><span data-stu-id="28c5a-149">Binary</span></span>|<span data-ttu-id="28c5a-150">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="28c5a-150">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="28c5a-151">state</span><span class="sxs-lookup"><span data-stu-id="28c5a-151">state</span></span>|[<span data-ttu-id="28c5a-152">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="28c5a-152">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="28c5a-153">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="28c5a-153">Current state of the imported device.</span></span>|
|<span data-ttu-id="28c5a-154">assignedUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="28c5a-154">assignedUserPrincipalName</span></span>|<span data-ttu-id="28c5a-155">Строка</span><span class="sxs-lookup"><span data-stu-id="28c5a-155">String</span></span>|<span data-ttu-id="28c5a-156">UPN пользователя, на которое будет назначено устройство</span><span class="sxs-lookup"><span data-stu-id="28c5a-156">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="28c5a-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="28c5a-157">Response</span></span>
<span data-ttu-id="28c5a-158">В случае успешного выполнения данный метод возвращает код отклика `201 Created` и объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="28c5a-158">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28c5a-159">Пример</span><span class="sxs-lookup"><span data-stu-id="28c5a-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="28c5a-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="28c5a-160">Request</span></span>
<span data-ttu-id="28c5a-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28c5a-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="28c5a-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="28c5a-162">Response</span></span>
<span data-ttu-id="28c5a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28c5a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




