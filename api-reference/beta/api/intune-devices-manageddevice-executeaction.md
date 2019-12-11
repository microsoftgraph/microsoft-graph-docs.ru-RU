---
title: Действие executeAction
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 88fe2a69b14b136e248580c1e36af8d8b928b089
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944801"
---
# <a name="executeaction-action"></a><span data-ttu-id="7e177-103">Действие executeAction</span><span class="sxs-lookup"><span data-stu-id="7e177-103">executeAction action</span></span>

> <span data-ttu-id="7e177-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e177-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e177-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e177-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e177-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7e177-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e177-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7e177-107">Prerequisites</span></span>
<span data-ttu-id="7e177-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e177-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e177-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e177-110">Permission type</span></span>|<span data-ttu-id="7e177-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e177-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e177-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e177-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e177-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="7e177-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="7e177-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e177-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e177-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e177-115">Not supported.</span></span>|
|<span data-ttu-id="7e177-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e177-116">Application</span></span>|<span data-ttu-id="7e177-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="7e177-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e177-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e177-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="7e177-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7e177-119">Request headers</span></span>
|<span data-ttu-id="7e177-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e177-120">Header</span></span>|<span data-ttu-id="7e177-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7e177-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e177-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e177-122">Authorization</span></span>|<span data-ttu-id="7e177-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e177-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e177-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7e177-124">Accept</span></span>|<span data-ttu-id="7e177-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7e177-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e177-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7e177-126">Request body</span></span>
<span data-ttu-id="7e177-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e177-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7e177-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="7e177-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7e177-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e177-129">Property</span></span>|<span data-ttu-id="7e177-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7e177-130">Type</span></span>|<span data-ttu-id="7e177-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7e177-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e177-132">actionName</span><span class="sxs-lookup"><span data-stu-id="7e177-132">actionName</span></span>|[<span data-ttu-id="7e177-133">манажеддевицеремотеактион</span><span class="sxs-lookup"><span data-stu-id="7e177-133">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="7e177-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7e177-134">Not yet documented</span></span>|
|<span data-ttu-id="7e177-135">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="7e177-135">keepEnrollmentData</span></span>|<span data-ttu-id="7e177-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e177-136">Boolean</span></span>|<span data-ttu-id="7e177-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7e177-137">Not yet documented</span></span>|
|<span data-ttu-id="7e177-138">keepUserData</span><span class="sxs-lookup"><span data-stu-id="7e177-138">keepUserData</span></span>|<span data-ttu-id="7e177-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e177-139">Boolean</span></span>|<span data-ttu-id="7e177-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7e177-140">Not yet documented</span></span>|
|<span data-ttu-id="7e177-141">девицеидс</span><span class="sxs-lookup"><span data-stu-id="7e177-141">deviceIds</span></span>|<span data-ttu-id="7e177-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7e177-142">String collection</span></span>|<span data-ttu-id="7e177-143">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7e177-143">Not yet documented</span></span>|
|<span data-ttu-id="7e177-144">нотификатионтитле</span><span class="sxs-lookup"><span data-stu-id="7e177-144">notificationTitle</span></span>|<span data-ttu-id="7e177-145">String</span><span class="sxs-lookup"><span data-stu-id="7e177-145">String</span></span>|<span data-ttu-id="7e177-146">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7e177-146">Not yet documented</span></span>|
|<span data-ttu-id="7e177-147">нотификатионбоди</span><span class="sxs-lookup"><span data-stu-id="7e177-147">notificationBody</span></span>|<span data-ttu-id="7e177-148">String</span><span class="sxs-lookup"><span data-stu-id="7e177-148">String</span></span>|<span data-ttu-id="7e177-149">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7e177-149">Not yet documented</span></span>|
|<span data-ttu-id="7e177-150">deviceName</span><span class="sxs-lookup"><span data-stu-id="7e177-150">deviceName</span></span>|<span data-ttu-id="7e177-151">String</span><span class="sxs-lookup"><span data-stu-id="7e177-151">String</span></span>|<span data-ttu-id="7e177-152">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7e177-152">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7e177-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e177-153">Response</span></span>
<span data-ttu-id="7e177-154">При успешном выполнении это действие возвращает `200 OK` код отклика и объект [булкманажеддевицеактионресулт](../resources/intune-devices-bulkmanageddeviceactionresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e177-154">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e177-155">Пример</span><span class="sxs-lookup"><span data-stu-id="7e177-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e177-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e177-156">Request</span></span>
<span data-ttu-id="7e177-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e177-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7e177-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e177-158">Response</span></span>
<span data-ttu-id="7e177-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e177-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





