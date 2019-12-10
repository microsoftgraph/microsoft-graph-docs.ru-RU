---
title: Создание Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус
description: Создание нового объекта Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3528cc2da190464ddfd60a013440ae9cd21c9d6b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39938735"
---
# <a name="create-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"></a><span data-ttu-id="2bdb3-103">Создание Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус</span><span class="sxs-lookup"><span data-stu-id="2bdb3-103">Create windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span></span>

> <span data-ttu-id="2bdb3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bdb3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bdb3-106">Создание нового объекта [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="2bdb3-106">Create a new [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bdb3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2bdb3-107">Prerequisites</span></span>
<span data-ttu-id="2bdb3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bdb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bdb3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2bdb3-110">Permission type</span></span>|<span data-ttu-id="2bdb3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2bdb3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bdb3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2bdb3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2bdb3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bdb3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2bdb3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2bdb3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bdb3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-115">Not supported.</span></span>|
|<span data-ttu-id="2bdb3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2bdb3-116">Application</span></span>|<span data-ttu-id="2bdb3-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bdb3-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bdb3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2bdb3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="2bdb3-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2bdb3-119">Request headers</span></span>
|<span data-ttu-id="2bdb3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2bdb3-120">Header</span></span>|<span data-ttu-id="2bdb3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2bdb3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bdb3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2bdb3-122">Authorization</span></span>|<span data-ttu-id="2bdb3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bdb3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2bdb3-124">Accept</span></span>|<span data-ttu-id="2bdb3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2bdb3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bdb3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2bdb3-126">Request body</span></span>
<span data-ttu-id="2bdb3-127">В тексте запроса добавьте представление объекта Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-127">In the request body, supply a JSON representation for the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus object.</span></span>

<span data-ttu-id="2bdb3-128">В следующей таблице приведены свойства, необходимые при создании Виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-128">The following table shows the properties that are required when you create the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.</span></span>

|<span data-ttu-id="2bdb3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2bdb3-129">Property</span></span>|<span data-ttu-id="2bdb3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2bdb3-130">Type</span></span>|<span data-ttu-id="2bdb3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2bdb3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bdb3-132">id</span><span class="sxs-lookup"><span data-stu-id="2bdb3-132">id</span></span>|<span data-ttu-id="2bdb3-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2bdb3-133">String</span></span>|<span data-ttu-id="2bdb3-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-134">Key of the entity.</span></span>|
|<span data-ttu-id="2bdb3-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="2bdb3-135">deviceName</span></span>|<span data-ttu-id="2bdb3-136">String</span><span class="sxs-lookup"><span data-stu-id="2bdb3-136">String</span></span>|<span data-ttu-id="2bdb3-137">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-137">Device name.</span></span>|
|<span data-ttu-id="2bdb3-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="2bdb3-138">deviceId</span></span>|<span data-ttu-id="2bdb3-139">Строка</span><span class="sxs-lookup"><span data-stu-id="2bdb3-139">String</span></span>|<span data-ttu-id="2bdb3-140">ИДЕНТИФИКАТОР устройства.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-140">Device ID.</span></span>|
|<span data-ttu-id="2bdb3-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2bdb3-141">lastSyncDateTime</span></span>|<span data-ttu-id="2bdb3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bdb3-142">DateTimeOffset</span></span>|<span data-ttu-id="2bdb3-143">Дата и время последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-143">Last sync date time.</span></span>|
|<span data-ttu-id="2bdb3-144">osVersion</span><span class="sxs-lookup"><span data-stu-id="2bdb3-144">osVersion</span></span>|<span data-ttu-id="2bdb3-145">Строка</span><span class="sxs-lookup"><span data-stu-id="2bdb3-145">String</span></span>|<span data-ttu-id="2bdb3-146">Версия ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-146">Windows OS Version.</span></span>|
|<span data-ttu-id="2bdb3-147">osDescription</span><span class="sxs-lookup"><span data-stu-id="2bdb3-147">osDescription</span></span>|<span data-ttu-id="2bdb3-148">Строка</span><span class="sxs-lookup"><span data-stu-id="2bdb3-148">String</span></span>|<span data-ttu-id="2bdb3-149">Описание версии ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-149">Windows OS Version Description.</span></span>|
|<span data-ttu-id="2bdb3-150">деплойментстатус</span><span class="sxs-lookup"><span data-stu-id="2bdb3-150">deploymentStatus</span></span>|[<span data-ttu-id="2bdb3-151">windowsDefenderApplicationControlSupplementalPolicyStatuses</span><span class="sxs-lookup"><span data-stu-id="2bdb3-151">windowsDefenderApplicationControlSupplementalPolicyStatuses</span></span>](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|<span data-ttu-id="2bdb3-152">Состояние развертывания политики.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-152">The deployment state of the policy.</span></span> <span data-ttu-id="2bdb3-153">Возможные значения: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-153">Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span></span>|
|<span data-ttu-id="2bdb3-154">userName</span><span class="sxs-lookup"><span data-stu-id="2bdb3-154">userName</span></span>|<span data-ttu-id="2bdb3-155">String</span><span class="sxs-lookup"><span data-stu-id="2bdb3-155">String</span></span>|<span data-ttu-id="2bdb3-156">Имя пользователя этого устройства.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-156">The name of the user of this device.</span></span>|
|<span data-ttu-id="2bdb3-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2bdb3-157">userPrincipalName</span></span>|<span data-ttu-id="2bdb3-158">String</span><span class="sxs-lookup"><span data-stu-id="2bdb3-158">String</span></span>|<span data-ttu-id="2bdb3-159">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-159">User Principal Name.</span></span>|
|<span data-ttu-id="2bdb3-160">полициверсион</span><span class="sxs-lookup"><span data-stu-id="2bdb3-160">policyVersion</span></span>|<span data-ttu-id="2bdb3-161">Строка</span><span class="sxs-lookup"><span data-stu-id="2bdb3-161">String</span></span>|<span data-ttu-id="2bdb3-162">Доступная для человека версия дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-162">Human readable version of the WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="2bdb3-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="2bdb3-163">Response</span></span>
<span data-ttu-id="2bdb3-164">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсдефендераппликатионконтролсупплементалполицидеплойментстатус](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-164">If successful, this method returns a `201 Created` response code and a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bdb3-165">Пример</span><span class="sxs-lookup"><span data-stu-id="2bdb3-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bdb3-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="2bdb3-166">Request</span></span>
<span data-ttu-id="2bdb3-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2bdb3-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bdb3-168">Response</span></span>
<span data-ttu-id="2bdb3-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





