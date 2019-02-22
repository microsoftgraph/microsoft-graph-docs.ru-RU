---
title: Обновление mobileAppInstallStatus
description: Обновление свойств объекта mobileAppInstallStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1efc73e81894cb6fdd7d352cb067cf164f8bb33c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165746"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="38533-103">Обновление mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="38533-103">Update mobileAppInstallStatus</span></span>

> <span data-ttu-id="38533-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38533-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38533-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38533-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38533-106">Обновление свойств объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="38533-106">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38533-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="38533-107">Prerequisites</span></span>
<span data-ttu-id="38533-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="38533-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="38533-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38533-110">Permission type</span></span>|<span data-ttu-id="38533-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38533-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38533-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38533-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38533-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38533-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="38533-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38533-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38533-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38533-115">Not supported.</span></span>|
|<span data-ttu-id="38533-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38533-116">Application</span></span>|<span data-ttu-id="38533-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38533-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38533-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38533-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="38533-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38533-119">Request headers</span></span>
|<span data-ttu-id="38533-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38533-120">Header</span></span>|<span data-ttu-id="38533-121">Значение</span><span class="sxs-lookup"><span data-stu-id="38533-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38533-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38533-122">Authorization</span></span>|<span data-ttu-id="38533-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="38533-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38533-124">Accept</span><span class="sxs-lookup"><span data-stu-id="38533-124">Accept</span></span>|<span data-ttu-id="38533-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38533-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38533-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38533-126">Request body</span></span>
<span data-ttu-id="38533-127">В тексте запроса добавьте представление объекта [MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38533-127">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="38533-128">В следующей таблице приведены свойства, необходимые при создании [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="38533-128">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="38533-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="38533-129">Property</span></span>|<span data-ttu-id="38533-130">Тип</span><span class="sxs-lookup"><span data-stu-id="38533-130">Type</span></span>|<span data-ttu-id="38533-131">Описание</span><span class="sxs-lookup"><span data-stu-id="38533-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38533-132">id</span><span class="sxs-lookup"><span data-stu-id="38533-132">id</span></span>|<span data-ttu-id="38533-133">String</span><span class="sxs-lookup"><span data-stu-id="38533-133">String</span></span>|<span data-ttu-id="38533-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="38533-134">Key of the entity.</span></span>|
|<span data-ttu-id="38533-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="38533-135">deviceName</span></span>|<span data-ttu-id="38533-136">String</span><span class="sxs-lookup"><span data-stu-id="38533-136">String</span></span>|<span data-ttu-id="38533-137">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="38533-137">Device name</span></span>|
|<span data-ttu-id="38533-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="38533-138">deviceId</span></span>|<span data-ttu-id="38533-139">String</span><span class="sxs-lookup"><span data-stu-id="38533-139">String</span></span>|<span data-ttu-id="38533-140">ИДЕНТИФИКАТОР устройства</span><span class="sxs-lookup"><span data-stu-id="38533-140">Device ID</span></span>|
|<span data-ttu-id="38533-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="38533-141">lastSyncDateTime</span></span>|<span data-ttu-id="38533-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38533-142">DateTimeOffset</span></span>|<span data-ttu-id="38533-143">Дата и время последней синхронизации</span><span class="sxs-lookup"><span data-stu-id="38533-143">Last sync date time</span></span>|
|<span data-ttu-id="38533-144">Mobileappinstallstatusvalue (</span><span class="sxs-lookup"><span data-stu-id="38533-144">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="38533-145">Ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="38533-145">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="38533-146">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="38533-146">The install state of the app.</span></span> <span data-ttu-id="38533-147">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="38533-147">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="38533-148">installState</span><span class="sxs-lookup"><span data-stu-id="38533-148">installState</span></span>|[<span data-ttu-id="38533-149">Ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="38533-149">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="38533-150">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="38533-150">The install state of the app.</span></span> <span data-ttu-id="38533-151">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="38533-151">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="38533-152">Инсталлстатедетаил</span><span class="sxs-lookup"><span data-stu-id="38533-152">installStateDetail</span></span>|[<span data-ttu-id="38533-153">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="38533-153">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="38533-154">Сведения о состоянии установки приложения.</span><span class="sxs-lookup"><span data-stu-id="38533-154">The install state detail of the app.</span></span> <span data-ttu-id="38533-155">Возможные значения: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="38533-155">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="38533-156">errorCode</span><span class="sxs-lookup"><span data-stu-id="38533-156">errorCode</span></span>|<span data-ttu-id="38533-157">Int32</span><span class="sxs-lookup"><span data-stu-id="38533-157">Int32</span></span>|<span data-ttu-id="38533-158">Код ошибки для установки или удаления сбоев.</span><span class="sxs-lookup"><span data-stu-id="38533-158">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="38533-159">osVersion</span><span class="sxs-lookup"><span data-stu-id="38533-159">osVersion</span></span>|<span data-ttu-id="38533-160">String</span><span class="sxs-lookup"><span data-stu-id="38533-160">String</span></span>|<span data-ttu-id="38533-161">Версия ОС</span><span class="sxs-lookup"><span data-stu-id="38533-161">OS Version</span></span>|
|<span data-ttu-id="38533-162">osDescription</span><span class="sxs-lookup"><span data-stu-id="38533-162">osDescription</span></span>|<span data-ttu-id="38533-163">String</span><span class="sxs-lookup"><span data-stu-id="38533-163">String</span></span>|<span data-ttu-id="38533-164">Описание ОС</span><span class="sxs-lookup"><span data-stu-id="38533-164">OS Description</span></span>|
|<span data-ttu-id="38533-165">userName</span><span class="sxs-lookup"><span data-stu-id="38533-165">userName</span></span>|<span data-ttu-id="38533-166">String</span><span class="sxs-lookup"><span data-stu-id="38533-166">String</span></span>|<span data-ttu-id="38533-167">Имя пользователя устройства</span><span class="sxs-lookup"><span data-stu-id="38533-167">Device User Name</span></span>|
|<span data-ttu-id="38533-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="38533-168">userPrincipalName</span></span>|<span data-ttu-id="38533-169">Строка</span><span class="sxs-lookup"><span data-stu-id="38533-169">String</span></span>|<span data-ttu-id="38533-170">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="38533-170">User Principal Name</span></span>|
|<span data-ttu-id="38533-171">Дисплайверсион</span><span class="sxs-lookup"><span data-stu-id="38533-171">displayVersion</span></span>|<span data-ttu-id="38533-172">String</span><span class="sxs-lookup"><span data-stu-id="38533-172">String</span></span>|<span data-ttu-id="38533-173">Доступная для человека версия приложения</span><span class="sxs-lookup"><span data-stu-id="38533-173">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="38533-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="38533-174">Response</span></span>
<span data-ttu-id="38533-175">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="38533-175">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38533-176">Пример</span><span class="sxs-lookup"><span data-stu-id="38533-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="38533-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="38533-177">Request</span></span>
<span data-ttu-id="38533-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38533-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
Content-type: application/json
Content-length: 549

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "seeInstallErrorCode",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```

### <a name="response"></a><span data-ttu-id="38533-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="38533-179">Response</span></span>
<span data-ttu-id="38533-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38533-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 598

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "7560ee45-ee45-7560-45ee-607545ee6075",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "seeInstallErrorCode",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```




