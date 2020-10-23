---
title: Действие executeAction
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3e64ed7ab003ae340cbcab24bc093843b01e23c0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708237"
---
# <a name="executeaction-action"></a><span data-ttu-id="cee41-103">Действие executeAction</span><span class="sxs-lookup"><span data-stu-id="cee41-103">executeAction action</span></span>

<span data-ttu-id="cee41-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cee41-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cee41-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cee41-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cee41-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cee41-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cee41-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cee41-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cee41-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cee41-108">Prerequisites</span></span>
<span data-ttu-id="cee41-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cee41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cee41-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cee41-111">Permission type</span></span>|<span data-ttu-id="cee41-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cee41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cee41-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cee41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cee41-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="cee41-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="cee41-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cee41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cee41-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cee41-116">Not supported.</span></span>|
|<span data-ttu-id="cee41-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cee41-117">Application</span></span>|<span data-ttu-id="cee41-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="cee41-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cee41-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cee41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/comanagedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="cee41-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cee41-120">Request headers</span></span>
|<span data-ttu-id="cee41-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cee41-121">Header</span></span>|<span data-ttu-id="cee41-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cee41-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cee41-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cee41-123">Authorization</span></span>|<span data-ttu-id="cee41-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cee41-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cee41-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cee41-125">Accept</span></span>|<span data-ttu-id="cee41-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cee41-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cee41-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cee41-127">Request body</span></span>
<span data-ttu-id="cee41-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cee41-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="cee41-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="cee41-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cee41-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cee41-130">Property</span></span>|<span data-ttu-id="cee41-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cee41-131">Type</span></span>|<span data-ttu-id="cee41-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cee41-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cee41-133">actionName</span><span class="sxs-lookup"><span data-stu-id="cee41-133">actionName</span></span>|[<span data-ttu-id="cee41-134">манажеддевицеремотеактион</span><span class="sxs-lookup"><span data-stu-id="cee41-134">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="cee41-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cee41-135">Not yet documented</span></span>|
|<span data-ttu-id="cee41-136">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="cee41-136">keepEnrollmentData</span></span>|<span data-ttu-id="cee41-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="cee41-137">Boolean</span></span>|<span data-ttu-id="cee41-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cee41-138">Not yet documented</span></span>|
|<span data-ttu-id="cee41-139">keepUserData</span><span class="sxs-lookup"><span data-stu-id="cee41-139">keepUserData</span></span>|<span data-ttu-id="cee41-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="cee41-140">Boolean</span></span>|<span data-ttu-id="cee41-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cee41-141">Not yet documented</span></span>|
|<span data-ttu-id="cee41-142">девицеидс</span><span class="sxs-lookup"><span data-stu-id="cee41-142">deviceIds</span></span>|<span data-ttu-id="cee41-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cee41-143">String collection</span></span>|<span data-ttu-id="cee41-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cee41-144">Not yet documented</span></span>|
|<span data-ttu-id="cee41-145">нотификатионтитле</span><span class="sxs-lookup"><span data-stu-id="cee41-145">notificationTitle</span></span>|<span data-ttu-id="cee41-146">String</span><span class="sxs-lookup"><span data-stu-id="cee41-146">String</span></span>|<span data-ttu-id="cee41-147">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cee41-147">Not yet documented</span></span>|
|<span data-ttu-id="cee41-148">нотификатионбоди</span><span class="sxs-lookup"><span data-stu-id="cee41-148">notificationBody</span></span>|<span data-ttu-id="cee41-149">String</span><span class="sxs-lookup"><span data-stu-id="cee41-149">String</span></span>|<span data-ttu-id="cee41-150">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cee41-150">Not yet documented</span></span>|
|<span data-ttu-id="cee41-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="cee41-151">deviceName</span></span>|<span data-ttu-id="cee41-152">String</span><span class="sxs-lookup"><span data-stu-id="cee41-152">String</span></span>|<span data-ttu-id="cee41-153">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cee41-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cee41-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="cee41-154">Response</span></span>
<span data-ttu-id="cee41-155">При успешном выполнении это действие возвращает `200 OK` код отклика и объект [булкманажеддевицеактионресулт](../resources/intune-devices-bulkmanageddeviceactionresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cee41-155">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cee41-156">Пример</span><span class="sxs-lookup"><span data-stu-id="cee41-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="cee41-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="cee41-157">Request</span></span>
<span data-ttu-id="cee41-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cee41-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cee41-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="cee41-159">Response</span></span>
<span data-ttu-id="cee41-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cee41-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





