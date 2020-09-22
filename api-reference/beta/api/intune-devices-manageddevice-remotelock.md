---
title: Действие remoteLock
description: Удаленная блокировка
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 36ee54a1192881b11d08d176728801321a4ce39d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48005273"
---
# <a name="remotelock-action"></a><span data-ttu-id="1c4fa-103">Действие remoteLock</span><span class="sxs-lookup"><span data-stu-id="1c4fa-103">remoteLock action</span></span>

<span data-ttu-id="1c4fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c4fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c4fa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c4fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c4fa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c4fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c4fa-107">Удаленная блокировка</span><span class="sxs-lookup"><span data-stu-id="1c4fa-107">Remote lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c4fa-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1c4fa-108">Prerequisites</span></span>
<span data-ttu-id="1c4fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c4fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c4fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c4fa-111">Permission type</span></span>|<span data-ttu-id="1c4fa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c4fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c4fa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c4fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c4fa-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="1c4fa-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="1c4fa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c4fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c4fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c4fa-116">Not supported.</span></span>|
|<span data-ttu-id="1c4fa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c4fa-117">Application</span></span>|<span data-ttu-id="1c4fa-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="1c4fa-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c4fa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c4fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/comanagedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/remoteLock
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/remoteLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/remoteLock
```

## <a name="request-headers"></a><span data-ttu-id="1c4fa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1c4fa-120">Request headers</span></span>
|<span data-ttu-id="1c4fa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c4fa-121">Header</span></span>|<span data-ttu-id="1c4fa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1c4fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c4fa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c4fa-123">Authorization</span></span>|<span data-ttu-id="1c4fa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c4fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c4fa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1c4fa-125">Accept</span></span>|<span data-ttu-id="1c4fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c4fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c4fa-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1c4fa-127">Request body</span></span>
<span data-ttu-id="1c4fa-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c4fa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c4fa-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c4fa-129">Response</span></span>
<span data-ttu-id="1c4fa-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1c4fa-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1c4fa-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1c4fa-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c4fa-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c4fa-132">Request</span></span>
<span data-ttu-id="1c4fa-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c4fa-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/remoteLock
```

### <a name="response"></a><span data-ttu-id="1c4fa-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c4fa-134">Response</span></span>
<span data-ttu-id="1c4fa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c4fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






