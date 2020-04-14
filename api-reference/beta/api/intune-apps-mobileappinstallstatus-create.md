---
title: Создание mobileAppInstallStatus
description: Создание нового объекта mobileAppInstallStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2cf896807b1bce39b8f83a956ead7531a7c0d0b3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43414969"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="fdea6-103">Создание mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="fdea6-103">Create mobileAppInstallStatus</span></span>

<span data-ttu-id="fdea6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdea6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fdea6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdea6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdea6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fdea6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdea6-107">Создание нового объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="fdea6-107">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdea6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fdea6-108">Prerequisites</span></span>
<span data-ttu-id="fdea6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdea6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdea6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdea6-111">Permission type</span></span>|<span data-ttu-id="fdea6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdea6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdea6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdea6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fdea6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdea6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fdea6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdea6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdea6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdea6-116">Not supported.</span></span>|
|<span data-ttu-id="fdea6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fdea6-117">Application</span></span>|<span data-ttu-id="fdea6-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdea6-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdea6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdea6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="fdea6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fdea6-120">Request headers</span></span>
|<span data-ttu-id="fdea6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fdea6-121">Header</span></span>|<span data-ttu-id="fdea6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fdea6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdea6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdea6-123">Authorization</span></span>|<span data-ttu-id="fdea6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fdea6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdea6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fdea6-125">Accept</span></span>|<span data-ttu-id="fdea6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdea6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdea6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fdea6-127">Request body</span></span>
<span data-ttu-id="fdea6-128">В тексте запроса добавьте представление объекта mobileAppInstallStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdea6-128">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="fdea6-129">В следующей таблице приведены свойства, необходимые при создании mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="fdea6-129">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="fdea6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdea6-130">Property</span></span>|<span data-ttu-id="fdea6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fdea6-131">Type</span></span>|<span data-ttu-id="fdea6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fdea6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdea6-133">id</span><span class="sxs-lookup"><span data-stu-id="fdea6-133">id</span></span>|<span data-ttu-id="fdea6-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fdea6-134">String</span></span>|<span data-ttu-id="fdea6-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fdea6-135">Key of the entity.</span></span>|
|<span data-ttu-id="fdea6-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="fdea6-136">deviceName</span></span>|<span data-ttu-id="fdea6-137">String</span><span class="sxs-lookup"><span data-stu-id="fdea6-137">String</span></span>|<span data-ttu-id="fdea6-138">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="fdea6-138">Device name</span></span>|
|<span data-ttu-id="fdea6-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="fdea6-139">deviceId</span></span>|<span data-ttu-id="fdea6-140">String</span><span class="sxs-lookup"><span data-stu-id="fdea6-140">String</span></span>|<span data-ttu-id="fdea6-141">ИДЕНТИФИКАТОР устройства</span><span class="sxs-lookup"><span data-stu-id="fdea6-141">Device ID</span></span>|
|<span data-ttu-id="fdea6-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="fdea6-142">lastSyncDateTime</span></span>|<span data-ttu-id="fdea6-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdea6-143">DateTimeOffset</span></span>|<span data-ttu-id="fdea6-144">Дата и время последней синхронизации</span><span class="sxs-lookup"><span data-stu-id="fdea6-144">Last sync date time</span></span>|
|<span data-ttu-id="fdea6-145">Mobileappinstallstatusvalue (</span><span class="sxs-lookup"><span data-stu-id="fdea6-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="fdea6-146">ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="fdea6-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="fdea6-147">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="fdea6-147">The install state of the app.</span></span> <span data-ttu-id="fdea6-148">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="fdea6-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="fdea6-149">installState</span><span class="sxs-lookup"><span data-stu-id="fdea6-149">installState</span></span>|[<span data-ttu-id="fdea6-150">ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="fdea6-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="fdea6-151">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="fdea6-151">The install state of the app.</span></span> <span data-ttu-id="fdea6-152">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="fdea6-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="fdea6-153">инсталлстатедетаил</span><span class="sxs-lookup"><span data-stu-id="fdea6-153">installStateDetail</span></span>|[<span data-ttu-id="fdea6-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="fdea6-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="fdea6-155">Сведения о состоянии установки приложения.</span><span class="sxs-lookup"><span data-stu-id="fdea6-155">The install state detail of the app.</span></span> <span data-ttu-id="fdea6-156">Возможные значения: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="fdea6-156">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="fdea6-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="fdea6-157">errorCode</span></span>|<span data-ttu-id="fdea6-158">Int32</span><span class="sxs-lookup"><span data-stu-id="fdea6-158">Int32</span></span>|<span data-ttu-id="fdea6-159">Код ошибки для установки или удаления сбоев.</span><span class="sxs-lookup"><span data-stu-id="fdea6-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="fdea6-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="fdea6-160">osVersion</span></span>|<span data-ttu-id="fdea6-161">String</span><span class="sxs-lookup"><span data-stu-id="fdea6-161">String</span></span>|<span data-ttu-id="fdea6-162">Версия ОС</span><span class="sxs-lookup"><span data-stu-id="fdea6-162">OS Version</span></span>|
|<span data-ttu-id="fdea6-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="fdea6-163">osDescription</span></span>|<span data-ttu-id="fdea6-164">String</span><span class="sxs-lookup"><span data-stu-id="fdea6-164">String</span></span>|<span data-ttu-id="fdea6-165">Описание ОС</span><span class="sxs-lookup"><span data-stu-id="fdea6-165">OS Description</span></span>|
|<span data-ttu-id="fdea6-166">userName</span><span class="sxs-lookup"><span data-stu-id="fdea6-166">userName</span></span>|<span data-ttu-id="fdea6-167">String</span><span class="sxs-lookup"><span data-stu-id="fdea6-167">String</span></span>|<span data-ttu-id="fdea6-168">Имя пользователя устройства</span><span class="sxs-lookup"><span data-stu-id="fdea6-168">Device User Name</span></span>|
|<span data-ttu-id="fdea6-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fdea6-169">userPrincipalName</span></span>|<span data-ttu-id="fdea6-170">String</span><span class="sxs-lookup"><span data-stu-id="fdea6-170">String</span></span>|<span data-ttu-id="fdea6-171">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="fdea6-171">User Principal Name</span></span>|
|<span data-ttu-id="fdea6-172">дисплайверсион</span><span class="sxs-lookup"><span data-stu-id="fdea6-172">displayVersion</span></span>|<span data-ttu-id="fdea6-173">String</span><span class="sxs-lookup"><span data-stu-id="fdea6-173">String</span></span>|<span data-ttu-id="fdea6-174">Доступная для человека версия приложения</span><span class="sxs-lookup"><span data-stu-id="fdea6-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="fdea6-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdea6-175">Response</span></span>
<span data-ttu-id="fdea6-176">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fdea6-176">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdea6-177">Пример</span><span class="sxs-lookup"><span data-stu-id="fdea6-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdea6-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdea6-178">Request</span></span>
<span data-ttu-id="fdea6-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdea6-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fdea6-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdea6-180">Response</span></span>
<span data-ttu-id="fdea6-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fdea6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



