---
title: Действие syncDevice
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: af31de2cf3e803abc239732a48e7fbb22dd8a1a1
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37528362"
---
# <a name="syncdevice-action"></a><span data-ttu-id="79665-103">Действие syncDevice</span><span class="sxs-lookup"><span data-stu-id="79665-103">syncDevice action</span></span>

> <span data-ttu-id="79665-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79665-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79665-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79665-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79665-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="79665-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79665-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="79665-107">Prerequisites</span></span>
<span data-ttu-id="79665-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79665-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79665-110">Permission type</span></span>|<span data-ttu-id="79665-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="79665-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79665-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79665-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79665-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="79665-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="79665-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79665-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79665-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79665-115">Not supported.</span></span>|
|<span data-ttu-id="79665-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="79665-116">Application</span></span>|<span data-ttu-id="79665-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="79665-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79665-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79665-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/syncDevice
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/syncDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/syncDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/syncDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/syncDevice
```

## <a name="request-headers"></a><span data-ttu-id="79665-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79665-119">Request headers</span></span>
|<span data-ttu-id="79665-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79665-120">Header</span></span>|<span data-ttu-id="79665-121">Значение</span><span class="sxs-lookup"><span data-stu-id="79665-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79665-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79665-122">Authorization</span></span>|<span data-ttu-id="79665-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79665-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79665-124">Accept</span><span class="sxs-lookup"><span data-stu-id="79665-124">Accept</span></span>|<span data-ttu-id="79665-125">application/json</span><span class="sxs-lookup"><span data-stu-id="79665-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79665-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79665-126">Request body</span></span>
<span data-ttu-id="79665-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79665-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79665-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="79665-128">Response</span></span>
<span data-ttu-id="79665-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="79665-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="79665-130">Пример</span><span class="sxs-lookup"><span data-stu-id="79665-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="79665-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="79665-131">Request</span></span>
<span data-ttu-id="79665-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79665-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/syncDevice
```

### <a name="response"></a><span data-ttu-id="79665-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="79665-133">Response</span></span>
<span data-ttu-id="79665-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79665-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






