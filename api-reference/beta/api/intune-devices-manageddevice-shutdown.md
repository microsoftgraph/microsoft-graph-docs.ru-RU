---
title: Действие shutDown
description: Завершение работы устройства
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 775202ca6115de703877448d1bf0121c73369504
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43425153"
---
# <a name="shutdown-action"></a><span data-ttu-id="19366-103">Действие shutDown</span><span class="sxs-lookup"><span data-stu-id="19366-103">shutDown action</span></span>

<span data-ttu-id="19366-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19366-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19366-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19366-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19366-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19366-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19366-107">Завершение работы устройства</span><span class="sxs-lookup"><span data-stu-id="19366-107">Shut down device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19366-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="19366-108">Prerequisites</span></span>
<span data-ttu-id="19366-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19366-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19366-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19366-111">Permission type</span></span>|<span data-ttu-id="19366-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19366-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19366-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19366-113">Delegated (work or school account)</span></span>|<span data-ttu-id="19366-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="19366-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="19366-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19366-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19366-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19366-116">Not supported.</span></span>|
|<span data-ttu-id="19366-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="19366-117">Application</span></span>|<span data-ttu-id="19366-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="19366-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19366-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19366-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/shutDown
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/shutDown
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/shutDown
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/shutDown
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/shutDown
```

## <a name="request-headers"></a><span data-ttu-id="19366-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="19366-120">Request headers</span></span>
|<span data-ttu-id="19366-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19366-121">Header</span></span>|<span data-ttu-id="19366-122">Значение</span><span class="sxs-lookup"><span data-stu-id="19366-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19366-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19366-123">Authorization</span></span>|<span data-ttu-id="19366-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19366-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19366-125">Accept</span><span class="sxs-lookup"><span data-stu-id="19366-125">Accept</span></span>|<span data-ttu-id="19366-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19366-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19366-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19366-127">Request body</span></span>
<span data-ttu-id="19366-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19366-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19366-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="19366-129">Response</span></span>
<span data-ttu-id="19366-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="19366-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="19366-131">Пример</span><span class="sxs-lookup"><span data-stu-id="19366-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="19366-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="19366-132">Request</span></span>
<span data-ttu-id="19366-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19366-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/shutDown
```

### <a name="response"></a><span data-ttu-id="19366-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="19366-134">Response</span></span>
<span data-ttu-id="19366-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19366-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



