---
title: Действие disableLostMode
description: Отключение режима пропажи устройства
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 60f000fa5fb234d2091bc1ab4c4a42384bf85059
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792312"
---
# <a name="disablelostmode-action"></a><span data-ttu-id="f3028-103">Действие disableLostMode</span><span class="sxs-lookup"><span data-stu-id="f3028-103">disableLostMode action</span></span>

<span data-ttu-id="f3028-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3028-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3028-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3028-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3028-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3028-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3028-107">Отключение режима пропажи устройства</span><span class="sxs-lookup"><span data-stu-id="f3028-107">Disable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3028-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f3028-108">Prerequisites</span></span>
<span data-ttu-id="f3028-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f3028-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f3028-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3028-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3028-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3028-111">Permission type</span></span>|<span data-ttu-id="f3028-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3028-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3028-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3028-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3028-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="f3028-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="f3028-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3028-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3028-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3028-116">Not supported.</span></span>|
|<span data-ttu-id="f3028-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3028-117">Application</span></span>|<span data-ttu-id="f3028-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="f3028-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3028-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3028-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/disableLostMode
POST /deviceManagement/comanagedDevices/{managedDeviceId}/disableLostMode
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/disableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/disableLostMode
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/disableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/disableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/disableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="f3028-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f3028-120">Request headers</span></span>
|<span data-ttu-id="f3028-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3028-121">Header</span></span>|<span data-ttu-id="f3028-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f3028-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3028-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3028-123">Authorization</span></span>|<span data-ttu-id="f3028-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3028-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3028-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3028-125">Accept</span></span>|<span data-ttu-id="f3028-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3028-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3028-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f3028-127">Request body</span></span>
<span data-ttu-id="f3028-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3028-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3028-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3028-129">Response</span></span>
<span data-ttu-id="f3028-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f3028-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f3028-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f3028-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3028-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3028-132">Request</span></span>
<span data-ttu-id="f3028-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3028-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/disableLostMode
```

### <a name="response"></a><span data-ttu-id="f3028-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3028-134">Response</span></span>
<span data-ttu-id="f3028-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="f3028-135">Here is an example of the response.</span></span> <span data-ttu-id="f3028-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="f3028-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f3028-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f3028-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



