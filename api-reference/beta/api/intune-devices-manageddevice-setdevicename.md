---
title: Действие setDeviceName
description: Задание имени устройства для устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ac8b7c926066325651665e7ef6178c95372cf16f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729175"
---
# <a name="setdevicename-action"></a><span data-ttu-id="f3b1e-103">Действие setDeviceName</span><span class="sxs-lookup"><span data-stu-id="f3b1e-103">setDeviceName action</span></span>

<span data-ttu-id="f3b1e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3b1e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3b1e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3b1e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3b1e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3b1e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3b1e-107">Задание имени устройства для устройства.</span><span class="sxs-lookup"><span data-stu-id="f3b1e-107">Set device name of the device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3b1e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f3b1e-108">Prerequisites</span></span>
<span data-ttu-id="f3b1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3b1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3b1e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3b1e-111">Permission type</span></span>|<span data-ttu-id="f3b1e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3b1e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3b1e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3b1e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3b1e-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="f3b1e-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="f3b1e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3b1e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3b1e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3b1e-116">Not supported.</span></span>|
|<span data-ttu-id="f3b1e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3b1e-117">Application</span></span>|<span data-ttu-id="f3b1e-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="f3b1e-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3b1e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3b1e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/setDeviceName
POST /deviceManagement/comanagedDevices/{managedDeviceId}/setDeviceName
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/setDeviceName
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/setDeviceName
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/setDeviceName
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/setDeviceName
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/setDeviceName
```

## <a name="request-headers"></a><span data-ttu-id="f3b1e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f3b1e-120">Request headers</span></span>
|<span data-ttu-id="f3b1e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3b1e-121">Header</span></span>|<span data-ttu-id="f3b1e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f3b1e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3b1e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3b1e-123">Authorization</span></span>|<span data-ttu-id="f3b1e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3b1e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3b1e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3b1e-125">Accept</span></span>|<span data-ttu-id="f3b1e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3b1e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3b1e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f3b1e-127">Request body</span></span>
<span data-ttu-id="f3b1e-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3b1e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f3b1e-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f3b1e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f3b1e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3b1e-130">Property</span></span>|<span data-ttu-id="f3b1e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f3b1e-131">Type</span></span>|<span data-ttu-id="f3b1e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f3b1e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3b1e-133">deviceName</span><span class="sxs-lookup"><span data-stu-id="f3b1e-133">deviceName</span></span>|<span data-ttu-id="f3b1e-134">String</span><span class="sxs-lookup"><span data-stu-id="f3b1e-134">String</span></span>|<span data-ttu-id="f3b1e-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f3b1e-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f3b1e-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3b1e-136">Response</span></span>
<span data-ttu-id="f3b1e-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f3b1e-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f3b1e-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f3b1e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3b1e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3b1e-139">Request</span></span>
<span data-ttu-id="f3b1e-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3b1e-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/setDeviceName

Content-type: application/json
Content-length: 41

{
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="f3b1e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3b1e-141">Response</span></span>
<span data-ttu-id="f3b1e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3b1e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





