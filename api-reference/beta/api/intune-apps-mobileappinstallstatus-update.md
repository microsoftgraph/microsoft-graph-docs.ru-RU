---
title: Обновление mobileAppInstallStatus
description: Обновление свойства объекта mobileAppInstallStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e28404181248cef1deae4bec2752de51f553373b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394546"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="b07ea-103">Обновление mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="b07ea-103">Update mobileAppInstallStatus</span></span>

> <span data-ttu-id="b07ea-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b07ea-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b07ea-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b07ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b07ea-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b07ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b07ea-107">Обновление свойства объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="b07ea-107">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b07ea-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="b07ea-108">Prerequisites</span></span>
<span data-ttu-id="b07ea-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b07ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b07ea-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b07ea-111">Permission type</span></span>|<span data-ttu-id="b07ea-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b07ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b07ea-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b07ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b07ea-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b07ea-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b07ea-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b07ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b07ea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b07ea-116">Not supported.</span></span>|
|<span data-ttu-id="b07ea-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b07ea-117">Application</span></span>|<span data-ttu-id="b07ea-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b07ea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b07ea-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b07ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="b07ea-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b07ea-120">Request headers</span></span>
|<span data-ttu-id="b07ea-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b07ea-121">Header</span></span>|<span data-ttu-id="b07ea-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b07ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b07ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b07ea-123">Authorization</span></span>|<span data-ttu-id="b07ea-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b07ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b07ea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b07ea-125">Accept</span></span>|<span data-ttu-id="b07ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b07ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b07ea-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b07ea-127">Request body</span></span>
<span data-ttu-id="b07ea-128">В тексте запроса укажите представление JSON для объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="b07ea-128">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="b07ea-129">В следующей таблице показаны свойства, которые необходимы для создания [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="b07ea-129">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="b07ea-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b07ea-130">Property</span></span>|<span data-ttu-id="b07ea-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b07ea-131">Type</span></span>|<span data-ttu-id="b07ea-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b07ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b07ea-133">id</span><span class="sxs-lookup"><span data-stu-id="b07ea-133">id</span></span>|<span data-ttu-id="b07ea-134">String</span><span class="sxs-lookup"><span data-stu-id="b07ea-134">String</span></span>|<span data-ttu-id="b07ea-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b07ea-135">Key of the entity.</span></span>|
|<span data-ttu-id="b07ea-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="b07ea-136">deviceName</span></span>|<span data-ttu-id="b07ea-137">String</span><span class="sxs-lookup"><span data-stu-id="b07ea-137">String</span></span>|<span data-ttu-id="b07ea-138">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="b07ea-138">Device name</span></span>|
|<span data-ttu-id="b07ea-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="b07ea-139">deviceId</span></span>|<span data-ttu-id="b07ea-140">String</span><span class="sxs-lookup"><span data-stu-id="b07ea-140">String</span></span>|<span data-ttu-id="b07ea-141">Идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="b07ea-141">Device ID</span></span>|
|<span data-ttu-id="b07ea-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b07ea-142">lastSyncDateTime</span></span>|<span data-ttu-id="b07ea-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b07ea-143">DateTimeOffset</span></span>|<span data-ttu-id="b07ea-144">Дата и время последней синхронизации</span><span class="sxs-lookup"><span data-stu-id="b07ea-144">Last sync date time</span></span>|
|<span data-ttu-id="b07ea-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="b07ea-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="b07ea-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="b07ea-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="b07ea-147">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="b07ea-147">The install state of the app.</span></span> <span data-ttu-id="b07ea-148">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="b07ea-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="b07ea-149">installState</span><span class="sxs-lookup"><span data-stu-id="b07ea-149">installState</span></span>|[<span data-ttu-id="b07ea-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="b07ea-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="b07ea-151">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="b07ea-151">The install state of the app.</span></span> <span data-ttu-id="b07ea-152">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="b07ea-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="b07ea-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="b07ea-153">installStateDetail</span></span>|[<span data-ttu-id="b07ea-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="b07ea-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="b07ea-155">Сведений о состоянии установки приложения.</span><span class="sxs-lookup"><span data-stu-id="b07ea-155">The install state detail of the app.</span></span> <span data-ttu-id="b07ea-156">Возможные значения: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="b07ea-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="b07ea-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="b07ea-157">errorCode</span></span>|<span data-ttu-id="b07ea-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b07ea-158">Int32</span></span>|<span data-ttu-id="b07ea-159">Сообщение об ошибке примеры кода для установки или удаления сбоев.</span><span class="sxs-lookup"><span data-stu-id="b07ea-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="b07ea-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="b07ea-160">osVersion</span></span>|<span data-ttu-id="b07ea-161">String</span><span class="sxs-lookup"><span data-stu-id="b07ea-161">String</span></span>|<span data-ttu-id="b07ea-162">Версия операционной системы</span><span class="sxs-lookup"><span data-stu-id="b07ea-162">OS Version</span></span>|
|<span data-ttu-id="b07ea-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="b07ea-163">osDescription</span></span>|<span data-ttu-id="b07ea-164">String</span><span class="sxs-lookup"><span data-stu-id="b07ea-164">String</span></span>|<span data-ttu-id="b07ea-165">Описание операционная система</span><span class="sxs-lookup"><span data-stu-id="b07ea-165">OS Description</span></span>|
|<span data-ttu-id="b07ea-166">userName</span><span class="sxs-lookup"><span data-stu-id="b07ea-166">userName</span></span>|<span data-ttu-id="b07ea-167">String</span><span class="sxs-lookup"><span data-stu-id="b07ea-167">String</span></span>|<span data-ttu-id="b07ea-168">Имя пользователя устройства</span><span class="sxs-lookup"><span data-stu-id="b07ea-168">Device User Name</span></span>|
|<span data-ttu-id="b07ea-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b07ea-169">userPrincipalName</span></span>|<span data-ttu-id="b07ea-170">String</span><span class="sxs-lookup"><span data-stu-id="b07ea-170">String</span></span>|<span data-ttu-id="b07ea-171">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="b07ea-171">User Principal Name</span></span>|
|<span data-ttu-id="b07ea-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="b07ea-172">displayVersion</span></span>|<span data-ttu-id="b07ea-173">String</span><span class="sxs-lookup"><span data-stu-id="b07ea-173">String</span></span>|<span data-ttu-id="b07ea-174">Человеческого для чтения версию приложения</span><span class="sxs-lookup"><span data-stu-id="b07ea-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="b07ea-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="b07ea-175">Response</span></span>
<span data-ttu-id="b07ea-176">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b07ea-176">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b07ea-177">Пример</span><span class="sxs-lookup"><span data-stu-id="b07ea-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="b07ea-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="b07ea-178">Request</span></span>
<span data-ttu-id="b07ea-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b07ea-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b07ea-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="b07ea-180">Response</span></span>
<span data-ttu-id="b07ea-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b07ea-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




