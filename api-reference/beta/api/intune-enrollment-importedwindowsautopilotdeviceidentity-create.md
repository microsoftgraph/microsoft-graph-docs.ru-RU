---
title: Создать importedWindowsAutopilotDeviceIdentity
description: Создать новый объект importedWindowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6d49e760511e8764e875368cfe81a909c9e098be
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943798"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="baba0-103">Создать importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="baba0-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="baba0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="baba0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="baba0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="baba0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="baba0-106">Создать новый объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="baba0-106">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="baba0-107">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="baba0-107">Prerequisites</span></span>
<span data-ttu-id="baba0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="baba0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baba0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="baba0-110">Permission type</span></span>|<span data-ttu-id="baba0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="baba0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="baba0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="baba0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="baba0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baba0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="baba0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="baba0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="baba0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="baba0-115">Not supported.</span></span>|
|<span data-ttu-id="baba0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="baba0-116">Application</span></span>|<span data-ttu-id="baba0-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baba0-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="baba0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="baba0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="baba0-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="baba0-119">Request headers</span></span>
|<span data-ttu-id="baba0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="baba0-120">Header</span></span>|<span data-ttu-id="baba0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="baba0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="baba0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="baba0-122">Authorization</span></span>|<span data-ttu-id="baba0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="baba0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="baba0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="baba0-124">Accept</span></span>|<span data-ttu-id="baba0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="baba0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="baba0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="baba0-126">Request body</span></span>
<span data-ttu-id="baba0-127">В тексте запроса добавьте представление объекта importedWindowsAutopilotDeviceIdentity в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="baba0-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="baba0-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="baba0-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="baba0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="baba0-129">Property</span></span>|<span data-ttu-id="baba0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="baba0-130">Type</span></span>|<span data-ttu-id="baba0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="baba0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baba0-132">id</span><span class="sxs-lookup"><span data-stu-id="baba0-132">id</span></span>|<span data-ttu-id="baba0-133">Строка</span><span class="sxs-lookup"><span data-stu-id="baba0-133">String</span></span>|<span data-ttu-id="baba0-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="baba0-134">The GUID for the object</span></span>|
|<span data-ttu-id="baba0-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="baba0-135">orderIdentifier</span></span>|<span data-ttu-id="baba0-136">Строка</span><span class="sxs-lookup"><span data-stu-id="baba0-136">String</span></span>|<span data-ttu-id="baba0-137">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="baba0-137">Order Id of the Windows autopilot device.</span></span> <span data-ttu-id="baba0-138">— Устаревшее</span><span class="sxs-lookup"><span data-stu-id="baba0-138">- Deprecate</span></span>|
|<span data-ttu-id="baba0-139">грауптаг</span><span class="sxs-lookup"><span data-stu-id="baba0-139">groupTag</span></span>|<span data-ttu-id="baba0-140">Строка</span><span class="sxs-lookup"><span data-stu-id="baba0-140">String</span></span>|<span data-ttu-id="baba0-141">Тег Group для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="baba0-141">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="baba0-142">serialNumber</span><span class="sxs-lookup"><span data-stu-id="baba0-142">serialNumber</span></span>|<span data-ttu-id="baba0-143">String</span><span class="sxs-lookup"><span data-stu-id="baba0-143">String</span></span>|<span data-ttu-id="baba0-144">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="baba0-144">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="baba0-145">productKey</span><span class="sxs-lookup"><span data-stu-id="baba0-145">productKey</span></span>|<span data-ttu-id="baba0-146">Строка</span><span class="sxs-lookup"><span data-stu-id="baba0-146">String</span></span>|<span data-ttu-id="baba0-147">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="baba0-147">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="baba0-148">импортид</span><span class="sxs-lookup"><span data-stu-id="baba0-148">importId</span></span>|<span data-ttu-id="baba0-149">Строка</span><span class="sxs-lookup"><span data-stu-id="baba0-149">String</span></span>|<span data-ttu-id="baba0-150">Идентификатор импорта для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="baba0-150">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="baba0-151">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="baba0-151">hardwareIdentifier</span></span>|<span data-ttu-id="baba0-152">Двоичный</span><span class="sxs-lookup"><span data-stu-id="baba0-152">Binary</span></span>|<span data-ttu-id="baba0-153">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="baba0-153">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="baba0-154">state</span><span class="sxs-lookup"><span data-stu-id="baba0-154">state</span></span>|[<span data-ttu-id="baba0-155">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="baba0-155">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="baba0-156">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="baba0-156">Current state of the imported device.</span></span>|
|<span data-ttu-id="baba0-157">ассигнедусерпринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="baba0-157">assignedUserPrincipalName</span></span>|<span data-ttu-id="baba0-158">Строка</span><span class="sxs-lookup"><span data-stu-id="baba0-158">String</span></span>|<span data-ttu-id="baba0-159">Имя участника-пользователя для пользователя, которому будет назначено устройство</span><span class="sxs-lookup"><span data-stu-id="baba0-159">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="baba0-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="baba0-160">Response</span></span>
<span data-ttu-id="baba0-161">В случае успешного выполнения данный метод возвращает код отклика `201 Created` и объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="baba0-161">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baba0-162">Пример</span><span class="sxs-lookup"><span data-stu-id="baba0-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="baba0-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="baba0-163">Request</span></span>
<span data-ttu-id="baba0-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="baba0-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="baba0-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="baba0-165">Response</span></span>
<span data-ttu-id="baba0-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="baba0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





