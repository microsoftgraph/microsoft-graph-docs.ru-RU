---
title: Действие updateWindowsDeviceAccount
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d3645b1aa22c01bfc8f9d317e0d1c21e771570c9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158327"
---
# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="c0e49-103">Действие updateWindowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="c0e49-103">updateWindowsDeviceAccount action</span></span>

<span data-ttu-id="c0e49-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0e49-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0e49-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0e49-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0e49-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0e49-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0e49-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c0e49-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0e49-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c0e49-108">Prerequisites</span></span>
<span data-ttu-id="c0e49-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0e49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0e49-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0e49-111">Permission type</span></span>|<span data-ttu-id="c0e49-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0e49-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0e49-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0e49-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0e49-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="c0e49-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="c0e49-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0e49-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0e49-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0e49-116">Not supported.</span></span>|
|<span data-ttu-id="c0e49-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c0e49-117">Application</span></span>|<span data-ttu-id="c0e49-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="c0e49-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0e49-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0e49-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c0e49-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c0e49-120">Request headers</span></span>
|<span data-ttu-id="c0e49-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c0e49-121">Header</span></span>|<span data-ttu-id="c0e49-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c0e49-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0e49-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0e49-123">Authorization</span></span>|<span data-ttu-id="c0e49-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0e49-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0e49-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c0e49-125">Accept</span></span>|<span data-ttu-id="c0e49-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0e49-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0e49-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0e49-127">Request body</span></span>
<span data-ttu-id="c0e49-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0e49-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c0e49-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c0e49-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c0e49-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0e49-130">Property</span></span>|<span data-ttu-id="c0e49-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c0e49-131">Type</span></span>|<span data-ttu-id="c0e49-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c0e49-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0e49-133">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="c0e49-133">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="c0e49-134">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="c0e49-134">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune-devices-updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="c0e49-135">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="c0e49-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c0e49-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0e49-136">Response</span></span>
<span data-ttu-id="c0e49-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c0e49-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c0e49-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c0e49-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0e49-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0e49-139">Request</span></span>
<span data-ttu-id="c0e49-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0e49-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c0e49-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0e49-141">Response</span></span>
<span data-ttu-id="c0e49-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c0e49-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




