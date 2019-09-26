---
title: Действие executeAction
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 998df1092df19ad52a8cb40225b410a23ee21cc1
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188439"
---
# <a name="executeaction-action"></a><span data-ttu-id="05892-103">Действие executeAction</span><span class="sxs-lookup"><span data-stu-id="05892-103">executeAction action</span></span>

> <span data-ttu-id="05892-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05892-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05892-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05892-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05892-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="05892-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05892-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="05892-107">Prerequisites</span></span>
<span data-ttu-id="05892-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05892-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05892-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05892-110">Permission type</span></span>|<span data-ttu-id="05892-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05892-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05892-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05892-112">Delegated (work or school account)</span></span>|<span data-ttu-id="05892-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="05892-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="05892-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05892-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05892-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05892-115">Not supported.</span></span>|
|<span data-ttu-id="05892-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05892-116">Application</span></span>|<span data-ttu-id="05892-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="05892-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05892-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05892-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="05892-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05892-119">Request headers</span></span>
|<span data-ttu-id="05892-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05892-120">Header</span></span>|<span data-ttu-id="05892-121">Значение</span><span class="sxs-lookup"><span data-stu-id="05892-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05892-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05892-122">Authorization</span></span>|<span data-ttu-id="05892-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05892-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05892-124">Accept</span><span class="sxs-lookup"><span data-stu-id="05892-124">Accept</span></span>|<span data-ttu-id="05892-125">application/json</span><span class="sxs-lookup"><span data-stu-id="05892-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05892-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05892-126">Request body</span></span>
<span data-ttu-id="05892-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05892-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="05892-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="05892-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="05892-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="05892-129">Property</span></span>|<span data-ttu-id="05892-130">Тип</span><span class="sxs-lookup"><span data-stu-id="05892-130">Type</span></span>|<span data-ttu-id="05892-131">Описание</span><span class="sxs-lookup"><span data-stu-id="05892-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05892-132">actionName</span><span class="sxs-lookup"><span data-stu-id="05892-132">actionName</span></span>|[<span data-ttu-id="05892-133">манажеддевицеремотеактион</span><span class="sxs-lookup"><span data-stu-id="05892-133">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="05892-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="05892-134">Not yet documented</span></span>|
|<span data-ttu-id="05892-135">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="05892-135">keepEnrollmentData</span></span>|<span data-ttu-id="05892-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="05892-136">Boolean</span></span>|<span data-ttu-id="05892-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="05892-137">Not yet documented</span></span>|
|<span data-ttu-id="05892-138">keepUserData</span><span class="sxs-lookup"><span data-stu-id="05892-138">keepUserData</span></span>|<span data-ttu-id="05892-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="05892-139">Boolean</span></span>|<span data-ttu-id="05892-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="05892-140">Not yet documented</span></span>|
|<span data-ttu-id="05892-141">девицеидс</span><span class="sxs-lookup"><span data-stu-id="05892-141">deviceIds</span></span>|<span data-ttu-id="05892-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="05892-142">String collection</span></span>|<span data-ttu-id="05892-143">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="05892-143">Not yet documented</span></span>|
|<span data-ttu-id="05892-144">нотификатионтитле</span><span class="sxs-lookup"><span data-stu-id="05892-144">notificationTitle</span></span>|<span data-ttu-id="05892-145">String</span><span class="sxs-lookup"><span data-stu-id="05892-145">String</span></span>|<span data-ttu-id="05892-146">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="05892-146">Not yet documented</span></span>|
|<span data-ttu-id="05892-147">нотификатионбоди</span><span class="sxs-lookup"><span data-stu-id="05892-147">notificationBody</span></span>|<span data-ttu-id="05892-148">String</span><span class="sxs-lookup"><span data-stu-id="05892-148">String</span></span>|<span data-ttu-id="05892-149">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="05892-149">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="05892-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="05892-150">Response</span></span>
<span data-ttu-id="05892-151">При успешном выполнении это действие возвращает `200 OK` код отклика и объект [булкманажеддевицеактионресулт](../resources/intune-devices-bulkmanageddeviceactionresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="05892-151">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05892-152">Пример</span><span class="sxs-lookup"><span data-stu-id="05892-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="05892-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="05892-153">Request</span></span>
<span data-ttu-id="05892-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05892-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/executeAction

Content-type: application/json
Content-length: 236

{
  "actionName": "delete",
  "keepEnrollmentData": true,
  "keepUserData": true,
  "deviceIds": [
    "Device Ids value"
  ],
  "notificationTitle": "Notification Title value",
  "notificationBody": "Notification Body value"
}
```

### <a name="response"></a><span data-ttu-id="05892-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="05892-155">Response</span></span>
<span data-ttu-id="05892-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05892-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




