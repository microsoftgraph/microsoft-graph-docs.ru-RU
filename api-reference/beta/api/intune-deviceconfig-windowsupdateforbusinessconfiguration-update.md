---
title: Обновление объекта windowsUpdateForBusinessConfiguration
description: Обновление свойств объекта windowsUpdateForBusinessConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b178b614f12ae193b1e2369a9c71e337978dde93
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961289"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="1b0e2-103">Обновление объекта windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="1b0e2-103">Update windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="1b0e2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b0e2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b0e2-106">Обновление свойств объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b0e2-106">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b0e2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1b0e2-107">Prerequisites</span></span>
<span data-ttu-id="1b0e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b0e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b0e2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b0e2-110">Permission type</span></span>|<span data-ttu-id="1b0e2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b0e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b0e2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b0e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1b0e2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b0e2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1b0e2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b0e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b0e2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-115">Not supported.</span></span>|
|<span data-ttu-id="1b0e2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b0e2-116">Application</span></span>|<span data-ttu-id="1b0e2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b0e2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b0e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1b0e2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b0e2-119">Request headers</span></span>
|<span data-ttu-id="1b0e2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b0e2-120">Header</span></span>|<span data-ttu-id="1b0e2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1b0e2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b0e2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b0e2-122">Authorization</span></span>|<span data-ttu-id="1b0e2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b0e2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1b0e2-124">Accept</span></span>|<span data-ttu-id="1b0e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1b0e2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b0e2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1b0e2-126">Request body</span></span>
<span data-ttu-id="1b0e2-127">В теле запроса добавьте представление объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-127">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="1b0e2-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b0e2-128">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="1b0e2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b0e2-129">Property</span></span>|<span data-ttu-id="1b0e2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1b0e2-130">Type</span></span>|<span data-ttu-id="1b0e2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1b0e2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b0e2-132">id</span><span class="sxs-lookup"><span data-stu-id="1b0e2-132">id</span></span>|<span data-ttu-id="1b0e2-133">String</span><span class="sxs-lookup"><span data-stu-id="1b0e2-133">String</span></span>|<span data-ttu-id="1b0e2-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-134">Key of the entity.</span></span> <span data-ttu-id="1b0e2-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b0e2-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b0e2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b0e2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1b0e2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b0e2-137">DateTimeOffset</span></span>|<span data-ttu-id="1b0e2-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1b0e2-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b0e2-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b0e2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1b0e2-140">roleScopeTagIds</span></span>|<span data-ttu-id="1b0e2-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1b0e2-141">String collection</span></span>|<span data-ttu-id="1b0e2-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1b0e2-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b0e2-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b0e2-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="1b0e2-144">supportsScopeTags</span></span>|<span data-ttu-id="1b0e2-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e2-145">Boolean</span></span>|<span data-ttu-id="1b0e2-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1b0e2-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1b0e2-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1b0e2-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-149">This property is read-only.</span></span> <span data-ttu-id="1b0e2-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b0e2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b0e2-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1b0e2-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1b0e2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1b0e2-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1b0e2-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1b0e2-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b0e2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b0e2-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1b0e2-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1b0e2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1b0e2-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1b0e2-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1b0e2-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b0e2-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b0e2-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="1b0e2-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1b0e2-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="1b0e2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1b0e2-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1b0e2-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b0e2-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b0e2-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b0e2-163">createdDateTime</span></span>|<span data-ttu-id="1b0e2-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b0e2-164">DateTimeOffset</span></span>|<span data-ttu-id="1b0e2-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-165">DateTime the object was created.</span></span> <span data-ttu-id="1b0e2-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b0e2-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b0e2-167">description</span><span class="sxs-lookup"><span data-stu-id="1b0e2-167">description</span></span>|<span data-ttu-id="1b0e2-168">String</span><span class="sxs-lookup"><span data-stu-id="1b0e2-168">String</span></span>|<span data-ttu-id="1b0e2-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1b0e2-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b0e2-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b0e2-171">displayName</span><span class="sxs-lookup"><span data-stu-id="1b0e2-171">displayName</span></span>|<span data-ttu-id="1b0e2-172">Строка</span><span class="sxs-lookup"><span data-stu-id="1b0e2-172">String</span></span>|<span data-ttu-id="1b0e2-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1b0e2-174">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b0e2-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b0e2-175">version</span><span class="sxs-lookup"><span data-stu-id="1b0e2-175">version</span></span>|<span data-ttu-id="1b0e2-176">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0e2-176">Int32</span></span>|<span data-ttu-id="1b0e2-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-177">Version of the device configuration.</span></span> <span data-ttu-id="1b0e2-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1b0e2-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b0e2-179">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="1b0e2-179">deliveryOptimizationMode</span></span>|[<span data-ttu-id="1b0e2-180">Виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="1b0e2-180">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="1b0e2-181">Режим оптимизации доставки.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-181">Delivery Optimization Mode.</span></span> <span data-ttu-id="1b0e2-182">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-182">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="1b0e2-183">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="1b0e2-183">prereleaseFeatures</span></span>|[<span data-ttu-id="1b0e2-184">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="1b0e2-184">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="1b0e2-185">Функции предварительного выпуска.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-185">The pre-release features.</span></span> <span data-ttu-id="1b0e2-186">Возможные значения: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-186">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="1b0e2-187">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="1b0e2-187">automaticUpdateMode</span></span>|[<span data-ttu-id="1b0e2-188">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="1b0e2-188">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="1b0e2-189">Режим автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-189">Automatic update mode.</span></span> <span data-ttu-id="1b0e2-190">Возможные значения: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-190">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="1b0e2-191">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="1b0e2-191">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="1b0e2-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e2-192">Boolean</span></span>|<span data-ttu-id="1b0e2-193">Разрешение использования службы обновлений (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="1b0e2-193">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="1b0e2-194">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="1b0e2-194">driversExcluded</span></span>|<span data-ttu-id="1b0e2-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e2-195">Boolean</span></span>|<span data-ttu-id="1b0e2-196">Исключение драйверов из Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-196">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="1b0e2-197">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="1b0e2-197">installationSchedule</span></span>|[<span data-ttu-id="1b0e2-198">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="1b0e2-198">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="1b0e2-199">Расписание установки.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-199">Installation schedule</span></span>|
|<span data-ttu-id="1b0e2-200">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="1b0e2-200">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="1b0e2-201">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0e2-201">Int32</span></span>|<span data-ttu-id="1b0e2-202">Откладывание исправлений на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-202">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="1b0e2-203">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="1b0e2-203">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="1b0e2-204">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0e2-204">Int32</span></span>|<span data-ttu-id="1b0e2-205">Откладывание обновлений компонентов на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-205">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="1b0e2-206">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="1b0e2-206">qualityUpdatesPaused</span></span>|<span data-ttu-id="1b0e2-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e2-207">Boolean</span></span>|<span data-ttu-id="1b0e2-208">Приостановка исправлений.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-208">Pause Quality Updates</span></span>|
|<span data-ttu-id="1b0e2-209">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="1b0e2-209">featureUpdatesPaused</span></span>|<span data-ttu-id="1b0e2-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e2-210">Boolean</span></span>|<span data-ttu-id="1b0e2-211">Приостановка обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-211">Pause Feature Updates</span></span>|
|<span data-ttu-id="1b0e2-212">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="1b0e2-212">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="1b0e2-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b0e2-213">DateTimeOffset</span></span>|<span data-ttu-id="1b0e2-214">Дата и время завершения срока приостановки исправлений.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-214">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="1b0e2-215">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="1b0e2-215">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="1b0e2-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b0e2-216">DateTimeOffset</span></span>|<span data-ttu-id="1b0e2-217">Дата и время, когда будет завершен срок приостановки обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-217">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="1b0e2-218">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="1b0e2-218">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="1b0e2-219">Виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="1b0e2-219">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="1b0e2-220">Определяет, от каких устройств филиала будут получаться обновления.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-220">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="1b0e2-221">Возможные значения: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-221">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="1b0e2-222">Скипчекксбефоререстарт</span><span class="sxs-lookup"><span data-stu-id="1b0e2-222">skipChecksBeforeRestart</span></span>|<span data-ttu-id="1b0e2-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e2-223">Boolean</span></span>|<span data-ttu-id="1b0e2-224">Установить для пропуска всех проверок перед перезапуском: уровень аккумулятора = 40%, присутствие пользователя, требуемое отображение, режим презентации, полноэкранный режим, состояние телефонного звонка, игровой режим и т. д.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-224">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="1b0e2-225">Упдатевикс</span><span class="sxs-lookup"><span data-stu-id="1b0e2-225">updateWeeks</span></span>|[<span data-ttu-id="1b0e2-226">Виндовсупдатефорбусинессупдатевикс</span><span class="sxs-lookup"><span data-stu-id="1b0e2-226">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="1b0e2-227">Установка обновления запланирована на недели месяца.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-227">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="1b0e2-228">Возможные значения: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-228">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="1b0e2-229">Куалитюпдатеспаусестартдате</span><span class="sxs-lookup"><span data-stu-id="1b0e2-229">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="1b0e2-230">Дата</span><span class="sxs-lookup"><span data-stu-id="1b0e2-230">Date</span></span>|<span data-ttu-id="1b0e2-231">Дата начала паузы обновлений.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-231">Quality Updates Pause start date.</span></span> <span data-ttu-id="1b0e2-232">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-232">This property is read-only.</span></span>|
|<span data-ttu-id="1b0e2-233">Феатуреупдатеспаусестартдате</span><span class="sxs-lookup"><span data-stu-id="1b0e2-233">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="1b0e2-234">Дата</span><span class="sxs-lookup"><span data-stu-id="1b0e2-234">Date</span></span>|<span data-ttu-id="1b0e2-235">Дата начала паузы обновления компонентов.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-235">Feature Updates Pause start date.</span></span> <span data-ttu-id="1b0e2-236">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-236">This property is read-only.</span></span>|
|<span data-ttu-id="1b0e2-237">Феатуреупдатесроллбакквиндовиндайс</span><span class="sxs-lookup"><span data-stu-id="1b0e2-237">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="1b0e2-238">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0e2-238">Int32</span></span>|<span data-ttu-id="1b0e2-239">Количество дней после обновления компонента, для которого действует откат</span><span class="sxs-lookup"><span data-stu-id="1b0e2-239">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="1b0e2-240">Куалитюпдатесвиллберолледбакк</span><span class="sxs-lookup"><span data-stu-id="1b0e2-240">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="1b0e2-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e2-241">Boolean</span></span>|<span data-ttu-id="1b0e2-242">Указывает, следует ли откатить обновление для следующего возврата устройства</span><span class="sxs-lookup"><span data-stu-id="1b0e2-242">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="1b0e2-243">Феатуреупдатесвиллберолледбакк</span><span class="sxs-lookup"><span data-stu-id="1b0e2-243">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="1b0e2-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e2-244">Boolean</span></span>|<span data-ttu-id="1b0e2-245">Указывает, следует ли откатить обновления компонентов при следующем возврате устройства</span><span class="sxs-lookup"><span data-stu-id="1b0e2-245">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="1b0e2-246">Куалитюпдатесроллбаккстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="1b0e2-246">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="1b0e2-247">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b0e2-247">DateTimeOffset</span></span>|<span data-ttu-id="1b0e2-248">Дата и время начала отката обновлений качества</span><span class="sxs-lookup"><span data-stu-id="1b0e2-248">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="1b0e2-249">Феатуреупдатесроллбаккстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="1b0e2-249">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="1b0e2-250">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b0e2-250">DateTimeOffset</span></span>|<span data-ttu-id="1b0e2-251">Дата и время начала отката обновлений компонентов</span><span class="sxs-lookup"><span data-stu-id="1b0e2-251">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="1b0e2-252">Енгажедрестартдеадлинеиндайс</span><span class="sxs-lookup"><span data-stu-id="1b0e2-252">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="1b0e2-253">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0e2-253">Int32</span></span>|<span data-ttu-id="1b0e2-254">Крайний срок в днях перед автоматическим планированием и выполнением ожидающего перезапуска за пределами периода активности, с допустимым диапазоном от 2 до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-254">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="1b0e2-255">Енгажедрестартснузесчедулеиндайс</span><span class="sxs-lookup"><span data-stu-id="1b0e2-255">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="1b0e2-256">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0e2-256">Int32</span></span>|<span data-ttu-id="1b0e2-257">Количество дней, в течение которых пользователь может отложить уведомления о перезапуске с допустимым диапазоном от 1 до 3 дней</span><span class="sxs-lookup"><span data-stu-id="1b0e2-257">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="1b0e2-258">Енгажедрестарттранситионсчедулеиндайс</span><span class="sxs-lookup"><span data-stu-id="1b0e2-258">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="1b0e2-259">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0e2-259">Int32</span></span>|<span data-ttu-id="1b0e2-260">Количество дней перед переходом с автоматических перезапусков, запланированных за пределами активного времени до запланированного перезапуска, для которого пользователь должен запланировать, с допустимым диапазоном от 0 до 30 дней</span><span class="sxs-lookup"><span data-stu-id="1b0e2-260">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="1b0e2-261">Ауторестартнотификатиондисмиссал</span><span class="sxs-lookup"><span data-stu-id="1b0e2-261">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="1b0e2-262">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="1b0e2-262">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="1b0e2-263">Укажите метод закрытия уведомления об обязательном автоматическом перезапуске.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-263">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="1b0e2-264">Возможные значения: `notConfigured`, `automatic`, `user`.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-264">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="1b0e2-265">Счедулерестартварнингинхаурс</span><span class="sxs-lookup"><span data-stu-id="1b0e2-265">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="1b0e2-266">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0e2-266">Int32</span></span>|<span data-ttu-id="1b0e2-267">Укажите период уведомлений с напоминанием об автоматическом перезапуске.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-267">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="1b0e2-268">Поддерживаемые значения: 2, 4, 8, 12 или 24 (часы).</span><span class="sxs-lookup"><span data-stu-id="1b0e2-268">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="1b0e2-269">Счедулеимминентрестартварнингинминутес</span><span class="sxs-lookup"><span data-stu-id="1b0e2-269">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="1b0e2-270">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0e2-270">Int32</span></span>|<span data-ttu-id="1b0e2-271">Укажите период, в котором автоматически перезапускаются уведомления о приближениях.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-271">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="1b0e2-272">Поддерживаемые значения: 15, 30 или 60 (минут).</span><span class="sxs-lookup"><span data-stu-id="1b0e2-272">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="1b0e2-273">Усерпаусеакцесс</span><span class="sxs-lookup"><span data-stu-id="1b0e2-273">userPauseAccess</span></span>|[<span data-ttu-id="1b0e2-274">Включение</span><span class="sxs-lookup"><span data-stu-id="1b0e2-274">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="1b0e2-275">Указывает, следует ли включить доступ конечного пользователя для приостановки обновлений программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-275">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="1b0e2-276">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-276">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="1b0e2-277">Усервиндовсупдатесканакцесс</span><span class="sxs-lookup"><span data-stu-id="1b0e2-277">userWindowsUpdateScanAccess</span></span>|[<span data-ttu-id="1b0e2-278">Включение</span><span class="sxs-lookup"><span data-stu-id="1b0e2-278">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="1b0e2-279">Указывает, следует ли запретить доступ пользователя для сканирования центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-279">Specifies whether to disable user’s access to scan Windows Update.</span></span> <span data-ttu-id="1b0e2-280">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-280">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="1b0e2-281">Упдатенотификатионлевел</span><span class="sxs-lookup"><span data-stu-id="1b0e2-281">updateNotificationLevel</span></span>|[<span data-ttu-id="1b0e2-282">windowsUpdateNotificationDisplayOption</span><span class="sxs-lookup"><span data-stu-id="1b0e2-282">windowsUpdateNotificationDisplayOption</span></span>](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|<span data-ttu-id="1b0e2-283">Указывает, что увидят пользователи уведомлений центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-283">Specifies what Windows Update notifications users see.</span></span> <span data-ttu-id="1b0e2-284">Возможные значения: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-284">Possible values are: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span></span>|



## <a name="response"></a><span data-ttu-id="1b0e2-285">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b0e2-285">Response</span></span>
<span data-ttu-id="1b0e2-286">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-286">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b0e2-287">Пример</span><span class="sxs-lookup"><span data-stu-id="1b0e2-287">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b0e2-288">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b0e2-288">Request</span></span>
<span data-ttu-id="1b0e2-289">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-289">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2676

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
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```

### <a name="response"></a><span data-ttu-id="1b0e2-290">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b0e2-290">Response</span></span>
<span data-ttu-id="1b0e2-p126">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b0e2-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2848

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
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```





