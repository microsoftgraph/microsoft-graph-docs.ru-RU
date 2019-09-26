---
title: Create windowsUpdateForBusinessConfiguration
description: Создание объекта windowsUpdateForBusinessConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db97f2d8450211a0d6c7684a89b6411879463585
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37186479"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="0bdbf-103">Create windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="0bdbf-103">Create windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="0bdbf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bdbf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bdbf-106">Создание объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0bdbf-106">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bdbf-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0bdbf-107">Prerequisites</span></span>
<span data-ttu-id="0bdbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bdbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bdbf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0bdbf-110">Permission type</span></span>|<span data-ttu-id="0bdbf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0bdbf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bdbf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0bdbf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0bdbf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bdbf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0bdbf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0bdbf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bdbf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-115">Not supported.</span></span>|
|<span data-ttu-id="0bdbf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0bdbf-116">Application</span></span>|<span data-ttu-id="0bdbf-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bdbf-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bdbf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0bdbf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0bdbf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0bdbf-119">Request headers</span></span>
|<span data-ttu-id="0bdbf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0bdbf-120">Header</span></span>|<span data-ttu-id="0bdbf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0bdbf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bdbf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0bdbf-122">Authorization</span></span>|<span data-ttu-id="0bdbf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bdbf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0bdbf-124">Accept</span></span>|<span data-ttu-id="0bdbf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0bdbf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bdbf-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0bdbf-126">Request body</span></span>
<span data-ttu-id="0bdbf-127">В тексте запроса добавьте представление объекта windowsUpdateForBusinessConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-127">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="0bdbf-128">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-128">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="0bdbf-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0bdbf-129">Property</span></span>|<span data-ttu-id="0bdbf-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0bdbf-130">Type</span></span>|<span data-ttu-id="0bdbf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0bdbf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bdbf-132">id</span><span class="sxs-lookup"><span data-stu-id="0bdbf-132">id</span></span>|<span data-ttu-id="0bdbf-133">String</span><span class="sxs-lookup"><span data-stu-id="0bdbf-133">String</span></span>|<span data-ttu-id="0bdbf-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-134">Key of the entity.</span></span> <span data-ttu-id="0bdbf-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0bdbf-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bdbf-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0bdbf-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0bdbf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bdbf-137">DateTimeOffset</span></span>|<span data-ttu-id="0bdbf-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0bdbf-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0bdbf-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bdbf-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0bdbf-140">roleScopeTagIds</span></span>|<span data-ttu-id="0bdbf-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0bdbf-141">String collection</span></span>|<span data-ttu-id="0bdbf-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0bdbf-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0bdbf-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bdbf-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="0bdbf-144">supportsScopeTags</span></span>|<span data-ttu-id="0bdbf-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-145">Boolean</span></span>|<span data-ttu-id="0bdbf-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0bdbf-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0bdbf-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0bdbf-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-149">This property is read-only.</span></span> <span data-ttu-id="0bdbf-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0bdbf-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bdbf-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0bdbf-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0bdbf-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0bdbf-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0bdbf-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0bdbf-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0bdbf-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bdbf-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0bdbf-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0bdbf-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0bdbf-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0bdbf-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0bdbf-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0bdbf-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bdbf-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="0bdbf-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0bdbf-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="0bdbf-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0bdbf-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0bdbf-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0bdbf-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bdbf-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0bdbf-163">createdDateTime</span></span>|<span data-ttu-id="0bdbf-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bdbf-164">DateTimeOffset</span></span>|<span data-ttu-id="0bdbf-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-165">DateTime the object was created.</span></span> <span data-ttu-id="0bdbf-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0bdbf-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bdbf-167">description</span><span class="sxs-lookup"><span data-stu-id="0bdbf-167">description</span></span>|<span data-ttu-id="0bdbf-168">String</span><span class="sxs-lookup"><span data-stu-id="0bdbf-168">String</span></span>|<span data-ttu-id="0bdbf-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0bdbf-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0bdbf-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bdbf-171">displayName</span><span class="sxs-lookup"><span data-stu-id="0bdbf-171">displayName</span></span>|<span data-ttu-id="0bdbf-172">Строка</span><span class="sxs-lookup"><span data-stu-id="0bdbf-172">String</span></span>|<span data-ttu-id="0bdbf-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0bdbf-174">Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bdbf-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bdbf-175">version</span><span class="sxs-lookup"><span data-stu-id="0bdbf-175">version</span></span>|<span data-ttu-id="0bdbf-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0bdbf-176">Int32</span></span>|<span data-ttu-id="0bdbf-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-177">Version of the device configuration.</span></span> <span data-ttu-id="0bdbf-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0bdbf-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bdbf-179">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="0bdbf-179">deliveryOptimizationMode</span></span>|[<span data-ttu-id="0bdbf-180">виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="0bdbf-180">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="0bdbf-181">Режим оптимизации доставки.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-181">Delivery Optimization Mode.</span></span> <span data-ttu-id="0bdbf-182">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-182">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="0bdbf-183">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="0bdbf-183">prereleaseFeatures</span></span>|[<span data-ttu-id="0bdbf-184">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="0bdbf-184">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="0bdbf-185">Функции предварительного выпуска.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-185">The pre-release features.</span></span> <span data-ttu-id="0bdbf-186">Возможные значения: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-186">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="0bdbf-187">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="0bdbf-187">automaticUpdateMode</span></span>|[<span data-ttu-id="0bdbf-188">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="0bdbf-188">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="0bdbf-189">Режим автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-189">Automatic update mode.</span></span> <span data-ttu-id="0bdbf-190">Возможные значения: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-190">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="0bdbf-191">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="0bdbf-191">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="0bdbf-192">Boolean.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-192">Boolean</span></span>|<span data-ttu-id="0bdbf-193">Разрешение использования службы обновлений (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="0bdbf-193">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="0bdbf-194">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="0bdbf-194">driversExcluded</span></span>|<span data-ttu-id="0bdbf-195">Boolean.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-195">Boolean</span></span>|<span data-ttu-id="0bdbf-196">Исключение драйверов из Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-196">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="0bdbf-197">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="0bdbf-197">installationSchedule</span></span>|[<span data-ttu-id="0bdbf-198">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="0bdbf-198">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="0bdbf-199">Расписание установки.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-199">Installation schedule</span></span>|
|<span data-ttu-id="0bdbf-200">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="0bdbf-200">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="0bdbf-201">Int32</span><span class="sxs-lookup"><span data-stu-id="0bdbf-201">Int32</span></span>|<span data-ttu-id="0bdbf-202">Откладывание исправлений на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-202">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="0bdbf-203">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="0bdbf-203">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="0bdbf-204">Int32</span><span class="sxs-lookup"><span data-stu-id="0bdbf-204">Int32</span></span>|<span data-ttu-id="0bdbf-205">Откладывание обновлений компонентов на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-205">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="0bdbf-206">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="0bdbf-206">qualityUpdatesPaused</span></span>|<span data-ttu-id="0bdbf-207">Boolean.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-207">Boolean</span></span>|<span data-ttu-id="0bdbf-208">Приостановка исправлений.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-208">Pause Quality Updates</span></span>|
|<span data-ttu-id="0bdbf-209">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="0bdbf-209">featureUpdatesPaused</span></span>|<span data-ttu-id="0bdbf-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bdbf-210">Boolean</span></span>|<span data-ttu-id="0bdbf-211">Приостановка обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-211">Pause Feature Updates</span></span>|
|<span data-ttu-id="0bdbf-212">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="0bdbf-212">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="0bdbf-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bdbf-213">DateTimeOffset</span></span>|<span data-ttu-id="0bdbf-214">Дата и время завершения срока приостановки исправлений.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-214">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="0bdbf-215">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="0bdbf-215">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="0bdbf-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bdbf-216">DateTimeOffset</span></span>|<span data-ttu-id="0bdbf-217">Дата и время, когда будет завершен срок приостановки обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-217">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="0bdbf-218">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="0bdbf-218">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="0bdbf-219">виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="0bdbf-219">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="0bdbf-220">Определяет, от каких устройств филиала будут получаться обновления.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-220">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="0bdbf-221">Возможные значения: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-221">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="0bdbf-222">скипчекксбефоререстарт</span><span class="sxs-lookup"><span data-stu-id="0bdbf-222">skipChecksBeforeRestart</span></span>|<span data-ttu-id="0bdbf-223">Boolean.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-223">Boolean</span></span>|<span data-ttu-id="0bdbf-224">Установить для пропуска всех проверок перед перезапуском: уровень аккумулятора = 40%, присутствие пользователя, требуемое отображение, режим презентации, полноэкранный режим, состояние телефонного звонка, игровой режим и т. д.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-224">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="0bdbf-225">упдатевикс</span><span class="sxs-lookup"><span data-stu-id="0bdbf-225">updateWeeks</span></span>|[<span data-ttu-id="0bdbf-226">виндовсупдатефорбусинессупдатевикс</span><span class="sxs-lookup"><span data-stu-id="0bdbf-226">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="0bdbf-227">Установка обновления запланирована на недели месяца.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-227">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="0bdbf-228">Возможные значения: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-228">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="0bdbf-229">куалитюпдатеспаусестартдате</span><span class="sxs-lookup"><span data-stu-id="0bdbf-229">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="0bdbf-230">Дата</span><span class="sxs-lookup"><span data-stu-id="0bdbf-230">Date</span></span>|<span data-ttu-id="0bdbf-231">Дата начала паузы обновлений.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-231">Quality Updates Pause start date.</span></span> <span data-ttu-id="0bdbf-232">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-232">This property is read-only.</span></span>|
|<span data-ttu-id="0bdbf-233">феатуреупдатеспаусестартдате</span><span class="sxs-lookup"><span data-stu-id="0bdbf-233">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="0bdbf-234">Дата</span><span class="sxs-lookup"><span data-stu-id="0bdbf-234">Date</span></span>|<span data-ttu-id="0bdbf-235">Дата начала паузы обновления компонентов.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-235">Feature Updates Pause start date.</span></span> <span data-ttu-id="0bdbf-236">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-236">This property is read-only.</span></span>|
|<span data-ttu-id="0bdbf-237">феатуреупдатесроллбакквиндовиндайс</span><span class="sxs-lookup"><span data-stu-id="0bdbf-237">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="0bdbf-238">Int32</span><span class="sxs-lookup"><span data-stu-id="0bdbf-238">Int32</span></span>|<span data-ttu-id="0bdbf-239">Количество дней после обновления компонента, для которого действует откат</span><span class="sxs-lookup"><span data-stu-id="0bdbf-239">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="0bdbf-240">куалитюпдатесвиллберолледбакк</span><span class="sxs-lookup"><span data-stu-id="0bdbf-240">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="0bdbf-241">Boolean.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-241">Boolean</span></span>|<span data-ttu-id="0bdbf-242">Указывает, следует ли откатить обновление для следующего возврата устройства</span><span class="sxs-lookup"><span data-stu-id="0bdbf-242">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="0bdbf-243">феатуреупдатесвиллберолледбакк</span><span class="sxs-lookup"><span data-stu-id="0bdbf-243">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="0bdbf-244">Boolean.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-244">Boolean</span></span>|<span data-ttu-id="0bdbf-245">Указывает, следует ли откатить обновления компонентов при следующем возврате устройства</span><span class="sxs-lookup"><span data-stu-id="0bdbf-245">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="0bdbf-246">куалитюпдатесроллбаккстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="0bdbf-246">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="0bdbf-247">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bdbf-247">DateTimeOffset</span></span>|<span data-ttu-id="0bdbf-248">Дата и время начала отката обновлений качества</span><span class="sxs-lookup"><span data-stu-id="0bdbf-248">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="0bdbf-249">феатуреупдатесроллбаккстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="0bdbf-249">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="0bdbf-250">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bdbf-250">DateTimeOffset</span></span>|<span data-ttu-id="0bdbf-251">Дата и время начала отката обновлений компонентов</span><span class="sxs-lookup"><span data-stu-id="0bdbf-251">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="0bdbf-252">енгажедрестартдеадлинеиндайс</span><span class="sxs-lookup"><span data-stu-id="0bdbf-252">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="0bdbf-253">Int32</span><span class="sxs-lookup"><span data-stu-id="0bdbf-253">Int32</span></span>|<span data-ttu-id="0bdbf-254">Крайний срок в днях перед автоматическим планированием и выполнением ожидающего перезапуска за пределами периода активности, с допустимым диапазоном от 2 до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-254">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="0bdbf-255">енгажедрестартснузесчедулеиндайс</span><span class="sxs-lookup"><span data-stu-id="0bdbf-255">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="0bdbf-256">Int32</span><span class="sxs-lookup"><span data-stu-id="0bdbf-256">Int32</span></span>|<span data-ttu-id="0bdbf-257">Количество дней, в течение которых пользователь может отложить уведомления о перезапуске с допустимым диапазоном от 1 до 3 дней</span><span class="sxs-lookup"><span data-stu-id="0bdbf-257">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="0bdbf-258">енгажедрестарттранситионсчедулеиндайс</span><span class="sxs-lookup"><span data-stu-id="0bdbf-258">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="0bdbf-259">Int32</span><span class="sxs-lookup"><span data-stu-id="0bdbf-259">Int32</span></span>|<span data-ttu-id="0bdbf-260">Количество дней перед переходом с автоматических перезапусков, запланированных за пределами активного времени до запланированного перезапуска, для которого пользователь должен запланировать, с допустимым диапазоном от 0 до 30 дней</span><span class="sxs-lookup"><span data-stu-id="0bdbf-260">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="0bdbf-261">деадлинефорфеатуреупдатесиндайс</span><span class="sxs-lookup"><span data-stu-id="0bdbf-261">deadlineForFeatureUpdatesInDays</span></span>|<span data-ttu-id="0bdbf-262">Int32</span><span class="sxs-lookup"><span data-stu-id="0bdbf-262">Int32</span></span>|<span data-ttu-id="0bdbf-263">Число дней до автоматического установки обновлений компонентов с допустимым диапазоном от 2 до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-263">Number of days before feature updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="0bdbf-264">деадлинефоркуалитюпдатесиндайс</span><span class="sxs-lookup"><span data-stu-id="0bdbf-264">deadlineForQualityUpdatesInDays</span></span>|<span data-ttu-id="0bdbf-265">Int32</span><span class="sxs-lookup"><span data-stu-id="0bdbf-265">Int32</span></span>|<span data-ttu-id="0bdbf-266">Количество дней до автоматического установления обновлений качества с допустимым диапазоном от 2 до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-266">Number of days before quality updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="0bdbf-267">деадлинеграцепериодиндайс</span><span class="sxs-lookup"><span data-stu-id="0bdbf-267">deadlineGracePeriodInDays</span></span>|<span data-ttu-id="0bdbf-268">Int32</span><span class="sxs-lookup"><span data-stu-id="0bdbf-268">Int32</span></span>|<span data-ttu-id="0bdbf-269">Срок действия перезапуска (в днях), по истечении которого он будет выполняться автоматически (от 0 до 7 дней)</span><span class="sxs-lookup"><span data-stu-id="0bdbf-269">Number of days after deadline  until restarts occur automatically with valid range from 0 to 7 days</span></span>|
|<span data-ttu-id="0bdbf-270">постпонеребутунтилафтердеадлине</span><span class="sxs-lookup"><span data-stu-id="0bdbf-270">postponeRebootUntilAfterDeadline</span></span>|<span data-ttu-id="0bdbf-271">Boolean.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-271">Boolean</span></span>|<span data-ttu-id="0bdbf-272">Указывает, должно ли устройство ждать, пока не истечет время для перезагрузки в течение периода активности</span><span class="sxs-lookup"><span data-stu-id="0bdbf-272">Specifies if the device should wait until deadline for rebooting outside of active hours</span></span>|
|<span data-ttu-id="0bdbf-273">ауторестартнотификатиондисмиссал</span><span class="sxs-lookup"><span data-stu-id="0bdbf-273">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="0bdbf-274">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="0bdbf-274">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="0bdbf-275">Укажите метод закрытия уведомления об обязательном автоматическом перезапуске.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-275">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="0bdbf-276">Возможные значения: `notConfigured`, `automatic`, `user`.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-276">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="0bdbf-277">счедулерестартварнингинхаурс</span><span class="sxs-lookup"><span data-stu-id="0bdbf-277">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="0bdbf-278">Int32</span><span class="sxs-lookup"><span data-stu-id="0bdbf-278">Int32</span></span>|<span data-ttu-id="0bdbf-279">Укажите период уведомлений с напоминанием об автоматическом перезапуске.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-279">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="0bdbf-280">Поддерживаемые значения: 2, 4, 8, 12 или 24 (часы).</span><span class="sxs-lookup"><span data-stu-id="0bdbf-280">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="0bdbf-281">счедулеимминентрестартварнингинминутес</span><span class="sxs-lookup"><span data-stu-id="0bdbf-281">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="0bdbf-282">Int32</span><span class="sxs-lookup"><span data-stu-id="0bdbf-282">Int32</span></span>|<span data-ttu-id="0bdbf-283">Укажите период, в котором автоматически перезапускаются уведомления о приближениях.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-283">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="0bdbf-284">Поддерживаемые значения: 15, 30 или 60 (минут).</span><span class="sxs-lookup"><span data-stu-id="0bdbf-284">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="0bdbf-285">усерпаусеакцесс</span><span class="sxs-lookup"><span data-stu-id="0bdbf-285">userPauseAccess</span></span>|[<span data-ttu-id="0bdbf-286">Включение</span><span class="sxs-lookup"><span data-stu-id="0bdbf-286">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="0bdbf-287">Указывает, следует ли включить доступ конечного пользователя для приостановки обновлений программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-287">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="0bdbf-288">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-288">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="0bdbf-289">усервиндовсупдатесканакцесс</span><span class="sxs-lookup"><span data-stu-id="0bdbf-289">userWindowsUpdateScanAccess</span></span>|[<span data-ttu-id="0bdbf-290">Включение</span><span class="sxs-lookup"><span data-stu-id="0bdbf-290">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="0bdbf-291">Указывает, следует ли запретить доступ пользователя для сканирования центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-291">Specifies whether to disable user’s access to scan Windows Update.</span></span> <span data-ttu-id="0bdbf-292">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-292">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="0bdbf-293">упдатенотификатионлевел</span><span class="sxs-lookup"><span data-stu-id="0bdbf-293">updateNotificationLevel</span></span>|[<span data-ttu-id="0bdbf-294">windowsUpdateNotificationDisplayOption</span><span class="sxs-lookup"><span data-stu-id="0bdbf-294">windowsUpdateNotificationDisplayOption</span></span>](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|<span data-ttu-id="0bdbf-295">Указывает, что увидят пользователи уведомлений центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-295">Specifies what Windows Update notifications users see.</span></span> <span data-ttu-id="0bdbf-296">Возможные значения: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-296">Possible values are: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span></span>|



## <a name="response"></a><span data-ttu-id="0bdbf-297">Ответ</span><span class="sxs-lookup"><span data-stu-id="0bdbf-297">Response</span></span>
<span data-ttu-id="0bdbf-298">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-298">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bdbf-299">Пример</span><span class="sxs-lookup"><span data-stu-id="0bdbf-299">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bdbf-300">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bdbf-300">Request</span></span>
<span data-ttu-id="0bdbf-301">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-301">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2840

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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
  "deadlineForFeatureUpdatesInDays": 15,
  "deadlineForQualityUpdatesInDays": 15,
  "deadlineGracePeriodInDays": 9,
  "postponeRebootUntilAfterDeadline": true,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```

### <a name="response"></a><span data-ttu-id="0bdbf-302">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bdbf-302">Response</span></span>
<span data-ttu-id="0bdbf-p126">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0bdbf-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3012

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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
  "deadlineForFeatureUpdatesInDays": 15,
  "deadlineForQualityUpdatesInDays": 15,
  "deadlineGracePeriodInDays": 9,
  "postponeRebootUntilAfterDeadline": true,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```




