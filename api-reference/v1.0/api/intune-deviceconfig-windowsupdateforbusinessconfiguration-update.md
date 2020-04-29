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
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="0f09b-103">Обновление объекта windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f09b-103">Update windowsUpdateForBusinessConfiguration</span></span>

<span data-ttu-id="0f09b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f09b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f09b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f09b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f09b-106">Обновление свойств объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f09b-106">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f09b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0f09b-107">Prerequisites</span></span>
<span data-ttu-id="0f09b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f09b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f09b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f09b-110">Permission type</span></span>|<span data-ttu-id="0f09b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f09b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f09b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f09b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0f09b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f09b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0f09b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f09b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f09b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f09b-115">Not supported.</span></span>|
|<span data-ttu-id="0f09b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f09b-116">Application</span></span>|<span data-ttu-id="0f09b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f09b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f09b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f09b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0f09b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0f09b-119">Request headers</span></span>
|<span data-ttu-id="0f09b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0f09b-120">Header</span></span>|<span data-ttu-id="0f09b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0f09b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f09b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f09b-122">Authorization</span></span>|<span data-ttu-id="0f09b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f09b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f09b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0f09b-124">Accept</span></span>|<span data-ttu-id="0f09b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0f09b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f09b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0f09b-126">Request body</span></span>
<span data-ttu-id="0f09b-127">В теле запроса добавьте представление объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f09b-127">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="0f09b-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f09b-128">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="0f09b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f09b-129">Property</span></span>|<span data-ttu-id="0f09b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0f09b-130">Type</span></span>|<span data-ttu-id="0f09b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0f09b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f09b-132">id</span><span class="sxs-lookup"><span data-stu-id="0f09b-132">id</span></span>|<span data-ttu-id="0f09b-133">String</span><span class="sxs-lookup"><span data-stu-id="0f09b-133">String</span></span>|<span data-ttu-id="0f09b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0f09b-134">Key of the entity.</span></span> <span data-ttu-id="0f09b-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f09b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f09b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f09b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0f09b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f09b-137">DateTimeOffset</span></span>|<span data-ttu-id="0f09b-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0f09b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0f09b-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f09b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f09b-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f09b-140">createdDateTime</span></span>|<span data-ttu-id="0f09b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f09b-141">DateTimeOffset</span></span>|<span data-ttu-id="0f09b-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0f09b-142">DateTime the object was created.</span></span> <span data-ttu-id="0f09b-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f09b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f09b-144">description</span><span class="sxs-lookup"><span data-stu-id="0f09b-144">description</span></span>|<span data-ttu-id="0f09b-145">String</span><span class="sxs-lookup"><span data-stu-id="0f09b-145">String</span></span>|<span data-ttu-id="0f09b-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0f09b-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0f09b-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f09b-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f09b-148">displayName</span><span class="sxs-lookup"><span data-stu-id="0f09b-148">displayName</span></span>|<span data-ttu-id="0f09b-149">Строка</span><span class="sxs-lookup"><span data-stu-id="0f09b-149">String</span></span>|<span data-ttu-id="0f09b-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0f09b-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0f09b-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f09b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f09b-152">version</span><span class="sxs-lookup"><span data-stu-id="0f09b-152">version</span></span>|<span data-ttu-id="0f09b-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0f09b-153">Int32</span></span>|<span data-ttu-id="0f09b-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0f09b-154">Version of the device configuration.</span></span> <span data-ttu-id="0f09b-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f09b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f09b-156">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="0f09b-156">deliveryOptimizationMode</span></span>|[<span data-ttu-id="0f09b-157">виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="0f09b-157">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="0f09b-158">Режим оптимизации доставки.</span><span class="sxs-lookup"><span data-stu-id="0f09b-158">Delivery Optimization Mode.</span></span> <span data-ttu-id="0f09b-159">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="0f09b-159">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="0f09b-160">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="0f09b-160">prereleaseFeatures</span></span>|[<span data-ttu-id="0f09b-161">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="0f09b-161">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="0f09b-162">Функции предварительного выпуска.</span><span class="sxs-lookup"><span data-stu-id="0f09b-162">The pre-release features.</span></span> <span data-ttu-id="0f09b-163">Возможные значения: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="0f09b-163">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="0f09b-164">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="0f09b-164">automaticUpdateMode</span></span>|[<span data-ttu-id="0f09b-165">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="0f09b-165">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="0f09b-166">Режим автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="0f09b-166">Automatic update mode.</span></span> <span data-ttu-id="0f09b-167">Возможные значения: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span><span class="sxs-lookup"><span data-stu-id="0f09b-167">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="0f09b-168">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="0f09b-168">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="0f09b-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f09b-169">Boolean</span></span>|<span data-ttu-id="0f09b-170">Разрешение использования службы обновлений (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="0f09b-170">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="0f09b-171">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="0f09b-171">driversExcluded</span></span>|<span data-ttu-id="0f09b-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f09b-172">Boolean</span></span>|<span data-ttu-id="0f09b-173">Исключение драйверов из Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="0f09b-173">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="0f09b-174">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="0f09b-174">installationSchedule</span></span>|[<span data-ttu-id="0f09b-175">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="0f09b-175">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="0f09b-176">Расписание установки.</span><span class="sxs-lookup"><span data-stu-id="0f09b-176">Installation schedule</span></span>|
|<span data-ttu-id="0f09b-177">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="0f09b-177">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="0f09b-178">Int32</span><span class="sxs-lookup"><span data-stu-id="0f09b-178">Int32</span></span>|<span data-ttu-id="0f09b-179">Откладывание исправлений на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="0f09b-179">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="0f09b-180">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="0f09b-180">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="0f09b-181">Int32</span><span class="sxs-lookup"><span data-stu-id="0f09b-181">Int32</span></span>|<span data-ttu-id="0f09b-182">Откладывание обновлений компонентов на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="0f09b-182">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="0f09b-183">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="0f09b-183">qualityUpdatesPaused</span></span>|<span data-ttu-id="0f09b-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f09b-184">Boolean</span></span>|<span data-ttu-id="0f09b-185">Приостановка исправлений.</span><span class="sxs-lookup"><span data-stu-id="0f09b-185">Pause Quality Updates</span></span>|
|<span data-ttu-id="0f09b-186">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="0f09b-186">featureUpdatesPaused</span></span>|<span data-ttu-id="0f09b-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f09b-187">Boolean</span></span>|<span data-ttu-id="0f09b-188">Приостановка обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="0f09b-188">Pause Feature Updates</span></span>|
|<span data-ttu-id="0f09b-189">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="0f09b-189">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="0f09b-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f09b-190">DateTimeOffset</span></span>|<span data-ttu-id="0f09b-191">Дата и время завершения срока приостановки исправлений.</span><span class="sxs-lookup"><span data-stu-id="0f09b-191">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="0f09b-192">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="0f09b-192">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="0f09b-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f09b-193">DateTimeOffset</span></span>|<span data-ttu-id="0f09b-194">Дата и время, когда будет завершен срок приостановки обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="0f09b-194">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="0f09b-195">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="0f09b-195">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="0f09b-196">виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="0f09b-196">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="0f09b-197">Определяет, от каких устройств филиала будут получаться обновления.</span><span class="sxs-lookup"><span data-stu-id="0f09b-197">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="0f09b-198">Возможные значения: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="0f09b-198">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="0f09b-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f09b-199">Response</span></span>
<span data-ttu-id="0f09b-200">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0f09b-200">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f09b-201">Пример</span><span class="sxs-lookup"><span data-stu-id="0f09b-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f09b-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f09b-202">Request</span></span>
<span data-ttu-id="0f09b-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f09b-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0f09b-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f09b-204">Response</span></span>
<span data-ttu-id="0f09b-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0f09b-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






