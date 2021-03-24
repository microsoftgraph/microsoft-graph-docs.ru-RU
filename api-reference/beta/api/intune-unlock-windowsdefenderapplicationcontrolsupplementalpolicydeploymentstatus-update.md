---
title: Обновление windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus
description: Обновление свойств объекта WindowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3007947742489f11b8c5d7b5e6f3cb1caf6dcaea
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133908"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"></a><span data-ttu-id="25898-103">Обновление windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="25898-103">Update windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span></span>

<span data-ttu-id="25898-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25898-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25898-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25898-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25898-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25898-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25898-107">Обновление свойств объекта [WindowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)</span><span class="sxs-lookup"><span data-stu-id="25898-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25898-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="25898-108">Prerequisites</span></span>
<span data-ttu-id="25898-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25898-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25898-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25898-111">Permission type</span></span>|<span data-ttu-id="25898-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25898-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25898-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25898-113">Delegated (work or school account)</span></span>|<span data-ttu-id="25898-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25898-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="25898-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25898-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25898-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25898-116">Not supported.</span></span>|
|<span data-ttu-id="25898-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="25898-117">Application</span></span>|<span data-ttu-id="25898-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25898-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="25898-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25898-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="25898-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="25898-120">Request headers</span></span>
|<span data-ttu-id="25898-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25898-121">Header</span></span>|<span data-ttu-id="25898-122">Значение</span><span class="sxs-lookup"><span data-stu-id="25898-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25898-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="25898-123">Authorization</span></span>|<span data-ttu-id="25898-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25898-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25898-125">Accept</span><span class="sxs-lookup"><span data-stu-id="25898-125">Accept</span></span>|<span data-ttu-id="25898-126">application/json</span><span class="sxs-lookup"><span data-stu-id="25898-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25898-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25898-127">Request body</span></span>
<span data-ttu-id="25898-128">В корпусе запроса поставляем представление JSON для [объекта WindowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)</span><span class="sxs-lookup"><span data-stu-id="25898-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

<span data-ttu-id="25898-129">В следующей таблице показаны свойства, необходимые при создании [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)</span><span class="sxs-lookup"><span data-stu-id="25898-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md).</span></span>

|<span data-ttu-id="25898-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="25898-130">Property</span></span>|<span data-ttu-id="25898-131">Тип</span><span class="sxs-lookup"><span data-stu-id="25898-131">Type</span></span>|<span data-ttu-id="25898-132">Описание</span><span class="sxs-lookup"><span data-stu-id="25898-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25898-133">id</span><span class="sxs-lookup"><span data-stu-id="25898-133">id</span></span>|<span data-ttu-id="25898-134">Строка</span><span class="sxs-lookup"><span data-stu-id="25898-134">String</span></span>|<span data-ttu-id="25898-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="25898-135">Key of the entity.</span></span>|
|<span data-ttu-id="25898-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="25898-136">deviceName</span></span>|<span data-ttu-id="25898-137">String</span><span class="sxs-lookup"><span data-stu-id="25898-137">String</span></span>|<span data-ttu-id="25898-138">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="25898-138">Device name.</span></span>|
|<span data-ttu-id="25898-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="25898-139">deviceId</span></span>|<span data-ttu-id="25898-140">String</span><span class="sxs-lookup"><span data-stu-id="25898-140">String</span></span>|<span data-ttu-id="25898-141">ID устройства.</span><span class="sxs-lookup"><span data-stu-id="25898-141">Device ID.</span></span>|
|<span data-ttu-id="25898-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="25898-142">lastSyncDateTime</span></span>|<span data-ttu-id="25898-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25898-143">DateTimeOffset</span></span>|<span data-ttu-id="25898-144">Дата последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="25898-144">Last sync date time.</span></span>|
|<span data-ttu-id="25898-145">osVersion</span><span class="sxs-lookup"><span data-stu-id="25898-145">osVersion</span></span>|<span data-ttu-id="25898-146">String</span><span class="sxs-lookup"><span data-stu-id="25898-146">String</span></span>|<span data-ttu-id="25898-147">Windows OS Version.</span><span class="sxs-lookup"><span data-stu-id="25898-147">Windows OS Version.</span></span>|
|<span data-ttu-id="25898-148">osDescription</span><span class="sxs-lookup"><span data-stu-id="25898-148">osDescription</span></span>|<span data-ttu-id="25898-149">String</span><span class="sxs-lookup"><span data-stu-id="25898-149">String</span></span>|<span data-ttu-id="25898-150">Описание версии ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="25898-150">Windows OS Version Description.</span></span>|
|<span data-ttu-id="25898-151">deploymentStatus</span><span class="sxs-lookup"><span data-stu-id="25898-151">deploymentStatus</span></span>|[<span data-ttu-id="25898-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span><span class="sxs-lookup"><span data-stu-id="25898-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span></span>](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|<span data-ttu-id="25898-153">Состояние развертывания политики.</span><span class="sxs-lookup"><span data-stu-id="25898-153">The deployment state of the policy.</span></span> <span data-ttu-id="25898-154">Возможные значения: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span><span class="sxs-lookup"><span data-stu-id="25898-154">Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span></span>|
|<span data-ttu-id="25898-155">userName</span><span class="sxs-lookup"><span data-stu-id="25898-155">userName</span></span>|<span data-ttu-id="25898-156">String</span><span class="sxs-lookup"><span data-stu-id="25898-156">String</span></span>|<span data-ttu-id="25898-157">Имя пользователя этого устройства.</span><span class="sxs-lookup"><span data-stu-id="25898-157">The name of the user of this device.</span></span>|
|<span data-ttu-id="25898-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="25898-158">userPrincipalName</span></span>|<span data-ttu-id="25898-159">String</span><span class="sxs-lookup"><span data-stu-id="25898-159">String</span></span>|<span data-ttu-id="25898-160">Имя главного пользователя.</span><span class="sxs-lookup"><span data-stu-id="25898-160">User Principal Name.</span></span>|
|<span data-ttu-id="25898-161">policyVersion</span><span class="sxs-lookup"><span data-stu-id="25898-161">policyVersion</span></span>|<span data-ttu-id="25898-162">Строка</span><span class="sxs-lookup"><span data-stu-id="25898-162">String</span></span>|<span data-ttu-id="25898-163">Человеческая читаемая версия дополнительной политики WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="25898-163">Human readable version of the WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="25898-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="25898-164">Response</span></span>
<span data-ttu-id="25898-165">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект WindowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="25898-165">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25898-166">Пример</span><span class="sxs-lookup"><span data-stu-id="25898-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="25898-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="25898-167">Request</span></span>
<span data-ttu-id="25898-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25898-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="25898-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="25898-169">Response</span></span>
<span data-ttu-id="25898-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25898-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




