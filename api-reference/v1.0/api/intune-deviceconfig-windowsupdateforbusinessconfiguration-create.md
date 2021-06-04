---
title: Create windowsUpdateForBusinessConfiguration
description: Создание объекта windowsUpdateForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1e47aa6db924d18e1c6f84bedf877722ec4e6521
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753792"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="89e77-103">Create windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="89e77-103">Create windowsUpdateForBusinessConfiguration</span></span>

<span data-ttu-id="89e77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89e77-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89e77-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89e77-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89e77-106">Создание объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89e77-106">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89e77-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="89e77-107">Prerequisites</span></span>
<span data-ttu-id="89e77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89e77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89e77-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89e77-110">Permission type</span></span>|<span data-ttu-id="89e77-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89e77-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89e77-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89e77-112">Delegated (work or school account)</span></span>|<span data-ttu-id="89e77-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89e77-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="89e77-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89e77-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89e77-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89e77-115">Not supported.</span></span>|
|<span data-ttu-id="89e77-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="89e77-116">Application</span></span>|<span data-ttu-id="89e77-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89e77-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89e77-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89e77-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="89e77-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="89e77-119">Request headers</span></span>
|<span data-ttu-id="89e77-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89e77-120">Header</span></span>|<span data-ttu-id="89e77-121">Значение</span><span class="sxs-lookup"><span data-stu-id="89e77-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89e77-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="89e77-122">Authorization</span></span>|<span data-ttu-id="89e77-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89e77-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89e77-124">Accept</span><span class="sxs-lookup"><span data-stu-id="89e77-124">Accept</span></span>|<span data-ttu-id="89e77-125">application/json</span><span class="sxs-lookup"><span data-stu-id="89e77-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89e77-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89e77-126">Request body</span></span>
<span data-ttu-id="89e77-127">В тексте запроса добавьте представление объекта windowsUpdateForBusinessConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89e77-127">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="89e77-128">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="89e77-128">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="89e77-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="89e77-129">Property</span></span>|<span data-ttu-id="89e77-130">Тип</span><span class="sxs-lookup"><span data-stu-id="89e77-130">Type</span></span>|<span data-ttu-id="89e77-131">Описание</span><span class="sxs-lookup"><span data-stu-id="89e77-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89e77-132">id</span><span class="sxs-lookup"><span data-stu-id="89e77-132">id</span></span>|<span data-ttu-id="89e77-133">String</span><span class="sxs-lookup"><span data-stu-id="89e77-133">String</span></span>|<span data-ttu-id="89e77-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="89e77-134">Key of the entity.</span></span> <span data-ttu-id="89e77-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89e77-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89e77-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89e77-136">lastModifiedDateTime</span></span>|<span data-ttu-id="89e77-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89e77-137">DateTimeOffset</span></span>|<span data-ttu-id="89e77-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="89e77-138">DateTime the object was last modified.</span></span> <span data-ttu-id="89e77-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89e77-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89e77-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89e77-140">createdDateTime</span></span>|<span data-ttu-id="89e77-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89e77-141">DateTimeOffset</span></span>|<span data-ttu-id="89e77-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="89e77-142">DateTime the object was created.</span></span> <span data-ttu-id="89e77-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89e77-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89e77-144">description</span><span class="sxs-lookup"><span data-stu-id="89e77-144">description</span></span>|<span data-ttu-id="89e77-145">String</span><span class="sxs-lookup"><span data-stu-id="89e77-145">String</span></span>|<span data-ttu-id="89e77-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="89e77-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="89e77-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89e77-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89e77-148">displayName</span><span class="sxs-lookup"><span data-stu-id="89e77-148">displayName</span></span>|<span data-ttu-id="89e77-149">String</span><span class="sxs-lookup"><span data-stu-id="89e77-149">String</span></span>|<span data-ttu-id="89e77-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="89e77-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="89e77-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89e77-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89e77-152">version</span><span class="sxs-lookup"><span data-stu-id="89e77-152">version</span></span>|<span data-ttu-id="89e77-153">Int32</span><span class="sxs-lookup"><span data-stu-id="89e77-153">Int32</span></span>|<span data-ttu-id="89e77-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="89e77-154">Version of the device configuration.</span></span> <span data-ttu-id="89e77-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89e77-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89e77-156">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="89e77-156">deliveryOptimizationMode</span></span>|[<span data-ttu-id="89e77-157">WindowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="89e77-157">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="89e77-158">Режим оптимизации доставки.</span><span class="sxs-lookup"><span data-stu-id="89e77-158">Delivery Optimization Mode.</span></span> <span data-ttu-id="89e77-159">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="89e77-159">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="89e77-160">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="89e77-160">prereleaseFeatures</span></span>|[<span data-ttu-id="89e77-161">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="89e77-161">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="89e77-162">Функции предварительного выпуска.</span><span class="sxs-lookup"><span data-stu-id="89e77-162">The pre-release features.</span></span> <span data-ttu-id="89e77-163">Возможные значения: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="89e77-163">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="89e77-164">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="89e77-164">automaticUpdateMode</span></span>|[<span data-ttu-id="89e77-165">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="89e77-165">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="89e77-166">Режим автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="89e77-166">Automatic update mode.</span></span> <span data-ttu-id="89e77-167">Возможные значения: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="89e77-167">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="89e77-168">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="89e77-168">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="89e77-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="89e77-169">Boolean</span></span>|<span data-ttu-id="89e77-170">Разрешение использования службы обновлений (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="89e77-170">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="89e77-171">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="89e77-171">driversExcluded</span></span>|<span data-ttu-id="89e77-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="89e77-172">Boolean</span></span>|<span data-ttu-id="89e77-173">Исключение драйверов из Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="89e77-173">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="89e77-174">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="89e77-174">installationSchedule</span></span>|[<span data-ttu-id="89e77-175">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="89e77-175">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="89e77-176">Расписание установки.</span><span class="sxs-lookup"><span data-stu-id="89e77-176">Installation schedule</span></span>|
|<span data-ttu-id="89e77-177">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="89e77-177">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="89e77-178">Int32</span><span class="sxs-lookup"><span data-stu-id="89e77-178">Int32</span></span>|<span data-ttu-id="89e77-179">Откладывание исправлений на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="89e77-179">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="89e77-180">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="89e77-180">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="89e77-181">Int32</span><span class="sxs-lookup"><span data-stu-id="89e77-181">Int32</span></span>|<span data-ttu-id="89e77-182">Откладывание обновлений компонентов на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="89e77-182">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="89e77-183">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="89e77-183">qualityUpdatesPaused</span></span>|<span data-ttu-id="89e77-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="89e77-184">Boolean</span></span>|<span data-ttu-id="89e77-185">Приостановка исправлений.</span><span class="sxs-lookup"><span data-stu-id="89e77-185">Pause Quality Updates</span></span>|
|<span data-ttu-id="89e77-186">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="89e77-186">featureUpdatesPaused</span></span>|<span data-ttu-id="89e77-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="89e77-187">Boolean</span></span>|<span data-ttu-id="89e77-188">Приостановка обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="89e77-188">Pause Feature Updates</span></span>|
|<span data-ttu-id="89e77-189">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="89e77-189">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="89e77-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89e77-190">DateTimeOffset</span></span>|<span data-ttu-id="89e77-191">Дата и время завершения срока приостановки исправлений.</span><span class="sxs-lookup"><span data-stu-id="89e77-191">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="89e77-192">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="89e77-192">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="89e77-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89e77-193">DateTimeOffset</span></span>|<span data-ttu-id="89e77-194">Дата и время, когда будет завершен срок приостановки обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="89e77-194">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="89e77-195">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="89e77-195">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="89e77-196">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="89e77-196">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="89e77-197">Определяет, из каких устройств филиалов будут получаться обновления.</span><span class="sxs-lookup"><span data-stu-id="89e77-197">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="89e77-198">Возможные значения: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="89e77-198">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="89e77-199">Ответ</span><span class="sxs-lookup"><span data-stu-id="89e77-199">Response</span></span>
<span data-ttu-id="89e77-200">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="89e77-200">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89e77-201">Пример</span><span class="sxs-lookup"><span data-stu-id="89e77-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="89e77-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="89e77-202">Request</span></span>
<span data-ttu-id="89e77-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89e77-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="89e77-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="89e77-204">Response</span></span>
<span data-ttu-id="89e77-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89e77-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




