---
title: Обновление mobileAppInstallStatus
description: Обновление свойств объекта mobileAppInstallStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: edc76c98d48c9aa9ba2eb2d10f99b83e1a144038
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143159"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="13d4c-103">Обновление mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="13d4c-103">Update mobileAppInstallStatus</span></span>

<span data-ttu-id="13d4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13d4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13d4c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13d4c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13d4c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13d4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13d4c-107">Обновление свойств объекта [mobileAppInstallStatus.](../resources/intune-apps-mobileappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="13d4c-107">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13d4c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="13d4c-108">Prerequisites</span></span>
<span data-ttu-id="13d4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13d4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13d4c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13d4c-111">Permission type</span></span>|<span data-ttu-id="13d4c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13d4c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13d4c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13d4c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13d4c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13d4c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="13d4c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13d4c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13d4c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13d4c-116">Not supported.</span></span>|
|<span data-ttu-id="13d4c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="13d4c-117">Application</span></span>|<span data-ttu-id="13d4c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13d4c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13d4c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13d4c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="13d4c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="13d4c-120">Request headers</span></span>
|<span data-ttu-id="13d4c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13d4c-121">Header</span></span>|<span data-ttu-id="13d4c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="13d4c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13d4c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="13d4c-123">Authorization</span></span>|<span data-ttu-id="13d4c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13d4c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13d4c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="13d4c-125">Accept</span></span>|<span data-ttu-id="13d4c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13d4c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13d4c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13d4c-127">Request body</span></span>
<span data-ttu-id="13d4c-128">В теле запроса устрой представление JSON для [объекта mobileAppInstallStatus.](../resources/intune-apps-mobileappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="13d4c-128">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="13d4c-129">В следующей таблице показаны свойства, необходимые при создании [mobileAppInstallStatus.](../resources/intune-apps-mobileappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="13d4c-129">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="13d4c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="13d4c-130">Property</span></span>|<span data-ttu-id="13d4c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="13d4c-131">Type</span></span>|<span data-ttu-id="13d4c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="13d4c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13d4c-133">id</span><span class="sxs-lookup"><span data-stu-id="13d4c-133">id</span></span>|<span data-ttu-id="13d4c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="13d4c-134">String</span></span>|<span data-ttu-id="13d4c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="13d4c-135">Key of the entity.</span></span>|
|<span data-ttu-id="13d4c-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="13d4c-136">deviceName</span></span>|<span data-ttu-id="13d4c-137">String</span><span class="sxs-lookup"><span data-stu-id="13d4c-137">String</span></span>|<span data-ttu-id="13d4c-138">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="13d4c-138">Device name</span></span>|
|<span data-ttu-id="13d4c-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="13d4c-139">deviceId</span></span>|<span data-ttu-id="13d4c-140">String</span><span class="sxs-lookup"><span data-stu-id="13d4c-140">String</span></span>|<span data-ttu-id="13d4c-141">ID устройства</span><span class="sxs-lookup"><span data-stu-id="13d4c-141">Device ID</span></span>|
|<span data-ttu-id="13d4c-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="13d4c-142">lastSyncDateTime</span></span>|<span data-ttu-id="13d4c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13d4c-143">DateTimeOffset</span></span>|<span data-ttu-id="13d4c-144">Время последней даты синхронизации</span><span class="sxs-lookup"><span data-stu-id="13d4c-144">Last sync date time</span></span>|
|<span data-ttu-id="13d4c-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="13d4c-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="13d4c-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="13d4c-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="13d4c-147">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="13d4c-147">The install state of the app.</span></span> <span data-ttu-id="13d4c-148">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="13d4c-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="13d4c-149">installState</span><span class="sxs-lookup"><span data-stu-id="13d4c-149">installState</span></span>|[<span data-ttu-id="13d4c-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="13d4c-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="13d4c-151">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="13d4c-151">The install state of the app.</span></span> <span data-ttu-id="13d4c-152">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="13d4c-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="13d4c-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="13d4c-153">installStateDetail</span></span>|[<span data-ttu-id="13d4c-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="13d4c-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="13d4c-155">Деталь состояния установки приложения.</span><span class="sxs-lookup"><span data-stu-id="13d4c-155">The install state detail of the app.</span></span> <span data-ttu-id="13d4c-156">Возможные значения: `noAdditionalDetails` `dependencyFailedToInstall` , `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `contentDownloaded` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` , `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable` , .</span><span class="sxs-lookup"><span data-stu-id="13d4c-156">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `iosAppStoreUpdateFailedToInstall`, `vppAppHasUpdateAvailable`, `userRejectedUpdate`, `seeInstallErrorCode`, `autoInstallDisabled`, `managedAppNoLongerPresent`, `userRejectedInstall`, `userIsNotLoggedIntoAppStore`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="13d4c-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="13d4c-157">errorCode</span></span>|<span data-ttu-id="13d4c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="13d4c-158">Int32</span></span>|<span data-ttu-id="13d4c-159">Код ошибки для установки или отказа от сбоев.</span><span class="sxs-lookup"><span data-stu-id="13d4c-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="13d4c-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="13d4c-160">osVersion</span></span>|<span data-ttu-id="13d4c-161">String</span><span class="sxs-lookup"><span data-stu-id="13d4c-161">String</span></span>|<span data-ttu-id="13d4c-162">ВЕРСИЯ ОС</span><span class="sxs-lookup"><span data-stu-id="13d4c-162">OS Version</span></span>|
|<span data-ttu-id="13d4c-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="13d4c-163">osDescription</span></span>|<span data-ttu-id="13d4c-164">String</span><span class="sxs-lookup"><span data-stu-id="13d4c-164">String</span></span>|<span data-ttu-id="13d4c-165">Описание ОС</span><span class="sxs-lookup"><span data-stu-id="13d4c-165">OS Description</span></span>|
|<span data-ttu-id="13d4c-166">userName</span><span class="sxs-lookup"><span data-stu-id="13d4c-166">userName</span></span>|<span data-ttu-id="13d4c-167">String</span><span class="sxs-lookup"><span data-stu-id="13d4c-167">String</span></span>|<span data-ttu-id="13d4c-168">Имя пользователя устройства</span><span class="sxs-lookup"><span data-stu-id="13d4c-168">Device User Name</span></span>|
|<span data-ttu-id="13d4c-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="13d4c-169">userPrincipalName</span></span>|<span data-ttu-id="13d4c-170">String</span><span class="sxs-lookup"><span data-stu-id="13d4c-170">String</span></span>|<span data-ttu-id="13d4c-171">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="13d4c-171">User Principal Name</span></span>|
|<span data-ttu-id="13d4c-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="13d4c-172">displayVersion</span></span>|<span data-ttu-id="13d4c-173">Строка</span><span class="sxs-lookup"><span data-stu-id="13d4c-173">String</span></span>|<span data-ttu-id="13d4c-174">Читаемая для человека версия приложения</span><span class="sxs-lookup"><span data-stu-id="13d4c-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="13d4c-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="13d4c-175">Response</span></span>
<span data-ttu-id="13d4c-176">В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="13d4c-176">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13d4c-177">Пример</span><span class="sxs-lookup"><span data-stu-id="13d4c-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="13d4c-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="13d4c-178">Request</span></span>
<span data-ttu-id="13d4c-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13d4c-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="13d4c-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="13d4c-180">Response</span></span>
<span data-ttu-id="13d4c-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13d4c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




