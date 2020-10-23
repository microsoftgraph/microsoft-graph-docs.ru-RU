---
title: Обновление mobileAppInstallStatus
description: Обновление свойств объекта mobileAppInstallStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 45f4aeefe5063c3c8775fe50d1ba2a1c87cc0ff2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723716"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="f1a69-103">Обновление mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="f1a69-103">Update mobileAppInstallStatus</span></span>

<span data-ttu-id="f1a69-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1a69-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1a69-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1a69-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1a69-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1a69-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1a69-107">Обновление свойств объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="f1a69-107">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1a69-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f1a69-108">Prerequisites</span></span>
<span data-ttu-id="f1a69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1a69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1a69-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1a69-111">Permission type</span></span>|<span data-ttu-id="f1a69-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1a69-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1a69-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1a69-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1a69-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1a69-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f1a69-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1a69-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1a69-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1a69-116">Not supported.</span></span>|
|<span data-ttu-id="f1a69-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1a69-117">Application</span></span>|<span data-ttu-id="f1a69-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1a69-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1a69-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1a69-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="f1a69-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f1a69-120">Request headers</span></span>
|<span data-ttu-id="f1a69-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1a69-121">Header</span></span>|<span data-ttu-id="f1a69-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f1a69-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1a69-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1a69-123">Authorization</span></span>|<span data-ttu-id="f1a69-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1a69-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1a69-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f1a69-125">Accept</span></span>|<span data-ttu-id="f1a69-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1a69-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1a69-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f1a69-127">Request body</span></span>
<span data-ttu-id="f1a69-128">В тексте запроса добавьте представление объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1a69-128">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="f1a69-129">В следующей таблице приведены свойства, необходимые при создании [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="f1a69-129">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="f1a69-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1a69-130">Property</span></span>|<span data-ttu-id="f1a69-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f1a69-131">Type</span></span>|<span data-ttu-id="f1a69-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f1a69-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1a69-133">id</span><span class="sxs-lookup"><span data-stu-id="f1a69-133">id</span></span>|<span data-ttu-id="f1a69-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f1a69-134">String</span></span>|<span data-ttu-id="f1a69-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f1a69-135">Key of the entity.</span></span>|
|<span data-ttu-id="f1a69-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="f1a69-136">deviceName</span></span>|<span data-ttu-id="f1a69-137">String</span><span class="sxs-lookup"><span data-stu-id="f1a69-137">String</span></span>|<span data-ttu-id="f1a69-138">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="f1a69-138">Device name</span></span>|
|<span data-ttu-id="f1a69-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="f1a69-139">deviceId</span></span>|<span data-ttu-id="f1a69-140">String</span><span class="sxs-lookup"><span data-stu-id="f1a69-140">String</span></span>|<span data-ttu-id="f1a69-141">ИДЕНТИФИКАТОР устройства</span><span class="sxs-lookup"><span data-stu-id="f1a69-141">Device ID</span></span>|
|<span data-ttu-id="f1a69-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f1a69-142">lastSyncDateTime</span></span>|<span data-ttu-id="f1a69-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1a69-143">DateTimeOffset</span></span>|<span data-ttu-id="f1a69-144">Дата и время последней синхронизации</span><span class="sxs-lookup"><span data-stu-id="f1a69-144">Last sync date time</span></span>|
|<span data-ttu-id="f1a69-145">Mobileappinstallstatusvalue (</span><span class="sxs-lookup"><span data-stu-id="f1a69-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="f1a69-146">ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="f1a69-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="f1a69-147">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="f1a69-147">The install state of the app.</span></span> <span data-ttu-id="f1a69-148">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="f1a69-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="f1a69-149">installState</span><span class="sxs-lookup"><span data-stu-id="f1a69-149">installState</span></span>|[<span data-ttu-id="f1a69-150">ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="f1a69-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="f1a69-151">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="f1a69-151">The install state of the app.</span></span> <span data-ttu-id="f1a69-152">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="f1a69-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="f1a69-153">инсталлстатедетаил</span><span class="sxs-lookup"><span data-stu-id="f1a69-153">installStateDetail</span></span>|[<span data-ttu-id="f1a69-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="f1a69-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="f1a69-155">Сведения о состоянии установки приложения.</span><span class="sxs-lookup"><span data-stu-id="f1a69-155">The install state detail of the app.</span></span> <span data-ttu-id="f1a69-156">Возможные значения:,,,,,,,,,,,,,,,,,, `noAdditionalDetails` `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` , `seeUninstallErrorCode` , `pendingReboot` , `installingDependencies` `contentDownloaded` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable` ,,,,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="f1a69-156">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `iosAppStoreUpdateFailedToInstall`, `vppAppHasUpdateAvailable`, `userRejectedUpdate`, `seeInstallErrorCode`, `autoInstallDisabled`, `managedAppNoLongerPresent`, `userRejectedInstall`, `userIsNotLoggedIntoAppStore`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="f1a69-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="f1a69-157">errorCode</span></span>|<span data-ttu-id="f1a69-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f1a69-158">Int32</span></span>|<span data-ttu-id="f1a69-159">Код ошибки для установки или удаления сбоев.</span><span class="sxs-lookup"><span data-stu-id="f1a69-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="f1a69-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="f1a69-160">osVersion</span></span>|<span data-ttu-id="f1a69-161">String</span><span class="sxs-lookup"><span data-stu-id="f1a69-161">String</span></span>|<span data-ttu-id="f1a69-162">Версия ОС</span><span class="sxs-lookup"><span data-stu-id="f1a69-162">OS Version</span></span>|
|<span data-ttu-id="f1a69-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="f1a69-163">osDescription</span></span>|<span data-ttu-id="f1a69-164">String</span><span class="sxs-lookup"><span data-stu-id="f1a69-164">String</span></span>|<span data-ttu-id="f1a69-165">Описание ОС</span><span class="sxs-lookup"><span data-stu-id="f1a69-165">OS Description</span></span>|
|<span data-ttu-id="f1a69-166">userName</span><span class="sxs-lookup"><span data-stu-id="f1a69-166">userName</span></span>|<span data-ttu-id="f1a69-167">String</span><span class="sxs-lookup"><span data-stu-id="f1a69-167">String</span></span>|<span data-ttu-id="f1a69-168">Имя пользователя устройства</span><span class="sxs-lookup"><span data-stu-id="f1a69-168">Device User Name</span></span>|
|<span data-ttu-id="f1a69-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f1a69-169">userPrincipalName</span></span>|<span data-ttu-id="f1a69-170">String</span><span class="sxs-lookup"><span data-stu-id="f1a69-170">String</span></span>|<span data-ttu-id="f1a69-171">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="f1a69-171">User Principal Name</span></span>|
|<span data-ttu-id="f1a69-172">дисплайверсион</span><span class="sxs-lookup"><span data-stu-id="f1a69-172">displayVersion</span></span>|<span data-ttu-id="f1a69-173">Строка</span><span class="sxs-lookup"><span data-stu-id="f1a69-173">String</span></span>|<span data-ttu-id="f1a69-174">Доступная для человека версия приложения</span><span class="sxs-lookup"><span data-stu-id="f1a69-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="f1a69-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1a69-175">Response</span></span>
<span data-ttu-id="f1a69-176">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1a69-176">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1a69-177">Пример</span><span class="sxs-lookup"><span data-stu-id="f1a69-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1a69-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1a69-178">Request</span></span>
<span data-ttu-id="f1a69-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1a69-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f1a69-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1a69-180">Response</span></span>
<span data-ttu-id="f1a69-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1a69-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





