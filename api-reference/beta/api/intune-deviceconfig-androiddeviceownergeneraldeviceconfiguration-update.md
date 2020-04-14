---
title: Обновление androidDeviceOwnerGeneralDeviceConfiguration
description: Обновление свойств объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 60276dd6bbfd3d7359d50eda398c0f16ea690fad
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436242"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="1bbbe-103">Обновление androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1bbbe-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="1bbbe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bbbe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bbbe-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bbbe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bbbe-107">Обновление свойств объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1bbbe-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bbbe-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1bbbe-108">Prerequisites</span></span>
<span data-ttu-id="1bbbe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bbbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bbbe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bbbe-111">Permission type</span></span>|<span data-ttu-id="1bbbe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bbbe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bbbe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bbbe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1bbbe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bbbe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1bbbe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bbbe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bbbe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-116">Not supported.</span></span>|
|<span data-ttu-id="1bbbe-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1bbbe-117">Application</span></span>|<span data-ttu-id="1bbbe-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bbbe-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bbbe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bbbe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1bbbe-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1bbbe-120">Request headers</span></span>
|<span data-ttu-id="1bbbe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1bbbe-121">Header</span></span>|<span data-ttu-id="1bbbe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1bbbe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bbbe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bbbe-123">Authorization</span></span>|<span data-ttu-id="1bbbe-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bbbe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1bbbe-125">Accept</span></span>|<span data-ttu-id="1bbbe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1bbbe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bbbe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1bbbe-127">Request body</span></span>
<span data-ttu-id="1bbbe-128">В тексте запроса добавьте представление объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="1bbbe-129">В следующей таблице приведены свойства, необходимые при создании [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1bbbe-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="1bbbe-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1bbbe-130">Property</span></span>|<span data-ttu-id="1bbbe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1bbbe-131">Type</span></span>|<span data-ttu-id="1bbbe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1bbbe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bbbe-133">id</span><span class="sxs-lookup"><span data-stu-id="1bbbe-133">id</span></span>|<span data-ttu-id="1bbbe-134">String</span><span class="sxs-lookup"><span data-stu-id="1bbbe-134">String</span></span>|<span data-ttu-id="1bbbe-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-135">Key of the entity.</span></span> <span data-ttu-id="1bbbe-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1bbbe-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1bbbe-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1bbbe-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1bbbe-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bbbe-138">DateTimeOffset</span></span>|<span data-ttu-id="1bbbe-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1bbbe-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1bbbe-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1bbbe-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1bbbe-141">roleScopeTagIds</span></span>|<span data-ttu-id="1bbbe-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1bbbe-142">String collection</span></span>|<span data-ttu-id="1bbbe-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1bbbe-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1bbbe-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1bbbe-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="1bbbe-145">supportsScopeTags</span></span>|<span data-ttu-id="1bbbe-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-146">Boolean</span></span>|<span data-ttu-id="1bbbe-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1bbbe-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1bbbe-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1bbbe-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-150">This property is read-only.</span></span> <span data-ttu-id="1bbbe-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1bbbe-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1bbbe-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1bbbe-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1bbbe-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1bbbe-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1bbbe-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1bbbe-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1bbbe-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1bbbe-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1bbbe-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1bbbe-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1bbbe-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1bbbe-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1bbbe-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1bbbe-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1bbbe-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1bbbe-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1bbbe-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1bbbe-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1bbbe-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1bbbe-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1bbbe-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1bbbe-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1bbbe-164">createdDateTime</span></span>|<span data-ttu-id="1bbbe-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bbbe-165">DateTimeOffset</span></span>|<span data-ttu-id="1bbbe-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-166">DateTime the object was created.</span></span> <span data-ttu-id="1bbbe-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1bbbe-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1bbbe-168">description</span><span class="sxs-lookup"><span data-stu-id="1bbbe-168">description</span></span>|<span data-ttu-id="1bbbe-169">String</span><span class="sxs-lookup"><span data-stu-id="1bbbe-169">String</span></span>|<span data-ttu-id="1bbbe-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1bbbe-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1bbbe-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1bbbe-172">displayName</span><span class="sxs-lookup"><span data-stu-id="1bbbe-172">displayName</span></span>|<span data-ttu-id="1bbbe-173">Строка</span><span class="sxs-lookup"><span data-stu-id="1bbbe-173">String</span></span>|<span data-ttu-id="1bbbe-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1bbbe-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1bbbe-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1bbbe-176">version</span><span class="sxs-lookup"><span data-stu-id="1bbbe-176">version</span></span>|<span data-ttu-id="1bbbe-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbbe-177">Int32</span></span>|<span data-ttu-id="1bbbe-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-178">Version of the device configuration.</span></span> <span data-ttu-id="1bbbe-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1bbbe-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1bbbe-180">аккаунтсблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="1bbbe-180">accountsBlockModification</span></span>|<span data-ttu-id="1bbbe-181">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-181">Boolean</span></span>|<span data-ttu-id="1bbbe-182">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="1bbbe-183">аппсалловинсталлфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="1bbbe-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="1bbbe-184">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-184">Boolean</span></span>|<span data-ttu-id="1bbbe-185">Указывает, может ли пользователь включить параметр "неизвестные источники".</span><span class="sxs-lookup"><span data-stu-id="1bbbe-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="1bbbe-186">аппсаутаупдатеполици</span><span class="sxs-lookup"><span data-stu-id="1bbbe-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="1bbbe-187">андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="1bbbe-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="1bbbe-188">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="1bbbe-189">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="1bbbe-190">аппсдефаултпермиссионполици</span><span class="sxs-lookup"><span data-stu-id="1bbbe-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="1bbbe-191">андроиддевицеовнердефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="1bbbe-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="1bbbe-192">Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="1bbbe-193">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="1bbbe-194">аппсрекоммендскиппингфирстусехинтс</span><span class="sxs-lookup"><span data-stu-id="1bbbe-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="1bbbe-195">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-195">Boolean</span></span>|<span data-ttu-id="1bbbe-196">Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="1bbbe-197">блуетусблоккконфигуратион</span><span class="sxs-lookup"><span data-stu-id="1bbbe-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="1bbbe-198">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-198">Boolean</span></span>|<span data-ttu-id="1bbbe-199">Указывает, следует ли запретить пользователю настраивать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="1bbbe-200">блуетусблоккконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="1bbbe-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="1bbbe-201">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-201">Boolean</span></span>|<span data-ttu-id="1bbbe-202">Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="1bbbe-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="1bbbe-203">cameraBlocked</span></span>|<span data-ttu-id="1bbbe-204">Логический</span><span class="sxs-lookup"><span data-stu-id="1bbbe-204">Boolean</span></span>|<span data-ttu-id="1bbbe-205">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="1bbbe-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="1bbbe-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="1bbbe-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="1bbbe-207">Boolean</span></span>|<span data-ttu-id="1bbbe-208">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="1bbbe-209">цертификатекредентиалконфигуратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="1bbbe-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="1bbbe-210">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-210">Boolean</span></span>|<span data-ttu-id="1bbbe-211">Указывает, следует ли запретить пользователям настраивать учетные данные сертификатов.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="1bbbe-212">датароамингблоккед</span><span class="sxs-lookup"><span data-stu-id="1bbbe-212">dataRoamingBlocked</span></span>|<span data-ttu-id="1bbbe-213">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-213">Boolean</span></span>|<span data-ttu-id="1bbbe-214">Указывает, следует ли запретить пользователю перемещать данные.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-214">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="1bbbe-215">датетимеконфигуратионблоккед</span><span class="sxs-lookup"><span data-stu-id="1bbbe-215">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="1bbbe-216">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-216">Boolean</span></span>|<span data-ttu-id="1bbbe-217">Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-217">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="1bbbe-218">факториресетдевицеадминистраторемаилс</span><span class="sxs-lookup"><span data-stu-id="1bbbe-218">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="1bbbe-219">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1bbbe-219">String collection</span></span>|<span data-ttu-id="1bbbe-220">Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-220">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="1bbbe-221">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="1bbbe-221">factoryResetBlocked</span></span>|<span data-ttu-id="1bbbe-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="1bbbe-222">Boolean</span></span>|<span data-ttu-id="1bbbe-223">Указывает, отключен ли параметр Reset фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-223">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="1bbbe-224">глобалпрокси</span><span class="sxs-lookup"><span data-stu-id="1bbbe-224">globalProxy</span></span>|[<span data-ttu-id="1bbbe-225">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="1bbbe-225">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="1bbbe-226">Прокси-сервер настраивается напрямую с узлом, портом и исключенными узлами.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-226">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="1bbbe-227">гуглеаккаунтсблоккед</span><span class="sxs-lookup"><span data-stu-id="1bbbe-227">googleAccountsBlocked</span></span>|<span data-ttu-id="1bbbe-228">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-228">Boolean</span></span>|<span data-ttu-id="1bbbe-229">Указывает, будут ли блокироваться учетные записи Google.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-229">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="1bbbe-230">киоскмодескринсаверконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="1bbbe-230">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="1bbbe-231">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-231">Boolean</span></span>|<span data-ttu-id="1bbbe-232">Указывает, следует ли включить режим экранной заставки или не в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-232">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="1bbbe-233">киоскмодескринсаверимажеурл</span><span class="sxs-lookup"><span data-stu-id="1bbbe-233">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="1bbbe-234">String</span><span class="sxs-lookup"><span data-stu-id="1bbbe-234">String</span></span>|<span data-ttu-id="1bbbe-235">URL-адрес изображения, которое будет экранной заставкой устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-235">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="1bbbe-236">киоскмодескринсавердисплайтимеинсекондс</span><span class="sxs-lookup"><span data-stu-id="1bbbe-236">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="1bbbe-237">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbbe-237">Int32</span></span>|<span data-ttu-id="1bbbe-238">Время (в секундах), в течение которого устройство будет отображать экранную заставку в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-238">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="1bbbe-239">Допустимые значения — от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="1bbbe-239">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="1bbbe-240">киоскмодескринсаверстартделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="1bbbe-240">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="1bbbe-241">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbbe-241">Int32</span></span>|<span data-ttu-id="1bbbe-242">Время (в секундах), в течение которого устройство должно быть неактивным, чтобы экранная заставка отображалась в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-242">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="1bbbe-243">Допустимые значения — от 1 до 9999999</span><span class="sxs-lookup"><span data-stu-id="1bbbe-243">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="1bbbe-244">киоскмодескринсавердетектмедиадисаблед</span><span class="sxs-lookup"><span data-stu-id="1bbbe-244">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="1bbbe-245">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-245">Boolean</span></span>|<span data-ttu-id="1bbbe-246">Указывает, должно ли устройство отображать экранную заставку при воспроизведении аудио-и видеоконференций в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-246">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="1bbbe-247">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="1bbbe-247">kioskModeApps</span></span>|<span data-ttu-id="1bbbe-248">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="1bbbe-248">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="1bbbe-249">Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-249">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="1bbbe-250">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-250">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1bbbe-251">киоскмодеваллпаперурл</span><span class="sxs-lookup"><span data-stu-id="1bbbe-251">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="1bbbe-252">String</span><span class="sxs-lookup"><span data-stu-id="1bbbe-252">String</span></span>|<span data-ttu-id="1bbbe-253">URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-253">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="1bbbe-254">киоскмодикситкоде</span><span class="sxs-lookup"><span data-stu-id="1bbbe-254">kioskModeExitCode</span></span>|<span data-ttu-id="1bbbe-255">String</span><span class="sxs-lookup"><span data-stu-id="1bbbe-255">String</span></span>|<span data-ttu-id="1bbbe-256">Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-256">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="1bbbe-257">киоскмодевиртуалхомебуттоненаблед</span><span class="sxs-lookup"><span data-stu-id="1bbbe-257">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="1bbbe-258">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-258">Boolean</span></span>|<span data-ttu-id="1bbbe-259">Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-259">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="1bbbe-260">киоскмодевиртуалхомебуттонтипе</span><span class="sxs-lookup"><span data-stu-id="1bbbe-260">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="1bbbe-261">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="1bbbe-261">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="1bbbe-262">Указывает, является ли кнопка "Виртуальная Домашняя страница" кнопкой "Прокрутка вверх" или плавающей кнопкой "домой".</span><span class="sxs-lookup"><span data-stu-id="1bbbe-262">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="1bbbe-263">Возможные значения: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-263">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="1bbbe-264">киоскмодеблуетусконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="1bbbe-264">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="1bbbe-265">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-265">Boolean</span></span>|<span data-ttu-id="1bbbe-266">Указывает, следует ли запретить пользователю настраивать параметры Bluetooth в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-266">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="1bbbe-267">киоскмодевификонфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="1bbbe-267">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="1bbbe-268">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-268">Boolean</span></span>|<span data-ttu-id="1bbbe-269">Указывает, следует ли разрешить пользователю настраивать параметры Wi/Fi в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-269">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="1bbbe-270">киоскмодефлашлигхтконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="1bbbe-270">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="1bbbe-271">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-271">Boolean</span></span>|<span data-ttu-id="1bbbe-272">Указывает, следует ли разрешить пользователю использовать флашлигхт в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-272">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="1bbbe-273">киоскмодемедиаволумеконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="1bbbe-273">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="1bbbe-274">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-274">Boolean</span></span>|<span data-ttu-id="1bbbe-275">Указывает, следует ли запретить пользователю изменять громкость мультимедиа в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-275">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="1bbbe-276">микрофонефорцемуте</span><span class="sxs-lookup"><span data-stu-id="1bbbe-276">microphoneForceMute</span></span>|<span data-ttu-id="1bbbe-277">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-277">Boolean</span></span>|<span data-ttu-id="1bbbe-278">Указывает, следует ли запретить разблокирование микрофона устройства.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-278">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="1bbbe-279">нетворкескапехатчалловед</span><span class="sxs-lookup"><span data-stu-id="1bbbe-279">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="1bbbe-280">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-280">Boolean</span></span>|<span data-ttu-id="1bbbe-281">Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-281">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="1bbbe-282">нфкблоккаутгоингбеам</span><span class="sxs-lookup"><span data-stu-id="1bbbe-282">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="1bbbe-283">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-283">Boolean</span></span>|<span data-ttu-id="1bbbe-284">Указывает, следует ли заблокировать исходящую форму NFC.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-284">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="1bbbe-285">пассвордблокккэйгуард</span><span class="sxs-lookup"><span data-stu-id="1bbbe-285">passwordBlockKeyguard</span></span>|<span data-ttu-id="1bbbe-286">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-286">Boolean</span></span>|<span data-ttu-id="1bbbe-287">Указывает, отключен ли кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-287">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="1bbbe-288">пассвордблокккэйгуардфеатурес</span><span class="sxs-lookup"><span data-stu-id="1bbbe-288">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="1bbbe-289">Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="1bbbe-289">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="1bbbe-290">Список компонентов кэйгуард устройств, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-290">List of device keyguard features to block.</span></span> <span data-ttu-id="1bbbe-291">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-291">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="1bbbe-292">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-292">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="1bbbe-293">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1bbbe-293">passwordExpirationDays</span></span>|<span data-ttu-id="1bbbe-294">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbbe-294">Int32</span></span>|<span data-ttu-id="1bbbe-295">Указывает время в секундах, в течение которого можно задать пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-295">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="1bbbe-296">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-296">Valid values 1 to 365</span></span>|
|<span data-ttu-id="1bbbe-297">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1bbbe-297">passwordMinimumLength</span></span>|<span data-ttu-id="1bbbe-298">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbbe-298">Int32</span></span>|<span data-ttu-id="1bbbe-299">Указывает минимальную длину пароля, необходимого для устройства.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-299">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="1bbbe-300">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-300">Valid values 4 to 16</span></span>|
|<span data-ttu-id="1bbbe-301">пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="1bbbe-301">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="1bbbe-302">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbbe-302">Int32</span></span>|<span data-ttu-id="1bbbe-303">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-303">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="1bbbe-304">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-304">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1bbbe-305">пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="1bbbe-305">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="1bbbe-306">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbbe-306">Int32</span></span>|<span data-ttu-id="1bbbe-307">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-307">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="1bbbe-308">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-308">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1bbbe-309">пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="1bbbe-309">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="1bbbe-310">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbbe-310">Int32</span></span>|<span data-ttu-id="1bbbe-311">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-311">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="1bbbe-312">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-312">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1bbbe-313">пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="1bbbe-313">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="1bbbe-314">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbbe-314">Int32</span></span>|<span data-ttu-id="1bbbe-315">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-315">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="1bbbe-316">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-316">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1bbbe-317">пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="1bbbe-317">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="1bbbe-318">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbbe-318">Int32</span></span>|<span data-ttu-id="1bbbe-319">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-319">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="1bbbe-320">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-320">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1bbbe-321">пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="1bbbe-321">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="1bbbe-322">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbbe-322">Int32</span></span>|<span data-ttu-id="1bbbe-323">Указывает минимальное число символов верхнего каселеттер, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-323">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="1bbbe-324">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-324">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1bbbe-325">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="1bbbe-325">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="1bbbe-326">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbbe-326">Int32</span></span>|<span data-ttu-id="1bbbe-327">Миллисекунды бездействия до истечения времени ожидания экрана.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-327">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="1bbbe-328">пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="1bbbe-328">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="1bbbe-329">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbbe-329">Int32</span></span>|<span data-ttu-id="1bbbe-330">Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-330">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="1bbbe-331">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-331">Valid values 0 to 24</span></span>|
|<span data-ttu-id="1bbbe-332">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1bbbe-332">passwordRequiredType</span></span>|[<span data-ttu-id="1bbbe-333">андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="1bbbe-333">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="1bbbe-334">Указывает минимальное качество пароля, необходимое для устройства.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-334">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="1bbbe-335">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-335">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="1bbbe-336">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="1bbbe-336">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="1bbbe-337">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbbe-337">Int32</span></span>|<span data-ttu-id="1bbbe-338">Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-338">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="1bbbe-339">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-339">Valid values 4 to 11</span></span>|
|<span data-ttu-id="1bbbe-340">плайсторемоде</span><span class="sxs-lookup"><span data-stu-id="1bbbe-340">playStoreMode</span></span>|[<span data-ttu-id="1bbbe-341">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="1bbbe-341">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="1bbbe-342">Указывает режим проигрывания устройства в хранилище.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-342">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="1bbbe-343">Возможные значения: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-343">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="1bbbe-344">сафебутблоккед</span><span class="sxs-lookup"><span data-stu-id="1bbbe-344">safeBootBlocked</span></span>|<span data-ttu-id="1bbbe-345">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-345">Boolean</span></span>|<span data-ttu-id="1bbbe-346">Указывает, отключена ли загрузка устройства в "безопасная загрузка".</span><span class="sxs-lookup"><span data-stu-id="1bbbe-346">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="1bbbe-347">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="1bbbe-347">screenCaptureBlocked</span></span>|<span data-ttu-id="1bbbe-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="1bbbe-348">Boolean</span></span>|<span data-ttu-id="1bbbe-349">Указывает, следует ли отключить возможность использования снимков экрана.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-349">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="1bbbe-350">секуритялловдебуггингфеатурес</span><span class="sxs-lookup"><span data-stu-id="1bbbe-350">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="1bbbe-351">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-351">Boolean</span></span>|<span data-ttu-id="1bbbe-352">Указывает, следует ли запретить пользователю включать функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-352">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="1bbbe-353">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="1bbbe-353">securityRequireVerifyApps</span></span>|<span data-ttu-id="1bbbe-354">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-354">Boolean</span></span>|<span data-ttu-id="1bbbe-355">Указывает, требуется ли проверка приложений.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-355">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="1bbbe-356">статусбарблоккед</span><span class="sxs-lookup"><span data-stu-id="1bbbe-356">statusBarBlocked</span></span>|<span data-ttu-id="1bbbe-357">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-357">Boolean</span></span>|<span data-ttu-id="1bbbe-358">Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-358">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="1bbbe-359">стайонмодес</span><span class="sxs-lookup"><span data-stu-id="1bbbe-359">stayOnModes</span></span>|<span data-ttu-id="1bbbe-360">Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="1bbbe-360">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="1bbbe-361">Список режимов, в которых дисплей устройства остается включенным.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-361">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="1bbbe-362">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-362">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="1bbbe-363">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-363">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="1bbbe-364">сторажеалловусб</span><span class="sxs-lookup"><span data-stu-id="1bbbe-364">storageAllowUsb</span></span>|<span data-ttu-id="1bbbe-365">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-365">Boolean</span></span>|<span data-ttu-id="1bbbe-366">Указывает, следует ли разрешить запоминающее устройство USB.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-366">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="1bbbe-367">сторажеблоккекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="1bbbe-367">storageBlockExternalMedia</span></span>|<span data-ttu-id="1bbbe-368">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-368">Boolean</span></span>|<span data-ttu-id="1bbbe-369">Указывает, следует ли заблокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-369">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="1bbbe-370">сторажеблоккусбфилетрансфер</span><span class="sxs-lookup"><span data-stu-id="1bbbe-370">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="1bbbe-371">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-371">Boolean</span></span>|<span data-ttu-id="1bbbe-372">Указывает, следует ли запретить передачу файлов через USB.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-372">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="1bbbe-373">системупдатевиндовстартминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="1bbbe-373">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="1bbbe-374">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbbe-374">Int32</span></span>|<span data-ttu-id="1bbbe-375">Указывает количество минут после полуночи, когда запустится окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-375">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="1bbbe-376">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="1bbbe-376">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="1bbbe-377">системупдатевиндовендминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="1bbbe-377">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="1bbbe-378">Int32</span><span class="sxs-lookup"><span data-stu-id="1bbbe-378">Int32</span></span>|<span data-ttu-id="1bbbe-379">Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-379">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="1bbbe-380">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="1bbbe-380">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="1bbbe-381">системупдатеинсталлтипе</span><span class="sxs-lookup"><span data-stu-id="1bbbe-381">systemUpdateInstallType</span></span>|[<span data-ttu-id="1bbbe-382">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="1bbbe-382">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="1bbbe-383">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-383">The type of system update configuration.</span></span> <span data-ttu-id="1bbbe-384">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-384">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="1bbbe-385">системвиндовсблоккед</span><span class="sxs-lookup"><span data-stu-id="1bbbe-385">systemWindowsBlocked</span></span>|<span data-ttu-id="1bbbe-386">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-386">Boolean</span></span>|<span data-ttu-id="1bbbe-387">Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-387">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="1bbbe-388">усерсблоккадд</span><span class="sxs-lookup"><span data-stu-id="1bbbe-388">usersBlockAdd</span></span>|<span data-ttu-id="1bbbe-389">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-389">Boolean</span></span>|<span data-ttu-id="1bbbe-390">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-390">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="1bbbe-391">усерсблоккремове</span><span class="sxs-lookup"><span data-stu-id="1bbbe-391">usersBlockRemove</span></span>|<span data-ttu-id="1bbbe-392">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-392">Boolean</span></span>|<span data-ttu-id="1bbbe-393">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-393">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="1bbbe-394">волумеблоккаджустмент</span><span class="sxs-lookup"><span data-stu-id="1bbbe-394">volumeBlockAdjustment</span></span>|<span data-ttu-id="1bbbe-395">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-395">Boolean</span></span>|<span data-ttu-id="1bbbe-396">Указывает, отключена ли настройка главного тома.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-396">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="1bbbe-397">впналвайсонлоккдовнмоде</span><span class="sxs-lookup"><span data-stu-id="1bbbe-397">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="1bbbe-398">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-398">Boolean</span></span>|<span data-ttu-id="1bbbe-399">Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-399">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="1bbbe-400">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="1bbbe-400">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="1bbbe-401">String</span><span class="sxs-lookup"><span data-stu-id="1bbbe-401">String</span></span>|<span data-ttu-id="1bbbe-402">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-402">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="1bbbe-403">вифиблоккедитконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="1bbbe-403">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="1bbbe-404">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-404">Boolean</span></span>|<span data-ttu-id="1bbbe-405">Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-405">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="1bbbe-406">вифиблоккедитполицидефинедконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="1bbbe-406">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="1bbbe-407">Логическое</span><span class="sxs-lookup"><span data-stu-id="1bbbe-407">Boolean</span></span>|<span data-ttu-id="1bbbe-408">Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-408">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="1bbbe-409">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bbbe-409">Response</span></span>
<span data-ttu-id="1bbbe-410">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-410">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bbbe-411">Пример</span><span class="sxs-lookup"><span data-stu-id="1bbbe-411">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bbbe-412">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bbbe-412">Request</span></span>
<span data-ttu-id="1bbbe-413">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-413">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4374

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
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
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "certificateCredentialConfigurationDisabled": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "Proxy Auto Config URL value"
  },
  "googleAccountsBlocked": true,
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
  "kioskModeScreenSaverDisplayTimeInSeconds": 8,
  "kioskModeScreenSaverStartDelayInSeconds": 7,
  "kioskModeScreenSaverDetectMediaDisabled": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeVirtualHomeButtonType": "swipeUp",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="1bbbe-414">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bbbe-414">Response</span></span>
<span data-ttu-id="1bbbe-p136">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1bbbe-p136">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4546

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
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
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "certificateCredentialConfigurationDisabled": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "Proxy Auto Config URL value"
  },
  "googleAccountsBlocked": true,
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
  "kioskModeScreenSaverDisplayTimeInSeconds": 8,
  "kioskModeScreenSaverStartDelayInSeconds": 7,
  "kioskModeScreenSaverDetectMediaDisabled": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeVirtualHomeButtonType": "swipeUp",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```



