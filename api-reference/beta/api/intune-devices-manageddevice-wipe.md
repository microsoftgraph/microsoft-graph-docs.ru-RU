---
title: Действие wipe
description: Очистка устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 59d9e4efc22364f815588d86c08625f31a195f38
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188306"
---
# <a name="wipe-action"></a><span data-ttu-id="2c96e-103">Действие wipe</span><span class="sxs-lookup"><span data-stu-id="2c96e-103">wipe action</span></span>

> <span data-ttu-id="2c96e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c96e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c96e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c96e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c96e-106">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="2c96e-106">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c96e-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2c96e-107">Prerequisites</span></span>
<span data-ttu-id="2c96e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c96e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c96e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c96e-110">Permission type</span></span>|<span data-ttu-id="2c96e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c96e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c96e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c96e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c96e-113">DeviceManagementManagedDevices. Привилижедоператион. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2c96e-113">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2c96e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c96e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c96e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c96e-115">Not supported.</span></span>|
|<span data-ttu-id="2c96e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c96e-116">Application</span></span>|<span data-ttu-id="2c96e-117">DeviceManagementManagedDevices. Привилижедоператион. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2c96e-117">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c96e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c96e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="2c96e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c96e-119">Request headers</span></span>
|<span data-ttu-id="2c96e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2c96e-120">Header</span></span>|<span data-ttu-id="2c96e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2c96e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c96e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c96e-122">Authorization</span></span>|<span data-ttu-id="2c96e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c96e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c96e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2c96e-124">Accept</span></span>|<span data-ttu-id="2c96e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2c96e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c96e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2c96e-126">Request body</span></span>
<span data-ttu-id="2c96e-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c96e-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2c96e-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2c96e-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2c96e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c96e-129">Property</span></span>|<span data-ttu-id="2c96e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2c96e-130">Type</span></span>|<span data-ttu-id="2c96e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2c96e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c96e-132">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="2c96e-132">keepEnrollmentData</span></span>|<span data-ttu-id="2c96e-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c96e-133">Boolean</span></span>|<span data-ttu-id="2c96e-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2c96e-134">Not yet documented</span></span>|
|<span data-ttu-id="2c96e-135">keepUserData</span><span class="sxs-lookup"><span data-stu-id="2c96e-135">keepUserData</span></span>|<span data-ttu-id="2c96e-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c96e-136">Boolean</span></span>|<span data-ttu-id="2c96e-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2c96e-137">Not yet documented</span></span>|
|<span data-ttu-id="2c96e-138">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="2c96e-138">macOsUnlockCode</span></span>|<span data-ttu-id="2c96e-139">String</span><span class="sxs-lookup"><span data-stu-id="2c96e-139">String</span></span>|<span data-ttu-id="2c96e-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2c96e-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2c96e-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="2c96e-141">Response</span></span>
<span data-ttu-id="2c96e-142">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2c96e-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2c96e-143">Пример</span><span class="sxs-lookup"><span data-stu-id="2c96e-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c96e-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c96e-144">Request</span></span>
<span data-ttu-id="2c96e-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c96e-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="2c96e-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c96e-146">Response</span></span>
<span data-ttu-id="2c96e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c96e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




