---
title: Создать importedWindowsAutopilotDeviceIdentity
description: Создать новый объект importedWindowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 125a36a7dd400ffcb57928b5744cf14f44d21d01
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35986780"
---
# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="e06b8-103">Создать importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="e06b8-103">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="e06b8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e06b8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e06b8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e06b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e06b8-106">Создать новый объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="e06b8-106">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e06b8-107">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="e06b8-107">Prerequisites</span></span>
<span data-ttu-id="e06b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e06b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e06b8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e06b8-110">Permission type</span></span>|<span data-ttu-id="e06b8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e06b8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e06b8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e06b8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e06b8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e06b8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e06b8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e06b8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e06b8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e06b8-115">Not supported.</span></span>|
|<span data-ttu-id="e06b8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e06b8-116">Application</span></span>|<span data-ttu-id="e06b8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e06b8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e06b8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e06b8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="e06b8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e06b8-119">Request headers</span></span>
|<span data-ttu-id="e06b8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e06b8-120">Header</span></span>|<span data-ttu-id="e06b8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e06b8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e06b8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e06b8-122">Authorization</span></span>|<span data-ttu-id="e06b8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e06b8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e06b8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e06b8-124">Accept</span></span>|<span data-ttu-id="e06b8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e06b8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e06b8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e06b8-126">Request body</span></span>
<span data-ttu-id="e06b8-127">В тексте запроса добавьте представление объекта importedWindowsAutopilotDeviceIdentity в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e06b8-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="e06b8-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта importedWindowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="e06b8-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="e06b8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e06b8-129">Property</span></span>|<span data-ttu-id="e06b8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e06b8-130">Type</span></span>|<span data-ttu-id="e06b8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e06b8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e06b8-132">id</span><span class="sxs-lookup"><span data-stu-id="e06b8-132">id</span></span>|<span data-ttu-id="e06b8-133">String</span><span class="sxs-lookup"><span data-stu-id="e06b8-133">String</span></span>|<span data-ttu-id="e06b8-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="e06b8-134">The GUID for the object</span></span>|
|<span data-ttu-id="e06b8-135">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="e06b8-135">orderIdentifier</span></span>|<span data-ttu-id="e06b8-136">String</span><span class="sxs-lookup"><span data-stu-id="e06b8-136">String</span></span>|<span data-ttu-id="e06b8-137">Номер заказа устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="e06b8-137">Order Id of the Windows autopilot device.</span></span> <span data-ttu-id="e06b8-138">— Устаревшее</span><span class="sxs-lookup"><span data-stu-id="e06b8-138">- Deprecate</span></span>|
|<span data-ttu-id="e06b8-139">Грауптаг</span><span class="sxs-lookup"><span data-stu-id="e06b8-139">groupTag</span></span>|<span data-ttu-id="e06b8-140">String</span><span class="sxs-lookup"><span data-stu-id="e06b8-140">String</span></span>|<span data-ttu-id="e06b8-141">Тег Group для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="e06b8-141">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e06b8-142">serialNumber</span><span class="sxs-lookup"><span data-stu-id="e06b8-142">serialNumber</span></span>|<span data-ttu-id="e06b8-143">String</span><span class="sxs-lookup"><span data-stu-id="e06b8-143">String</span></span>|<span data-ttu-id="e06b8-144">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="e06b8-144">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e06b8-145">productKey</span><span class="sxs-lookup"><span data-stu-id="e06b8-145">productKey</span></span>|<span data-ttu-id="e06b8-146">Строка</span><span class="sxs-lookup"><span data-stu-id="e06b8-146">String</span></span>|<span data-ttu-id="e06b8-147">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="e06b8-147">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e06b8-148">Импортид</span><span class="sxs-lookup"><span data-stu-id="e06b8-148">importId</span></span>|<span data-ttu-id="e06b8-149">String</span><span class="sxs-lookup"><span data-stu-id="e06b8-149">String</span></span>|<span data-ttu-id="e06b8-150">Идентификатор импорта для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="e06b8-150">The Import Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e06b8-151">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="e06b8-151">hardwareIdentifier</span></span>|<span data-ttu-id="e06b8-152">Двоичный</span><span class="sxs-lookup"><span data-stu-id="e06b8-152">Binary</span></span>|<span data-ttu-id="e06b8-153">Аппаратный большой двоичный объект (BLOB) устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="e06b8-153">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="e06b8-154">state</span><span class="sxs-lookup"><span data-stu-id="e06b8-154">state</span></span>|[<span data-ttu-id="e06b8-155">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="e06b8-155">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="e06b8-156">Текущее состояние импортированного устройства.</span><span class="sxs-lookup"><span data-stu-id="e06b8-156">Current state of the imported device.</span></span>|
|<span data-ttu-id="e06b8-157">АссигнедусерпринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="e06b8-157">assignedUserPrincipalName</span></span>|<span data-ttu-id="e06b8-158">String</span><span class="sxs-lookup"><span data-stu-id="e06b8-158">String</span></span>|<span data-ttu-id="e06b8-159">Имя участника-пользователя для пользователя, которому будет назначено устройство</span><span class="sxs-lookup"><span data-stu-id="e06b8-159">UPN of the user the device will be assigned</span></span>|



## <a name="response"></a><span data-ttu-id="e06b8-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="e06b8-160">Response</span></span>
<span data-ttu-id="e06b8-161">В случае успешного выполнения данный метод возвращает код отклика `201 Created` и объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="e06b8-161">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e06b8-162">Пример</span><span class="sxs-lookup"><span data-stu-id="e06b8-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="e06b8-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="e06b8-163">Request</span></span>
<span data-ttu-id="e06b8-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e06b8-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e06b8-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="e06b8-165">Response</span></span>
<span data-ttu-id="e06b8-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e06b8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





