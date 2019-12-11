---
title: Обновление объекта windowsUpdateForBusinessConfiguration
description: Обновление свойств объекта windowsUpdateForBusinessConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d4aa3a5c3d81deb2d59c6a669569d0a035fef34c
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946345"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="2a60c-103">Обновление объекта windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="2a60c-103">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="2a60c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a60c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a60c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a60c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a60c-106">Обновление свойств объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a60c-106">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a60c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2a60c-107">Prerequisites</span></span>
<span data-ttu-id="2a60c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a60c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a60c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a60c-110">Permission type</span></span>|<span data-ttu-id="2a60c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a60c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a60c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a60c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a60c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a60c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2a60c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a60c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a60c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a60c-115">Not supported.</span></span>|
|<span data-ttu-id="2a60c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a60c-116">Application</span></span>|<span data-ttu-id="2a60c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a60c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a60c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a60c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2a60c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2a60c-119">Request headers</span></span>
|<span data-ttu-id="2a60c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a60c-120">Header</span></span>|<span data-ttu-id="2a60c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2a60c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a60c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a60c-122">Authorization</span></span>|<span data-ttu-id="2a60c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a60c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a60c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2a60c-124">Accept</span></span>|<span data-ttu-id="2a60c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2a60c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a60c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2a60c-126">Request body</span></span>
<span data-ttu-id="2a60c-127">В теле запроса добавьте представление объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a60c-127">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="2a60c-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a60c-128">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="2a60c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a60c-129">Property</span></span>|<span data-ttu-id="2a60c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2a60c-130">Type</span></span>|<span data-ttu-id="2a60c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2a60c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a60c-132">id</span><span class="sxs-lookup"><span data-stu-id="2a60c-132">id</span></span>|<span data-ttu-id="2a60c-133">String</span><span class="sxs-lookup"><span data-stu-id="2a60c-133">String</span></span>|<span data-ttu-id="2a60c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2a60c-134">Key of the entity.</span></span> <span data-ttu-id="2a60c-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a60c-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a60c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a60c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2a60c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a60c-137">DateTimeOffset</span></span>|<span data-ttu-id="2a60c-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2a60c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2a60c-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a60c-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a60c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2a60c-140">roleScopeTagIds</span></span>|<span data-ttu-id="2a60c-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2a60c-141">String collection</span></span>|<span data-ttu-id="2a60c-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2a60c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2a60c-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a60c-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a60c-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="2a60c-144">supportsScopeTags</span></span>|<span data-ttu-id="2a60c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a60c-145">Boolean</span></span>|<span data-ttu-id="2a60c-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="2a60c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2a60c-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="2a60c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2a60c-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2a60c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2a60c-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2a60c-149">This property is read-only.</span></span> <span data-ttu-id="2a60c-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a60c-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a60c-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2a60c-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2a60c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2a60c-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2a60c-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2a60c-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2a60c-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a60c-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a60c-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2a60c-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2a60c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2a60c-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2a60c-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2a60c-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2a60c-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a60c-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a60c-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2a60c-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2a60c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2a60c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2a60c-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2a60c-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2a60c-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a60c-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a60c-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a60c-163">createdDateTime</span></span>|<span data-ttu-id="2a60c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a60c-164">DateTimeOffset</span></span>|<span data-ttu-id="2a60c-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2a60c-165">DateTime the object was created.</span></span> <span data-ttu-id="2a60c-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a60c-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a60c-167">description</span><span class="sxs-lookup"><span data-stu-id="2a60c-167">description</span></span>|<span data-ttu-id="2a60c-168">String</span><span class="sxs-lookup"><span data-stu-id="2a60c-168">String</span></span>|<span data-ttu-id="2a60c-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2a60c-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2a60c-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a60c-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a60c-171">displayName</span><span class="sxs-lookup"><span data-stu-id="2a60c-171">displayName</span></span>|<span data-ttu-id="2a60c-172">Строка</span><span class="sxs-lookup"><span data-stu-id="2a60c-172">String</span></span>|<span data-ttu-id="2a60c-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2a60c-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2a60c-174">Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2a60c-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a60c-175">version</span><span class="sxs-lookup"><span data-stu-id="2a60c-175">version</span></span>|<span data-ttu-id="2a60c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2a60c-176">Int32</span></span>|<span data-ttu-id="2a60c-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2a60c-177">Version of the device configuration.</span></span> <span data-ttu-id="2a60c-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2a60c-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2a60c-179">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="2a60c-179">deliveryOptimizationMode</span></span>|[<span data-ttu-id="2a60c-180">виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="2a60c-180">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="2a60c-181">Режим оптимизации доставки.</span><span class="sxs-lookup"><span data-stu-id="2a60c-181">Delivery Optimization Mode.</span></span> <span data-ttu-id="2a60c-182">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="2a60c-182">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="2a60c-183">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="2a60c-183">prereleaseFeatures</span></span>|[<span data-ttu-id="2a60c-184">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="2a60c-184">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="2a60c-185">Функции предварительного выпуска.</span><span class="sxs-lookup"><span data-stu-id="2a60c-185">The pre-release features.</span></span> <span data-ttu-id="2a60c-186">Возможные значения: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="2a60c-186">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="2a60c-187">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="2a60c-187">automaticUpdateMode</span></span>|[<span data-ttu-id="2a60c-188">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="2a60c-188">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="2a60c-189">Режим автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="2a60c-189">Automatic update mode.</span></span> <span data-ttu-id="2a60c-190">Возможные значения: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span><span class="sxs-lookup"><span data-stu-id="2a60c-190">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="2a60c-191">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="2a60c-191">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="2a60c-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a60c-192">Boolean</span></span>|<span data-ttu-id="2a60c-193">Разрешение использования службы обновлений (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="2a60c-193">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="2a60c-194">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="2a60c-194">driversExcluded</span></span>|<span data-ttu-id="2a60c-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a60c-195">Boolean</span></span>|<span data-ttu-id="2a60c-196">Исключение драйверов из Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="2a60c-196">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="2a60c-197">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="2a60c-197">installationSchedule</span></span>|[<span data-ttu-id="2a60c-198">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="2a60c-198">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="2a60c-199">Расписание установки.</span><span class="sxs-lookup"><span data-stu-id="2a60c-199">Installation schedule</span></span>|
|<span data-ttu-id="2a60c-200">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="2a60c-200">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="2a60c-201">Int32</span><span class="sxs-lookup"><span data-stu-id="2a60c-201">Int32</span></span>|<span data-ttu-id="2a60c-202">Откладывание исправлений на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="2a60c-202">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="2a60c-203">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="2a60c-203">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="2a60c-204">Int32</span><span class="sxs-lookup"><span data-stu-id="2a60c-204">Int32</span></span>|<span data-ttu-id="2a60c-205">Откладывание обновлений компонентов на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="2a60c-205">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="2a60c-206">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="2a60c-206">qualityUpdatesPaused</span></span>|<span data-ttu-id="2a60c-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a60c-207">Boolean</span></span>|<span data-ttu-id="2a60c-208">Приостановка исправлений.</span><span class="sxs-lookup"><span data-stu-id="2a60c-208">Pause Quality Updates</span></span>|
|<span data-ttu-id="2a60c-209">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="2a60c-209">featureUpdatesPaused</span></span>|<span data-ttu-id="2a60c-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a60c-210">Boolean</span></span>|<span data-ttu-id="2a60c-211">Приостановка обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="2a60c-211">Pause Feature Updates</span></span>|
|<span data-ttu-id="2a60c-212">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="2a60c-212">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="2a60c-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a60c-213">DateTimeOffset</span></span>|<span data-ttu-id="2a60c-214">Дата и время завершения срока приостановки исправлений.</span><span class="sxs-lookup"><span data-stu-id="2a60c-214">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="2a60c-215">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="2a60c-215">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="2a60c-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a60c-216">DateTimeOffset</span></span>|<span data-ttu-id="2a60c-217">Дата и время, когда будет завершен срок приостановки обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="2a60c-217">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="2a60c-218">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="2a60c-218">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="2a60c-219">виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="2a60c-219">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="2a60c-220">Определяет, от каких устройств филиала будут получаться обновления.</span><span class="sxs-lookup"><span data-stu-id="2a60c-220">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="2a60c-221">Возможные значения: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="2a60c-221">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="2a60c-222">скипчекксбефоререстарт</span><span class="sxs-lookup"><span data-stu-id="2a60c-222">skipChecksBeforeRestart</span></span>|<span data-ttu-id="2a60c-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a60c-223">Boolean</span></span>|<span data-ttu-id="2a60c-224">Установить для пропуска всех проверок перед перезапуском: уровень аккумулятора = 40%, присутствие пользователя, требуемое отображение, режим презентации, полноэкранный режим, состояние телефонного звонка, игровой режим и т. д.</span><span class="sxs-lookup"><span data-stu-id="2a60c-224">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="2a60c-225">упдатевикс</span><span class="sxs-lookup"><span data-stu-id="2a60c-225">updateWeeks</span></span>|[<span data-ttu-id="2a60c-226">виндовсупдатефорбусинессупдатевикс</span><span class="sxs-lookup"><span data-stu-id="2a60c-226">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="2a60c-227">Установка обновления запланирована на недели месяца.</span><span class="sxs-lookup"><span data-stu-id="2a60c-227">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="2a60c-228">Возможные значения: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span><span class="sxs-lookup"><span data-stu-id="2a60c-228">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="2a60c-229">куалитюпдатеспаусестартдате</span><span class="sxs-lookup"><span data-stu-id="2a60c-229">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="2a60c-230">Дата</span><span class="sxs-lookup"><span data-stu-id="2a60c-230">Date</span></span>|<span data-ttu-id="2a60c-231">Дата начала паузы обновлений.</span><span class="sxs-lookup"><span data-stu-id="2a60c-231">Quality Updates Pause start date.</span></span> <span data-ttu-id="2a60c-232">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2a60c-232">This property is read-only.</span></span>|
|<span data-ttu-id="2a60c-233">феатуреупдатеспаусестартдате</span><span class="sxs-lookup"><span data-stu-id="2a60c-233">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="2a60c-234">Дата</span><span class="sxs-lookup"><span data-stu-id="2a60c-234">Date</span></span>|<span data-ttu-id="2a60c-235">Дата начала паузы обновления компонентов.</span><span class="sxs-lookup"><span data-stu-id="2a60c-235">Feature Updates Pause start date.</span></span> <span data-ttu-id="2a60c-236">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2a60c-236">This property is read-only.</span></span>|
|<span data-ttu-id="2a60c-237">феатуреупдатесроллбакквиндовиндайс</span><span class="sxs-lookup"><span data-stu-id="2a60c-237">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="2a60c-238">Int32</span><span class="sxs-lookup"><span data-stu-id="2a60c-238">Int32</span></span>|<span data-ttu-id="2a60c-239">Количество дней после обновления компонента, для которого действует откат</span><span class="sxs-lookup"><span data-stu-id="2a60c-239">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="2a60c-240">куалитюпдатесвиллберолледбакк</span><span class="sxs-lookup"><span data-stu-id="2a60c-240">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="2a60c-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a60c-241">Boolean</span></span>|<span data-ttu-id="2a60c-242">Указывает, следует ли откатить обновление для следующего возврата устройства</span><span class="sxs-lookup"><span data-stu-id="2a60c-242">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="2a60c-243">феатуреупдатесвиллберолледбакк</span><span class="sxs-lookup"><span data-stu-id="2a60c-243">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="2a60c-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a60c-244">Boolean</span></span>|<span data-ttu-id="2a60c-245">Указывает, следует ли откатить обновления компонентов при следующем возврате устройства</span><span class="sxs-lookup"><span data-stu-id="2a60c-245">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="2a60c-246">куалитюпдатесроллбаккстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="2a60c-246">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="2a60c-247">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a60c-247">DateTimeOffset</span></span>|<span data-ttu-id="2a60c-248">Дата и время начала отката обновлений качества</span><span class="sxs-lookup"><span data-stu-id="2a60c-248">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="2a60c-249">феатуреупдатесроллбаккстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="2a60c-249">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="2a60c-250">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a60c-250">DateTimeOffset</span></span>|<span data-ttu-id="2a60c-251">Дата и время начала отката обновлений компонентов</span><span class="sxs-lookup"><span data-stu-id="2a60c-251">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="2a60c-252">енгажедрестартдеадлинеиндайс</span><span class="sxs-lookup"><span data-stu-id="2a60c-252">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="2a60c-253">Int32</span><span class="sxs-lookup"><span data-stu-id="2a60c-253">Int32</span></span>|<span data-ttu-id="2a60c-254">Крайний срок в днях перед автоматическим планированием и выполнением ожидающего перезапуска за пределами периода активности, с допустимым диапазоном от 2 до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="2a60c-254">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="2a60c-255">енгажедрестартснузесчедулеиндайс</span><span class="sxs-lookup"><span data-stu-id="2a60c-255">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="2a60c-256">Int32</span><span class="sxs-lookup"><span data-stu-id="2a60c-256">Int32</span></span>|<span data-ttu-id="2a60c-257">Количество дней, в течение которых пользователь может отложить уведомления о перезапуске с допустимым диапазоном от 1 до 3 дней</span><span class="sxs-lookup"><span data-stu-id="2a60c-257">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="2a60c-258">енгажедрестарттранситионсчедулеиндайс</span><span class="sxs-lookup"><span data-stu-id="2a60c-258">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="2a60c-259">Int32</span><span class="sxs-lookup"><span data-stu-id="2a60c-259">Int32</span></span>|<span data-ttu-id="2a60c-260">Количество дней перед переходом с автоматических перезапусков, запланированных за пределами активного времени до запланированного перезапуска, для которого пользователь должен запланировать, с допустимым диапазоном от 0 до 30 дней</span><span class="sxs-lookup"><span data-stu-id="2a60c-260">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="2a60c-261">деадлинефорфеатуреупдатесиндайс</span><span class="sxs-lookup"><span data-stu-id="2a60c-261">deadlineForFeatureUpdatesInDays</span></span>|<span data-ttu-id="2a60c-262">Int32</span><span class="sxs-lookup"><span data-stu-id="2a60c-262">Int32</span></span>|<span data-ttu-id="2a60c-263">Число дней до автоматического установки обновлений компонентов с допустимым диапазоном от 2 до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="2a60c-263">Number of days before feature updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="2a60c-264">деадлинефоркуалитюпдатесиндайс</span><span class="sxs-lookup"><span data-stu-id="2a60c-264">deadlineForQualityUpdatesInDays</span></span>|<span data-ttu-id="2a60c-265">Int32</span><span class="sxs-lookup"><span data-stu-id="2a60c-265">Int32</span></span>|<span data-ttu-id="2a60c-266">Количество дней до автоматического установления обновлений качества с допустимым диапазоном от 2 до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="2a60c-266">Number of days before quality updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="2a60c-267">деадлинеграцепериодиндайс</span><span class="sxs-lookup"><span data-stu-id="2a60c-267">deadlineGracePeriodInDays</span></span>|<span data-ttu-id="2a60c-268">Int32</span><span class="sxs-lookup"><span data-stu-id="2a60c-268">Int32</span></span>|<span data-ttu-id="2a60c-269">Срок действия перезапуска (в днях), по истечении которого он будет выполняться автоматически (от 0 до 7 дней)</span><span class="sxs-lookup"><span data-stu-id="2a60c-269">Number of days after deadline  until restarts occur automatically with valid range from 0 to 7 days</span></span>|
|<span data-ttu-id="2a60c-270">постпонеребутунтилафтердеадлине</span><span class="sxs-lookup"><span data-stu-id="2a60c-270">postponeRebootUntilAfterDeadline</span></span>|<span data-ttu-id="2a60c-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a60c-271">Boolean</span></span>|<span data-ttu-id="2a60c-272">Указывает, должно ли устройство ждать, пока не истечет время для перезагрузки в течение периода активности</span><span class="sxs-lookup"><span data-stu-id="2a60c-272">Specifies if the device should wait until deadline for rebooting outside of active hours</span></span>|
|<span data-ttu-id="2a60c-273">ауторестартнотификатиондисмиссал</span><span class="sxs-lookup"><span data-stu-id="2a60c-273">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="2a60c-274">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="2a60c-274">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="2a60c-275">Укажите метод закрытия уведомления об обязательном автоматическом перезапуске.</span><span class="sxs-lookup"><span data-stu-id="2a60c-275">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="2a60c-276">Возможные значения: `notConfigured`, `automatic`, `user`.</span><span class="sxs-lookup"><span data-stu-id="2a60c-276">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="2a60c-277">счедулерестартварнингинхаурс</span><span class="sxs-lookup"><span data-stu-id="2a60c-277">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="2a60c-278">Int32</span><span class="sxs-lookup"><span data-stu-id="2a60c-278">Int32</span></span>|<span data-ttu-id="2a60c-279">Укажите период уведомлений с напоминанием об автоматическом перезапуске.</span><span class="sxs-lookup"><span data-stu-id="2a60c-279">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="2a60c-280">Поддерживаемые значения: 2, 4, 8, 12 или 24 (часы).</span><span class="sxs-lookup"><span data-stu-id="2a60c-280">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="2a60c-281">счедулеимминентрестартварнингинминутес</span><span class="sxs-lookup"><span data-stu-id="2a60c-281">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="2a60c-282">Int32</span><span class="sxs-lookup"><span data-stu-id="2a60c-282">Int32</span></span>|<span data-ttu-id="2a60c-283">Укажите период, в котором автоматически перезапускаются уведомления о приближениях.</span><span class="sxs-lookup"><span data-stu-id="2a60c-283">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="2a60c-284">Поддерживаемые значения: 15, 30 или 60 (минут).</span><span class="sxs-lookup"><span data-stu-id="2a60c-284">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="2a60c-285">усерпаусеакцесс</span><span class="sxs-lookup"><span data-stu-id="2a60c-285">userPauseAccess</span></span>|[<span data-ttu-id="2a60c-286">Включение</span><span class="sxs-lookup"><span data-stu-id="2a60c-286">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="2a60c-287">Указывает, следует ли включить доступ конечного пользователя для приостановки обновлений программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="2a60c-287">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="2a60c-288">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="2a60c-288">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="2a60c-289">усервиндовсупдатесканакцесс</span><span class="sxs-lookup"><span data-stu-id="2a60c-289">userWindowsUpdateScanAccess</span></span>|[<span data-ttu-id="2a60c-290">Включение</span><span class="sxs-lookup"><span data-stu-id="2a60c-290">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="2a60c-291">Указывает, следует ли запретить доступ пользователя для сканирования центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="2a60c-291">Specifies whether to disable user’s access to scan Windows Update.</span></span> <span data-ttu-id="2a60c-292">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="2a60c-292">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="2a60c-293">упдатенотификатионлевел</span><span class="sxs-lookup"><span data-stu-id="2a60c-293">updateNotificationLevel</span></span>|[<span data-ttu-id="2a60c-294">windowsUpdateNotificationDisplayOption</span><span class="sxs-lookup"><span data-stu-id="2a60c-294">windowsUpdateNotificationDisplayOption</span></span>](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|<span data-ttu-id="2a60c-295">Указывает, что увидят пользователи уведомлений центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="2a60c-295">Specifies what Windows Update notifications users see.</span></span> <span data-ttu-id="2a60c-296">Возможные значения: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="2a60c-296">Possible values are: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span></span>|



## <a name="response"></a><span data-ttu-id="2a60c-297">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a60c-297">Response</span></span>
<span data-ttu-id="2a60c-298">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2a60c-298">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a60c-299">Пример</span><span class="sxs-lookup"><span data-stu-id="2a60c-299">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a60c-300">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a60c-300">Request</span></span>
<span data-ttu-id="2a60c-301">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a60c-301">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="2a60c-302">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a60c-302">Response</span></span>
<span data-ttu-id="2a60c-p126">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a60c-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





