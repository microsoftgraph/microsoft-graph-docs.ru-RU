---
title: Обновление объекта windowsUpdateForBusinessConfiguration
description: Обновление свойств объекта windowsUpdateForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 17068d1ad12893cd490d913849399d21d74d992b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021090"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="21ef9-103">Обновление объекта windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="21ef9-103">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="21ef9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21ef9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21ef9-105">Обновление свойств объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="21ef9-105">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21ef9-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="21ef9-106">Prerequisites</span></span>
<span data-ttu-id="21ef9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21ef9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21ef9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21ef9-109">Permission type</span></span>|<span data-ttu-id="21ef9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="21ef9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21ef9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21ef9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="21ef9-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21ef9-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="21ef9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21ef9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21ef9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21ef9-114">Not supported.</span></span>|
|<span data-ttu-id="21ef9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21ef9-115">Application</span></span>|<span data-ttu-id="21ef9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21ef9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21ef9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21ef9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="21ef9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21ef9-118">Request headers</span></span>
|<span data-ttu-id="21ef9-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21ef9-119">Header</span></span>|<span data-ttu-id="21ef9-120">Значение</span><span class="sxs-lookup"><span data-stu-id="21ef9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21ef9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21ef9-121">Authorization</span></span>|<span data-ttu-id="21ef9-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21ef9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21ef9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="21ef9-123">Accept</span></span>|<span data-ttu-id="21ef9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="21ef9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21ef9-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="21ef9-125">Request body</span></span>
<span data-ttu-id="21ef9-126">В теле запроса добавьте представление объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21ef9-126">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="21ef9-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="21ef9-127">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="21ef9-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="21ef9-128">Property</span></span>|<span data-ttu-id="21ef9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="21ef9-129">Type</span></span>|<span data-ttu-id="21ef9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="21ef9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21ef9-131">id</span><span class="sxs-lookup"><span data-stu-id="21ef9-131">id</span></span>|<span data-ttu-id="21ef9-132">String</span><span class="sxs-lookup"><span data-stu-id="21ef9-132">String</span></span>|<span data-ttu-id="21ef9-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="21ef9-133">Key of the entity.</span></span> <span data-ttu-id="21ef9-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="21ef9-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21ef9-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21ef9-135">lastModifiedDateTime</span></span>|<span data-ttu-id="21ef9-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21ef9-136">DateTimeOffset</span></span>|<span data-ttu-id="21ef9-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="21ef9-137">DateTime the object was last modified.</span></span> <span data-ttu-id="21ef9-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="21ef9-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21ef9-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21ef9-139">createdDateTime</span></span>|<span data-ttu-id="21ef9-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21ef9-140">DateTimeOffset</span></span>|<span data-ttu-id="21ef9-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="21ef9-141">DateTime the object was created.</span></span> <span data-ttu-id="21ef9-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="21ef9-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21ef9-143">description</span><span class="sxs-lookup"><span data-stu-id="21ef9-143">description</span></span>|<span data-ttu-id="21ef9-144">String</span><span class="sxs-lookup"><span data-stu-id="21ef9-144">String</span></span>|<span data-ttu-id="21ef9-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="21ef9-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="21ef9-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="21ef9-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21ef9-147">displayName</span><span class="sxs-lookup"><span data-stu-id="21ef9-147">displayName</span></span>|<span data-ttu-id="21ef9-148">Строка</span><span class="sxs-lookup"><span data-stu-id="21ef9-148">String</span></span>|<span data-ttu-id="21ef9-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="21ef9-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="21ef9-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21ef9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21ef9-151">version</span><span class="sxs-lookup"><span data-stu-id="21ef9-151">version</span></span>|<span data-ttu-id="21ef9-152">Int32</span><span class="sxs-lookup"><span data-stu-id="21ef9-152">Int32</span></span>|<span data-ttu-id="21ef9-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="21ef9-153">Version of the device configuration.</span></span> <span data-ttu-id="21ef9-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="21ef9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21ef9-155">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="21ef9-155">deliveryOptimizationMode</span></span>|[<span data-ttu-id="21ef9-156">Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="21ef9-156">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="21ef9-157">Режим оптимизации доставки.</span><span class="sxs-lookup"><span data-stu-id="21ef9-157">Delivery Optimization Mode.</span></span> <span data-ttu-id="21ef9-158">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="21ef9-158">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="21ef9-159">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="21ef9-159">prereleaseFeatures</span></span>|[<span data-ttu-id="21ef9-160">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="21ef9-160">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="21ef9-161">Функции предварительного выпуска.</span><span class="sxs-lookup"><span data-stu-id="21ef9-161">The pre-release features.</span></span> <span data-ttu-id="21ef9-162">Возможные значения: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="21ef9-162">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="21ef9-163">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="21ef9-163">automaticUpdateMode</span></span>|[<span data-ttu-id="21ef9-164">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="21ef9-164">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="21ef9-165">Режим автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="21ef9-165">Automatic update mode.</span></span> <span data-ttu-id="21ef9-166">Возможные значения: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="21ef9-166">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="21ef9-167">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="21ef9-167">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="21ef9-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ef9-168">Boolean</span></span>|<span data-ttu-id="21ef9-169">Разрешение использования службы обновлений (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="21ef9-169">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="21ef9-170">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="21ef9-170">driversExcluded</span></span>|<span data-ttu-id="21ef9-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ef9-171">Boolean</span></span>|<span data-ttu-id="21ef9-172">Исключение драйверов из Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="21ef9-172">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="21ef9-173">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="21ef9-173">installationSchedule</span></span>|[<span data-ttu-id="21ef9-174">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="21ef9-174">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="21ef9-175">Расписание установки.</span><span class="sxs-lookup"><span data-stu-id="21ef9-175">Installation schedule</span></span>|
|<span data-ttu-id="21ef9-176">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="21ef9-176">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="21ef9-177">Int32</span><span class="sxs-lookup"><span data-stu-id="21ef9-177">Int32</span></span>|<span data-ttu-id="21ef9-178">Откладывание исправлений на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="21ef9-178">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="21ef9-179">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="21ef9-179">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="21ef9-180">Int32</span><span class="sxs-lookup"><span data-stu-id="21ef9-180">Int32</span></span>|<span data-ttu-id="21ef9-181">Откладывание обновлений компонентов на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="21ef9-181">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="21ef9-182">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="21ef9-182">qualityUpdatesPaused</span></span>|<span data-ttu-id="21ef9-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ef9-183">Boolean</span></span>|<span data-ttu-id="21ef9-184">Приостановка исправлений.</span><span class="sxs-lookup"><span data-stu-id="21ef9-184">Pause Quality Updates</span></span>|
|<span data-ttu-id="21ef9-185">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="21ef9-185">featureUpdatesPaused</span></span>|<span data-ttu-id="21ef9-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="21ef9-186">Boolean</span></span>|<span data-ttu-id="21ef9-187">Приостановка обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="21ef9-187">Pause Feature Updates</span></span>|
|<span data-ttu-id="21ef9-188">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="21ef9-188">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="21ef9-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21ef9-189">DateTimeOffset</span></span>|<span data-ttu-id="21ef9-190">Дата и время завершения срока приостановки исправлений.</span><span class="sxs-lookup"><span data-stu-id="21ef9-190">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="21ef9-191">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="21ef9-191">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="21ef9-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21ef9-192">DateTimeOffset</span></span>|<span data-ttu-id="21ef9-193">Дата и время, когда будет завершен срок приостановки обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="21ef9-193">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="21ef9-194">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="21ef9-194">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="21ef9-195">Виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="21ef9-195">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="21ef9-196">Определяет, от каких устройств филиала будут получаться обновления.</span><span class="sxs-lookup"><span data-stu-id="21ef9-196">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="21ef9-197">Возможные значения: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="21ef9-197">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="21ef9-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="21ef9-198">Response</span></span>
<span data-ttu-id="21ef9-199">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="21ef9-199">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21ef9-200">Пример</span><span class="sxs-lookup"><span data-stu-id="21ef9-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="21ef9-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="21ef9-201">Request</span></span>
<span data-ttu-id="21ef9-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21ef9-202">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="21ef9-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="21ef9-203">Response</span></span>
<span data-ttu-id="21ef9-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21ef9-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



