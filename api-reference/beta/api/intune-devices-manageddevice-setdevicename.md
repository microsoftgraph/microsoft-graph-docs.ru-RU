---
title: Действие setDeviceName
description: Установите имя устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fbe2b47cc66bf686b645201f316788f189d39780
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136267"
---
# <a name="setdevicename-action"></a><span data-ttu-id="db51b-103">Действие setDeviceName</span><span class="sxs-lookup"><span data-stu-id="db51b-103">setDeviceName action</span></span>

<span data-ttu-id="db51b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db51b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db51b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db51b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db51b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db51b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db51b-107">Установите имя устройства.</span><span class="sxs-lookup"><span data-stu-id="db51b-107">Set device name of the device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db51b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="db51b-108">Prerequisites</span></span>
<span data-ttu-id="db51b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db51b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db51b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db51b-111">Permission type</span></span>|<span data-ttu-id="db51b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db51b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db51b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db51b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db51b-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="db51b-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="db51b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db51b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db51b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db51b-116">Not supported.</span></span>|
|<span data-ttu-id="db51b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="db51b-117">Application</span></span>|<span data-ttu-id="db51b-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="db51b-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db51b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db51b-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="db51b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="db51b-120">Request headers</span></span>
|<span data-ttu-id="db51b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="db51b-121">Header</span></span>|<span data-ttu-id="db51b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="db51b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db51b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db51b-123">Authorization</span></span>|<span data-ttu-id="db51b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db51b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db51b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="db51b-125">Accept</span></span>|<span data-ttu-id="db51b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db51b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db51b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db51b-127">Request body</span></span>
<span data-ttu-id="db51b-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db51b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="db51b-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="db51b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="db51b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="db51b-130">Property</span></span>|<span data-ttu-id="db51b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="db51b-131">Type</span></span>|<span data-ttu-id="db51b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="db51b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db51b-133">deviceName</span><span class="sxs-lookup"><span data-stu-id="db51b-133">deviceName</span></span>|<span data-ttu-id="db51b-134">String</span><span class="sxs-lookup"><span data-stu-id="db51b-134">String</span></span>|<span data-ttu-id="db51b-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="db51b-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="db51b-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="db51b-136">Response</span></span>
<span data-ttu-id="db51b-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="db51b-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="db51b-138">Пример</span><span class="sxs-lookup"><span data-stu-id="db51b-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="db51b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="db51b-139">Request</span></span>
<span data-ttu-id="db51b-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db51b-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/setDeviceName

Content-type: application/json
Content-length: 41

{
  "deviceName": "Device Name value"
}
```

### <a name="response"></a><span data-ttu-id="db51b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="db51b-141">Response</span></span>
<span data-ttu-id="db51b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db51b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




