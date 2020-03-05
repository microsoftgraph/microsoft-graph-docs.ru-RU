---
title: Создание Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус
description: Создание нового объекта Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4ef710116ed829876a8dcfea99be472fbd11da4c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457519"
---
# <a name="create-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"></a><span data-ttu-id="0a547-103">Создание Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус</span><span class="sxs-lookup"><span data-stu-id="0a547-103">Create windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span></span>

<span data-ttu-id="0a547-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0a547-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a547-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a547-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a547-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a547-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a547-107">Создание нового объекта [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="0a547-107">Create a new [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a547-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0a547-108">Prerequisites</span></span>
<span data-ttu-id="0a547-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a547-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a547-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a547-111">Permission type</span></span>|<span data-ttu-id="0a547-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a547-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a547-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a547-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a547-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a547-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0a547-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a547-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a547-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a547-116">Not supported.</span></span>|
|<span data-ttu-id="0a547-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a547-117">Application</span></span>|<span data-ttu-id="0a547-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a547-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a547-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a547-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="0a547-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0a547-120">Request headers</span></span>
|<span data-ttu-id="0a547-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a547-121">Header</span></span>|<span data-ttu-id="0a547-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0a547-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a547-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a547-123">Authorization</span></span>|<span data-ttu-id="0a547-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a547-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a547-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0a547-125">Accept</span></span>|<span data-ttu-id="0a547-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a547-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a547-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a547-127">Request body</span></span>
<span data-ttu-id="0a547-128">В тексте запроса добавьте представление объекта Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a547-128">In the request body, supply a JSON representation for the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus object.</span></span>

<span data-ttu-id="0a547-129">В следующей таблице приведены свойства, необходимые при создании Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус.</span><span class="sxs-lookup"><span data-stu-id="0a547-129">The following table shows the properties that are required when you create the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.</span></span>

|<span data-ttu-id="0a547-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a547-130">Property</span></span>|<span data-ttu-id="0a547-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0a547-131">Type</span></span>|<span data-ttu-id="0a547-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0a547-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a547-133">id</span><span class="sxs-lookup"><span data-stu-id="0a547-133">id</span></span>|<span data-ttu-id="0a547-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0a547-134">String</span></span>|<span data-ttu-id="0a547-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0a547-135">Key of the entity.</span></span>|
|<span data-ttu-id="0a547-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="0a547-136">deviceName</span></span>|<span data-ttu-id="0a547-137">String</span><span class="sxs-lookup"><span data-stu-id="0a547-137">String</span></span>|<span data-ttu-id="0a547-138">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="0a547-138">Device name.</span></span>|
|<span data-ttu-id="0a547-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="0a547-139">deviceId</span></span>|<span data-ttu-id="0a547-140">String</span><span class="sxs-lookup"><span data-stu-id="0a547-140">String</span></span>|<span data-ttu-id="0a547-141">ИДЕНТИФИКАТОР устройства.</span><span class="sxs-lookup"><span data-stu-id="0a547-141">Device ID.</span></span>|
|<span data-ttu-id="0a547-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0a547-142">lastSyncDateTime</span></span>|<span data-ttu-id="0a547-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a547-143">DateTimeOffset</span></span>|<span data-ttu-id="0a547-144">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="0a547-144">Last sync date time.</span></span>|
|<span data-ttu-id="0a547-145">osVersion</span><span class="sxs-lookup"><span data-stu-id="0a547-145">osVersion</span></span>|<span data-ttu-id="0a547-146">String</span><span class="sxs-lookup"><span data-stu-id="0a547-146">String</span></span>|<span data-ttu-id="0a547-147">Версия ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="0a547-147">Windows OS Version.</span></span>|
|<span data-ttu-id="0a547-148">osDescription</span><span class="sxs-lookup"><span data-stu-id="0a547-148">osDescription</span></span>|<span data-ttu-id="0a547-149">String</span><span class="sxs-lookup"><span data-stu-id="0a547-149">String</span></span>|<span data-ttu-id="0a547-150">Описание версии ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="0a547-150">Windows OS Version Description.</span></span>|
|<span data-ttu-id="0a547-151">деплойментстатус</span><span class="sxs-lookup"><span data-stu-id="0a547-151">deploymentStatus</span></span>|[<span data-ttu-id="0a547-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span><span class="sxs-lookup"><span data-stu-id="0a547-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span></span>](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|<span data-ttu-id="0a547-153">Состояние развертывания политики.</span><span class="sxs-lookup"><span data-stu-id="0a547-153">The deployment state of the policy.</span></span> <span data-ttu-id="0a547-154">Возможные значения: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span><span class="sxs-lookup"><span data-stu-id="0a547-154">Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span></span>|
|<span data-ttu-id="0a547-155">userName</span><span class="sxs-lookup"><span data-stu-id="0a547-155">userName</span></span>|<span data-ttu-id="0a547-156">String</span><span class="sxs-lookup"><span data-stu-id="0a547-156">String</span></span>|<span data-ttu-id="0a547-157">Имя пользователя этого устройства.</span><span class="sxs-lookup"><span data-stu-id="0a547-157">The name of the user of this device.</span></span>|
|<span data-ttu-id="0a547-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0a547-158">userPrincipalName</span></span>|<span data-ttu-id="0a547-159">String</span><span class="sxs-lookup"><span data-stu-id="0a547-159">String</span></span>|<span data-ttu-id="0a547-160">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="0a547-160">User Principal Name.</span></span>|
|<span data-ttu-id="0a547-161">полициверсион</span><span class="sxs-lookup"><span data-stu-id="0a547-161">policyVersion</span></span>|<span data-ttu-id="0a547-162">String</span><span class="sxs-lookup"><span data-stu-id="0a547-162">String</span></span>|<span data-ttu-id="0a547-163">Доступная для человека версия дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="0a547-163">Human readable version of the WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="0a547-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a547-164">Response</span></span>
<span data-ttu-id="0a547-165">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0a547-165">If successful, this method returns a `201 Created` response code and a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a547-166">Пример</span><span class="sxs-lookup"><span data-stu-id="0a547-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a547-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a547-167">Request</span></span>
<span data-ttu-id="0a547-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a547-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses
Content-type: application/json
Content-length: 486

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "deploymentStatus": "success",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "policyVersion": "Policy Version value"
}
```

### <a name="response"></a><span data-ttu-id="0a547-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a547-169">Response</span></span>
<span data-ttu-id="0a547-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a547-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 535

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus",
  "id": "e3c01841-1841-e3c0-4118-c0e34118c0e3",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "deploymentStatus": "success",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "policyVersion": "Policy Version value"
}
```





