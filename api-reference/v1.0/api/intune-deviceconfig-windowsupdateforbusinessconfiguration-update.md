---
title: Обновление объекта windowsUpdateForBusinessConfiguration
description: Обновление свойств объекта windowsUpdateForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9afdfb8e55d15763b8023ef0ed0a28d1f64559d9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388871"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="751f0-103">Обновление объекта windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="751f0-103">Update windowsUpdateForBusinessConfiguration</span></span>

<span data-ttu-id="751f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="751f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="751f0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="751f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="751f0-106">Обновление свойств объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="751f0-106">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="751f0-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="751f0-107">Prerequisites</span></span>
<span data-ttu-id="751f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="751f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="751f0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="751f0-110">Permission type</span></span>|<span data-ttu-id="751f0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="751f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="751f0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="751f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="751f0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="751f0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="751f0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="751f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="751f0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="751f0-115">Not supported.</span></span>|
|<span data-ttu-id="751f0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="751f0-116">Application</span></span>|<span data-ttu-id="751f0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="751f0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="751f0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="751f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="751f0-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="751f0-119">Request headers</span></span>
|<span data-ttu-id="751f0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="751f0-120">Header</span></span>|<span data-ttu-id="751f0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="751f0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="751f0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="751f0-122">Authorization</span></span>|<span data-ttu-id="751f0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="751f0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="751f0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="751f0-124">Accept</span></span>|<span data-ttu-id="751f0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="751f0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="751f0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="751f0-126">Request body</span></span>
<span data-ttu-id="751f0-127">В теле запроса добавьте представление объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="751f0-127">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="751f0-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="751f0-128">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="751f0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="751f0-129">Property</span></span>|<span data-ttu-id="751f0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="751f0-130">Type</span></span>|<span data-ttu-id="751f0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="751f0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="751f0-132">id</span><span class="sxs-lookup"><span data-stu-id="751f0-132">id</span></span>|<span data-ttu-id="751f0-133">String</span><span class="sxs-lookup"><span data-stu-id="751f0-133">String</span></span>|<span data-ttu-id="751f0-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="751f0-134">Key of the entity.</span></span> <span data-ttu-id="751f0-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="751f0-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="751f0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="751f0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="751f0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="751f0-137">DateTimeOffset</span></span>|<span data-ttu-id="751f0-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="751f0-138">DateTime the object was last modified.</span></span> <span data-ttu-id="751f0-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="751f0-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="751f0-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="751f0-140">createdDateTime</span></span>|<span data-ttu-id="751f0-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="751f0-141">DateTimeOffset</span></span>|<span data-ttu-id="751f0-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="751f0-142">DateTime the object was created.</span></span> <span data-ttu-id="751f0-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="751f0-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="751f0-144">description</span><span class="sxs-lookup"><span data-stu-id="751f0-144">description</span></span>|<span data-ttu-id="751f0-145">String</span><span class="sxs-lookup"><span data-stu-id="751f0-145">String</span></span>|<span data-ttu-id="751f0-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="751f0-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="751f0-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="751f0-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="751f0-148">displayName</span><span class="sxs-lookup"><span data-stu-id="751f0-148">displayName</span></span>|<span data-ttu-id="751f0-149">Строка</span><span class="sxs-lookup"><span data-stu-id="751f0-149">String</span></span>|<span data-ttu-id="751f0-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="751f0-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="751f0-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="751f0-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="751f0-152">version</span><span class="sxs-lookup"><span data-stu-id="751f0-152">version</span></span>|<span data-ttu-id="751f0-153">Int32</span><span class="sxs-lookup"><span data-stu-id="751f0-153">Int32</span></span>|<span data-ttu-id="751f0-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="751f0-154">Version of the device configuration.</span></span> <span data-ttu-id="751f0-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="751f0-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="751f0-156">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="751f0-156">deliveryOptimizationMode</span></span>|[<span data-ttu-id="751f0-157">виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="751f0-157">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="751f0-158">Режим оптимизации доставки.</span><span class="sxs-lookup"><span data-stu-id="751f0-158">Delivery Optimization Mode.</span></span> <span data-ttu-id="751f0-159">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="751f0-159">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="751f0-160">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="751f0-160">prereleaseFeatures</span></span>|[<span data-ttu-id="751f0-161">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="751f0-161">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="751f0-162">Функции предварительного выпуска.</span><span class="sxs-lookup"><span data-stu-id="751f0-162">The pre-release features.</span></span> <span data-ttu-id="751f0-163">Возможные значения: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="751f0-163">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="751f0-164">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="751f0-164">automaticUpdateMode</span></span>|[<span data-ttu-id="751f0-165">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="751f0-165">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="751f0-166">Режим автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="751f0-166">Automatic update mode.</span></span> <span data-ttu-id="751f0-167">Возможные значения: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="751f0-167">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="751f0-168">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="751f0-168">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="751f0-169">Логический</span><span class="sxs-lookup"><span data-stu-id="751f0-169">Boolean</span></span>|<span data-ttu-id="751f0-170">Разрешение использования службы обновлений (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="751f0-170">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="751f0-171">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="751f0-171">driversExcluded</span></span>|<span data-ttu-id="751f0-172">Логический</span><span class="sxs-lookup"><span data-stu-id="751f0-172">Boolean</span></span>|<span data-ttu-id="751f0-173">Исключение драйверов из Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="751f0-173">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="751f0-174">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="751f0-174">installationSchedule</span></span>|[<span data-ttu-id="751f0-175">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="751f0-175">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="751f0-176">Расписание установки.</span><span class="sxs-lookup"><span data-stu-id="751f0-176">Installation schedule</span></span>|
|<span data-ttu-id="751f0-177">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="751f0-177">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="751f0-178">Int32</span><span class="sxs-lookup"><span data-stu-id="751f0-178">Int32</span></span>|<span data-ttu-id="751f0-179">Откладывание исправлений на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="751f0-179">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="751f0-180">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="751f0-180">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="751f0-181">Int32</span><span class="sxs-lookup"><span data-stu-id="751f0-181">Int32</span></span>|<span data-ttu-id="751f0-182">Откладывание обновлений компонентов на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="751f0-182">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="751f0-183">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="751f0-183">qualityUpdatesPaused</span></span>|<span data-ttu-id="751f0-184">Логический</span><span class="sxs-lookup"><span data-stu-id="751f0-184">Boolean</span></span>|<span data-ttu-id="751f0-185">Приостановка исправлений.</span><span class="sxs-lookup"><span data-stu-id="751f0-185">Pause Quality Updates</span></span>|
|<span data-ttu-id="751f0-186">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="751f0-186">featureUpdatesPaused</span></span>|<span data-ttu-id="751f0-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="751f0-187">Boolean</span></span>|<span data-ttu-id="751f0-188">Приостановка обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="751f0-188">Pause Feature Updates</span></span>|
|<span data-ttu-id="751f0-189">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="751f0-189">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="751f0-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="751f0-190">DateTimeOffset</span></span>|<span data-ttu-id="751f0-191">Дата и время завершения срока приостановки исправлений.</span><span class="sxs-lookup"><span data-stu-id="751f0-191">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="751f0-192">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="751f0-192">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="751f0-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="751f0-193">DateTimeOffset</span></span>|<span data-ttu-id="751f0-194">Дата и время, когда будет завершен срок приостановки обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="751f0-194">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="751f0-195">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="751f0-195">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="751f0-196">виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="751f0-196">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="751f0-197">Определяет, от каких устройств филиала будут получаться обновления.</span><span class="sxs-lookup"><span data-stu-id="751f0-197">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="751f0-198">Возможные значения: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="751f0-198">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="751f0-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="751f0-199">Response</span></span>
<span data-ttu-id="751f0-200">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="751f0-200">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="751f0-201">Пример</span><span class="sxs-lookup"><span data-stu-id="751f0-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="751f0-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="751f0-202">Request</span></span>
<span data-ttu-id="751f0-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="751f0-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 910

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all"
}
```

### <a name="response"></a><span data-ttu-id="751f0-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="751f0-204">Response</span></span>
<span data-ttu-id="751f0-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="751f0-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1082

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all"
}
```






