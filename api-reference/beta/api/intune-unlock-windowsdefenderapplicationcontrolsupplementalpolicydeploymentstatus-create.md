---
title: Создание Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус
description: Создание нового объекта Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6b352ff29bc3c05ef6cff49f4849dde5ce953d97
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799796"
---
# <a name="create-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"></a><span data-ttu-id="7da1d-103">Создание Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус</span><span class="sxs-lookup"><span data-stu-id="7da1d-103">Create windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span></span>

> <span data-ttu-id="7da1d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7da1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7da1d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7da1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7da1d-106">Создание нового объекта [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="7da1d-106">Create a new [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7da1d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7da1d-107">Prerequisites</span></span>
<span data-ttu-id="7da1d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7da1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7da1d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7da1d-110">Permission type</span></span>|<span data-ttu-id="7da1d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7da1d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7da1d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7da1d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7da1d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7da1d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7da1d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7da1d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7da1d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7da1d-115">Not supported.</span></span>|
|<span data-ttu-id="7da1d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7da1d-116">Application</span></span>|<span data-ttu-id="7da1d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7da1d-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7da1d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7da1d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="7da1d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7da1d-119">Request headers</span></span>
|<span data-ttu-id="7da1d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7da1d-120">Header</span></span>|<span data-ttu-id="7da1d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7da1d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7da1d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7da1d-122">Authorization</span></span>|<span data-ttu-id="7da1d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7da1d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7da1d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7da1d-124">Accept</span></span>|<span data-ttu-id="7da1d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7da1d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7da1d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7da1d-126">Request body</span></span>
<span data-ttu-id="7da1d-127">В тексте запроса добавьте представление объекта Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7da1d-127">In the request body, supply a JSON representation for the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus object.</span></span>

<span data-ttu-id="7da1d-128">В следующей таблице приведены свойства, необходимые при создании Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус.</span><span class="sxs-lookup"><span data-stu-id="7da1d-128">The following table shows the properties that are required when you create the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.</span></span>

|<span data-ttu-id="7da1d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7da1d-129">Property</span></span>|<span data-ttu-id="7da1d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7da1d-130">Type</span></span>|<span data-ttu-id="7da1d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7da1d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7da1d-132">id</span><span class="sxs-lookup"><span data-stu-id="7da1d-132">id</span></span>|<span data-ttu-id="7da1d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="7da1d-133">String</span></span>|<span data-ttu-id="7da1d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7da1d-134">Key of the entity.</span></span>|
|<span data-ttu-id="7da1d-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="7da1d-135">deviceName</span></span>|<span data-ttu-id="7da1d-136">String</span><span class="sxs-lookup"><span data-stu-id="7da1d-136">String</span></span>|<span data-ttu-id="7da1d-137">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="7da1d-137">Device name.</span></span>|
|<span data-ttu-id="7da1d-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="7da1d-138">deviceId</span></span>|<span data-ttu-id="7da1d-139">String</span><span class="sxs-lookup"><span data-stu-id="7da1d-139">String</span></span>|<span data-ttu-id="7da1d-140">ИДЕНТИФИКАТОР устройства.</span><span class="sxs-lookup"><span data-stu-id="7da1d-140">Device ID.</span></span>|
|<span data-ttu-id="7da1d-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7da1d-141">lastSyncDateTime</span></span>|<span data-ttu-id="7da1d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7da1d-142">DateTimeOffset</span></span>|<span data-ttu-id="7da1d-143">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="7da1d-143">Last sync date time.</span></span>|
|<span data-ttu-id="7da1d-144">osVersion</span><span class="sxs-lookup"><span data-stu-id="7da1d-144">osVersion</span></span>|<span data-ttu-id="7da1d-145">String</span><span class="sxs-lookup"><span data-stu-id="7da1d-145">String</span></span>|<span data-ttu-id="7da1d-146">Версия ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="7da1d-146">Windows OS Version.</span></span>|
|<span data-ttu-id="7da1d-147">osDescription</span><span class="sxs-lookup"><span data-stu-id="7da1d-147">osDescription</span></span>|<span data-ttu-id="7da1d-148">String</span><span class="sxs-lookup"><span data-stu-id="7da1d-148">String</span></span>|<span data-ttu-id="7da1d-149">Описание версии ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="7da1d-149">Windows OS Version Description.</span></span>|
|<span data-ttu-id="7da1d-150">деплойментстатус</span><span class="sxs-lookup"><span data-stu-id="7da1d-150">deploymentStatus</span></span>|[<span data-ttu-id="7da1d-151">windowsDefenderApplicationControlSupplementalPolicyStatuses</span><span class="sxs-lookup"><span data-stu-id="7da1d-151">windowsDefenderApplicationControlSupplementalPolicyStatuses</span></span>](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|<span data-ttu-id="7da1d-152">Состояние развертывания политики.</span><span class="sxs-lookup"><span data-stu-id="7da1d-152">The deployment state of the policy.</span></span> <span data-ttu-id="7da1d-153">Возможные значения: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span><span class="sxs-lookup"><span data-stu-id="7da1d-153">Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span></span>|
|<span data-ttu-id="7da1d-154">userName</span><span class="sxs-lookup"><span data-stu-id="7da1d-154">userName</span></span>|<span data-ttu-id="7da1d-155">String</span><span class="sxs-lookup"><span data-stu-id="7da1d-155">String</span></span>|<span data-ttu-id="7da1d-156">Имя пользователя этого устройства.</span><span class="sxs-lookup"><span data-stu-id="7da1d-156">The name of the user of this device.</span></span>|
|<span data-ttu-id="7da1d-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7da1d-157">userPrincipalName</span></span>|<span data-ttu-id="7da1d-158">String</span><span class="sxs-lookup"><span data-stu-id="7da1d-158">String</span></span>|<span data-ttu-id="7da1d-159">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="7da1d-159">User Principal Name.</span></span>|
|<span data-ttu-id="7da1d-160">полициверсион</span><span class="sxs-lookup"><span data-stu-id="7da1d-160">policyVersion</span></span>|<span data-ttu-id="7da1d-161">String</span><span class="sxs-lookup"><span data-stu-id="7da1d-161">String</span></span>|<span data-ttu-id="7da1d-162">Доступная для человека версия дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="7da1d-162">Human readable version of the WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="7da1d-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="7da1d-163">Response</span></span>
<span data-ttu-id="7da1d-164">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7da1d-164">If successful, this method returns a `201 Created` response code and a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7da1d-165">Пример</span><span class="sxs-lookup"><span data-stu-id="7da1d-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="7da1d-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="7da1d-166">Request</span></span>
<span data-ttu-id="7da1d-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7da1d-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7da1d-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="7da1d-168">Response</span></span>
<span data-ttu-id="7da1d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7da1d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




