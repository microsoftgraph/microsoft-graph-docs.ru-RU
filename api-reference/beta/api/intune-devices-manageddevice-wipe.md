---
title: Действие wipe
description: Очистка устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0a918466c49a5dbfdd8083d054dbc270a11fd78d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944619"
---
# <a name="wipe-action"></a><span data-ttu-id="ad0c2-103">Действие wipe</span><span class="sxs-lookup"><span data-stu-id="ad0c2-103">wipe action</span></span>

> <span data-ttu-id="ad0c2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad0c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad0c2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad0c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad0c2-106">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="ad0c2-106">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad0c2-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ad0c2-107">Prerequisites</span></span>
<span data-ttu-id="ad0c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad0c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad0c2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad0c2-110">Permission type</span></span>|<span data-ttu-id="ad0c2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad0c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad0c2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad0c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ad0c2-113">DeviceManagementManagedDevices. Привилижедоператион. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ad0c2-113">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ad0c2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad0c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad0c2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad0c2-115">Not supported.</span></span>|
|<span data-ttu-id="ad0c2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad0c2-116">Application</span></span>|<span data-ttu-id="ad0c2-117">DeviceManagementManagedDevices. Привилижедоператион. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ad0c2-117">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad0c2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad0c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="ad0c2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ad0c2-119">Request headers</span></span>
|<span data-ttu-id="ad0c2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad0c2-120">Header</span></span>|<span data-ttu-id="ad0c2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ad0c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad0c2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad0c2-122">Authorization</span></span>|<span data-ttu-id="ad0c2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad0c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad0c2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ad0c2-124">Accept</span></span>|<span data-ttu-id="ad0c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ad0c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad0c2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ad0c2-126">Request body</span></span>
<span data-ttu-id="ad0c2-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad0c2-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ad0c2-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="ad0c2-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ad0c2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad0c2-129">Property</span></span>|<span data-ttu-id="ad0c2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ad0c2-130">Type</span></span>|<span data-ttu-id="ad0c2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ad0c2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad0c2-132">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="ad0c2-132">keepEnrollmentData</span></span>|<span data-ttu-id="ad0c2-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad0c2-133">Boolean</span></span>|<span data-ttu-id="ad0c2-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ad0c2-134">Not yet documented</span></span>|
|<span data-ttu-id="ad0c2-135">keepUserData</span><span class="sxs-lookup"><span data-stu-id="ad0c2-135">keepUserData</span></span>|<span data-ttu-id="ad0c2-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad0c2-136">Boolean</span></span>|<span data-ttu-id="ad0c2-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ad0c2-137">Not yet documented</span></span>|
|<span data-ttu-id="ad0c2-138">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="ad0c2-138">macOsUnlockCode</span></span>|<span data-ttu-id="ad0c2-139">String</span><span class="sxs-lookup"><span data-stu-id="ad0c2-139">String</span></span>|<span data-ttu-id="ad0c2-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ad0c2-140">Not yet documented</span></span>|
|<span data-ttu-id="ad0c2-141">усепротектедвипе</span><span class="sxs-lookup"><span data-stu-id="ad0c2-141">useProtectedWipe</span></span>|<span data-ttu-id="ad0c2-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad0c2-142">Boolean</span></span>|<span data-ttu-id="ad0c2-143">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="ad0c2-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ad0c2-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad0c2-144">Response</span></span>
<span data-ttu-id="ad0c2-145">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ad0c2-145">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ad0c2-146">Пример</span><span class="sxs-lookup"><span data-stu-id="ad0c2-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad0c2-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad0c2-147">Request</span></span>
<span data-ttu-id="ad0c2-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad0c2-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 138

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value",
  "useProtectedWipe": true
}
```

### <a name="response"></a><span data-ttu-id="ad0c2-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad0c2-149">Response</span></span>
<span data-ttu-id="ad0c2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad0c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





