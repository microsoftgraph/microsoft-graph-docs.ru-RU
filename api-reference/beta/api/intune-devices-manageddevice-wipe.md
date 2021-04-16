---
title: Действие wipe
description: Очистка устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 760631b115d6a458556b476b28f6f996e259d2bd
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866624"
---
# <a name="wipe-action"></a><span data-ttu-id="b8ed8-103">Действие wipe</span><span class="sxs-lookup"><span data-stu-id="b8ed8-103">wipe action</span></span>

<span data-ttu-id="b8ed8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8ed8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8ed8-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8ed8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8ed8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8ed8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8ed8-107">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="b8ed8-107">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8ed8-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b8ed8-108">Prerequisites</span></span>
<span data-ttu-id="b8ed8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8ed8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8ed8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8ed8-111">Permission type</span></span>|<span data-ttu-id="b8ed8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8ed8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8ed8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8ed8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8ed8-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="b8ed8-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="b8ed8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8ed8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8ed8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8ed8-116">Not supported.</span></span>|
|<span data-ttu-id="b8ed8-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="b8ed8-117">Application</span></span>|<span data-ttu-id="b8ed8-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="b8ed8-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8ed8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8ed8-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b8ed8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b8ed8-120">Request headers</span></span>
|<span data-ttu-id="b8ed8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8ed8-121">Header</span></span>|<span data-ttu-id="b8ed8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b8ed8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8ed8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8ed8-123">Authorization</span></span>|<span data-ttu-id="b8ed8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8ed8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8ed8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b8ed8-125">Accept</span></span>|<span data-ttu-id="b8ed8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8ed8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8ed8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8ed8-127">Request body</span></span>
<span data-ttu-id="b8ed8-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8ed8-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b8ed8-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="b8ed8-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b8ed8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8ed8-130">Property</span></span>|<span data-ttu-id="b8ed8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b8ed8-131">Type</span></span>|<span data-ttu-id="b8ed8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b8ed8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8ed8-133">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="b8ed8-133">keepEnrollmentData</span></span>|<span data-ttu-id="b8ed8-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8ed8-134">Boolean</span></span>|<span data-ttu-id="b8ed8-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b8ed8-135">Not yet documented</span></span>|
|<span data-ttu-id="b8ed8-136">keepUserData</span><span class="sxs-lookup"><span data-stu-id="b8ed8-136">keepUserData</span></span>|<span data-ttu-id="b8ed8-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8ed8-137">Boolean</span></span>|<span data-ttu-id="b8ed8-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b8ed8-138">Not yet documented</span></span>|
|<span data-ttu-id="b8ed8-139">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="b8ed8-139">macOsUnlockCode</span></span>|<span data-ttu-id="b8ed8-140">String</span><span class="sxs-lookup"><span data-stu-id="b8ed8-140">String</span></span>|<span data-ttu-id="b8ed8-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b8ed8-141">Not yet documented</span></span>|
|<span data-ttu-id="b8ed8-142">persistEsimDataPlan</span><span class="sxs-lookup"><span data-stu-id="b8ed8-142">persistEsimDataPlan</span></span>|<span data-ttu-id="b8ed8-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8ed8-143">Boolean</span></span>|<span data-ttu-id="b8ed8-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b8ed8-144">Not yet documented</span></span>|
|<span data-ttu-id="b8ed8-145">useProtectedWipe</span><span class="sxs-lookup"><span data-stu-id="b8ed8-145">useProtectedWipe</span></span>|<span data-ttu-id="b8ed8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8ed8-146">Boolean</span></span>|<span data-ttu-id="b8ed8-147">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b8ed8-147">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b8ed8-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="b8ed8-148">Response</span></span>
<span data-ttu-id="b8ed8-149">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b8ed8-149">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b8ed8-150">Пример</span><span class="sxs-lookup"><span data-stu-id="b8ed8-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8ed8-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8ed8-151">Request</span></span>
<span data-ttu-id="b8ed8-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8ed8-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 170

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value",
  "persistEsimDataPlan": true,
  "useProtectedWipe": true
}
```

### <a name="response"></a><span data-ttu-id="b8ed8-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8ed8-153">Response</span></span>
<span data-ttu-id="b8ed8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8ed8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




