---
title: Функция Жетфилеваулткэй
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7afb1ed844b0742df81c2b35bafbf4360deafb26
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792284"
---
# <a name="getfilevaultkey-function"></a><span data-ttu-id="7e892-103">Функция Жетфилеваулткэй</span><span class="sxs-lookup"><span data-stu-id="7e892-103">getFileVaultKey function</span></span>

<span data-ttu-id="7e892-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e892-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e892-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e892-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e892-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e892-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e892-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7e892-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e892-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7e892-108">Prerequisites</span></span>
<span data-ttu-id="7e892-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="7e892-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7e892-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e892-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e892-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e892-111">Permission type</span></span>|<span data-ttu-id="7e892-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e892-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e892-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e892-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7e892-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e892-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7e892-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e892-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e892-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e892-116">Not supported.</span></span>|
|<span data-ttu-id="7e892-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e892-117">Application</span></span>|<span data-ttu-id="7e892-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e892-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e892-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e892-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDevices/{managedDeviceId}/getFileVaultKey
GET /deviceManagement/comanagedDevices/{managedDeviceId}/getFileVaultKey
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/getFileVaultKey
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/getFileVaultKey
GET /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/getFileVaultKey
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/getFileVaultKey
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/getFileVaultKey
```

## <a name="request-headers"></a><span data-ttu-id="7e892-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7e892-120">Request headers</span></span>
|<span data-ttu-id="7e892-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e892-121">Header</span></span>|<span data-ttu-id="7e892-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7e892-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e892-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e892-123">Authorization</span></span>|<span data-ttu-id="7e892-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e892-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e892-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7e892-125">Accept</span></span>|<span data-ttu-id="7e892-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7e892-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e892-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7e892-127">Request body</span></span>
<span data-ttu-id="7e892-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e892-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e892-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e892-129">Response</span></span>
<span data-ttu-id="7e892-130">В случае успеха эта функция возвращает `200 OK` код отклика и строку в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7e892-130">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e892-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7e892-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e892-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e892-132">Request</span></span>
<span data-ttu-id="7e892-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e892-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/getFileVaultKey
```

### <a name="response"></a><span data-ttu-id="7e892-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e892-134">Response</span></span>
<span data-ttu-id="7e892-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="7e892-135">Here is an example of the response.</span></span> <span data-ttu-id="7e892-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="7e892-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7e892-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="7e892-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 43

{
  "value": "Get File Vault Key value"
}
```



