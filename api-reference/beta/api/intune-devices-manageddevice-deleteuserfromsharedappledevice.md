---
title: Действие deleteUserFromSharedAppleDevice
description: Удаление пользователя на общем устройстве Apple
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1276351b8d0624bf8c54198f5e5d5b839a0e7406
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792319"
---
# <a name="deleteuserfromsharedappledevice-action"></a><span data-ttu-id="6d6fe-103">Действие deleteUserFromSharedAppleDevice</span><span class="sxs-lookup"><span data-stu-id="6d6fe-103">deleteUserFromSharedAppleDevice action</span></span>

<span data-ttu-id="6d6fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d6fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d6fe-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d6fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d6fe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d6fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d6fe-107">Удаление пользователя на общем устройстве Apple</span><span class="sxs-lookup"><span data-stu-id="6d6fe-107">Delete user from shared Apple device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d6fe-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6d6fe-108">Prerequisites</span></span>
<span data-ttu-id="6d6fe-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6d6fe-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6d6fe-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d6fe-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d6fe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d6fe-111">Permission type</span></span>|<span data-ttu-id="6d6fe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d6fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d6fe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d6fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d6fe-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="6d6fe-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="6d6fe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d6fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d6fe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d6fe-116">Not supported.</span></span>|
|<span data-ttu-id="6d6fe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d6fe-117">Application</span></span>|<span data-ttu-id="6d6fe-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="6d6fe-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d6fe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d6fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/comanagedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
```

## <a name="request-headers"></a><span data-ttu-id="6d6fe-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6d6fe-120">Request headers</span></span>
|<span data-ttu-id="6d6fe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d6fe-121">Header</span></span>|<span data-ttu-id="6d6fe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6d6fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d6fe-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d6fe-123">Authorization</span></span>|<span data-ttu-id="6d6fe-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d6fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d6fe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6d6fe-125">Accept</span></span>|<span data-ttu-id="6d6fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d6fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d6fe-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6d6fe-127">Request body</span></span>
<span data-ttu-id="6d6fe-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d6fe-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6d6fe-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="6d6fe-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6d6fe-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d6fe-130">Property</span></span>|<span data-ttu-id="6d6fe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6d6fe-131">Type</span></span>|<span data-ttu-id="6d6fe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6d6fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d6fe-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6d6fe-133">userPrincipalName</span></span>|<span data-ttu-id="6d6fe-134">String</span><span class="sxs-lookup"><span data-stu-id="6d6fe-134">String</span></span>|<span data-ttu-id="6d6fe-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6d6fe-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6d6fe-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d6fe-136">Response</span></span>
<span data-ttu-id="6d6fe-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6d6fe-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6d6fe-138">Пример</span><span class="sxs-lookup"><span data-stu-id="6d6fe-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d6fe-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d6fe-139">Request</span></span>
<span data-ttu-id="6d6fe-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d6fe-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice

Content-type: application/json
Content-length: 56

{
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="6d6fe-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d6fe-141">Response</span></span>
<span data-ttu-id="6d6fe-142">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="6d6fe-142">Here is an example of the response.</span></span> <span data-ttu-id="6d6fe-143">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="6d6fe-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6d6fe-144">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="6d6fe-144">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



