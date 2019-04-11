---
title: Создание mobileAppInstallStatus
description: Создание нового объекта mobileAppInstallStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bc9e512419110c610397e4655022f00249d4b3cb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792078"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="2b5b7-103">Создание mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="2b5b7-103">Create mobileAppInstallStatus</span></span>

> <span data-ttu-id="2b5b7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b5b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b5b7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b5b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b5b7-106">Создание нового объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="2b5b7-106">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b5b7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2b5b7-107">Prerequisites</span></span>
<span data-ttu-id="2b5b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b5b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b5b7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b5b7-110">Permission type</span></span>|<span data-ttu-id="2b5b7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b5b7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b5b7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b5b7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2b5b7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b5b7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2b5b7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b5b7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b5b7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b5b7-115">Not supported.</span></span>|
|<span data-ttu-id="2b5b7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b5b7-116">Application</span></span>|<span data-ttu-id="2b5b7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b5b7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b5b7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b5b7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="2b5b7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b5b7-119">Request headers</span></span>
|<span data-ttu-id="2b5b7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b5b7-120">Header</span></span>|<span data-ttu-id="2b5b7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2b5b7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b5b7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b5b7-122">Authorization</span></span>|<span data-ttu-id="2b5b7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b5b7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b5b7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2b5b7-124">Accept</span></span>|<span data-ttu-id="2b5b7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2b5b7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b5b7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b5b7-126">Request body</span></span>
<span data-ttu-id="2b5b7-127">В тексте запроса добавьте представление объекта mobileAppInstallStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b5b7-127">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="2b5b7-128">В следующей таблице приведены свойства, необходимые при создании mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="2b5b7-128">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="2b5b7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b5b7-129">Property</span></span>|<span data-ttu-id="2b5b7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2b5b7-130">Type</span></span>|<span data-ttu-id="2b5b7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2b5b7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b5b7-132">id</span><span class="sxs-lookup"><span data-stu-id="2b5b7-132">id</span></span>|<span data-ttu-id="2b5b7-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2b5b7-133">String</span></span>|<span data-ttu-id="2b5b7-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2b5b7-134">Key of the entity.</span></span>|
|<span data-ttu-id="2b5b7-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="2b5b7-135">deviceName</span></span>|<span data-ttu-id="2b5b7-136">String</span><span class="sxs-lookup"><span data-stu-id="2b5b7-136">String</span></span>|<span data-ttu-id="2b5b7-137">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="2b5b7-137">Device name</span></span>|
|<span data-ttu-id="2b5b7-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="2b5b7-138">deviceId</span></span>|<span data-ttu-id="2b5b7-139">String</span><span class="sxs-lookup"><span data-stu-id="2b5b7-139">String</span></span>|<span data-ttu-id="2b5b7-140">ИДЕНТИФИКАТОР устройства</span><span class="sxs-lookup"><span data-stu-id="2b5b7-140">Device ID</span></span>|
|<span data-ttu-id="2b5b7-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2b5b7-141">lastSyncDateTime</span></span>|<span data-ttu-id="2b5b7-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b5b7-142">DateTimeOffset</span></span>|<span data-ttu-id="2b5b7-143">Дата и время последней синхронизации</span><span class="sxs-lookup"><span data-stu-id="2b5b7-143">Last sync date time</span></span>|
|<span data-ttu-id="2b5b7-144">Mobileappinstallstatusvalue (</span><span class="sxs-lookup"><span data-stu-id="2b5b7-144">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="2b5b7-145">Ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="2b5b7-145">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="2b5b7-146">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="2b5b7-146">The install state of the app.</span></span> <span data-ttu-id="2b5b7-147">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="2b5b7-147">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="2b5b7-148">installState</span><span class="sxs-lookup"><span data-stu-id="2b5b7-148">installState</span></span>|[<span data-ttu-id="2b5b7-149">Ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="2b5b7-149">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="2b5b7-150">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="2b5b7-150">The install state of the app.</span></span> <span data-ttu-id="2b5b7-151">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="2b5b7-151">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="2b5b7-152">Инсталлстатедетаил</span><span class="sxs-lookup"><span data-stu-id="2b5b7-152">installStateDetail</span></span>|[<span data-ttu-id="2b5b7-153">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="2b5b7-153">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="2b5b7-154">Сведения о состоянии установки приложения.</span><span class="sxs-lookup"><span data-stu-id="2b5b7-154">The install state detail of the app.</span></span> <span data-ttu-id="2b5b7-155">Возможные значения: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `seeInstallErrorCode` `autoInstallDisabled` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet`,,,,,,,,,,,,,,,,,,,,, `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `powerShellScriptRequirementNotMet` , `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="2b5b7-155">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="2b5b7-156">errorCode</span><span class="sxs-lookup"><span data-stu-id="2b5b7-156">errorCode</span></span>|<span data-ttu-id="2b5b7-157">Int32</span><span class="sxs-lookup"><span data-stu-id="2b5b7-157">Int32</span></span>|<span data-ttu-id="2b5b7-158">Код ошибки для установки или удаления сбоев.</span><span class="sxs-lookup"><span data-stu-id="2b5b7-158">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="2b5b7-159">osVersion</span><span class="sxs-lookup"><span data-stu-id="2b5b7-159">osVersion</span></span>|<span data-ttu-id="2b5b7-160">String</span><span class="sxs-lookup"><span data-stu-id="2b5b7-160">String</span></span>|<span data-ttu-id="2b5b7-161">Версия ОС</span><span class="sxs-lookup"><span data-stu-id="2b5b7-161">OS Version</span></span>|
|<span data-ttu-id="2b5b7-162">osDescription</span><span class="sxs-lookup"><span data-stu-id="2b5b7-162">osDescription</span></span>|<span data-ttu-id="2b5b7-163">String</span><span class="sxs-lookup"><span data-stu-id="2b5b7-163">String</span></span>|<span data-ttu-id="2b5b7-164">Описание ОС</span><span class="sxs-lookup"><span data-stu-id="2b5b7-164">OS Description</span></span>|
|<span data-ttu-id="2b5b7-165">userName</span><span class="sxs-lookup"><span data-stu-id="2b5b7-165">userName</span></span>|<span data-ttu-id="2b5b7-166">String</span><span class="sxs-lookup"><span data-stu-id="2b5b7-166">String</span></span>|<span data-ttu-id="2b5b7-167">Имя пользователя устройства</span><span class="sxs-lookup"><span data-stu-id="2b5b7-167">Device User Name</span></span>|
|<span data-ttu-id="2b5b7-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2b5b7-168">userPrincipalName</span></span>|<span data-ttu-id="2b5b7-169">String</span><span class="sxs-lookup"><span data-stu-id="2b5b7-169">String</span></span>|<span data-ttu-id="2b5b7-170">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="2b5b7-170">User Principal Name</span></span>|
|<span data-ttu-id="2b5b7-171">Дисплайверсион</span><span class="sxs-lookup"><span data-stu-id="2b5b7-171">displayVersion</span></span>|<span data-ttu-id="2b5b7-172">String</span><span class="sxs-lookup"><span data-stu-id="2b5b7-172">String</span></span>|<span data-ttu-id="2b5b7-173">Доступная для человека версия приложения</span><span class="sxs-lookup"><span data-stu-id="2b5b7-173">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="2b5b7-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b5b7-174">Response</span></span>
<span data-ttu-id="2b5b7-175">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b5b7-175">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b5b7-176">Пример</span><span class="sxs-lookup"><span data-stu-id="2b5b7-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b5b7-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b5b7-177">Request</span></span>
<span data-ttu-id="2b5b7-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b5b7-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2b5b7-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b5b7-179">Response</span></span>
<span data-ttu-id="2b5b7-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b5b7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





