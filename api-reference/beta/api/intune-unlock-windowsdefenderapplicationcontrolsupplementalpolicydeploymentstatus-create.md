---
title: Создание Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус
description: Создание нового объекта Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d18274b97bf06a20d96e45c2b666b1e1f6a2157
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732018"
---
# <a name="create-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"></a><span data-ttu-id="8a71b-103">Создание Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус</span><span class="sxs-lookup"><span data-stu-id="8a71b-103">Create windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span></span>

<span data-ttu-id="8a71b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a71b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a71b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a71b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a71b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8a71b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a71b-107">Создание нового объекта [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="8a71b-107">Create a new [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a71b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8a71b-108">Prerequisites</span></span>
<span data-ttu-id="8a71b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a71b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a71b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a71b-111">Permission type</span></span>|<span data-ttu-id="8a71b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a71b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a71b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a71b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a71b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a71b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8a71b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a71b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a71b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a71b-116">Not supported.</span></span>|
|<span data-ttu-id="8a71b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a71b-117">Application</span></span>|<span data-ttu-id="8a71b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a71b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a71b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a71b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="8a71b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8a71b-120">Request headers</span></span>
|<span data-ttu-id="8a71b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8a71b-121">Header</span></span>|<span data-ttu-id="8a71b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8a71b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a71b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a71b-123">Authorization</span></span>|<span data-ttu-id="8a71b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a71b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a71b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8a71b-125">Accept</span></span>|<span data-ttu-id="8a71b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a71b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a71b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8a71b-127">Request body</span></span>
<span data-ttu-id="8a71b-128">В тексте запроса добавьте представление объекта Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a71b-128">In the request body, supply a JSON representation for the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus object.</span></span>

<span data-ttu-id="8a71b-129">В следующей таблице приведены свойства, необходимые при создании Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус.</span><span class="sxs-lookup"><span data-stu-id="8a71b-129">The following table shows the properties that are required when you create the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.</span></span>

|<span data-ttu-id="8a71b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a71b-130">Property</span></span>|<span data-ttu-id="8a71b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8a71b-131">Type</span></span>|<span data-ttu-id="8a71b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8a71b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a71b-133">id</span><span class="sxs-lookup"><span data-stu-id="8a71b-133">id</span></span>|<span data-ttu-id="8a71b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8a71b-134">String</span></span>|<span data-ttu-id="8a71b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8a71b-135">Key of the entity.</span></span>|
|<span data-ttu-id="8a71b-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="8a71b-136">deviceName</span></span>|<span data-ttu-id="8a71b-137">String</span><span class="sxs-lookup"><span data-stu-id="8a71b-137">String</span></span>|<span data-ttu-id="8a71b-138">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="8a71b-138">Device name.</span></span>|
|<span data-ttu-id="8a71b-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="8a71b-139">deviceId</span></span>|<span data-ttu-id="8a71b-140">String</span><span class="sxs-lookup"><span data-stu-id="8a71b-140">String</span></span>|<span data-ttu-id="8a71b-141">ИДЕНТИФИКАТОР устройства.</span><span class="sxs-lookup"><span data-stu-id="8a71b-141">Device ID.</span></span>|
|<span data-ttu-id="8a71b-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8a71b-142">lastSyncDateTime</span></span>|<span data-ttu-id="8a71b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a71b-143">DateTimeOffset</span></span>|<span data-ttu-id="8a71b-144">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="8a71b-144">Last sync date time.</span></span>|
|<span data-ttu-id="8a71b-145">osVersion</span><span class="sxs-lookup"><span data-stu-id="8a71b-145">osVersion</span></span>|<span data-ttu-id="8a71b-146">String</span><span class="sxs-lookup"><span data-stu-id="8a71b-146">String</span></span>|<span data-ttu-id="8a71b-147">Версия ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="8a71b-147">Windows OS Version.</span></span>|
|<span data-ttu-id="8a71b-148">osDescription</span><span class="sxs-lookup"><span data-stu-id="8a71b-148">osDescription</span></span>|<span data-ttu-id="8a71b-149">String</span><span class="sxs-lookup"><span data-stu-id="8a71b-149">String</span></span>|<span data-ttu-id="8a71b-150">Описание версии ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="8a71b-150">Windows OS Version Description.</span></span>|
|<span data-ttu-id="8a71b-151">деплойментстатус</span><span class="sxs-lookup"><span data-stu-id="8a71b-151">deploymentStatus</span></span>|[<span data-ttu-id="8a71b-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span><span class="sxs-lookup"><span data-stu-id="8a71b-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span></span>](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|<span data-ttu-id="8a71b-153">Состояние развертывания политики.</span><span class="sxs-lookup"><span data-stu-id="8a71b-153">The deployment state of the policy.</span></span> <span data-ttu-id="8a71b-154">Возможные значения: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span><span class="sxs-lookup"><span data-stu-id="8a71b-154">Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span></span>|
|<span data-ttu-id="8a71b-155">userName</span><span class="sxs-lookup"><span data-stu-id="8a71b-155">userName</span></span>|<span data-ttu-id="8a71b-156">String</span><span class="sxs-lookup"><span data-stu-id="8a71b-156">String</span></span>|<span data-ttu-id="8a71b-157">Имя пользователя этого устройства.</span><span class="sxs-lookup"><span data-stu-id="8a71b-157">The name of the user of this device.</span></span>|
|<span data-ttu-id="8a71b-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8a71b-158">userPrincipalName</span></span>|<span data-ttu-id="8a71b-159">String</span><span class="sxs-lookup"><span data-stu-id="8a71b-159">String</span></span>|<span data-ttu-id="8a71b-160">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="8a71b-160">User Principal Name.</span></span>|
|<span data-ttu-id="8a71b-161">полициверсион</span><span class="sxs-lookup"><span data-stu-id="8a71b-161">policyVersion</span></span>|<span data-ttu-id="8a71b-162">Строка</span><span class="sxs-lookup"><span data-stu-id="8a71b-162">String</span></span>|<span data-ttu-id="8a71b-163">Доступная для человека версия дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="8a71b-163">Human readable version of the WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="8a71b-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a71b-164">Response</span></span>
<span data-ttu-id="8a71b-165">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8a71b-165">If successful, this method returns a `201 Created` response code and a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a71b-166">Пример</span><span class="sxs-lookup"><span data-stu-id="8a71b-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a71b-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a71b-167">Request</span></span>
<span data-ttu-id="8a71b-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a71b-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8a71b-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a71b-169">Response</span></span>
<span data-ttu-id="8a71b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a71b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





