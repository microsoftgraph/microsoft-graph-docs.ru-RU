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
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="09324-103">Обновление androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="09324-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="09324-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09324-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09324-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09324-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09324-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09324-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09324-107">Обновление свойств объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="09324-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09324-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="09324-108">Prerequisites</span></span>
<span data-ttu-id="09324-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09324-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09324-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09324-111">Permission type</span></span>|<span data-ttu-id="09324-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="09324-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09324-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09324-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09324-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09324-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="09324-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09324-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09324-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09324-116">Not supported.</span></span>|
|<span data-ttu-id="09324-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09324-117">Application</span></span>|<span data-ttu-id="09324-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09324-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09324-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09324-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="09324-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="09324-120">Request headers</span></span>
|<span data-ttu-id="09324-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09324-121">Header</span></span>|<span data-ttu-id="09324-122">Значение</span><span class="sxs-lookup"><span data-stu-id="09324-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09324-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09324-123">Authorization</span></span>|<span data-ttu-id="09324-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09324-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09324-125">Accept</span><span class="sxs-lookup"><span data-stu-id="09324-125">Accept</span></span>|<span data-ttu-id="09324-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09324-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09324-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="09324-127">Request body</span></span>
<span data-ttu-id="09324-128">В тексте запроса добавьте представление объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09324-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="09324-129">В следующей таблице приведены свойства, необходимые при создании [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09324-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="09324-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="09324-130">Property</span></span>|<span data-ttu-id="09324-131">Тип</span><span class="sxs-lookup"><span data-stu-id="09324-131">Type</span></span>|<span data-ttu-id="09324-132">Описание</span><span class="sxs-lookup"><span data-stu-id="09324-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09324-133">id</span><span class="sxs-lookup"><span data-stu-id="09324-133">id</span></span>|<span data-ttu-id="09324-134">String</span><span class="sxs-lookup"><span data-stu-id="09324-134">String</span></span>|<span data-ttu-id="09324-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="09324-135">Key of the entity.</span></span> <span data-ttu-id="09324-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09324-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09324-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="09324-137">lastModifiedDateTime</span></span>|<span data-ttu-id="09324-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09324-138">DateTimeOffset</span></span>|<span data-ttu-id="09324-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="09324-139">DateTime the object was last modified.</span></span> <span data-ttu-id="09324-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09324-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09324-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="09324-141">roleScopeTagIds</span></span>|<span data-ttu-id="09324-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="09324-142">String collection</span></span>|<span data-ttu-id="09324-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="09324-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="09324-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09324-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09324-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="09324-145">supportsScopeTags</span></span>|<span data-ttu-id="09324-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-146">Boolean</span></span>|<span data-ttu-id="09324-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="09324-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="09324-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="09324-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="09324-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="09324-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="09324-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="09324-150">This property is read-only.</span></span> <span data-ttu-id="09324-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09324-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09324-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="09324-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="09324-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="09324-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="09324-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="09324-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="09324-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09324-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09324-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="09324-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="09324-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="09324-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="09324-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="09324-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="09324-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09324-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09324-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="09324-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="09324-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="09324-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="09324-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="09324-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="09324-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09324-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09324-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09324-164">createdDateTime</span></span>|<span data-ttu-id="09324-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09324-165">DateTimeOffset</span></span>|<span data-ttu-id="09324-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="09324-166">DateTime the object was created.</span></span> <span data-ttu-id="09324-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09324-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09324-168">description</span><span class="sxs-lookup"><span data-stu-id="09324-168">description</span></span>|<span data-ttu-id="09324-169">String</span><span class="sxs-lookup"><span data-stu-id="09324-169">String</span></span>|<span data-ttu-id="09324-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="09324-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="09324-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09324-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09324-172">displayName</span><span class="sxs-lookup"><span data-stu-id="09324-172">displayName</span></span>|<span data-ttu-id="09324-173">Строка</span><span class="sxs-lookup"><span data-stu-id="09324-173">String</span></span>|<span data-ttu-id="09324-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="09324-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="09324-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09324-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09324-176">version</span><span class="sxs-lookup"><span data-stu-id="09324-176">version</span></span>|<span data-ttu-id="09324-177">Int32</span><span class="sxs-lookup"><span data-stu-id="09324-177">Int32</span></span>|<span data-ttu-id="09324-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="09324-178">Version of the device configuration.</span></span> <span data-ttu-id="09324-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09324-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09324-180">аккаунтсблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="09324-180">accountsBlockModification</span></span>|<span data-ttu-id="09324-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-181">Boolean</span></span>|<span data-ttu-id="09324-182">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="09324-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="09324-183">аппсалловинсталлфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="09324-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="09324-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-184">Boolean</span></span>|<span data-ttu-id="09324-185">Указывает, может ли пользователь включить параметр "неизвестные источники".</span><span class="sxs-lookup"><span data-stu-id="09324-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="09324-186">аппсаутаупдатеполици</span><span class="sxs-lookup"><span data-stu-id="09324-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="09324-187">андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="09324-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="09324-188">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="09324-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="09324-189">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="09324-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="09324-190">аппсдефаултпермиссионполици</span><span class="sxs-lookup"><span data-stu-id="09324-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="09324-191">андроиддевицеовнердефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="09324-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="09324-192">Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом.</span><span class="sxs-lookup"><span data-stu-id="09324-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="09324-193">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="09324-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="09324-194">аппсрекоммендскиппингфирстусехинтс</span><span class="sxs-lookup"><span data-stu-id="09324-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="09324-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-195">Boolean</span></span>|<span data-ttu-id="09324-196">Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.</span><span class="sxs-lookup"><span data-stu-id="09324-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="09324-197">блуетусблоккконфигуратион</span><span class="sxs-lookup"><span data-stu-id="09324-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="09324-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-198">Boolean</span></span>|<span data-ttu-id="09324-199">Указывает, следует ли запретить пользователю настраивать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="09324-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="09324-200">блуетусблоккконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="09324-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="09324-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-201">Boolean</span></span>|<span data-ttu-id="09324-202">Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="09324-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="09324-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="09324-203">cameraBlocked</span></span>|<span data-ttu-id="09324-204">Логический</span><span class="sxs-lookup"><span data-stu-id="09324-204">Boolean</span></span>|<span data-ttu-id="09324-205">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="09324-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="09324-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="09324-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="09324-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-207">Boolean</span></span>|<span data-ttu-id="09324-208">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="09324-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="09324-209">цертификатекредентиалконфигуратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="09324-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="09324-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-210">Boolean</span></span>|<span data-ttu-id="09324-211">Указывает, следует ли запретить пользователям настраивать учетные данные сертификатов.</span><span class="sxs-lookup"><span data-stu-id="09324-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="09324-212">датароамингблоккед</span><span class="sxs-lookup"><span data-stu-id="09324-212">dataRoamingBlocked</span></span>|<span data-ttu-id="09324-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-213">Boolean</span></span>|<span data-ttu-id="09324-214">Указывает, следует ли запретить пользователю перемещать данные.</span><span class="sxs-lookup"><span data-stu-id="09324-214">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="09324-215">датетимеконфигуратионблоккед</span><span class="sxs-lookup"><span data-stu-id="09324-215">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="09324-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-216">Boolean</span></span>|<span data-ttu-id="09324-217">Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.</span><span class="sxs-lookup"><span data-stu-id="09324-217">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="09324-218">факториресетдевицеадминистраторемаилс</span><span class="sxs-lookup"><span data-stu-id="09324-218">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="09324-219">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="09324-219">String collection</span></span>|<span data-ttu-id="09324-220">Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.</span><span class="sxs-lookup"><span data-stu-id="09324-220">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="09324-221">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="09324-221">factoryResetBlocked</span></span>|<span data-ttu-id="09324-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-222">Boolean</span></span>|<span data-ttu-id="09324-223">Указывает, отключен ли параметр Reset фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="09324-223">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="09324-224">глобалпрокси</span><span class="sxs-lookup"><span data-stu-id="09324-224">globalProxy</span></span>|[<span data-ttu-id="09324-225">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="09324-225">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="09324-226">Прокси-сервер настраивается напрямую с узлом, портом и исключенными узлами.</span><span class="sxs-lookup"><span data-stu-id="09324-226">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="09324-227">гуглеаккаунтсблоккед</span><span class="sxs-lookup"><span data-stu-id="09324-227">googleAccountsBlocked</span></span>|<span data-ttu-id="09324-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-228">Boolean</span></span>|<span data-ttu-id="09324-229">Указывает, будут ли блокироваться учетные записи Google.</span><span class="sxs-lookup"><span data-stu-id="09324-229">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="09324-230">киоскмодескринсаверконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="09324-230">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="09324-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-231">Boolean</span></span>|<span data-ttu-id="09324-232">Указывает, следует ли включить режим экранной заставки или не в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="09324-232">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="09324-233">киоскмодескринсаверимажеурл</span><span class="sxs-lookup"><span data-stu-id="09324-233">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="09324-234">String</span><span class="sxs-lookup"><span data-stu-id="09324-234">String</span></span>|<span data-ttu-id="09324-235">URL-адрес изображения, которое будет экранной заставкой устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="09324-235">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="09324-236">киоскмодескринсавердисплайтимеинсекондс</span><span class="sxs-lookup"><span data-stu-id="09324-236">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="09324-237">Int32</span><span class="sxs-lookup"><span data-stu-id="09324-237">Int32</span></span>|<span data-ttu-id="09324-238">Время (в секундах), в течение которого устройство будет отображать экранную заставку в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="09324-238">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="09324-239">Допустимые значения — от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="09324-239">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="09324-240">киоскмодескринсаверстартделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="09324-240">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="09324-241">Int32</span><span class="sxs-lookup"><span data-stu-id="09324-241">Int32</span></span>|<span data-ttu-id="09324-242">Время (в секундах), в течение которого устройство должно быть неактивным, чтобы экранная заставка отображалась в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="09324-242">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="09324-243">Допустимые значения — от 1 до 9999999</span><span class="sxs-lookup"><span data-stu-id="09324-243">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="09324-244">киоскмодескринсавердетектмедиадисаблед</span><span class="sxs-lookup"><span data-stu-id="09324-244">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="09324-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-245">Boolean</span></span>|<span data-ttu-id="09324-246">Указывает, должно ли устройство отображать экранную заставку при воспроизведении аудио-и видеоконференций в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="09324-246">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="09324-247">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="09324-247">kioskModeApps</span></span>|<span data-ttu-id="09324-248">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="09324-248">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="09324-249">Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="09324-249">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="09324-250">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="09324-250">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="09324-251">киоскмодеваллпаперурл</span><span class="sxs-lookup"><span data-stu-id="09324-251">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="09324-252">String</span><span class="sxs-lookup"><span data-stu-id="09324-252">String</span></span>|<span data-ttu-id="09324-253">URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="09324-253">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="09324-254">киоскмодикситкоде</span><span class="sxs-lookup"><span data-stu-id="09324-254">kioskModeExitCode</span></span>|<span data-ttu-id="09324-255">String</span><span class="sxs-lookup"><span data-stu-id="09324-255">String</span></span>|<span data-ttu-id="09324-256">Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="09324-256">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="09324-257">киоскмодевиртуалхомебуттоненаблед</span><span class="sxs-lookup"><span data-stu-id="09324-257">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="09324-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-258">Boolean</span></span>|<span data-ttu-id="09324-259">Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="09324-259">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="09324-260">киоскмодевиртуалхомебуттонтипе</span><span class="sxs-lookup"><span data-stu-id="09324-260">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="09324-261">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="09324-261">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="09324-262">Указывает, является ли кнопка "Виртуальная Домашняя страница" кнопкой "Прокрутка вверх" или плавающей кнопкой "домой".</span><span class="sxs-lookup"><span data-stu-id="09324-262">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="09324-263">Возможные значения: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="09324-263">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="09324-264">киоскмодеблуетусконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="09324-264">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="09324-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-265">Boolean</span></span>|<span data-ttu-id="09324-266">Указывает, следует ли запретить пользователю настраивать параметры Bluetooth в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="09324-266">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="09324-267">киоскмодевификонфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="09324-267">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="09324-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-268">Boolean</span></span>|<span data-ttu-id="09324-269">Указывает, следует ли разрешить пользователю настраивать параметры Wi/Fi в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="09324-269">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="09324-270">киоскмодефлашлигхтконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="09324-270">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="09324-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-271">Boolean</span></span>|<span data-ttu-id="09324-272">Указывает, следует ли разрешить пользователю использовать флашлигхт в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="09324-272">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="09324-273">киоскмодемедиаволумеконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="09324-273">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="09324-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-274">Boolean</span></span>|<span data-ttu-id="09324-275">Указывает, следует ли запретить пользователю изменять громкость мультимедиа в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="09324-275">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="09324-276">микрофонефорцемуте</span><span class="sxs-lookup"><span data-stu-id="09324-276">microphoneForceMute</span></span>|<span data-ttu-id="09324-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-277">Boolean</span></span>|<span data-ttu-id="09324-278">Указывает, следует ли запретить разблокирование микрофона устройства.</span><span class="sxs-lookup"><span data-stu-id="09324-278">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="09324-279">нетворкескапехатчалловед</span><span class="sxs-lookup"><span data-stu-id="09324-279">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="09324-280">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-280">Boolean</span></span>|<span data-ttu-id="09324-281">Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="09324-281">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="09324-282">нфкблоккаутгоингбеам</span><span class="sxs-lookup"><span data-stu-id="09324-282">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="09324-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-283">Boolean</span></span>|<span data-ttu-id="09324-284">Указывает, следует ли заблокировать исходящую форму NFC.</span><span class="sxs-lookup"><span data-stu-id="09324-284">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="09324-285">пассвордблокккэйгуард</span><span class="sxs-lookup"><span data-stu-id="09324-285">passwordBlockKeyguard</span></span>|<span data-ttu-id="09324-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-286">Boolean</span></span>|<span data-ttu-id="09324-287">Указывает, отключен ли кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="09324-287">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="09324-288">пассвордблокккэйгуардфеатурес</span><span class="sxs-lookup"><span data-stu-id="09324-288">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="09324-289">Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="09324-289">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="09324-290">Список компонентов кэйгуард устройств, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="09324-290">List of device keyguard features to block.</span></span> <span data-ttu-id="09324-291">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="09324-291">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="09324-292">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="09324-292">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="09324-293">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="09324-293">passwordExpirationDays</span></span>|<span data-ttu-id="09324-294">Int32</span><span class="sxs-lookup"><span data-stu-id="09324-294">Int32</span></span>|<span data-ttu-id="09324-295">Указывает время в секундах, в течение которого можно задать пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="09324-295">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="09324-296">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="09324-296">Valid values 1 to 365</span></span>|
|<span data-ttu-id="09324-297">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="09324-297">passwordMinimumLength</span></span>|<span data-ttu-id="09324-298">Int32</span><span class="sxs-lookup"><span data-stu-id="09324-298">Int32</span></span>|<span data-ttu-id="09324-299">Указывает минимальную длину пароля, необходимого для устройства.</span><span class="sxs-lookup"><span data-stu-id="09324-299">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="09324-300">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="09324-300">Valid values 4 to 16</span></span>|
|<span data-ttu-id="09324-301">пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="09324-301">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="09324-302">Int32</span><span class="sxs-lookup"><span data-stu-id="09324-302">Int32</span></span>|<span data-ttu-id="09324-303">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="09324-303">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="09324-304">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="09324-304">Valid values 1 to 16</span></span>|
|<span data-ttu-id="09324-305">пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="09324-305">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="09324-306">Int32</span><span class="sxs-lookup"><span data-stu-id="09324-306">Int32</span></span>|<span data-ttu-id="09324-307">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="09324-307">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="09324-308">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="09324-308">Valid values 1 to 16</span></span>|
|<span data-ttu-id="09324-309">пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="09324-309">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="09324-310">Int32</span><span class="sxs-lookup"><span data-stu-id="09324-310">Int32</span></span>|<span data-ttu-id="09324-311">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="09324-311">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="09324-312">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="09324-312">Valid values 1 to 16</span></span>|
|<span data-ttu-id="09324-313">пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="09324-313">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="09324-314">Int32</span><span class="sxs-lookup"><span data-stu-id="09324-314">Int32</span></span>|<span data-ttu-id="09324-315">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="09324-315">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="09324-316">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="09324-316">Valid values 1 to 16</span></span>|
|<span data-ttu-id="09324-317">пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="09324-317">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="09324-318">Int32</span><span class="sxs-lookup"><span data-stu-id="09324-318">Int32</span></span>|<span data-ttu-id="09324-319">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="09324-319">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="09324-320">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="09324-320">Valid values 1 to 16</span></span>|
|<span data-ttu-id="09324-321">пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="09324-321">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="09324-322">Int32</span><span class="sxs-lookup"><span data-stu-id="09324-322">Int32</span></span>|<span data-ttu-id="09324-323">Указывает минимальное число символов верхнего каселеттер, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="09324-323">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="09324-324">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="09324-324">Valid values 1 to 16</span></span>|
|<span data-ttu-id="09324-325">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="09324-325">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="09324-326">Int32</span><span class="sxs-lookup"><span data-stu-id="09324-326">Int32</span></span>|<span data-ttu-id="09324-327">Миллисекунды бездействия до истечения времени ожидания экрана.</span><span class="sxs-lookup"><span data-stu-id="09324-327">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="09324-328">пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="09324-328">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="09324-329">Int32</span><span class="sxs-lookup"><span data-stu-id="09324-329">Int32</span></span>|<span data-ttu-id="09324-330">Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале.</span><span class="sxs-lookup"><span data-stu-id="09324-330">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="09324-331">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="09324-331">Valid values 0 to 24</span></span>|
|<span data-ttu-id="09324-332">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="09324-332">passwordRequiredType</span></span>|[<span data-ttu-id="09324-333">андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="09324-333">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="09324-334">Указывает минимальное качество пароля, необходимое для устройства.</span><span class="sxs-lookup"><span data-stu-id="09324-334">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="09324-335">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="09324-335">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="09324-336">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="09324-336">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="09324-337">Int32</span><span class="sxs-lookup"><span data-stu-id="09324-337">Int32</span></span>|<span data-ttu-id="09324-338">Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="09324-338">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="09324-339">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="09324-339">Valid values 4 to 11</span></span>|
|<span data-ttu-id="09324-340">плайсторемоде</span><span class="sxs-lookup"><span data-stu-id="09324-340">playStoreMode</span></span>|[<span data-ttu-id="09324-341">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="09324-341">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="09324-342">Указывает режим проигрывания устройства в хранилище.</span><span class="sxs-lookup"><span data-stu-id="09324-342">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="09324-343">Возможные значения: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="09324-343">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="09324-344">сафебутблоккед</span><span class="sxs-lookup"><span data-stu-id="09324-344">safeBootBlocked</span></span>|<span data-ttu-id="09324-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-345">Boolean</span></span>|<span data-ttu-id="09324-346">Указывает, отключена ли загрузка устройства в "безопасная загрузка".</span><span class="sxs-lookup"><span data-stu-id="09324-346">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="09324-347">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="09324-347">screenCaptureBlocked</span></span>|<span data-ttu-id="09324-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-348">Boolean</span></span>|<span data-ttu-id="09324-349">Указывает, следует ли отключить возможность использования снимков экрана.</span><span class="sxs-lookup"><span data-stu-id="09324-349">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="09324-350">секуритялловдебуггингфеатурес</span><span class="sxs-lookup"><span data-stu-id="09324-350">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="09324-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-351">Boolean</span></span>|<span data-ttu-id="09324-352">Указывает, следует ли запретить пользователю включать функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="09324-352">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="09324-353">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="09324-353">securityRequireVerifyApps</span></span>|<span data-ttu-id="09324-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-354">Boolean</span></span>|<span data-ttu-id="09324-355">Указывает, требуется ли проверка приложений.</span><span class="sxs-lookup"><span data-stu-id="09324-355">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="09324-356">статусбарблоккед</span><span class="sxs-lookup"><span data-stu-id="09324-356">statusBarBlocked</span></span>|<span data-ttu-id="09324-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-357">Boolean</span></span>|<span data-ttu-id="09324-358">Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.</span><span class="sxs-lookup"><span data-stu-id="09324-358">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="09324-359">стайонмодес</span><span class="sxs-lookup"><span data-stu-id="09324-359">stayOnModes</span></span>|<span data-ttu-id="09324-360">Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="09324-360">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="09324-361">Список режимов, в которых дисплей устройства остается включенным.</span><span class="sxs-lookup"><span data-stu-id="09324-361">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="09324-362">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="09324-362">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="09324-363">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="09324-363">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="09324-364">сторажеалловусб</span><span class="sxs-lookup"><span data-stu-id="09324-364">storageAllowUsb</span></span>|<span data-ttu-id="09324-365">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-365">Boolean</span></span>|<span data-ttu-id="09324-366">Указывает, следует ли разрешить запоминающее устройство USB.</span><span class="sxs-lookup"><span data-stu-id="09324-366">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="09324-367">сторажеблоккекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="09324-367">storageBlockExternalMedia</span></span>|<span data-ttu-id="09324-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-368">Boolean</span></span>|<span data-ttu-id="09324-369">Указывает, следует ли заблокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="09324-369">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="09324-370">сторажеблоккусбфилетрансфер</span><span class="sxs-lookup"><span data-stu-id="09324-370">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="09324-371">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-371">Boolean</span></span>|<span data-ttu-id="09324-372">Указывает, следует ли запретить передачу файлов через USB.</span><span class="sxs-lookup"><span data-stu-id="09324-372">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="09324-373">системупдатевиндовстартминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="09324-373">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="09324-374">Int32</span><span class="sxs-lookup"><span data-stu-id="09324-374">Int32</span></span>|<span data-ttu-id="09324-375">Указывает количество минут после полуночи, когда запустится окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="09324-375">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="09324-376">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="09324-376">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="09324-377">системупдатевиндовендминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="09324-377">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="09324-378">Int32</span><span class="sxs-lookup"><span data-stu-id="09324-378">Int32</span></span>|<span data-ttu-id="09324-379">Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="09324-379">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="09324-380">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="09324-380">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="09324-381">системупдатеинсталлтипе</span><span class="sxs-lookup"><span data-stu-id="09324-381">systemUpdateInstallType</span></span>|[<span data-ttu-id="09324-382">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="09324-382">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="09324-383">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="09324-383">The type of system update configuration.</span></span> <span data-ttu-id="09324-384">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="09324-384">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="09324-385">системвиндовсблоккед</span><span class="sxs-lookup"><span data-stu-id="09324-385">systemWindowsBlocked</span></span>|<span data-ttu-id="09324-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-386">Boolean</span></span>|<span data-ttu-id="09324-387">Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="09324-387">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="09324-388">усерсблоккадд</span><span class="sxs-lookup"><span data-stu-id="09324-388">usersBlockAdd</span></span>|<span data-ttu-id="09324-389">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-389">Boolean</span></span>|<span data-ttu-id="09324-390">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="09324-390">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="09324-391">усерсблоккремове</span><span class="sxs-lookup"><span data-stu-id="09324-391">usersBlockRemove</span></span>|<span data-ttu-id="09324-392">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-392">Boolean</span></span>|<span data-ttu-id="09324-393">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="09324-393">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="09324-394">волумеблоккаджустмент</span><span class="sxs-lookup"><span data-stu-id="09324-394">volumeBlockAdjustment</span></span>|<span data-ttu-id="09324-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-395">Boolean</span></span>|<span data-ttu-id="09324-396">Указывает, отключена ли настройка главного тома.</span><span class="sxs-lookup"><span data-stu-id="09324-396">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="09324-397">впналвайсонлоккдовнмоде</span><span class="sxs-lookup"><span data-stu-id="09324-397">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="09324-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-398">Boolean</span></span>|<span data-ttu-id="09324-399">Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="09324-399">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="09324-400">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="09324-400">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="09324-401">String</span><span class="sxs-lookup"><span data-stu-id="09324-401">String</span></span>|<span data-ttu-id="09324-402">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="09324-402">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="09324-403">вифиблоккедитконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="09324-403">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="09324-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-404">Boolean</span></span>|<span data-ttu-id="09324-405">Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="09324-405">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="09324-406">вифиблоккедитполицидефинедконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="09324-406">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="09324-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="09324-407">Boolean</span></span>|<span data-ttu-id="09324-408">Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="09324-408">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="09324-409">Ответ</span><span class="sxs-lookup"><span data-stu-id="09324-409">Response</span></span>
<span data-ttu-id="09324-410">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="09324-410">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09324-411">Пример</span><span class="sxs-lookup"><span data-stu-id="09324-411">Example</span></span>

### <a name="request"></a><span data-ttu-id="09324-412">Запрос</span><span class="sxs-lookup"><span data-stu-id="09324-412">Request</span></span>
<span data-ttu-id="09324-413">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09324-413">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="09324-414">Отклик</span><span class="sxs-lookup"><span data-stu-id="09324-414">Response</span></span>
<span data-ttu-id="09324-p136">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09324-p136">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



