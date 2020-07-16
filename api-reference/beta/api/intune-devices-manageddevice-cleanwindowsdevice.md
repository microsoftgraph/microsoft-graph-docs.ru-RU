---
title: Действие cleanWindowsDevice
description: Очистка устройства с Windows
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1b6322a473d30a8a032448aacbe4f25c86c4fca7
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792326"
---
# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="d6074-103">Действие cleanWindowsDevice</span><span class="sxs-lookup"><span data-stu-id="d6074-103">cleanWindowsDevice action</span></span>

<span data-ttu-id="d6074-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6074-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6074-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6074-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6074-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6074-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6074-107">Очистка устройства с Windows</span><span class="sxs-lookup"><span data-stu-id="d6074-107">Clean Windows device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6074-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d6074-108">Prerequisites</span></span>
<span data-ttu-id="d6074-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6074-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6074-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6074-111">Permission type</span></span>|<span data-ttu-id="d6074-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6074-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6074-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6074-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6074-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="d6074-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="d6074-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6074-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6074-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6074-116">Not supported.</span></span>|
|<span data-ttu-id="d6074-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6074-117">Application</span></span>|<span data-ttu-id="d6074-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="d6074-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6074-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6074-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/comanagedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/cleanWindowsDevice
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="d6074-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d6074-120">Request headers</span></span>
|<span data-ttu-id="d6074-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6074-121">Header</span></span>|<span data-ttu-id="d6074-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d6074-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6074-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6074-123">Authorization</span></span>|<span data-ttu-id="d6074-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6074-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6074-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d6074-125">Accept</span></span>|<span data-ttu-id="d6074-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6074-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6074-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d6074-127">Request body</span></span>
<span data-ttu-id="d6074-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6074-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d6074-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d6074-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d6074-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6074-130">Property</span></span>|<span data-ttu-id="d6074-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d6074-131">Type</span></span>|<span data-ttu-id="d6074-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d6074-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6074-133">keepUserData</span><span class="sxs-lookup"><span data-stu-id="d6074-133">keepUserData</span></span>|<span data-ttu-id="d6074-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6074-134">Boolean</span></span>|<span data-ttu-id="d6074-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d6074-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d6074-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6074-136">Response</span></span>
<span data-ttu-id="d6074-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d6074-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d6074-138">Пример</span><span class="sxs-lookup"><span data-stu-id="d6074-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6074-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6074-139">Request</span></span>
<span data-ttu-id="d6074-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6074-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="d6074-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6074-141">Response</span></span>
<span data-ttu-id="d6074-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6074-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



