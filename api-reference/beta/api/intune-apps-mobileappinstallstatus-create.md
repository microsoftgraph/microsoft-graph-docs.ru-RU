---
title: Создание mobileAppInstallStatus
description: Создание нового объекта mobileAppInstallStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 123a07d7b7576bfc94011e20d45a6d0c8e65abc0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394196"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="452b2-103">Создание mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="452b2-103">Create mobileAppInstallStatus</span></span>

> <span data-ttu-id="452b2-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="452b2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="452b2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="452b2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="452b2-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="452b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="452b2-107">Создание нового объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="452b2-107">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="452b2-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="452b2-108">Prerequisites</span></span>
<span data-ttu-id="452b2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="452b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="452b2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="452b2-111">Permission type</span></span>|<span data-ttu-id="452b2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="452b2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="452b2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="452b2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="452b2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="452b2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="452b2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="452b2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="452b2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="452b2-116">Not supported.</span></span>|
|<span data-ttu-id="452b2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="452b2-117">Application</span></span>|<span data-ttu-id="452b2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="452b2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="452b2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="452b2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="452b2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="452b2-120">Request headers</span></span>
|<span data-ttu-id="452b2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="452b2-121">Header</span></span>|<span data-ttu-id="452b2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="452b2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="452b2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="452b2-123">Authorization</span></span>|<span data-ttu-id="452b2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="452b2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="452b2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="452b2-125">Accept</span></span>|<span data-ttu-id="452b2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="452b2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="452b2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="452b2-127">Request body</span></span>
<span data-ttu-id="452b2-128">В тексте запроса укажите представление JSON для объекта mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="452b2-128">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="452b2-129">В следующей таблице показаны свойства, которые необходимы для создания mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="452b2-129">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="452b2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="452b2-130">Property</span></span>|<span data-ttu-id="452b2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="452b2-131">Type</span></span>|<span data-ttu-id="452b2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="452b2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="452b2-133">id</span><span class="sxs-lookup"><span data-stu-id="452b2-133">id</span></span>|<span data-ttu-id="452b2-134">String</span><span class="sxs-lookup"><span data-stu-id="452b2-134">String</span></span>|<span data-ttu-id="452b2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="452b2-135">Key of the entity.</span></span>|
|<span data-ttu-id="452b2-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="452b2-136">deviceName</span></span>|<span data-ttu-id="452b2-137">String</span><span class="sxs-lookup"><span data-stu-id="452b2-137">String</span></span>|<span data-ttu-id="452b2-138">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="452b2-138">Device name</span></span>|
|<span data-ttu-id="452b2-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="452b2-139">deviceId</span></span>|<span data-ttu-id="452b2-140">String</span><span class="sxs-lookup"><span data-stu-id="452b2-140">String</span></span>|<span data-ttu-id="452b2-141">Идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="452b2-141">Device ID</span></span>|
|<span data-ttu-id="452b2-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="452b2-142">lastSyncDateTime</span></span>|<span data-ttu-id="452b2-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="452b2-143">DateTimeOffset</span></span>|<span data-ttu-id="452b2-144">Дата и время последней синхронизации</span><span class="sxs-lookup"><span data-stu-id="452b2-144">Last sync date time</span></span>|
|<span data-ttu-id="452b2-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="452b2-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="452b2-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="452b2-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="452b2-147">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="452b2-147">The install state of the app.</span></span> <span data-ttu-id="452b2-148">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="452b2-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="452b2-149">installState</span><span class="sxs-lookup"><span data-stu-id="452b2-149">installState</span></span>|[<span data-ttu-id="452b2-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="452b2-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="452b2-151">Состояние установки приложения.</span><span class="sxs-lookup"><span data-stu-id="452b2-151">The install state of the app.</span></span> <span data-ttu-id="452b2-152">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="452b2-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="452b2-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="452b2-153">installStateDetail</span></span>|[<span data-ttu-id="452b2-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="452b2-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="452b2-155">Сведений о состоянии установки приложения.</span><span class="sxs-lookup"><span data-stu-id="452b2-155">The install state detail of the app.</span></span> <span data-ttu-id="452b2-156">Возможные значения: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="452b2-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="452b2-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="452b2-157">errorCode</span></span>|<span data-ttu-id="452b2-158">Int32</span><span class="sxs-lookup"><span data-stu-id="452b2-158">Int32</span></span>|<span data-ttu-id="452b2-159">Сообщение об ошибке примеры кода для установки или удаления сбоев.</span><span class="sxs-lookup"><span data-stu-id="452b2-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="452b2-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="452b2-160">osVersion</span></span>|<span data-ttu-id="452b2-161">String</span><span class="sxs-lookup"><span data-stu-id="452b2-161">String</span></span>|<span data-ttu-id="452b2-162">Версия операционной системы</span><span class="sxs-lookup"><span data-stu-id="452b2-162">OS Version</span></span>|
|<span data-ttu-id="452b2-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="452b2-163">osDescription</span></span>|<span data-ttu-id="452b2-164">String</span><span class="sxs-lookup"><span data-stu-id="452b2-164">String</span></span>|<span data-ttu-id="452b2-165">Описание операционная система</span><span class="sxs-lookup"><span data-stu-id="452b2-165">OS Description</span></span>|
|<span data-ttu-id="452b2-166">userName</span><span class="sxs-lookup"><span data-stu-id="452b2-166">userName</span></span>|<span data-ttu-id="452b2-167">String</span><span class="sxs-lookup"><span data-stu-id="452b2-167">String</span></span>|<span data-ttu-id="452b2-168">Имя пользователя устройства</span><span class="sxs-lookup"><span data-stu-id="452b2-168">Device User Name</span></span>|
|<span data-ttu-id="452b2-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="452b2-169">userPrincipalName</span></span>|<span data-ttu-id="452b2-170">String</span><span class="sxs-lookup"><span data-stu-id="452b2-170">String</span></span>|<span data-ttu-id="452b2-171">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="452b2-171">User Principal Name</span></span>|
|<span data-ttu-id="452b2-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="452b2-172">displayVersion</span></span>|<span data-ttu-id="452b2-173">String</span><span class="sxs-lookup"><span data-stu-id="452b2-173">String</span></span>|<span data-ttu-id="452b2-174">Человеческого для чтения версию приложения</span><span class="sxs-lookup"><span data-stu-id="452b2-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="452b2-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="452b2-175">Response</span></span>
<span data-ttu-id="452b2-176">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="452b2-176">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="452b2-177">Пример</span><span class="sxs-lookup"><span data-stu-id="452b2-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="452b2-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="452b2-178">Request</span></span>
<span data-ttu-id="452b2-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="452b2-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="452b2-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="452b2-180">Response</span></span>
<span data-ttu-id="452b2-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="452b2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




