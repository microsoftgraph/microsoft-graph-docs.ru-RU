---
title: Действие locateDevice
description: Поиск устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9b58b025482c1bdcf57dbdc1dc5ea5056b80b68d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036585"
---
# <a name="locatedevice-action"></a><span data-ttu-id="3d283-103">Действие locateDevice</span><span class="sxs-lookup"><span data-stu-id="3d283-103">locateDevice action</span></span>

<span data-ttu-id="3d283-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d283-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d283-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d283-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d283-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d283-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d283-107">Поиск устройства</span><span class="sxs-lookup"><span data-stu-id="3d283-107">Locate a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d283-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3d283-108">Prerequisites</span></span>
<span data-ttu-id="3d283-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d283-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d283-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d283-111">Permission type</span></span>|<span data-ttu-id="3d283-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d283-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d283-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d283-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d283-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="3d283-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="3d283-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d283-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d283-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d283-116">Not supported.</span></span>|
|<span data-ttu-id="3d283-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d283-117">Application</span></span>|<span data-ttu-id="3d283-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="3d283-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d283-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d283-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/comanagedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/locateDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/locateDevice
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/locateDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/locateDevice
```

## <a name="request-headers"></a><span data-ttu-id="3d283-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3d283-120">Request headers</span></span>
|<span data-ttu-id="3d283-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3d283-121">Header</span></span>|<span data-ttu-id="3d283-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3d283-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d283-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d283-123">Authorization</span></span>|<span data-ttu-id="3d283-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d283-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d283-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3d283-125">Accept</span></span>|<span data-ttu-id="3d283-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d283-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d283-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d283-127">Request body</span></span>
<span data-ttu-id="3d283-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3d283-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d283-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d283-129">Response</span></span>
<span data-ttu-id="3d283-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3d283-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3d283-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3d283-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d283-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d283-132">Request</span></span>
<span data-ttu-id="3d283-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d283-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/locateDevice
```

### <a name="response"></a><span data-ttu-id="3d283-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d283-134">Response</span></span>
<span data-ttu-id="3d283-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3d283-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






