---
title: Действие enableLostMode
description: Включение режима потери
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 26bbbe4e0e4761b4ba1ebfe2f87189cbc863392d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767752"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="4bfba-103">Действие enableLostMode</span><span class="sxs-lookup"><span data-stu-id="4bfba-103">enableLostMode action</span></span>

> <span data-ttu-id="4bfba-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bfba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bfba-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4bfba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bfba-106">Включение режима потери</span><span class="sxs-lookup"><span data-stu-id="4bfba-106">Enable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4bfba-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4bfba-107">Prerequisites</span></span>
<span data-ttu-id="4bfba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bfba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bfba-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bfba-110">Permission type</span></span>|<span data-ttu-id="4bfba-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bfba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bfba-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bfba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4bfba-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="4bfba-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="4bfba-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bfba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bfba-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bfba-115">Not supported.</span></span>|
|<span data-ttu-id="4bfba-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4bfba-116">Application</span></span>|<span data-ttu-id="4bfba-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="4bfba-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bfba-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bfba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/enableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="4bfba-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4bfba-119">Request headers</span></span>
|<span data-ttu-id="4bfba-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4bfba-120">Header</span></span>|<span data-ttu-id="4bfba-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4bfba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bfba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bfba-122">Authorization</span></span>|<span data-ttu-id="4bfba-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bfba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bfba-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4bfba-124">Accept</span></span>|<span data-ttu-id="4bfba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4bfba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bfba-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4bfba-126">Request body</span></span>
<span data-ttu-id="4bfba-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4bfba-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4bfba-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4bfba-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4bfba-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bfba-129">Property</span></span>|<span data-ttu-id="4bfba-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4bfba-130">Type</span></span>|<span data-ttu-id="4bfba-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4bfba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bfba-132">message</span><span class="sxs-lookup"><span data-stu-id="4bfba-132">message</span></span>|<span data-ttu-id="4bfba-133">String</span><span class="sxs-lookup"><span data-stu-id="4bfba-133">String</span></span>|<span data-ttu-id="4bfba-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4bfba-134">Not yet documented</span></span>|
|<span data-ttu-id="4bfba-135">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="4bfba-135">phoneNumber</span></span>|<span data-ttu-id="4bfba-136">String</span><span class="sxs-lookup"><span data-stu-id="4bfba-136">String</span></span>|<span data-ttu-id="4bfba-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4bfba-137">Not yet documented</span></span>|
|<span data-ttu-id="4bfba-138">нижний колонтитул</span><span class="sxs-lookup"><span data-stu-id="4bfba-138">footer</span></span>|<span data-ttu-id="4bfba-139">String</span><span class="sxs-lookup"><span data-stu-id="4bfba-139">String</span></span>|<span data-ttu-id="4bfba-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4bfba-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4bfba-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="4bfba-141">Response</span></span>
<span data-ttu-id="4bfba-142">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4bfba-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4bfba-143">Пример</span><span class="sxs-lookup"><span data-stu-id="4bfba-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="4bfba-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bfba-144">Request</span></span>
<span data-ttu-id="4bfba-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4bfba-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/enableLostMode

Content-type: application/json
Content-length: 103

{
  "message": "Message value",
  "phoneNumber": "Phone Number value",
  "footer": "Footer value"
}
```

### <a name="response"></a><span data-ttu-id="4bfba-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bfba-146">Response</span></span>
<span data-ttu-id="4bfba-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4bfba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




