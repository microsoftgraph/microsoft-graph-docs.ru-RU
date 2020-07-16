---
title: Действие updateWindowsDeviceAccount
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 52ddeb86f69ddc781633ffa87a02f261575c6791
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792144"
---
# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="ae8f9-103">Действие updateWindowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="ae8f9-103">updateWindowsDeviceAccount action</span></span>

<span data-ttu-id="ae8f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae8f9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae8f9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae8f9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae8f9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae8f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae8f9-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ae8f9-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae8f9-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ae8f9-108">Prerequisites</span></span>
<span data-ttu-id="ae8f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae8f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae8f9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae8f9-111">Permission type</span></span>|<span data-ttu-id="ae8f9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae8f9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae8f9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae8f9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae8f9-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ae8f9-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="ae8f9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae8f9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae8f9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae8f9-116">Not supported.</span></span>|
|<span data-ttu-id="ae8f9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae8f9-117">Application</span></span>|<span data-ttu-id="ae8f9-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ae8f9-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae8f9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae8f9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/comanagedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/updateWindowsDeviceAccount
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="ae8f9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ae8f9-120">Request headers</span></span>
|<span data-ttu-id="ae8f9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae8f9-121">Header</span></span>|<span data-ttu-id="ae8f9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ae8f9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae8f9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae8f9-123">Authorization</span></span>|<span data-ttu-id="ae8f9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae8f9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae8f9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ae8f9-125">Accept</span></span>|<span data-ttu-id="ae8f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae8f9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae8f9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ae8f9-127">Request body</span></span>
<span data-ttu-id="ae8f9-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae8f9-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ae8f9-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="ae8f9-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ae8f9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae8f9-130">Property</span></span>|<span data-ttu-id="ae8f9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ae8f9-131">Type</span></span>|<span data-ttu-id="ae8f9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ae8f9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae8f9-133">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="ae8f9-133">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="ae8f9-134">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="ae8f9-134">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune-devices-updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="ae8f9-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ae8f9-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ae8f9-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="ae8f9-136">Response</span></span>
<span data-ttu-id="ae8f9-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ae8f9-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ae8f9-138">Пример</span><span class="sxs-lookup"><span data-stu-id="ae8f9-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae8f9-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae8f9-139">Request</span></span>
<span data-ttu-id="ae8f9-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae8f9-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount

Content-type: application/json
Content-length: 532

{
  "updateWindowsDeviceAccountActionParameter": {
    "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter",
    "deviceAccount": {
      "@odata.type": "microsoft.graph.windowsDeviceAccount",
      "password": "Password value"
    },
    "passwordRotationEnabled": true,
    "calendarSyncEnabled": true,
    "deviceAccountEmail": "Device Account Email value",
    "exchangeServer": "Exchange Server value",
    "sessionInitiationProtocalAddress": "Session Initiation Protocal Address value"
  }
}
```

### <a name="response"></a><span data-ttu-id="ae8f9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae8f9-141">Response</span></span>
<span data-ttu-id="ae8f9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae8f9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



