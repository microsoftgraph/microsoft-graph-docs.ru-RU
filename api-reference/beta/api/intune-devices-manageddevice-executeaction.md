---
title: Действие executeAction
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10012020f0bebcfdd02891224bcc3d9cb803dbcb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814269"
---
# <a name="executeaction-action"></a><span data-ttu-id="d6429-103">Действие executeAction</span><span class="sxs-lookup"><span data-stu-id="d6429-103">executeAction action</span></span>

> <span data-ttu-id="d6429-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6429-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6429-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6429-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6429-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d6429-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6429-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d6429-107">Prerequisites</span></span>
<span data-ttu-id="d6429-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6429-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6429-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6429-110">Permission type</span></span>|<span data-ttu-id="d6429-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6429-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6429-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6429-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6429-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="d6429-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="d6429-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6429-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6429-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6429-115">Not supported.</span></span>|
|<span data-ttu-id="d6429-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d6429-116">Application</span></span>|<span data-ttu-id="d6429-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="d6429-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6429-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6429-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="d6429-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d6429-119">Request headers</span></span>
|<span data-ttu-id="d6429-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6429-120">Header</span></span>|<span data-ttu-id="d6429-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d6429-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6429-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6429-122">Authorization</span></span>|<span data-ttu-id="d6429-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6429-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6429-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d6429-124">Accept</span></span>|<span data-ttu-id="d6429-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d6429-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6429-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6429-126">Request body</span></span>
<span data-ttu-id="d6429-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6429-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d6429-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d6429-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d6429-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6429-129">Property</span></span>|<span data-ttu-id="d6429-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d6429-130">Type</span></span>|<span data-ttu-id="d6429-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d6429-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6429-132">actionName</span><span class="sxs-lookup"><span data-stu-id="d6429-132">actionName</span></span>|[<span data-ttu-id="d6429-133">манажеддевицеремотеактион</span><span class="sxs-lookup"><span data-stu-id="d6429-133">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="d6429-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d6429-134">Not yet documented</span></span>|
|<span data-ttu-id="d6429-135">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="d6429-135">keepEnrollmentData</span></span>|<span data-ttu-id="d6429-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6429-136">Boolean</span></span>|<span data-ttu-id="d6429-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d6429-137">Not yet documented</span></span>|
|<span data-ttu-id="d6429-138">keepUserData</span><span class="sxs-lookup"><span data-stu-id="d6429-138">keepUserData</span></span>|<span data-ttu-id="d6429-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6429-139">Boolean</span></span>|<span data-ttu-id="d6429-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d6429-140">Not yet documented</span></span>|
|<span data-ttu-id="d6429-141">девицеидс</span><span class="sxs-lookup"><span data-stu-id="d6429-141">deviceIds</span></span>|<span data-ttu-id="d6429-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d6429-142">String collection</span></span>|<span data-ttu-id="d6429-143">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d6429-143">Not yet documented</span></span>|
|<span data-ttu-id="d6429-144">нотификатионтитле</span><span class="sxs-lookup"><span data-stu-id="d6429-144">notificationTitle</span></span>|<span data-ttu-id="d6429-145">String</span><span class="sxs-lookup"><span data-stu-id="d6429-145">String</span></span>|<span data-ttu-id="d6429-146">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d6429-146">Not yet documented</span></span>|
|<span data-ttu-id="d6429-147">нотификатионбоди</span><span class="sxs-lookup"><span data-stu-id="d6429-147">notificationBody</span></span>|<span data-ttu-id="d6429-148">String</span><span class="sxs-lookup"><span data-stu-id="d6429-148">String</span></span>|<span data-ttu-id="d6429-149">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d6429-149">Not yet documented</span></span>|
|<span data-ttu-id="d6429-150">deviceName</span><span class="sxs-lookup"><span data-stu-id="d6429-150">deviceName</span></span>|<span data-ttu-id="d6429-151">String</span><span class="sxs-lookup"><span data-stu-id="d6429-151">String</span></span>|<span data-ttu-id="d6429-152">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d6429-152">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d6429-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6429-153">Response</span></span>
<span data-ttu-id="d6429-154">При успешном выполнении это действие возвращает `200 OK` код отклика и объект [булкманажеддевицеактионресулт](../resources/intune-devices-bulkmanageddeviceactionresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6429-154">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6429-155">Пример</span><span class="sxs-lookup"><span data-stu-id="d6429-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6429-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6429-156">Request</span></span>
<span data-ttu-id="d6429-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6429-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/executeAction

Content-type: application/json
Content-length: 274

{
  "actionName": "delete",
  "keepEnrollmentData": true,
  "keepUserData": true,
  "deviceIds": [
    "Device Ids value"
  ],
  "notificationTitle": "Notification Title value",
  "notificationBody": "Notification Body value",
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="d6429-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6429-158">Response</span></span>
<span data-ttu-id="d6429-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6429-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": {
    "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult",
    "successfulDeviceIds": [
      "Successful Device Ids value"
    ],
    "failedDeviceIds": [
      "Failed Device Ids value"
    ],
    "notFoundDeviceIds": [
      "Not Found Device Ids value"
    ],
    "notSupportedDeviceIds": [
      "Not Supported Device Ids value"
    ]
  }
}
```




