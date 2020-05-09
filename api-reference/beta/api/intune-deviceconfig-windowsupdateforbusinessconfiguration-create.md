---
title: Create windowsUpdateForBusinessConfiguration
description: Создание объекта windowsUpdateForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d825e9bef490a0a658416d086859bbc72e554e75
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178957"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="5f8eb-103">Create windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="5f8eb-103">Create windowsUpdateForBusinessConfiguration</span></span>

<span data-ttu-id="5f8eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f8eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f8eb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f8eb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f8eb-107">Создание объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f8eb-107">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f8eb-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5f8eb-108">Prerequisites</span></span>
<span data-ttu-id="5f8eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f8eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f8eb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f8eb-111">Permission type</span></span>|<span data-ttu-id="5f8eb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f8eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f8eb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f8eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5f8eb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f8eb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5f8eb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f8eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f8eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-116">Not supported.</span></span>|
|<span data-ttu-id="5f8eb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f8eb-117">Application</span></span>|<span data-ttu-id="5f8eb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f8eb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f8eb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f8eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5f8eb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5f8eb-120">Request headers</span></span>
|<span data-ttu-id="5f8eb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5f8eb-121">Header</span></span>|<span data-ttu-id="5f8eb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5f8eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f8eb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f8eb-123">Authorization</span></span>|<span data-ttu-id="5f8eb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f8eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5f8eb-125">Accept</span></span>|<span data-ttu-id="5f8eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f8eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f8eb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f8eb-127">Request body</span></span>
<span data-ttu-id="5f8eb-128">В тексте запроса добавьте представление объекта windowsUpdateForBusinessConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-128">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="5f8eb-129">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта windowsUpdateForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-129">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="5f8eb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f8eb-130">Property</span></span>|<span data-ttu-id="5f8eb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5f8eb-131">Type</span></span>|<span data-ttu-id="5f8eb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5f8eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f8eb-133">id</span><span class="sxs-lookup"><span data-stu-id="5f8eb-133">id</span></span>|<span data-ttu-id="5f8eb-134">String</span><span class="sxs-lookup"><span data-stu-id="5f8eb-134">String</span></span>|<span data-ttu-id="5f8eb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-135">Key of the entity.</span></span> <span data-ttu-id="5f8eb-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f8eb-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f8eb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f8eb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5f8eb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f8eb-138">DateTimeOffset</span></span>|<span data-ttu-id="5f8eb-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5f8eb-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f8eb-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f8eb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5f8eb-141">roleScopeTagIds</span></span>|<span data-ttu-id="5f8eb-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="5f8eb-142">String collection</span></span>|<span data-ttu-id="5f8eb-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5f8eb-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f8eb-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f8eb-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="5f8eb-145">supportsScopeTags</span></span>|<span data-ttu-id="5f8eb-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f8eb-146">Boolean</span></span>|<span data-ttu-id="5f8eb-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5f8eb-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5f8eb-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5f8eb-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-150">This property is read-only.</span></span> <span data-ttu-id="5f8eb-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f8eb-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f8eb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5f8eb-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5f8eb-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5f8eb-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5f8eb-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5f8eb-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f8eb-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f8eb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5f8eb-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5f8eb-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5f8eb-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5f8eb-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5f8eb-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f8eb-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f8eb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5f8eb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5f8eb-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5f8eb-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5f8eb-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5f8eb-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f8eb-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f8eb-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5f8eb-164">createdDateTime</span></span>|<span data-ttu-id="5f8eb-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f8eb-165">DateTimeOffset</span></span>|<span data-ttu-id="5f8eb-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-166">DateTime the object was created.</span></span> <span data-ttu-id="5f8eb-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f8eb-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f8eb-168">description</span><span class="sxs-lookup"><span data-stu-id="5f8eb-168">description</span></span>|<span data-ttu-id="5f8eb-169">String</span><span class="sxs-lookup"><span data-stu-id="5f8eb-169">String</span></span>|<span data-ttu-id="5f8eb-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5f8eb-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f8eb-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f8eb-172">displayName</span><span class="sxs-lookup"><span data-stu-id="5f8eb-172">displayName</span></span>|<span data-ttu-id="5f8eb-173">Строка</span><span class="sxs-lookup"><span data-stu-id="5f8eb-173">String</span></span>|<span data-ttu-id="5f8eb-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5f8eb-175">Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5f8eb-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f8eb-176">version</span><span class="sxs-lookup"><span data-stu-id="5f8eb-176">version</span></span>|<span data-ttu-id="5f8eb-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5f8eb-177">Int32</span></span>|<span data-ttu-id="5f8eb-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-178">Version of the device configuration.</span></span> <span data-ttu-id="5f8eb-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5f8eb-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5f8eb-180">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="5f8eb-180">deliveryOptimizationMode</span></span>|[<span data-ttu-id="5f8eb-181">виндовсделиверйоптимизатионмоде</span><span class="sxs-lookup"><span data-stu-id="5f8eb-181">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="5f8eb-182">Режим оптимизации доставки.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-182">Delivery Optimization Mode.</span></span> <span data-ttu-id="5f8eb-183">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-183">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="5f8eb-184">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="5f8eb-184">prereleaseFeatures</span></span>|[<span data-ttu-id="5f8eb-185">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="5f8eb-185">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="5f8eb-186">Функции предварительного выпуска.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-186">The pre-release features.</span></span> <span data-ttu-id="5f8eb-187">Возможные значения: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-187">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="5f8eb-188">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="5f8eb-188">automaticUpdateMode</span></span>|[<span data-ttu-id="5f8eb-189">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="5f8eb-189">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="5f8eb-190">Режим автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-190">Automatic update mode.</span></span> <span data-ttu-id="5f8eb-191">Возможные значения: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-191">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="5f8eb-192">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="5f8eb-192">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="5f8eb-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f8eb-193">Boolean</span></span>|<span data-ttu-id="5f8eb-194">Разрешение использования службы обновлений (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="5f8eb-194">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="5f8eb-195">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="5f8eb-195">driversExcluded</span></span>|<span data-ttu-id="5f8eb-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f8eb-196">Boolean</span></span>|<span data-ttu-id="5f8eb-197">Исключение драйверов из Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-197">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="5f8eb-198">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="5f8eb-198">installationSchedule</span></span>|[<span data-ttu-id="5f8eb-199">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="5f8eb-199">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="5f8eb-200">Расписание установки.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-200">Installation schedule</span></span>|
|<span data-ttu-id="5f8eb-201">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="5f8eb-201">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="5f8eb-202">Int32</span><span class="sxs-lookup"><span data-stu-id="5f8eb-202">Int32</span></span>|<span data-ttu-id="5f8eb-203">Откладывание исправлений на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-203">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="5f8eb-204">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="5f8eb-204">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="5f8eb-205">Int32</span><span class="sxs-lookup"><span data-stu-id="5f8eb-205">Int32</span></span>|<span data-ttu-id="5f8eb-206">Откладывание обновлений компонентов на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-206">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="5f8eb-207">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="5f8eb-207">qualityUpdatesPaused</span></span>|<span data-ttu-id="5f8eb-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f8eb-208">Boolean</span></span>|<span data-ttu-id="5f8eb-209">Приостановка исправлений.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-209">Pause Quality Updates</span></span>|
|<span data-ttu-id="5f8eb-210">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="5f8eb-210">featureUpdatesPaused</span></span>|<span data-ttu-id="5f8eb-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f8eb-211">Boolean</span></span>|<span data-ttu-id="5f8eb-212">Приостановка обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-212">Pause Feature Updates</span></span>|
|<span data-ttu-id="5f8eb-213">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="5f8eb-213">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="5f8eb-214">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f8eb-214">DateTimeOffset</span></span>|<span data-ttu-id="5f8eb-215">Дата и время завершения срока приостановки исправлений.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-215">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="5f8eb-216">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="5f8eb-216">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="5f8eb-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f8eb-217">DateTimeOffset</span></span>|<span data-ttu-id="5f8eb-218">Дата и время, когда будет завершен срок приостановки обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-218">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="5f8eb-219">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="5f8eb-219">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="5f8eb-220">виндовсупдатетипе</span><span class="sxs-lookup"><span data-stu-id="5f8eb-220">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="5f8eb-221">Определяет, от каких устройств филиала будут получаться обновления.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-221">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="5f8eb-222">Возможные значения: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-222">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="5f8eb-223">скипчекксбефоререстарт</span><span class="sxs-lookup"><span data-stu-id="5f8eb-223">skipChecksBeforeRestart</span></span>|<span data-ttu-id="5f8eb-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f8eb-224">Boolean</span></span>|<span data-ttu-id="5f8eb-225">Установить для пропуска всех проверок перед перезапуском: уровень аккумулятора = 40%, присутствие пользователя, требуемое отображение, режим презентации, полноэкранный режим, состояние телефонного звонка, игровой режим и т. д.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-225">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="5f8eb-226">упдатевикс</span><span class="sxs-lookup"><span data-stu-id="5f8eb-226">updateWeeks</span></span>|[<span data-ttu-id="5f8eb-227">виндовсупдатефорбусинессупдатевикс</span><span class="sxs-lookup"><span data-stu-id="5f8eb-227">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="5f8eb-228">Установка обновления запланирована на недели месяца.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-228">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="5f8eb-229">Возможные значения: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-229">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="5f8eb-230">куалитюпдатеспаусестартдате</span><span class="sxs-lookup"><span data-stu-id="5f8eb-230">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="5f8eb-231">Дата</span><span class="sxs-lookup"><span data-stu-id="5f8eb-231">Date</span></span>|<span data-ttu-id="5f8eb-232">Дата начала паузы обновлений.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-232">Quality Updates Pause start date.</span></span> <span data-ttu-id="5f8eb-233">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-233">This property is read-only.</span></span>|
|<span data-ttu-id="5f8eb-234">феатуреупдатеспаусестартдате</span><span class="sxs-lookup"><span data-stu-id="5f8eb-234">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="5f8eb-235">Дата</span><span class="sxs-lookup"><span data-stu-id="5f8eb-235">Date</span></span>|<span data-ttu-id="5f8eb-236">Дата начала паузы обновления компонентов.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-236">Feature Updates Pause start date.</span></span> <span data-ttu-id="5f8eb-237">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-237">This property is read-only.</span></span>|
|<span data-ttu-id="5f8eb-238">феатуреупдатесроллбакквиндовиндайс</span><span class="sxs-lookup"><span data-stu-id="5f8eb-238">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="5f8eb-239">Int32</span><span class="sxs-lookup"><span data-stu-id="5f8eb-239">Int32</span></span>|<span data-ttu-id="5f8eb-240">Количество дней после обновления компонента, для которого действует откат</span><span class="sxs-lookup"><span data-stu-id="5f8eb-240">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="5f8eb-241">куалитюпдатесвиллберолледбакк</span><span class="sxs-lookup"><span data-stu-id="5f8eb-241">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="5f8eb-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f8eb-242">Boolean</span></span>|<span data-ttu-id="5f8eb-243">Указывает, следует ли откатить обновление для следующего возврата устройства</span><span class="sxs-lookup"><span data-stu-id="5f8eb-243">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="5f8eb-244">феатуреупдатесвиллберолледбакк</span><span class="sxs-lookup"><span data-stu-id="5f8eb-244">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="5f8eb-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f8eb-245">Boolean</span></span>|<span data-ttu-id="5f8eb-246">Указывает, следует ли откатить обновления компонентов при следующем возврате устройства</span><span class="sxs-lookup"><span data-stu-id="5f8eb-246">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="5f8eb-247">куалитюпдатесроллбаккстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="5f8eb-247">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="5f8eb-248">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f8eb-248">DateTimeOffset</span></span>|<span data-ttu-id="5f8eb-249">Дата и время начала отката обновлений качества</span><span class="sxs-lookup"><span data-stu-id="5f8eb-249">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="5f8eb-250">феатуреупдатесроллбаккстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="5f8eb-250">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="5f8eb-251">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f8eb-251">DateTimeOffset</span></span>|<span data-ttu-id="5f8eb-252">Дата и время начала отката обновлений компонентов</span><span class="sxs-lookup"><span data-stu-id="5f8eb-252">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="5f8eb-253">енгажедрестартдеадлинеиндайс</span><span class="sxs-lookup"><span data-stu-id="5f8eb-253">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="5f8eb-254">Int32</span><span class="sxs-lookup"><span data-stu-id="5f8eb-254">Int32</span></span>|<span data-ttu-id="5f8eb-255">Крайний срок в днях перед автоматическим планированием и выполнением ожидающего перезапуска за пределами периода активности, с допустимым диапазоном от 2 до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-255">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="5f8eb-256">енгажедрестартснузесчедулеиндайс</span><span class="sxs-lookup"><span data-stu-id="5f8eb-256">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="5f8eb-257">Int32</span><span class="sxs-lookup"><span data-stu-id="5f8eb-257">Int32</span></span>|<span data-ttu-id="5f8eb-258">Количество дней, в течение которых пользователь может отложить уведомления о перезапуске с допустимым диапазоном от 1 до 3 дней</span><span class="sxs-lookup"><span data-stu-id="5f8eb-258">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="5f8eb-259">енгажедрестарттранситионсчедулеиндайс</span><span class="sxs-lookup"><span data-stu-id="5f8eb-259">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="5f8eb-260">Int32</span><span class="sxs-lookup"><span data-stu-id="5f8eb-260">Int32</span></span>|<span data-ttu-id="5f8eb-261">Количество дней перед переходом с автоматических перезапусков, запланированных за пределами активного времени до запланированного перезапуска, для которого пользователь должен запланировать, с допустимым диапазоном от 0 до 30 дней</span><span class="sxs-lookup"><span data-stu-id="5f8eb-261">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="5f8eb-262">деадлинефорфеатуреупдатесиндайс</span><span class="sxs-lookup"><span data-stu-id="5f8eb-262">deadlineForFeatureUpdatesInDays</span></span>|<span data-ttu-id="5f8eb-263">Int32</span><span class="sxs-lookup"><span data-stu-id="5f8eb-263">Int32</span></span>|<span data-ttu-id="5f8eb-264">Число дней до автоматического установки обновлений компонентов с допустимым диапазоном от 2 до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-264">Number of days before feature updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="5f8eb-265">деадлинефоркуалитюпдатесиндайс</span><span class="sxs-lookup"><span data-stu-id="5f8eb-265">deadlineForQualityUpdatesInDays</span></span>|<span data-ttu-id="5f8eb-266">Int32</span><span class="sxs-lookup"><span data-stu-id="5f8eb-266">Int32</span></span>|<span data-ttu-id="5f8eb-267">Количество дней до автоматического установления обновлений качества с допустимым диапазоном от 2 до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-267">Number of days before quality updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="5f8eb-268">деадлинеграцепериодиндайс</span><span class="sxs-lookup"><span data-stu-id="5f8eb-268">deadlineGracePeriodInDays</span></span>|<span data-ttu-id="5f8eb-269">Int32</span><span class="sxs-lookup"><span data-stu-id="5f8eb-269">Int32</span></span>|<span data-ttu-id="5f8eb-270">Срок действия перезапуска (в днях), по истечении которого он будет выполняться автоматически (от 0 до 7 дней)</span><span class="sxs-lookup"><span data-stu-id="5f8eb-270">Number of days after deadline  until restarts occur automatically with valid range from 0 to 7 days</span></span>|
|<span data-ttu-id="5f8eb-271">постпонеребутунтилафтердеадлине</span><span class="sxs-lookup"><span data-stu-id="5f8eb-271">postponeRebootUntilAfterDeadline</span></span>|<span data-ttu-id="5f8eb-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f8eb-272">Boolean</span></span>|<span data-ttu-id="5f8eb-273">Указывает, должно ли устройство ждать, пока не истечет время для перезагрузки в течение периода активности</span><span class="sxs-lookup"><span data-stu-id="5f8eb-273">Specifies if the device should wait until deadline for rebooting outside of active hours</span></span>|
|<span data-ttu-id="5f8eb-274">ауторестартнотификатиондисмиссал</span><span class="sxs-lookup"><span data-stu-id="5f8eb-274">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="5f8eb-275">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="5f8eb-275">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="5f8eb-276">Укажите метод закрытия уведомления об обязательном автоматическом перезапуске.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-276">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="5f8eb-277">Возможные значения: `notConfigured`, `automatic`, `user`.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-277">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="5f8eb-278">счедулерестартварнингинхаурс</span><span class="sxs-lookup"><span data-stu-id="5f8eb-278">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="5f8eb-279">Int32</span><span class="sxs-lookup"><span data-stu-id="5f8eb-279">Int32</span></span>|<span data-ttu-id="5f8eb-280">Укажите период уведомлений с напоминанием об автоматическом перезапуске.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-280">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="5f8eb-281">Поддерживаемые значения: 2, 4, 8, 12 или 24 (часы).</span><span class="sxs-lookup"><span data-stu-id="5f8eb-281">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="5f8eb-282">счедулеимминентрестартварнингинминутес</span><span class="sxs-lookup"><span data-stu-id="5f8eb-282">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="5f8eb-283">Int32</span><span class="sxs-lookup"><span data-stu-id="5f8eb-283">Int32</span></span>|<span data-ttu-id="5f8eb-284">Укажите период, в котором автоматически перезапускаются уведомления о приближениях.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-284">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="5f8eb-285">Поддерживаемые значения: 15, 30 или 60 (минут).</span><span class="sxs-lookup"><span data-stu-id="5f8eb-285">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="5f8eb-286">усерпаусеакцесс</span><span class="sxs-lookup"><span data-stu-id="5f8eb-286">userPauseAccess</span></span>|[<span data-ttu-id="5f8eb-287">Включение</span><span class="sxs-lookup"><span data-stu-id="5f8eb-287">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="5f8eb-288">Указывает, следует ли включить доступ конечного пользователя для приостановки обновлений программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-288">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="5f8eb-289">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-289">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="5f8eb-290">усервиндовсупдатесканакцесс</span><span class="sxs-lookup"><span data-stu-id="5f8eb-290">userWindowsUpdateScanAccess</span></span>|[<span data-ttu-id="5f8eb-291">Включение</span><span class="sxs-lookup"><span data-stu-id="5f8eb-291">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="5f8eb-292">Указывает, следует ли запретить доступ пользователя для сканирования центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-292">Specifies whether to disable user’s access to scan Windows Update.</span></span> <span data-ttu-id="5f8eb-293">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-293">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="5f8eb-294">упдатенотификатионлевел</span><span class="sxs-lookup"><span data-stu-id="5f8eb-294">updateNotificationLevel</span></span>|[<span data-ttu-id="5f8eb-295">windowsUpdateNotificationDisplayOption</span><span class="sxs-lookup"><span data-stu-id="5f8eb-295">windowsUpdateNotificationDisplayOption</span></span>](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|<span data-ttu-id="5f8eb-296">Указывает, что увидят пользователи уведомлений центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-296">Specifies what Windows Update notifications users see.</span></span> <span data-ttu-id="5f8eb-297">Возможные значения: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-297">Possible values are: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span></span>|



## <a name="response"></a><span data-ttu-id="5f8eb-298">Ответ</span><span class="sxs-lookup"><span data-stu-id="5f8eb-298">Response</span></span>
<span data-ttu-id="5f8eb-299">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-299">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f8eb-300">Пример</span><span class="sxs-lookup"><span data-stu-id="5f8eb-300">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f8eb-301">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f8eb-301">Request</span></span>
<span data-ttu-id="5f8eb-302">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-302">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2794

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
  "qualityUpdatesPauseStartDate": "2016-12-31",
  "featureUpdatesPauseStartDate": "2016-12-31",
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

### <a name="response"></a><span data-ttu-id="5f8eb-303">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f8eb-303">Response</span></span>
<span data-ttu-id="5f8eb-p126">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f8eb-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2966

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
  "qualityUpdatesPauseStartDate": "2016-12-31",
  "featureUpdatesPauseStartDate": "2016-12-31",
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



