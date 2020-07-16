---
title: Действие windowsDefenderUpdateSignatures
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0efb97522532a0ecdc02fdce73e92edde4c24f91
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792136"
---
# <a name="windowsdefenderupdatesignatures-action"></a><span data-ttu-id="0b361-103">Действие windowsDefenderUpdateSignatures</span><span class="sxs-lookup"><span data-stu-id="0b361-103">windowsDefenderUpdateSignatures action</span></span>

<span data-ttu-id="0b361-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b361-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b361-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b361-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b361-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b361-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b361-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0b361-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b361-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0b361-108">Prerequisites</span></span>
<span data-ttu-id="0b361-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b361-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b361-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b361-111">Permission type</span></span>|<span data-ttu-id="0b361-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b361-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b361-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b361-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b361-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="0b361-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="0b361-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b361-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b361-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b361-116">Not supported.</span></span>|
|<span data-ttu-id="0b361-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b361-117">Application</span></span>|<span data-ttu-id="0b361-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="0b361-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b361-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b361-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
POST /deviceManagement/comanagedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/windowsDefenderUpdateSignatures
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsDefenderUpdateSignatures
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/windowsDefenderUpdateSignatures
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
```

## <a name="request-headers"></a><span data-ttu-id="0b361-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0b361-120">Request headers</span></span>
|<span data-ttu-id="0b361-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b361-121">Header</span></span>|<span data-ttu-id="0b361-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0b361-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b361-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b361-123">Authorization</span></span>|<span data-ttu-id="0b361-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b361-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b361-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0b361-125">Accept</span></span>|<span data-ttu-id="0b361-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b361-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b361-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0b361-127">Request body</span></span>
<span data-ttu-id="0b361-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b361-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b361-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b361-129">Response</span></span>
<span data-ttu-id="0b361-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0b361-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0b361-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0b361-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b361-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b361-132">Request</span></span>
<span data-ttu-id="0b361-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b361-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
```

### <a name="response"></a><span data-ttu-id="0b361-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b361-134">Response</span></span>
<span data-ttu-id="0b361-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b361-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



