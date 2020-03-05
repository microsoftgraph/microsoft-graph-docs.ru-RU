---
title: Обновление mobileAppInstallStatus
description: Обновление свойств объекта mobileAppInstallStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 19a1c0e28abbdd43c7acc84e470fcf047e5d61b9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450694"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="9543f-103">Обновление mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="9543f-103">Update mobileAppInstallStatus</span></span>

<span data-ttu-id="9543f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9543f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9543f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9543f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9543f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9543f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9543f-107">Обновление свойств объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="9543f-107">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9543f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9543f-108">Prerequisites</span></span>
<span data-ttu-id="9543f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9543f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9543f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9543f-111">Permission type</span></span>|<span data-ttu-id="9543f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9543f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9543f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9543f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9543f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9543f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9543f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9543f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9543f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9543f-116">Not supported.</span></span>|
|<span data-ttu-id="9543f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9543f-117">Application</span></span>|<span data-ttu-id="9543f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9543f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9543f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9543f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="9543f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9543f-120">Request headers</span></span>
|<span data-ttu-id="9543f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9543f-121">Header</span></span>|<span data-ttu-id="9543f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9543f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9543f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9543f-123">Authorization</span></span>|<span data-ttu-id="9543f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9543f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9543f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9543f-125">Accept</span></span>|<span data-ttu-id="9543f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9543f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9543f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9543f-127">Request body</span></span>
<span data-ttu-id="9543f-128">В тексте запроса добавьте представление объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9543f-128">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="9543f-129">В следующей таблице приведены свойства, необходимые при создании [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="9543f-129">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="9543f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9543f-130">Property</span></span>|<span data-ttu-id="9543f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9543f-131">Type</span></span>|<span data-ttu-id="9543f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9543f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9543f-133">id</span><span class="sxs-lookup"><span data-stu-id="9543f-133">id</span></span>|<span data-ttu-id="9543f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9543f-134">String</span></span>|<span data-ttu-id="9543f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9543f-135">Key of the entity.</span></span>|
|<span data-ttu-id="9543f-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="9543f-136">deviceName</span></span>|<span data-ttu-id="9543f-137">String</span><span class="sxs-lookup"><span data-stu-id="9543f-137">String</span></span>|<span data-ttu-id="9543f-138">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="9543f-138">Device name</span></span>|
|<span data-ttu-id="9543f-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="9543f-139">deviceId</span></span>|<span data-ttu-id="9543f-140">String</span><span class="sxs-lookup"><span data-stu-id="9543f-140">String</span></span>|<span data-ttu-id="9543f-141">ИДЕНТИФИКАТОР устройства</span><span class="sxs-lookup"><span data-stu-id="9543f-141">Device ID</span></span>|
|<span data-ttu-id="9543f-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9543f-142">lastSyncDateTime</span></span>|<span data-ttu-id="9543f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9543f-143">DateTimeOffset</span></span>|<span data-ttu-id="9543f-144">Дата и время последней синхронизации</span><span class="sxs-lookup"><span data-stu-id="9543f-144">Last sync date time</span></span>|
|<span data-ttu-id="9543f-145">Mobileappinstallstatusvalue (</span><span class="sxs-lookup"><span data-stu-id="9543f-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="9543f-146">ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="9543f-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="9543f-147">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="9543f-147">The install state of the app.</span></span> <span data-ttu-id="9543f-148">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="9543f-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="9543f-149">installState</span><span class="sxs-lookup"><span data-stu-id="9543f-149">installState</span></span>|[<span data-ttu-id="9543f-150">ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="9543f-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="9543f-151">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="9543f-151">The install state of the app.</span></span> <span data-ttu-id="9543f-152">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="9543f-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="9543f-153">инсталлстатедетаил</span><span class="sxs-lookup"><span data-stu-id="9543f-153">installStateDetail</span></span>|[<span data-ttu-id="9543f-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="9543f-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="9543f-155">Сведения о состоянии установки приложения.</span><span class="sxs-lookup"><span data-stu-id="9543f-155">The install state detail of the app.</span></span> <span data-ttu-id="9543f-156">Возможные значения: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="9543f-156">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="9543f-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="9543f-157">errorCode</span></span>|<span data-ttu-id="9543f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="9543f-158">Int32</span></span>|<span data-ttu-id="9543f-159">Код ошибки для установки или удаления сбоев.</span><span class="sxs-lookup"><span data-stu-id="9543f-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="9543f-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="9543f-160">osVersion</span></span>|<span data-ttu-id="9543f-161">String</span><span class="sxs-lookup"><span data-stu-id="9543f-161">String</span></span>|<span data-ttu-id="9543f-162">Версия ОС</span><span class="sxs-lookup"><span data-stu-id="9543f-162">OS Version</span></span>|
|<span data-ttu-id="9543f-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="9543f-163">osDescription</span></span>|<span data-ttu-id="9543f-164">String</span><span class="sxs-lookup"><span data-stu-id="9543f-164">String</span></span>|<span data-ttu-id="9543f-165">Описание ОС</span><span class="sxs-lookup"><span data-stu-id="9543f-165">OS Description</span></span>|
|<span data-ttu-id="9543f-166">userName</span><span class="sxs-lookup"><span data-stu-id="9543f-166">userName</span></span>|<span data-ttu-id="9543f-167">String</span><span class="sxs-lookup"><span data-stu-id="9543f-167">String</span></span>|<span data-ttu-id="9543f-168">Имя пользователя устройства</span><span class="sxs-lookup"><span data-stu-id="9543f-168">Device User Name</span></span>|
|<span data-ttu-id="9543f-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9543f-169">userPrincipalName</span></span>|<span data-ttu-id="9543f-170">String</span><span class="sxs-lookup"><span data-stu-id="9543f-170">String</span></span>|<span data-ttu-id="9543f-171">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="9543f-171">User Principal Name</span></span>|
|<span data-ttu-id="9543f-172">дисплайверсион</span><span class="sxs-lookup"><span data-stu-id="9543f-172">displayVersion</span></span>|<span data-ttu-id="9543f-173">String</span><span class="sxs-lookup"><span data-stu-id="9543f-173">String</span></span>|<span data-ttu-id="9543f-174">Доступная для человека версия приложения</span><span class="sxs-lookup"><span data-stu-id="9543f-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="9543f-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="9543f-175">Response</span></span>
<span data-ttu-id="9543f-176">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9543f-176">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9543f-177">Пример</span><span class="sxs-lookup"><span data-stu-id="9543f-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="9543f-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="9543f-178">Request</span></span>
<span data-ttu-id="9543f-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9543f-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
Content-type: application/json
Content-length: 555

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "dependencyFailedToInstall",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```

### <a name="response"></a><span data-ttu-id="9543f-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="9543f-180">Response</span></span>
<span data-ttu-id="9543f-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9543f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 604

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "7560ee45-ee45-7560-45ee-607545ee6075",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "dependencyFailedToInstall",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```





