---
title: Создание mobileAppInstallStatus
description: Создание нового объекта mobileAppInstallStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f669f346ffca1a5bb1d37186efd539318fb1ef18
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693705"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="c5091-103">Создание mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="c5091-103">Create mobileAppInstallStatus</span></span>

<span data-ttu-id="c5091-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5091-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5091-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5091-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5091-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5091-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5091-107">Создание нового объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="c5091-107">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5091-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c5091-108">Prerequisites</span></span>
<span data-ttu-id="c5091-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5091-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5091-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5091-111">Permission type</span></span>|<span data-ttu-id="c5091-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5091-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5091-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5091-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5091-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5091-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c5091-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5091-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5091-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5091-116">Not supported.</span></span>|
|<span data-ttu-id="c5091-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5091-117">Application</span></span>|<span data-ttu-id="c5091-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5091-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5091-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5091-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="c5091-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c5091-120">Request headers</span></span>
|<span data-ttu-id="c5091-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5091-121">Header</span></span>|<span data-ttu-id="c5091-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c5091-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5091-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5091-123">Authorization</span></span>|<span data-ttu-id="c5091-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5091-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5091-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c5091-125">Accept</span></span>|<span data-ttu-id="c5091-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5091-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5091-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c5091-127">Request body</span></span>
<span data-ttu-id="c5091-128">В тексте запроса добавьте представление объекта mobileAppInstallStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5091-128">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="c5091-129">В следующей таблице приведены свойства, необходимые при создании mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="c5091-129">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="c5091-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5091-130">Property</span></span>|<span data-ttu-id="c5091-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c5091-131">Type</span></span>|<span data-ttu-id="c5091-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c5091-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5091-133">id</span><span class="sxs-lookup"><span data-stu-id="c5091-133">id</span></span>|<span data-ttu-id="c5091-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c5091-134">String</span></span>|<span data-ttu-id="c5091-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c5091-135">Key of the entity.</span></span>|
|<span data-ttu-id="c5091-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="c5091-136">deviceName</span></span>|<span data-ttu-id="c5091-137">String</span><span class="sxs-lookup"><span data-stu-id="c5091-137">String</span></span>|<span data-ttu-id="c5091-138">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="c5091-138">Device name</span></span>|
|<span data-ttu-id="c5091-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="c5091-139">deviceId</span></span>|<span data-ttu-id="c5091-140">String</span><span class="sxs-lookup"><span data-stu-id="c5091-140">String</span></span>|<span data-ttu-id="c5091-141">ИДЕНТИФИКАТОР устройства</span><span class="sxs-lookup"><span data-stu-id="c5091-141">Device ID</span></span>|
|<span data-ttu-id="c5091-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c5091-142">lastSyncDateTime</span></span>|<span data-ttu-id="c5091-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5091-143">DateTimeOffset</span></span>|<span data-ttu-id="c5091-144">Дата и время последней синхронизации</span><span class="sxs-lookup"><span data-stu-id="c5091-144">Last sync date time</span></span>|
|<span data-ttu-id="c5091-145">Mobileappinstallstatusvalue (</span><span class="sxs-lookup"><span data-stu-id="c5091-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="c5091-146">ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="c5091-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="c5091-147">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="c5091-147">The install state of the app.</span></span> <span data-ttu-id="c5091-148">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="c5091-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="c5091-149">installState</span><span class="sxs-lookup"><span data-stu-id="c5091-149">installState</span></span>|[<span data-ttu-id="c5091-150">ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="c5091-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="c5091-151">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="c5091-151">The install state of the app.</span></span> <span data-ttu-id="c5091-152">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="c5091-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="c5091-153">инсталлстатедетаил</span><span class="sxs-lookup"><span data-stu-id="c5091-153">installStateDetail</span></span>|[<span data-ttu-id="c5091-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="c5091-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="c5091-155">Сведения о состоянии установки приложения.</span><span class="sxs-lookup"><span data-stu-id="c5091-155">The install state detail of the app.</span></span> <span data-ttu-id="c5091-156">Возможные значения:,,,,,,,,,,,,,,,,,, `noAdditionalDetails` `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` , `seeUninstallErrorCode` , `pendingReboot` , `installingDependencies` `contentDownloaded` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable` ,,,,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="c5091-156">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `iosAppStoreUpdateFailedToInstall`, `vppAppHasUpdateAvailable`, `userRejectedUpdate`, `seeInstallErrorCode`, `autoInstallDisabled`, `managedAppNoLongerPresent`, `userRejectedInstall`, `userIsNotLoggedIntoAppStore`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="c5091-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="c5091-157">errorCode</span></span>|<span data-ttu-id="c5091-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c5091-158">Int32</span></span>|<span data-ttu-id="c5091-159">Код ошибки для установки или удаления сбоев.</span><span class="sxs-lookup"><span data-stu-id="c5091-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="c5091-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="c5091-160">osVersion</span></span>|<span data-ttu-id="c5091-161">String</span><span class="sxs-lookup"><span data-stu-id="c5091-161">String</span></span>|<span data-ttu-id="c5091-162">Версия ОС</span><span class="sxs-lookup"><span data-stu-id="c5091-162">OS Version</span></span>|
|<span data-ttu-id="c5091-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="c5091-163">osDescription</span></span>|<span data-ttu-id="c5091-164">String</span><span class="sxs-lookup"><span data-stu-id="c5091-164">String</span></span>|<span data-ttu-id="c5091-165">Описание ОС</span><span class="sxs-lookup"><span data-stu-id="c5091-165">OS Description</span></span>|
|<span data-ttu-id="c5091-166">userName</span><span class="sxs-lookup"><span data-stu-id="c5091-166">userName</span></span>|<span data-ttu-id="c5091-167">String</span><span class="sxs-lookup"><span data-stu-id="c5091-167">String</span></span>|<span data-ttu-id="c5091-168">Имя пользователя устройства</span><span class="sxs-lookup"><span data-stu-id="c5091-168">Device User Name</span></span>|
|<span data-ttu-id="c5091-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c5091-169">userPrincipalName</span></span>|<span data-ttu-id="c5091-170">String</span><span class="sxs-lookup"><span data-stu-id="c5091-170">String</span></span>|<span data-ttu-id="c5091-171">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="c5091-171">User Principal Name</span></span>|
|<span data-ttu-id="c5091-172">дисплайверсион</span><span class="sxs-lookup"><span data-stu-id="c5091-172">displayVersion</span></span>|<span data-ttu-id="c5091-173">Строка</span><span class="sxs-lookup"><span data-stu-id="c5091-173">String</span></span>|<span data-ttu-id="c5091-174">Доступная для человека версия приложения</span><span class="sxs-lookup"><span data-stu-id="c5091-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="c5091-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5091-175">Response</span></span>
<span data-ttu-id="c5091-176">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5091-176">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5091-177">Пример</span><span class="sxs-lookup"><span data-stu-id="c5091-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5091-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5091-178">Request</span></span>
<span data-ttu-id="c5091-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5091-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="c5091-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5091-180">Response</span></span>
<span data-ttu-id="c5091-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5091-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





