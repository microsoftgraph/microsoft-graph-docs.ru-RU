---
title: Действие disableLostMode
description: Отключение режима пропажи устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b938d79c7722ee56d456d098e4d42d2385f2f7d4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731703"
---
# <a name="disablelostmode-action"></a><span data-ttu-id="9fa97-103">Действие disableLostMode</span><span class="sxs-lookup"><span data-stu-id="9fa97-103">disableLostMode action</span></span>

<span data-ttu-id="9fa97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fa97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fa97-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fa97-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fa97-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9fa97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fa97-107">Отключение режима пропажи устройства</span><span class="sxs-lookup"><span data-stu-id="9fa97-107">Disable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fa97-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9fa97-108">Prerequisites</span></span>
<span data-ttu-id="9fa97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fa97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fa97-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fa97-111">Permission type</span></span>|<span data-ttu-id="9fa97-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fa97-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fa97-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fa97-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9fa97-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="9fa97-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="9fa97-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fa97-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fa97-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fa97-116">Not supported.</span></span>|
|<span data-ttu-id="9fa97-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9fa97-117">Application</span></span>|<span data-ttu-id="9fa97-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="9fa97-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fa97-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fa97-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9fa97-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9fa97-120">Request headers</span></span>
|<span data-ttu-id="9fa97-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9fa97-121">Header</span></span>|<span data-ttu-id="9fa97-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9fa97-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fa97-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9fa97-123">Authorization</span></span>|<span data-ttu-id="9fa97-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fa97-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fa97-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9fa97-125">Accept</span></span>|<span data-ttu-id="9fa97-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9fa97-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fa97-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9fa97-127">Request body</span></span>
<span data-ttu-id="9fa97-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9fa97-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fa97-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="9fa97-129">Response</span></span>
<span data-ttu-id="9fa97-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9fa97-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9fa97-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9fa97-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fa97-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fa97-132">Request</span></span>
<span data-ttu-id="9fa97-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fa97-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/disableLostMode
```

### <a name="response"></a><span data-ttu-id="9fa97-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fa97-134">Response</span></span>
<span data-ttu-id="9fa97-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9fa97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





