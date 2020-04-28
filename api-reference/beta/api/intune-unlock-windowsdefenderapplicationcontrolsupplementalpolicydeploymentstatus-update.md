---
title: Обновление Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус
description: Обновление свойств объекта Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e56d0aa964e341d231d7468328be32bb8c4f590f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457168"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"></a><span data-ttu-id="fcbfd-103">Обновление Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус</span><span class="sxs-lookup"><span data-stu-id="fcbfd-103">Update windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span></span>

<span data-ttu-id="fcbfd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcbfd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fcbfd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fcbfd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcbfd-107">Обновление свойств объекта [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="fcbfd-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fcbfd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fcbfd-108">Prerequisites</span></span>
<span data-ttu-id="fcbfd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcbfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcbfd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcbfd-111">Permission type</span></span>|<span data-ttu-id="fcbfd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcbfd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcbfd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcbfd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fcbfd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcbfd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fcbfd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcbfd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcbfd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-116">Not supported.</span></span>|
|<span data-ttu-id="fcbfd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcbfd-117">Application</span></span>|<span data-ttu-id="fcbfd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcbfd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcbfd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcbfd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="fcbfd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fcbfd-120">Request headers</span></span>
|<span data-ttu-id="fcbfd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fcbfd-121">Header</span></span>|<span data-ttu-id="fcbfd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fcbfd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcbfd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fcbfd-123">Authorization</span></span>|<span data-ttu-id="fcbfd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcbfd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fcbfd-125">Accept</span></span>|<span data-ttu-id="fcbfd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fcbfd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcbfd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fcbfd-127">Request body</span></span>
<span data-ttu-id="fcbfd-128">В тексте запроса добавьте представление объекта [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

<span data-ttu-id="fcbfd-129">В следующей таблице приведены свойства, необходимые при создании [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md).</span><span class="sxs-lookup"><span data-stu-id="fcbfd-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md).</span></span>

|<span data-ttu-id="fcbfd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcbfd-130">Property</span></span>|<span data-ttu-id="fcbfd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fcbfd-131">Type</span></span>|<span data-ttu-id="fcbfd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fcbfd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcbfd-133">id</span><span class="sxs-lookup"><span data-stu-id="fcbfd-133">id</span></span>|<span data-ttu-id="fcbfd-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fcbfd-134">String</span></span>|<span data-ttu-id="fcbfd-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-135">Key of the entity.</span></span>|
|<span data-ttu-id="fcbfd-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="fcbfd-136">deviceName</span></span>|<span data-ttu-id="fcbfd-137">String</span><span class="sxs-lookup"><span data-stu-id="fcbfd-137">String</span></span>|<span data-ttu-id="fcbfd-138">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-138">Device name.</span></span>|
|<span data-ttu-id="fcbfd-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="fcbfd-139">deviceId</span></span>|<span data-ttu-id="fcbfd-140">String</span><span class="sxs-lookup"><span data-stu-id="fcbfd-140">String</span></span>|<span data-ttu-id="fcbfd-141">ИДЕНТИФИКАТОР устройства.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-141">Device ID.</span></span>|
|<span data-ttu-id="fcbfd-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="fcbfd-142">lastSyncDateTime</span></span>|<span data-ttu-id="fcbfd-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcbfd-143">DateTimeOffset</span></span>|<span data-ttu-id="fcbfd-144">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-144">Last sync date time.</span></span>|
|<span data-ttu-id="fcbfd-145">osVersion</span><span class="sxs-lookup"><span data-stu-id="fcbfd-145">osVersion</span></span>|<span data-ttu-id="fcbfd-146">String</span><span class="sxs-lookup"><span data-stu-id="fcbfd-146">String</span></span>|<span data-ttu-id="fcbfd-147">Версия ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-147">Windows OS Version.</span></span>|
|<span data-ttu-id="fcbfd-148">osDescription</span><span class="sxs-lookup"><span data-stu-id="fcbfd-148">osDescription</span></span>|<span data-ttu-id="fcbfd-149">String</span><span class="sxs-lookup"><span data-stu-id="fcbfd-149">String</span></span>|<span data-ttu-id="fcbfd-150">Описание версии ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-150">Windows OS Version Description.</span></span>|
|<span data-ttu-id="fcbfd-151">деплойментстатус</span><span class="sxs-lookup"><span data-stu-id="fcbfd-151">deploymentStatus</span></span>|[<span data-ttu-id="fcbfd-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span><span class="sxs-lookup"><span data-stu-id="fcbfd-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span></span>](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|<span data-ttu-id="fcbfd-153">Состояние развертывания политики.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-153">The deployment state of the policy.</span></span> <span data-ttu-id="fcbfd-154">Возможные значения: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-154">Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span></span>|
|<span data-ttu-id="fcbfd-155">userName</span><span class="sxs-lookup"><span data-stu-id="fcbfd-155">userName</span></span>|<span data-ttu-id="fcbfd-156">String</span><span class="sxs-lookup"><span data-stu-id="fcbfd-156">String</span></span>|<span data-ttu-id="fcbfd-157">Имя пользователя этого устройства.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-157">The name of the user of this device.</span></span>|
|<span data-ttu-id="fcbfd-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fcbfd-158">userPrincipalName</span></span>|<span data-ttu-id="fcbfd-159">String</span><span class="sxs-lookup"><span data-stu-id="fcbfd-159">String</span></span>|<span data-ttu-id="fcbfd-160">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-160">User Principal Name.</span></span>|
|<span data-ttu-id="fcbfd-161">полициверсион</span><span class="sxs-lookup"><span data-stu-id="fcbfd-161">policyVersion</span></span>|<span data-ttu-id="fcbfd-162">String</span><span class="sxs-lookup"><span data-stu-id="fcbfd-162">String</span></span>|<span data-ttu-id="fcbfd-163">Доступная для человека версия дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-163">Human readable version of the WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="fcbfd-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="fcbfd-164">Response</span></span>
<span data-ttu-id="fcbfd-165">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-165">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcbfd-166">Пример</span><span class="sxs-lookup"><span data-stu-id="fcbfd-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcbfd-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcbfd-167">Request</span></span>
<span data-ttu-id="fcbfd-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}
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

### <a name="response"></a><span data-ttu-id="fcbfd-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcbfd-169">Response</span></span>
<span data-ttu-id="fcbfd-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fcbfd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



