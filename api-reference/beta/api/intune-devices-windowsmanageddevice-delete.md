---
title: Удаление Виндовсманажеддевице
description: Удаляет объект Виндовсманажеддевице.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 82e33fb3afda0275a2211c09428ce8048911e3a4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43321947"
---
# <a name="delete-windowsmanageddevice"></a><span data-ttu-id="f7532-103">Удаление Виндовсманажеддевице</span><span class="sxs-lookup"><span data-stu-id="f7532-103">Delete windowsManagedDevice</span></span>

<span data-ttu-id="f7532-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7532-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7532-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7532-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7532-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7532-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7532-107">Удаляет объект [виндовсманажеддевице](../resources/intune-devices-windowsmanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f7532-107">Deletes a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7532-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f7532-108">Prerequisites</span></span>
<span data-ttu-id="f7532-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7532-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7532-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7532-111">Permission type</span></span>|<span data-ttu-id="f7532-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7532-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7532-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7532-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7532-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7532-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f7532-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7532-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7532-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7532-116">Not supported.</span></span>|
|<span data-ttu-id="f7532-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7532-117">Application</span></span>|<span data-ttu-id="f7532-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7532-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7532-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7532-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/managedDevices/{managedDeviceId}
DELETE /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="f7532-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f7532-120">Request headers</span></span>
|<span data-ttu-id="f7532-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7532-121">Header</span></span>|<span data-ttu-id="f7532-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f7532-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7532-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7532-123">Authorization</span></span>|<span data-ttu-id="f7532-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7532-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7532-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f7532-125">Accept</span></span>|<span data-ttu-id="f7532-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7532-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7532-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f7532-127">Request body</span></span>
<span data-ttu-id="f7532-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7532-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7532-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7532-129">Response</span></span>
<span data-ttu-id="f7532-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f7532-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f7532-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f7532-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7532-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7532-132">Request</span></span>
<span data-ttu-id="f7532-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7532-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
```

### <a name="response"></a><span data-ttu-id="f7532-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7532-134">Response</span></span>
<span data-ttu-id="f7532-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7532-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



