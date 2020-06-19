---
title: действие Ротатебитлоккеркэйс
description: Поворот Битлоккеркэйс
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 98c848dc2482c5c92b4d722397feb2d06301ca38
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792207"
---
# <a name="rotatebitlockerkeys-action"></a><span data-ttu-id="e3943-103">действие Ротатебитлоккеркэйс</span><span class="sxs-lookup"><span data-stu-id="e3943-103">rotateBitLockerKeys action</span></span>

<span data-ttu-id="e3943-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3943-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3943-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3943-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3943-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3943-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3943-107">Поворот Битлоккеркэйс</span><span class="sxs-lookup"><span data-stu-id="e3943-107">Rotate BitLockerKeys</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3943-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e3943-108">Prerequisites</span></span>
<span data-ttu-id="e3943-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e3943-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e3943-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3943-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3943-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3943-111">Permission type</span></span>|<span data-ttu-id="e3943-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3943-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3943-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3943-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3943-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3943-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e3943-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3943-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3943-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3943-116">Not supported.</span></span>|
|<span data-ttu-id="e3943-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3943-117">Application</span></span>|<span data-ttu-id="e3943-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3943-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3943-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3943-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/rotateBitLockerKeys
POST /deviceManagement/comanagedDevices/{managedDeviceId}/rotateBitLockerKeys
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/rotateBitLockerKeys
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/rotateBitLockerKeys
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/rotateBitLockerKeys
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/rotateBitLockerKeys
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/rotateBitLockerKeys
```

## <a name="request-headers"></a><span data-ttu-id="e3943-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e3943-120">Request headers</span></span>
|<span data-ttu-id="e3943-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3943-121">Header</span></span>|<span data-ttu-id="e3943-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e3943-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3943-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3943-123">Authorization</span></span>|<span data-ttu-id="e3943-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3943-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3943-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e3943-125">Accept</span></span>|<span data-ttu-id="e3943-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3943-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3943-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e3943-127">Request body</span></span>
<span data-ttu-id="e3943-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3943-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3943-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3943-129">Response</span></span>
<span data-ttu-id="e3943-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e3943-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e3943-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e3943-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3943-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3943-132">Request</span></span>
<span data-ttu-id="e3943-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3943-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/rotateBitLockerKeys
```

### <a name="response"></a><span data-ttu-id="e3943-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3943-134">Response</span></span>
<span data-ttu-id="e3943-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="e3943-135">Here is an example of the response.</span></span> <span data-ttu-id="e3943-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="e3943-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e3943-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e3943-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



