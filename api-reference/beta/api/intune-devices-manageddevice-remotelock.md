---
title: Действие remoteLock
description: Удаленная блокировка
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3c5ba66de80f6876f8bb2648429a3c843101bfb7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708230"
---
# <a name="remotelock-action"></a><span data-ttu-id="b510b-103">Действие remoteLock</span><span class="sxs-lookup"><span data-stu-id="b510b-103">remoteLock action</span></span>

<span data-ttu-id="b510b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b510b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b510b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b510b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b510b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b510b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b510b-107">Удаленная блокировка</span><span class="sxs-lookup"><span data-stu-id="b510b-107">Remote lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b510b-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b510b-108">Prerequisites</span></span>
<span data-ttu-id="b510b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b510b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b510b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b510b-111">Permission type</span></span>|<span data-ttu-id="b510b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b510b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b510b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b510b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b510b-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="b510b-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="b510b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b510b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b510b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b510b-116">Not supported.</span></span>|
|<span data-ttu-id="b510b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b510b-117">Application</span></span>|<span data-ttu-id="b510b-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="b510b-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b510b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b510b-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b510b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b510b-120">Request headers</span></span>
|<span data-ttu-id="b510b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b510b-121">Header</span></span>|<span data-ttu-id="b510b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b510b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b510b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b510b-123">Authorization</span></span>|<span data-ttu-id="b510b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b510b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b510b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b510b-125">Accept</span></span>|<span data-ttu-id="b510b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b510b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b510b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b510b-127">Request body</span></span>
<span data-ttu-id="b510b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b510b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b510b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b510b-129">Response</span></span>
<span data-ttu-id="b510b-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b510b-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b510b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b510b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b510b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b510b-132">Request</span></span>
<span data-ttu-id="b510b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b510b-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/remoteLock
```

### <a name="response"></a><span data-ttu-id="b510b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b510b-134">Response</span></span>
<span data-ttu-id="b510b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b510b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





