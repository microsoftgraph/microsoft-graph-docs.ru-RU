---
title: Действие updateWindowsDeviceAccount
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 54facf0cf6921db940bd1f027a24ba4d2f0fd6c5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474494"
---
# <a name="updatewindowsdeviceaccount-action"></a><span data-ttu-id="e4dfe-103">Действие updateWindowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="e4dfe-103">updateWindowsDeviceAccount action</span></span>

<span data-ttu-id="e4dfe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4dfe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4dfe-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4dfe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4dfe-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e4dfe-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4dfe-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e4dfe-107">Prerequisites</span></span>
<span data-ttu-id="e4dfe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4dfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4dfe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4dfe-110">Permission type</span></span>|<span data-ttu-id="e4dfe-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4dfe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4dfe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4dfe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4dfe-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e4dfe-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="e4dfe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4dfe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4dfe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4dfe-115">Not supported.</span></span>|
|<span data-ttu-id="e4dfe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4dfe-116">Application</span></span>|<span data-ttu-id="e4dfe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4dfe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4dfe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4dfe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a><span data-ttu-id="e4dfe-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e4dfe-119">Request headers</span></span>
|<span data-ttu-id="e4dfe-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4dfe-120">Header</span></span>|<span data-ttu-id="e4dfe-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e4dfe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4dfe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4dfe-122">Authorization</span></span>|<span data-ttu-id="e4dfe-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4dfe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4dfe-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e4dfe-124">Accept</span></span>|<span data-ttu-id="e4dfe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e4dfe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4dfe-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e4dfe-126">Request body</span></span>
<span data-ttu-id="e4dfe-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4dfe-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e4dfe-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e4dfe-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e4dfe-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4dfe-129">Property</span></span>|<span data-ttu-id="e4dfe-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e4dfe-130">Type</span></span>|<span data-ttu-id="e4dfe-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e4dfe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4dfe-132">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="e4dfe-132">updateWindowsDeviceAccountActionParameter</span></span>|[<span data-ttu-id="e4dfe-133">updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="e4dfe-133">updateWindowsDeviceAccountActionParameter</span></span>](../resources/intune-devices-updatewindowsdeviceaccountactionparameter.md)|<span data-ttu-id="e4dfe-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e4dfe-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e4dfe-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4dfe-135">Response</span></span>
<span data-ttu-id="e4dfe-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e4dfe-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e4dfe-137">Пример</span><span class="sxs-lookup"><span data-stu-id="e4dfe-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4dfe-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4dfe-138">Request</span></span>
<span data-ttu-id="e4dfe-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4dfe-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount

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

### <a name="response"></a><span data-ttu-id="e4dfe-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4dfe-140">Response</span></span>
<span data-ttu-id="e4dfe-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4dfe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






