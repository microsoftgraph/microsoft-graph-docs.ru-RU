---
title: Обновление объекта windowsUpdateForBusinessConfiguration
description: Обновление свойств объекта windowsUpdateForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 09b07de86ae6611f4291a49820e1e92bf0609643
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146671"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="2e3fc-103">Обновление объекта windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="2e3fc-103">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="2e3fc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e3fc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e3fc-106">Обновление свойств объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e3fc-106">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e3fc-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2e3fc-107">Prerequisites</span></span>
<span data-ttu-id="2e3fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2e3fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2e3fc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e3fc-110">Permission type</span></span>|<span data-ttu-id="2e3fc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e3fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e3fc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e3fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2e3fc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e3fc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2e3fc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e3fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e3fc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-115">Not supported.</span></span>|
|<span data-ttu-id="2e3fc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e3fc-116">Application</span></span>|<span data-ttu-id="2e3fc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e3fc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e3fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2e3fc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e3fc-119">Request headers</span></span>
|<span data-ttu-id="2e3fc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e3fc-120">Header</span></span>|<span data-ttu-id="2e3fc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2e3fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e3fc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e3fc-122">Authorization</span></span>|<span data-ttu-id="2e3fc-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2e3fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e3fc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2e3fc-124">Accept</span></span>|<span data-ttu-id="2e3fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2e3fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e3fc-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2e3fc-126">Request body</span></span>
<span data-ttu-id="2e3fc-127">В теле запроса добавьте представление объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-127">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="2e3fc-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e3fc-128">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="2e3fc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e3fc-129">Property</span></span>|<span data-ttu-id="2e3fc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2e3fc-130">Type</span></span>|<span data-ttu-id="2e3fc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2e3fc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e3fc-132">id</span><span class="sxs-lookup"><span data-stu-id="2e3fc-132">id</span></span>|<span data-ttu-id="2e3fc-133">String</span><span class="sxs-lookup"><span data-stu-id="2e3fc-133">String</span></span>|<span data-ttu-id="2e3fc-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-134">Key of the entity.</span></span> <span data-ttu-id="2e3fc-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e3fc-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e3fc-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e3fc-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2e3fc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e3fc-137">DateTimeOffset</span></span>|<span data-ttu-id="2e3fc-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2e3fc-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e3fc-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e3fc-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2e3fc-140">roleScopeTagIds</span></span>|<span data-ttu-id="2e3fc-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2e3fc-141">String collection</span></span>|<span data-ttu-id="2e3fc-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2e3fc-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e3fc-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e3fc-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="2e3fc-144">supportsScopeTags</span></span>|<span data-ttu-id="2e3fc-145">Логический</span><span class="sxs-lookup"><span data-stu-id="2e3fc-145">Boolean</span></span>|<span data-ttu-id="2e3fc-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2e3fc-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2e3fc-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2e3fc-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-149">This property is read-only.</span></span> <span data-ttu-id="2e3fc-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e3fc-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e3fc-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2e3fc-151">createdDateTime</span></span>|<span data-ttu-id="2e3fc-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e3fc-152">DateTimeOffset</span></span>|<span data-ttu-id="2e3fc-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-153">DateTime the object was created.</span></span> <span data-ttu-id="2e3fc-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e3fc-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e3fc-155">description</span><span class="sxs-lookup"><span data-stu-id="2e3fc-155">description</span></span>|<span data-ttu-id="2e3fc-156">String</span><span class="sxs-lookup"><span data-stu-id="2e3fc-156">String</span></span>|<span data-ttu-id="2e3fc-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2e3fc-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e3fc-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e3fc-159">displayName</span><span class="sxs-lookup"><span data-stu-id="2e3fc-159">displayName</span></span>|<span data-ttu-id="2e3fc-160">String</span><span class="sxs-lookup"><span data-stu-id="2e3fc-160">String</span></span>|<span data-ttu-id="2e3fc-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2e3fc-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2e3fc-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e3fc-163">version</span><span class="sxs-lookup"><span data-stu-id="2e3fc-163">version</span></span>|<span data-ttu-id="2e3fc-164">Int32</span><span class="sxs-lookup"><span data-stu-id="2e3fc-164">Int32</span></span>|<span data-ttu-id="2e3fc-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-165">Version of the device configuration.</span></span> <span data-ttu-id="2e3fc-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2e3fc-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2e3fc-167">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="2e3fc-167">deliveryOptimizationMode</span></span>|[<span data-ttu-id="2e3fc-168">Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="2e3fc-168">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="2e3fc-169">Режим оптимизации доставки.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-169">Delivery Optimization Mode.</span></span> <span data-ttu-id="2e3fc-170">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-170">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="2e3fc-171">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="2e3fc-171">prereleaseFeatures</span></span>|[<span data-ttu-id="2e3fc-172">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="2e3fc-172">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="2e3fc-173">Экспериментальные функции.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-173">The pre-release features.</span></span> <span data-ttu-id="2e3fc-174">Возможные значения: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-174">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="2e3fc-175">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="2e3fc-175">automaticUpdateMode</span></span>|[<span data-ttu-id="2e3fc-176">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="2e3fc-176">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="2e3fc-177">Режим автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-177">Automatic update mode.</span></span> <span data-ttu-id="2e3fc-178">Возможные значения: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-178">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="2e3fc-179">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="2e3fc-179">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="2e3fc-180">Логический</span><span class="sxs-lookup"><span data-stu-id="2e3fc-180">Boolean</span></span>|<span data-ttu-id="2e3fc-181">Разрешение использования службы обновлений (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="2e3fc-181">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="2e3fc-182">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="2e3fc-182">driversExcluded</span></span>|<span data-ttu-id="2e3fc-183">Логический</span><span class="sxs-lookup"><span data-stu-id="2e3fc-183">Boolean</span></span>|<span data-ttu-id="2e3fc-184">Исключение драйверов из Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-184">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="2e3fc-185">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="2e3fc-185">installationSchedule</span></span>|[<span data-ttu-id="2e3fc-186">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="2e3fc-186">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="2e3fc-187">Расписание установки.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-187">Installation schedule</span></span>|
|<span data-ttu-id="2e3fc-188">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="2e3fc-188">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="2e3fc-189">Int32</span><span class="sxs-lookup"><span data-stu-id="2e3fc-189">Int32</span></span>|<span data-ttu-id="2e3fc-190">Откладывание исправлений на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-190">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="2e3fc-191">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="2e3fc-191">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="2e3fc-192">Int32</span><span class="sxs-lookup"><span data-stu-id="2e3fc-192">Int32</span></span>|<span data-ttu-id="2e3fc-193">Откладывание обновлений компонентов на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-193">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="2e3fc-194">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="2e3fc-194">qualityUpdatesPaused</span></span>|<span data-ttu-id="2e3fc-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e3fc-195">Boolean</span></span>|<span data-ttu-id="2e3fc-196">Приостановка исправлений.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-196">Pause Quality Updates</span></span>|
|<span data-ttu-id="2e3fc-197">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="2e3fc-197">featureUpdatesPaused</span></span>|<span data-ttu-id="2e3fc-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e3fc-198">Boolean</span></span>|<span data-ttu-id="2e3fc-199">Приостановка обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-199">Pause Feature Updates</span></span>|
|<span data-ttu-id="2e3fc-200">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="2e3fc-200">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="2e3fc-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e3fc-201">DateTimeOffset</span></span>|<span data-ttu-id="2e3fc-202">Дата и время завершения срока приостановки исправлений.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-202">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="2e3fc-203">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="2e3fc-203">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="2e3fc-204">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e3fc-204">DateTimeOffset</span></span>|<span data-ttu-id="2e3fc-205">Дата и время, когда будет завершен срок приостановки обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-205">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="2e3fc-206">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="2e3fc-206">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="2e3fc-207">Виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="2e3fc-207">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="2e3fc-208">Определяет, от каких устройств филиала будут получаться обновления.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-208">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="2e3fc-209">Возможные значения: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-209">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="2e3fc-210">Скипчекксбефоререстарт</span><span class="sxs-lookup"><span data-stu-id="2e3fc-210">skipChecksBeforeRestart</span></span>|<span data-ttu-id="2e3fc-211">Логический</span><span class="sxs-lookup"><span data-stu-id="2e3fc-211">Boolean</span></span>|<span data-ttu-id="2e3fc-212">Установить для пропуска всех проверок перед перезапуском: уровень аккумулятора = 40%, присутствие пользователя, требуемое отображение, режим презентации, полноэкранный режим, состояние телефонного звонка, игровой режим и т. д.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-212">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="2e3fc-213">Упдатевикс</span><span class="sxs-lookup"><span data-stu-id="2e3fc-213">updateWeeks</span></span>|[<span data-ttu-id="2e3fc-214">Виндовсупдатефорбусинессупдатевикс</span><span class="sxs-lookup"><span data-stu-id="2e3fc-214">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="2e3fc-215">Установка обновления запланирована на недели месяца.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-215">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="2e3fc-216">Возможные значения: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-216">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="2e3fc-217">Куалитюпдатеспаусестартдате</span><span class="sxs-lookup"><span data-stu-id="2e3fc-217">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="2e3fc-218">Дата</span><span class="sxs-lookup"><span data-stu-id="2e3fc-218">Date</span></span>|<span data-ttu-id="2e3fc-219">Дата начала паузы обновлений.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-219">Quality Updates Pause start date.</span></span> <span data-ttu-id="2e3fc-220">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-220">This property is read-only.</span></span>|
|<span data-ttu-id="2e3fc-221">Феатуреупдатеспаусестартдате</span><span class="sxs-lookup"><span data-stu-id="2e3fc-221">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="2e3fc-222">Дата</span><span class="sxs-lookup"><span data-stu-id="2e3fc-222">Date</span></span>|<span data-ttu-id="2e3fc-223">Дата начала паузы обновления компонентов.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-223">Feature Updates Pause start date.</span></span> <span data-ttu-id="2e3fc-224">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-224">This property is read-only.</span></span>|
|<span data-ttu-id="2e3fc-225">Феатуреупдатесроллбакквиндовиндайс</span><span class="sxs-lookup"><span data-stu-id="2e3fc-225">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="2e3fc-226">Int32</span><span class="sxs-lookup"><span data-stu-id="2e3fc-226">Int32</span></span>|<span data-ttu-id="2e3fc-227">Количество дней после обновления компонента, для которого действует откат</span><span class="sxs-lookup"><span data-stu-id="2e3fc-227">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="2e3fc-228">Куалитюпдатесвиллберолледбакк</span><span class="sxs-lookup"><span data-stu-id="2e3fc-228">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="2e3fc-229">Логический</span><span class="sxs-lookup"><span data-stu-id="2e3fc-229">Boolean</span></span>|<span data-ttu-id="2e3fc-230">Указывает, следует ли откатить обновление для следующего возврата устройства</span><span class="sxs-lookup"><span data-stu-id="2e3fc-230">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="2e3fc-231">Феатуреупдатесвиллберолледбакк</span><span class="sxs-lookup"><span data-stu-id="2e3fc-231">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="2e3fc-232">Логический</span><span class="sxs-lookup"><span data-stu-id="2e3fc-232">Boolean</span></span>|<span data-ttu-id="2e3fc-233">Указывает, следует ли откатить обновления компонентов при следующем возврате устройства</span><span class="sxs-lookup"><span data-stu-id="2e3fc-233">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="2e3fc-234">Куалитюпдатесроллбаккстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="2e3fc-234">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="2e3fc-235">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e3fc-235">DateTimeOffset</span></span>|<span data-ttu-id="2e3fc-236">Дата и время начала отката обновлений качества</span><span class="sxs-lookup"><span data-stu-id="2e3fc-236">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="2e3fc-237">Феатуреупдатесроллбаккстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="2e3fc-237">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="2e3fc-238">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e3fc-238">DateTimeOffset</span></span>|<span data-ttu-id="2e3fc-239">Дата и время начала отката обновлений компонентов</span><span class="sxs-lookup"><span data-stu-id="2e3fc-239">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="2e3fc-240">Енгажедрестартдеадлинеиндайс</span><span class="sxs-lookup"><span data-stu-id="2e3fc-240">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="2e3fc-241">Int32</span><span class="sxs-lookup"><span data-stu-id="2e3fc-241">Int32</span></span>|<span data-ttu-id="2e3fc-242">Крайний срок в днях перед автоматическим планированием и выполнением ожидающего перезапуска за пределами периода активности, с допустимым диапазоном от 2 до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-242">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="2e3fc-243">Енгажедрестартснузесчедулеиндайс</span><span class="sxs-lookup"><span data-stu-id="2e3fc-243">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="2e3fc-244">Int32</span><span class="sxs-lookup"><span data-stu-id="2e3fc-244">Int32</span></span>|<span data-ttu-id="2e3fc-245">Количество дней, в течение которых пользователь может отложить уведомления о переЗапуске с допустимым диапазоном от 1 до 3 дней</span><span class="sxs-lookup"><span data-stu-id="2e3fc-245">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="2e3fc-246">Енгажедрестарттранситионсчедулеиндайс</span><span class="sxs-lookup"><span data-stu-id="2e3fc-246">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="2e3fc-247">Int32</span><span class="sxs-lookup"><span data-stu-id="2e3fc-247">Int32</span></span>|<span data-ttu-id="2e3fc-248">Количество дней перед переходом с автоматических перезапусков, запланированных за пределами активного времени до запланированного переЗапуска, для которого пользователь должен запланировать, с допустимым диапазоном от 0 до 30 дней</span><span class="sxs-lookup"><span data-stu-id="2e3fc-248">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="2e3fc-249">Ауторестартнотификатиондисмиссал</span><span class="sxs-lookup"><span data-stu-id="2e3fc-249">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="2e3fc-250">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="2e3fc-250">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="2e3fc-251">Укажите метод закрытия уведомления об обязательном автоматическом перезапуске.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-251">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="2e3fc-252">Возможные значения: `notConfigured`, `automatic`, `user`.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-252">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="2e3fc-253">Счедулерестартварнингинхаурс</span><span class="sxs-lookup"><span data-stu-id="2e3fc-253">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="2e3fc-254">Int32</span><span class="sxs-lookup"><span data-stu-id="2e3fc-254">Int32</span></span>|<span data-ttu-id="2e3fc-255">Укажите период уведомлений с напоминанием об автоматическом перезапуске.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-255">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="2e3fc-256">Поддерживаемые значения: 2, 4, 8, 12 или 24 (часы).</span><span class="sxs-lookup"><span data-stu-id="2e3fc-256">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="2e3fc-257">Счедулеимминентрестартварнингинминутес</span><span class="sxs-lookup"><span data-stu-id="2e3fc-257">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="2e3fc-258">Int32</span><span class="sxs-lookup"><span data-stu-id="2e3fc-258">Int32</span></span>|<span data-ttu-id="2e3fc-259">Укажите период, в котором автоматически перезапускаются уведомления о приближениях.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-259">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="2e3fc-260">Поддерживаемые значения: 15, 30 или 60 (минут).</span><span class="sxs-lookup"><span data-stu-id="2e3fc-260">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="2e3fc-261">Усерпаусеакцесс</span><span class="sxs-lookup"><span data-stu-id="2e3fc-261">userPauseAccess</span></span>|[<span data-ttu-id="2e3fc-262">Включение</span><span class="sxs-lookup"><span data-stu-id="2e3fc-262">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="2e3fc-263">Указывает, следует ли включить доступ конечного пользователя для приостановки обновлений программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-263">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="2e3fc-264">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-264">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="2e3fc-265">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e3fc-265">Response</span></span>
<span data-ttu-id="2e3fc-266">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-266">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e3fc-267">Пример</span><span class="sxs-lookup"><span data-stu-id="2e3fc-267">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e3fc-268">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e3fc-268">Request</span></span>
<span data-ttu-id="2e3fc-269">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-269">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1804

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "businessReadyUpdatesOnly": "all",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "firstWeek",
  "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesRollbackWindowInDays": 2,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
  "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
  "engagedRestartDeadlineInDays": 12,
  "engagedRestartSnoozeScheduleInDays": 2,
  "engagedRestartTransitionScheduleInDays": 6,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="2e3fc-270">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e3fc-270">Response</span></span>
<span data-ttu-id="2e3fc-p121">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e3fc-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1976

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "businessReadyUpdatesOnly": "all",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "firstWeek",
  "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesRollbackWindowInDays": 2,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
  "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
  "engagedRestartDeadlineInDays": 12,
  "engagedRestartSnoozeScheduleInDays": 2,
  "engagedRestartTransitionScheduleInDays": 6,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled"
}
```




