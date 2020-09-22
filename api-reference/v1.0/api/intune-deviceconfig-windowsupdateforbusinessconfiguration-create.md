---
title: Create windowsUpdateForBusinessConfiguration
description: Создание объекта windowsUpdateForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a01211834213f7abdad2120cce899305fca33d3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063228"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="fb79f-103">Create windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb79f-103">Create windowsUpdateForBusinessConfiguration</span></span>

<span data-ttu-id="fb79f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb79f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb79f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb79f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb79f-106">Создание объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb79f-106">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb79f-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fb79f-107">Prerequisites</span></span>
<span data-ttu-id="fb79f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb79f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb79f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb79f-110">Permission type</span></span>|<span data-ttu-id="fb79f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb79f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb79f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb79f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fb79f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb79f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb79f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb79f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb79f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb79f-115">Not supported.</span></span>|
|<span data-ttu-id="fb79f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb79f-116">Application</span></span>|<span data-ttu-id="fb79f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb79f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb79f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb79f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fb79f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fb79f-119">Request headers</span></span>
|<span data-ttu-id="fb79f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb79f-120">Header</span></span>|<span data-ttu-id="fb79f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fb79f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb79f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb79f-122">Authorization</span></span>|<span data-ttu-id="fb79f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb79f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb79f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fb79f-124">Accept</span></span>|<span data-ttu-id="fb79f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fb79f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb79f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fb79f-126">Request body</span></span>
<span data-ttu-id="fb79f-127">В тексте запроса добавьте представление объекта windowsUpdateForBusinessConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb79f-127">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="fb79f-128">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fb79f-128">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="fb79f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb79f-129">Property</span></span>|<span data-ttu-id="fb79f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fb79f-130">Type</span></span>|<span data-ttu-id="fb79f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fb79f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb79f-132">id</span><span class="sxs-lookup"><span data-stu-id="fb79f-132">id</span></span>|<span data-ttu-id="fb79f-133">String</span><span class="sxs-lookup"><span data-stu-id="fb79f-133">String</span></span>|<span data-ttu-id="fb79f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fb79f-134">Key of the entity.</span></span> <span data-ttu-id="fb79f-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb79f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb79f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb79f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fb79f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb79f-137">DateTimeOffset</span></span>|<span data-ttu-id="fb79f-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fb79f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="fb79f-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb79f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb79f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb79f-140">createdDateTime</span></span>|<span data-ttu-id="fb79f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb79f-141">DateTimeOffset</span></span>|<span data-ttu-id="fb79f-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fb79f-142">DateTime the object was created.</span></span> <span data-ttu-id="fb79f-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb79f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb79f-144">description</span><span class="sxs-lookup"><span data-stu-id="fb79f-144">description</span></span>|<span data-ttu-id="fb79f-145">String</span><span class="sxs-lookup"><span data-stu-id="fb79f-145">String</span></span>|<span data-ttu-id="fb79f-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fb79f-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fb79f-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb79f-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb79f-148">displayName</span><span class="sxs-lookup"><span data-stu-id="fb79f-148">displayName</span></span>|<span data-ttu-id="fb79f-149">String</span><span class="sxs-lookup"><span data-stu-id="fb79f-149">String</span></span>|<span data-ttu-id="fb79f-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fb79f-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fb79f-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb79f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb79f-152">version</span><span class="sxs-lookup"><span data-stu-id="fb79f-152">version</span></span>|<span data-ttu-id="fb79f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="fb79f-153">Int32</span></span>|<span data-ttu-id="fb79f-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fb79f-154">Version of the device configuration.</span></span> <span data-ttu-id="fb79f-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb79f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb79f-156">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="fb79f-156">deliveryOptimizationMode</span></span>|[<span data-ttu-id="fb79f-157">виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="fb79f-157">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="fb79f-158">Режим оптимизации доставки.</span><span class="sxs-lookup"><span data-stu-id="fb79f-158">Delivery Optimization Mode.</span></span> <span data-ttu-id="fb79f-159">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="fb79f-159">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="fb79f-160">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="fb79f-160">prereleaseFeatures</span></span>|[<span data-ttu-id="fb79f-161">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="fb79f-161">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="fb79f-162">Функции предварительного выпуска.</span><span class="sxs-lookup"><span data-stu-id="fb79f-162">The pre-release features.</span></span> <span data-ttu-id="fb79f-163">Возможные значения: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="fb79f-163">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="fb79f-164">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="fb79f-164">automaticUpdateMode</span></span>|[<span data-ttu-id="fb79f-165">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="fb79f-165">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="fb79f-166">Режим автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="fb79f-166">Automatic update mode.</span></span> <span data-ttu-id="fb79f-167">Возможные значения: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="fb79f-167">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="fb79f-168">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="fb79f-168">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="fb79f-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb79f-169">Boolean</span></span>|<span data-ttu-id="fb79f-170">Разрешение использования службы обновлений (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="fb79f-170">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="fb79f-171">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="fb79f-171">driversExcluded</span></span>|<span data-ttu-id="fb79f-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb79f-172">Boolean</span></span>|<span data-ttu-id="fb79f-173">Исключение драйверов из Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="fb79f-173">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="fb79f-174">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="fb79f-174">installationSchedule</span></span>|[<span data-ttu-id="fb79f-175">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="fb79f-175">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="fb79f-176">Расписание установки.</span><span class="sxs-lookup"><span data-stu-id="fb79f-176">Installation schedule</span></span>|
|<span data-ttu-id="fb79f-177">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="fb79f-177">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="fb79f-178">Int32</span><span class="sxs-lookup"><span data-stu-id="fb79f-178">Int32</span></span>|<span data-ttu-id="fb79f-179">Откладывание исправлений на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="fb79f-179">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="fb79f-180">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="fb79f-180">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="fb79f-181">Int32</span><span class="sxs-lookup"><span data-stu-id="fb79f-181">Int32</span></span>|<span data-ttu-id="fb79f-182">Откладывание обновлений компонентов на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="fb79f-182">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="fb79f-183">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="fb79f-183">qualityUpdatesPaused</span></span>|<span data-ttu-id="fb79f-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb79f-184">Boolean</span></span>|<span data-ttu-id="fb79f-185">Приостановка исправлений.</span><span class="sxs-lookup"><span data-stu-id="fb79f-185">Pause Quality Updates</span></span>|
|<span data-ttu-id="fb79f-186">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="fb79f-186">featureUpdatesPaused</span></span>|<span data-ttu-id="fb79f-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb79f-187">Boolean</span></span>|<span data-ttu-id="fb79f-188">Приостановка обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="fb79f-188">Pause Feature Updates</span></span>|
|<span data-ttu-id="fb79f-189">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="fb79f-189">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="fb79f-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb79f-190">DateTimeOffset</span></span>|<span data-ttu-id="fb79f-191">Дата и время завершения срока приостановки исправлений.</span><span class="sxs-lookup"><span data-stu-id="fb79f-191">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="fb79f-192">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="fb79f-192">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="fb79f-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb79f-193">DateTimeOffset</span></span>|<span data-ttu-id="fb79f-194">Дата и время, когда будет завершен срок приостановки обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="fb79f-194">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="fb79f-195">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="fb79f-195">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="fb79f-196">виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="fb79f-196">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="fb79f-197">Определяет, от каких устройств филиала будут получаться обновления.</span><span class="sxs-lookup"><span data-stu-id="fb79f-197">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="fb79f-198">Возможные значения: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="fb79f-198">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="fb79f-199">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb79f-199">Response</span></span>
<span data-ttu-id="fb79f-200">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fb79f-200">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb79f-201">Пример</span><span class="sxs-lookup"><span data-stu-id="fb79f-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb79f-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb79f-202">Request</span></span>
<span data-ttu-id="fb79f-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb79f-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="fb79f-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb79f-204">Response</span></span>
<span data-ttu-id="fb79f-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb79f-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









