---
title: Обновление объекта windowsUpdateForBusinessConfiguration
description: Обновление свойств объекта windowsUpdateForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cf6816b8aa6a79a7f4b2b6f1a56f91a4ef319de1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127223"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="a49f8-103">Обновление объекта windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="a49f8-103">Update windowsUpdateForBusinessConfiguration</span></span>

<span data-ttu-id="a49f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a49f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a49f8-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a49f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a49f8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a49f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a49f8-107">Обновление свойств объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a49f8-107">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a49f8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a49f8-108">Prerequisites</span></span>
<span data-ttu-id="a49f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a49f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a49f8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a49f8-111">Permission type</span></span>|<span data-ttu-id="a49f8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a49f8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a49f8-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a49f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a49f8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a49f8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a49f8-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a49f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a49f8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a49f8-116">Not supported.</span></span>|
|<span data-ttu-id="a49f8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a49f8-117">Application</span></span>|<span data-ttu-id="a49f8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a49f8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a49f8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a49f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a49f8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a49f8-120">Request headers</span></span>
|<span data-ttu-id="a49f8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a49f8-121">Header</span></span>|<span data-ttu-id="a49f8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a49f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a49f8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a49f8-123">Authorization</span></span>|<span data-ttu-id="a49f8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a49f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a49f8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a49f8-125">Accept</span></span>|<span data-ttu-id="a49f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a49f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a49f8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a49f8-127">Request body</span></span>
<span data-ttu-id="a49f8-128">В теле запроса добавьте представление объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a49f8-128">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="a49f8-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a49f8-129">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="a49f8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a49f8-130">Property</span></span>|<span data-ttu-id="a49f8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a49f8-131">Type</span></span>|<span data-ttu-id="a49f8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a49f8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a49f8-133">id</span><span class="sxs-lookup"><span data-stu-id="a49f8-133">id</span></span>|<span data-ttu-id="a49f8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a49f8-134">String</span></span>|<span data-ttu-id="a49f8-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a49f8-135">Key of the entity.</span></span> <span data-ttu-id="a49f8-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a49f8-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a49f8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a49f8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a49f8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a49f8-138">DateTimeOffset</span></span>|<span data-ttu-id="a49f8-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a49f8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a49f8-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a49f8-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a49f8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a49f8-141">roleScopeTagIds</span></span>|<span data-ttu-id="a49f8-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a49f8-142">String collection</span></span>|<span data-ttu-id="a49f8-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="a49f8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a49f8-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a49f8-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a49f8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a49f8-145">supportsScopeTags</span></span>|<span data-ttu-id="a49f8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a49f8-146">Boolean</span></span>|<span data-ttu-id="a49f8-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a49f8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a49f8-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="a49f8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a49f8-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a49f8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a49f8-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a49f8-150">This property is read-only.</span></span> <span data-ttu-id="a49f8-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a49f8-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a49f8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a49f8-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a49f8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a49f8-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a49f8-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a49f8-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a49f8-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a49f8-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a49f8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a49f8-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a49f8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a49f8-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a49f8-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a49f8-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a49f8-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a49f8-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a49f8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a49f8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a49f8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a49f8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a49f8-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a49f8-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a49f8-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a49f8-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a49f8-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a49f8-164">createdDateTime</span></span>|<span data-ttu-id="a49f8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a49f8-165">DateTimeOffset</span></span>|<span data-ttu-id="a49f8-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a49f8-166">DateTime the object was created.</span></span> <span data-ttu-id="a49f8-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a49f8-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a49f8-168">description</span><span class="sxs-lookup"><span data-stu-id="a49f8-168">description</span></span>|<span data-ttu-id="a49f8-169">Строка</span><span class="sxs-lookup"><span data-stu-id="a49f8-169">String</span></span>|<span data-ttu-id="a49f8-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a49f8-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a49f8-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a49f8-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a49f8-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a49f8-172">displayName</span></span>|<span data-ttu-id="a49f8-173">Строка</span><span class="sxs-lookup"><span data-stu-id="a49f8-173">String</span></span>|<span data-ttu-id="a49f8-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a49f8-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a49f8-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a49f8-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a49f8-176">version</span><span class="sxs-lookup"><span data-stu-id="a49f8-176">version</span></span>|<span data-ttu-id="a49f8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a49f8-177">Int32</span></span>|<span data-ttu-id="a49f8-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a49f8-178">Version of the device configuration.</span></span> <span data-ttu-id="a49f8-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a49f8-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a49f8-180">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="a49f8-180">deliveryOptimizationMode</span></span>|[<span data-ttu-id="a49f8-181">WindowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="a49f8-181">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="a49f8-182">Режим оптимизации доставки.</span><span class="sxs-lookup"><span data-stu-id="a49f8-182">Delivery Optimization Mode.</span></span> <span data-ttu-id="a49f8-183">Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span><span class="sxs-lookup"><span data-stu-id="a49f8-183">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="a49f8-184">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="a49f8-184">prereleaseFeatures</span></span>|[<span data-ttu-id="a49f8-185">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="a49f8-185">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="a49f8-186">Функции предварительного выпуска.</span><span class="sxs-lookup"><span data-stu-id="a49f8-186">The pre-release features.</span></span> <span data-ttu-id="a49f8-187">Возможные значения: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span><span class="sxs-lookup"><span data-stu-id="a49f8-187">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="a49f8-188">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="a49f8-188">automaticUpdateMode</span></span>|[<span data-ttu-id="a49f8-189">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="a49f8-189">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="a49f8-190">Режим автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="a49f8-190">Automatic update mode.</span></span> <span data-ttu-id="a49f8-191">Возможные значения: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span><span class="sxs-lookup"><span data-stu-id="a49f8-191">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="a49f8-192">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="a49f8-192">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="a49f8-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="a49f8-193">Boolean</span></span>|<span data-ttu-id="a49f8-194">Разрешение использования службы обновлений (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="a49f8-194">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="a49f8-195">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="a49f8-195">driversExcluded</span></span>|<span data-ttu-id="a49f8-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="a49f8-196">Boolean</span></span>|<span data-ttu-id="a49f8-197">Исключение драйверов из Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="a49f8-197">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="a49f8-198">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="a49f8-198">installationSchedule</span></span>|[<span data-ttu-id="a49f8-199">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="a49f8-199">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="a49f8-200">Расписание установки.</span><span class="sxs-lookup"><span data-stu-id="a49f8-200">Installation schedule</span></span>|
|<span data-ttu-id="a49f8-201">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="a49f8-201">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="a49f8-202">Int32</span><span class="sxs-lookup"><span data-stu-id="a49f8-202">Int32</span></span>|<span data-ttu-id="a49f8-203">Откладывание исправлений на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="a49f8-203">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="a49f8-204">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="a49f8-204">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="a49f8-205">Int32</span><span class="sxs-lookup"><span data-stu-id="a49f8-205">Int32</span></span>|<span data-ttu-id="a49f8-206">Откладывание обновлений компонентов на заданное количество дней.</span><span class="sxs-lookup"><span data-stu-id="a49f8-206">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="a49f8-207">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="a49f8-207">qualityUpdatesPaused</span></span>|<span data-ttu-id="a49f8-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="a49f8-208">Boolean</span></span>|<span data-ttu-id="a49f8-209">Приостановка исправлений.</span><span class="sxs-lookup"><span data-stu-id="a49f8-209">Pause Quality Updates</span></span>|
|<span data-ttu-id="a49f8-210">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="a49f8-210">featureUpdatesPaused</span></span>|<span data-ttu-id="a49f8-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="a49f8-211">Boolean</span></span>|<span data-ttu-id="a49f8-212">Приостановка обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="a49f8-212">Pause Feature Updates</span></span>|
|<span data-ttu-id="a49f8-213">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="a49f8-213">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="a49f8-214">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a49f8-214">DateTimeOffset</span></span>|<span data-ttu-id="a49f8-215">Дата и время завершения срока приостановки исправлений.</span><span class="sxs-lookup"><span data-stu-id="a49f8-215">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="a49f8-216">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="a49f8-216">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="a49f8-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a49f8-217">DateTimeOffset</span></span>|<span data-ttu-id="a49f8-218">Дата и время, когда будет завершен срок приостановки обновлений компонентов.</span><span class="sxs-lookup"><span data-stu-id="a49f8-218">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="a49f8-219">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="a49f8-219">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="a49f8-220">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="a49f8-220">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="a49f8-221">Определяет, из каких устройств филиалов будут получаться обновления.</span><span class="sxs-lookup"><span data-stu-id="a49f8-221">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="a49f8-222">Возможные значения: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span><span class="sxs-lookup"><span data-stu-id="a49f8-222">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="a49f8-223">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="a49f8-223">skipChecksBeforeRestart</span></span>|<span data-ttu-id="a49f8-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="a49f8-224">Boolean</span></span>|<span data-ttu-id="a49f8-225">Установите, чтобы пропустить все проверки перед перезапуском: уровень батареи = 40%, присутствие пользователя, отображение необходимо, режим презентации, полноэкранный режим, состояние телефонных звонков, режим игры и т. д.</span><span class="sxs-lookup"><span data-stu-id="a49f8-225">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="a49f8-226">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="a49f8-226">updateWeeks</span></span>|[<span data-ttu-id="a49f8-227">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="a49f8-227">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="a49f8-228">Запланирована установка обновления в течение нескольких недель месяца.</span><span class="sxs-lookup"><span data-stu-id="a49f8-228">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="a49f8-229">Возможные значения: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span><span class="sxs-lookup"><span data-stu-id="a49f8-229">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="a49f8-230">qualityUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="a49f8-230">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="a49f8-231">Дата</span><span class="sxs-lookup"><span data-stu-id="a49f8-231">Date</span></span>|<span data-ttu-id="a49f8-232">Дата начала приостановки обновления качества.</span><span class="sxs-lookup"><span data-stu-id="a49f8-232">Quality Updates Pause start date.</span></span> <span data-ttu-id="a49f8-233">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a49f8-233">This property is read-only.</span></span>|
|<span data-ttu-id="a49f8-234">featureUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="a49f8-234">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="a49f8-235">Дата</span><span class="sxs-lookup"><span data-stu-id="a49f8-235">Date</span></span>|<span data-ttu-id="a49f8-236">Дата начала приостановки обновления функций.</span><span class="sxs-lookup"><span data-stu-id="a49f8-236">Feature Updates Pause start date.</span></span> <span data-ttu-id="a49f8-237">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a49f8-237">This property is read-only.</span></span>|
|<span data-ttu-id="a49f8-238">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="a49f8-238">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="a49f8-239">Int32</span><span class="sxs-lookup"><span data-stu-id="a49f8-239">Int32</span></span>|<span data-ttu-id="a49f8-240">Количество дней после обновления функции, для которого допустим откат</span><span class="sxs-lookup"><span data-stu-id="a49f8-240">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="a49f8-241">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="a49f8-241">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="a49f8-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="a49f8-242">Boolean</span></span>|<span data-ttu-id="a49f8-243">Указывает, следует ли откат обновлений качества при следующей проверке устройства</span><span class="sxs-lookup"><span data-stu-id="a49f8-243">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="a49f8-244">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="a49f8-244">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="a49f8-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="a49f8-245">Boolean</span></span>|<span data-ttu-id="a49f8-246">Указывает, следует ли откат обновлений функций при следующей проверке устройства</span><span class="sxs-lookup"><span data-stu-id="a49f8-246">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="a49f8-247">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="a49f8-247">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="a49f8-248">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a49f8-248">DateTimeOffset</span></span>|<span data-ttu-id="a49f8-249">Дата начала отката обновлений качества</span><span class="sxs-lookup"><span data-stu-id="a49f8-249">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="a49f8-250">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="a49f8-250">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="a49f8-251">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a49f8-251">DateTimeOffset</span></span>|<span data-ttu-id="a49f8-252">Дата начала отката обновлений функций</span><span class="sxs-lookup"><span data-stu-id="a49f8-252">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="a49f8-253">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="a49f8-253">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="a49f8-254">Int32</span><span class="sxs-lookup"><span data-stu-id="a49f8-254">Int32</span></span>|<span data-ttu-id="a49f8-255">Крайний срок за несколько дней до автоматического планирования и выполнения ожидающих перезагрузки вне активных часов с допустимым диапазоном от 2 до 30 дней</span><span class="sxs-lookup"><span data-stu-id="a49f8-255">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="a49f8-256">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="a49f8-256">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="a49f8-257">Int32</span><span class="sxs-lookup"><span data-stu-id="a49f8-257">Int32</span></span>|<span data-ttu-id="a49f8-258">Количество дней, за которые пользователь может отсмеять уведомления об уведомлении о перезапуске с допустимым диапазоном от 1 до 3 дней</span><span class="sxs-lookup"><span data-stu-id="a49f8-258">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="a49f8-259">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="a49f8-259">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="a49f8-260">Int32</span><span class="sxs-lookup"><span data-stu-id="a49f8-260">Int32</span></span>|<span data-ttu-id="a49f8-261">Количество дней до перехода из автоматической перезапусков, запланированных вне активных часов, в режим "Активный перезапуск", который требует от пользователя расписания, с допустимым диапазоном от 0 до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="a49f8-261">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="a49f8-262">deadlineForFeatureUpdatesInDays</span><span class="sxs-lookup"><span data-stu-id="a49f8-262">deadlineForFeatureUpdatesInDays</span></span>|<span data-ttu-id="a49f8-263">Int32</span><span class="sxs-lookup"><span data-stu-id="a49f8-263">Int32</span></span>|<span data-ttu-id="a49f8-264">Количество дней до установки обновлений функций автоматически с допустимым диапазоном от 2 до 30 дней</span><span class="sxs-lookup"><span data-stu-id="a49f8-264">Number of days before feature updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="a49f8-265">deadlineForQualityUpdatesInDays</span><span class="sxs-lookup"><span data-stu-id="a49f8-265">deadlineForQualityUpdatesInDays</span></span>|<span data-ttu-id="a49f8-266">Int32</span><span class="sxs-lookup"><span data-stu-id="a49f8-266">Int32</span></span>|<span data-ttu-id="a49f8-267">Количество дней до установки обновлений качества автоматически с допустимым диапазоном от 2 до 30 дней</span><span class="sxs-lookup"><span data-stu-id="a49f8-267">Number of days before quality updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="a49f8-268">deadlineGracePeriodInDays</span><span class="sxs-lookup"><span data-stu-id="a49f8-268">deadlineGracePeriodInDays</span></span>|<span data-ttu-id="a49f8-269">Int32</span><span class="sxs-lookup"><span data-stu-id="a49f8-269">Int32</span></span>|<span data-ttu-id="a49f8-270">Количество дней после крайнего срока до автоматического перезапуска с допустимым диапазоном от 0 до 7 дней</span><span class="sxs-lookup"><span data-stu-id="a49f8-270">Number of days after deadline  until restarts occur automatically with valid range from 0 to 7 days</span></span>|
|<span data-ttu-id="a49f8-271">postponeRebootUntilAfterDeadline</span><span class="sxs-lookup"><span data-stu-id="a49f8-271">postponeRebootUntilAfterDeadline</span></span>|<span data-ttu-id="a49f8-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="a49f8-272">Boolean</span></span>|<span data-ttu-id="a49f8-273">Указывает, следует ли устройству дождаться крайнего срока для перезагрузки вне активных часов</span><span class="sxs-lookup"><span data-stu-id="a49f8-273">Specifies if the device should wait until deadline for rebooting outside of active hours</span></span>|
|<span data-ttu-id="a49f8-274">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="a49f8-274">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="a49f8-275">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="a49f8-275">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="a49f8-276">Укажите метод, с помощью которого необходимое уведомление автоматически перезапустится.</span><span class="sxs-lookup"><span data-stu-id="a49f8-276">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="a49f8-277">Возможные значения: `notConfigured`, `automatic`, `user`.</span><span class="sxs-lookup"><span data-stu-id="a49f8-277">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="a49f8-278">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="a49f8-278">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="a49f8-279">Int32</span><span class="sxs-lookup"><span data-stu-id="a49f8-279">Int32</span></span>|<span data-ttu-id="a49f8-280">Укажите период для уведомлений о предупреждении автоматической перезапуска.</span><span class="sxs-lookup"><span data-stu-id="a49f8-280">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="a49f8-281">Поддерживаемые значения: 2, 4, 8, 12 или 24 (часы).</span><span class="sxs-lookup"><span data-stu-id="a49f8-281">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="a49f8-282">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="a49f8-282">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="a49f8-283">Int32</span><span class="sxs-lookup"><span data-stu-id="a49f8-283">Int32</span></span>|<span data-ttu-id="a49f8-284">Укажите период автоматического перезапуска оповещений о неминуемом предупреждении.</span><span class="sxs-lookup"><span data-stu-id="a49f8-284">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="a49f8-285">Поддерживаемые значения: 15, 30 или 60 (минут).</span><span class="sxs-lookup"><span data-stu-id="a49f8-285">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="a49f8-286">userPauseAccess</span><span class="sxs-lookup"><span data-stu-id="a49f8-286">userPauseAccess</span></span>|[<span data-ttu-id="a49f8-287">включить</span><span class="sxs-lookup"><span data-stu-id="a49f8-287">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a49f8-288">Указывает, следует ли включить доступ конечных пользователей к приостановке обновлений программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="a49f8-288">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="a49f8-289">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="a49f8-289">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a49f8-290">userWindowsUpdateScanAccess</span><span class="sxs-lookup"><span data-stu-id="a49f8-290">userWindowsUpdateScanAccess</span></span>|[<span data-ttu-id="a49f8-291">включить</span><span class="sxs-lookup"><span data-stu-id="a49f8-291">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a49f8-292">Указывает, следует ли отключить доступ пользователя к проверке обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="a49f8-292">Specifies whether to disable user’s access to scan Windows Update.</span></span> <span data-ttu-id="a49f8-293">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="a49f8-293">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a49f8-294">updateNotificationLevel</span><span class="sxs-lookup"><span data-stu-id="a49f8-294">updateNotificationLevel</span></span>|[<span data-ttu-id="a49f8-295">windowsUpdateNotificationDisplayOption</span><span class="sxs-lookup"><span data-stu-id="a49f8-295">windowsUpdateNotificationDisplayOption</span></span>](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|<span data-ttu-id="a49f8-296">Указывает, какие уведомления об обновлении Windows видят пользователи.</span><span class="sxs-lookup"><span data-stu-id="a49f8-296">Specifies what Windows Update notifications users see.</span></span> <span data-ttu-id="a49f8-297">Возможные значения: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="a49f8-297">Possible values are: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span></span>|



## <a name="response"></a><span data-ttu-id="a49f8-298">Отклик</span><span class="sxs-lookup"><span data-stu-id="a49f8-298">Response</span></span>
<span data-ttu-id="a49f8-299">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a49f8-299">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a49f8-300">Пример</span><span class="sxs-lookup"><span data-stu-id="a49f8-300">Example</span></span>

### <a name="request"></a><span data-ttu-id="a49f8-301">Запрос</span><span class="sxs-lookup"><span data-stu-id="a49f8-301">Request</span></span>
<span data-ttu-id="a49f8-302">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a49f8-302">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="a49f8-303">Отклик</span><span class="sxs-lookup"><span data-stu-id="a49f8-303">Response</span></span>
<span data-ttu-id="a49f8-p126">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a49f8-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




