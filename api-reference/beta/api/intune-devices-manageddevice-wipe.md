---
title: Действие wipe
description: Очистка устройства
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ea07fd650a00e91896639d0312b48bb787b2b54
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792129"
---
# <a name="wipe-action"></a><span data-ttu-id="4c4f3-103">Действие wipe</span><span class="sxs-lookup"><span data-stu-id="4c4f3-103">wipe action</span></span>

<span data-ttu-id="4c4f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c4f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c4f3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c4f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c4f3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4c4f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c4f3-107">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="4c4f3-107">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c4f3-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4c4f3-108">Prerequisites</span></span>
<span data-ttu-id="4c4f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c4f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c4f3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c4f3-111">Permission type</span></span>|<span data-ttu-id="4c4f3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c4f3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c4f3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c4f3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c4f3-114">DeviceManagementManagedDevices. Привилижедоператион. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4c4f3-114">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4c4f3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c4f3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c4f3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c4f3-116">Not supported.</span></span>|
|<span data-ttu-id="4c4f3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c4f3-117">Application</span></span>|<span data-ttu-id="4c4f3-118">DeviceManagementManagedDevices. Привилижедоператион. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4c4f3-118">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c4f3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c4f3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/comanagedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="4c4f3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4c4f3-120">Request headers</span></span>
|<span data-ttu-id="4c4f3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c4f3-121">Header</span></span>|<span data-ttu-id="4c4f3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4c4f3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c4f3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c4f3-123">Authorization</span></span>|<span data-ttu-id="4c4f3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c4f3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c4f3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4c4f3-125">Accept</span></span>|<span data-ttu-id="4c4f3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c4f3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c4f3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c4f3-127">Request body</span></span>
<span data-ttu-id="4c4f3-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c4f3-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4c4f3-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4c4f3-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4c4f3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c4f3-130">Property</span></span>|<span data-ttu-id="4c4f3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4c4f3-131">Type</span></span>|<span data-ttu-id="4c4f3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4c4f3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c4f3-133">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="4c4f3-133">keepEnrollmentData</span></span>|<span data-ttu-id="4c4f3-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c4f3-134">Boolean</span></span>|<span data-ttu-id="4c4f3-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4c4f3-135">Not yet documented</span></span>|
|<span data-ttu-id="4c4f3-136">keepUserData</span><span class="sxs-lookup"><span data-stu-id="4c4f3-136">keepUserData</span></span>|<span data-ttu-id="4c4f3-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c4f3-137">Boolean</span></span>|<span data-ttu-id="4c4f3-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4c4f3-138">Not yet documented</span></span>|
|<span data-ttu-id="4c4f3-139">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="4c4f3-139">macOsUnlockCode</span></span>|<span data-ttu-id="4c4f3-140">String</span><span class="sxs-lookup"><span data-stu-id="4c4f3-140">String</span></span>|<span data-ttu-id="4c4f3-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4c4f3-141">Not yet documented</span></span>|
|<span data-ttu-id="4c4f3-142">усепротектедвипе</span><span class="sxs-lookup"><span data-stu-id="4c4f3-142">useProtectedWipe</span></span>|<span data-ttu-id="4c4f3-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c4f3-143">Boolean</span></span>|<span data-ttu-id="4c4f3-144">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="4c4f3-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4c4f3-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c4f3-145">Response</span></span>
<span data-ttu-id="4c4f3-146">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4c4f3-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4c4f3-147">Пример</span><span class="sxs-lookup"><span data-stu-id="4c4f3-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c4f3-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c4f3-148">Request</span></span>
<span data-ttu-id="4c4f3-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c4f3-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4c4f3-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c4f3-150">Response</span></span>
<span data-ttu-id="4c4f3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c4f3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



