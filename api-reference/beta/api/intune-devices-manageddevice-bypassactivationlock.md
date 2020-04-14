---
title: Действие bypassActivationLock
description: Обход блокировки активации
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c8c47e15a3f3c682b930f540c5f4f5b71d4227df
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43325010"
---
# <a name="bypassactivationlock-action"></a><span data-ttu-id="fc68f-103">Действие bypassActivationLock</span><span class="sxs-lookup"><span data-stu-id="fc68f-103">bypassActivationLock action</span></span>

<span data-ttu-id="fc68f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc68f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc68f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc68f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc68f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc68f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc68f-107">Обход блокировки активации</span><span class="sxs-lookup"><span data-stu-id="fc68f-107">Bypass activation lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc68f-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fc68f-108">Prerequisites</span></span>
<span data-ttu-id="fc68f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc68f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc68f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc68f-111">Permission type</span></span>|<span data-ttu-id="fc68f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc68f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc68f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc68f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc68f-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="fc68f-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="fc68f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc68f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc68f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc68f-116">Not supported.</span></span>|
|<span data-ttu-id="fc68f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc68f-117">Application</span></span>|<span data-ttu-id="fc68f-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="fc68f-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc68f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc68f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/bypassActivationLock
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/bypassActivationLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/bypassActivationLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/bypassActivationLock
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/bypassActivationLock
```

## <a name="request-headers"></a><span data-ttu-id="fc68f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fc68f-120">Request headers</span></span>
|<span data-ttu-id="fc68f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc68f-121">Header</span></span>|<span data-ttu-id="fc68f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fc68f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc68f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc68f-123">Authorization</span></span>|<span data-ttu-id="fc68f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc68f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc68f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fc68f-125">Accept</span></span>|<span data-ttu-id="fc68f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc68f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc68f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc68f-127">Request body</span></span>
<span data-ttu-id="fc68f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fc68f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc68f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="fc68f-129">Response</span></span>
<span data-ttu-id="fc68f-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fc68f-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fc68f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fc68f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc68f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc68f-132">Request</span></span>
<span data-ttu-id="fc68f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc68f-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/bypassActivationLock
```

### <a name="response"></a><span data-ttu-id="fc68f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc68f-134">Response</span></span>
<span data-ttu-id="fc68f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc68f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



