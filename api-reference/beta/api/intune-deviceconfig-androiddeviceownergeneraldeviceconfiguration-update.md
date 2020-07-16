---
title: Обновление androidDeviceOwnerGeneralDeviceConfiguration
description: Обновление свойств объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0ca9452f034600275acbd59d9a86b7d0c7487910
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123346"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="44fc4-103">Обновление androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="44fc4-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="44fc4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44fc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44fc4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44fc4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44fc4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44fc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44fc4-107">Обновление свойств объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="44fc4-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44fc4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="44fc4-108">Prerequisites</span></span>
<span data-ttu-id="44fc4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44fc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44fc4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44fc4-111">Permission type</span></span>|<span data-ttu-id="44fc4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44fc4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44fc4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44fc4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44fc4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44fc4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44fc4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44fc4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44fc4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44fc4-116">Not supported.</span></span>|
|<span data-ttu-id="44fc4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44fc4-117">Application</span></span>|<span data-ttu-id="44fc4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44fc4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44fc4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44fc4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="44fc4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="44fc4-120">Request headers</span></span>
|<span data-ttu-id="44fc4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44fc4-121">Header</span></span>|<span data-ttu-id="44fc4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="44fc4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44fc4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44fc4-123">Authorization</span></span>|<span data-ttu-id="44fc4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44fc4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44fc4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="44fc4-125">Accept</span></span>|<span data-ttu-id="44fc4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44fc4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44fc4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44fc4-127">Request body</span></span>
<span data-ttu-id="44fc4-128">В тексте запроса добавьте представление объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44fc4-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="44fc4-129">В следующей таблице приведены свойства, необходимые при создании [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44fc4-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="44fc4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="44fc4-130">Property</span></span>|<span data-ttu-id="44fc4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="44fc4-131">Type</span></span>|<span data-ttu-id="44fc4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="44fc4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44fc4-133">id</span><span class="sxs-lookup"><span data-stu-id="44fc4-133">id</span></span>|<span data-ttu-id="44fc4-134">String</span><span class="sxs-lookup"><span data-stu-id="44fc4-134">String</span></span>|<span data-ttu-id="44fc4-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="44fc4-135">Key of the entity.</span></span> <span data-ttu-id="44fc4-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44fc4-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44fc4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44fc4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="44fc4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44fc4-138">DateTimeOffset</span></span>|<span data-ttu-id="44fc4-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="44fc4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="44fc4-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44fc4-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44fc4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="44fc4-141">roleScopeTagIds</span></span>|<span data-ttu-id="44fc4-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="44fc4-142">String collection</span></span>|<span data-ttu-id="44fc4-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="44fc4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="44fc4-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44fc4-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44fc4-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="44fc4-145">supportsScopeTags</span></span>|<span data-ttu-id="44fc4-146">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-146">Boolean</span></span>|<span data-ttu-id="44fc4-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="44fc4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="44fc4-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="44fc4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="44fc4-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="44fc4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="44fc4-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="44fc4-150">This property is read-only.</span></span> <span data-ttu-id="44fc4-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44fc4-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44fc4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="44fc4-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="44fc4-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="44fc4-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="44fc4-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="44fc4-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="44fc4-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44fc4-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44fc4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="44fc4-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="44fc4-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="44fc4-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="44fc4-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="44fc4-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="44fc4-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44fc4-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44fc4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="44fc4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="44fc4-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="44fc4-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="44fc4-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="44fc4-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="44fc4-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44fc4-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44fc4-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44fc4-164">createdDateTime</span></span>|<span data-ttu-id="44fc4-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44fc4-165">DateTimeOffset</span></span>|<span data-ttu-id="44fc4-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="44fc4-166">DateTime the object was created.</span></span> <span data-ttu-id="44fc4-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44fc4-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44fc4-168">description</span><span class="sxs-lookup"><span data-stu-id="44fc4-168">description</span></span>|<span data-ttu-id="44fc4-169">String</span><span class="sxs-lookup"><span data-stu-id="44fc4-169">String</span></span>|<span data-ttu-id="44fc4-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="44fc4-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="44fc4-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44fc4-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44fc4-172">displayName</span><span class="sxs-lookup"><span data-stu-id="44fc4-172">displayName</span></span>|<span data-ttu-id="44fc4-173">Строка</span><span class="sxs-lookup"><span data-stu-id="44fc4-173">String</span></span>|<span data-ttu-id="44fc4-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="44fc4-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="44fc4-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44fc4-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44fc4-176">version</span><span class="sxs-lookup"><span data-stu-id="44fc4-176">version</span></span>|<span data-ttu-id="44fc4-177">Int32</span><span class="sxs-lookup"><span data-stu-id="44fc4-177">Int32</span></span>|<span data-ttu-id="44fc4-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="44fc4-178">Version of the device configuration.</span></span> <span data-ttu-id="44fc4-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44fc4-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44fc4-180">аккаунтсблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="44fc4-180">accountsBlockModification</span></span>|<span data-ttu-id="44fc4-181">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-181">Boolean</span></span>|<span data-ttu-id="44fc4-182">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="44fc4-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="44fc4-183">аппсалловинсталлфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="44fc4-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="44fc4-184">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-184">Boolean</span></span>|<span data-ttu-id="44fc4-185">Указывает, может ли пользователь включить параметр "неизвестные источники".</span><span class="sxs-lookup"><span data-stu-id="44fc4-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="44fc4-186">аппсаутаупдатеполици</span><span class="sxs-lookup"><span data-stu-id="44fc4-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="44fc4-187">андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="44fc4-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="44fc4-188">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="44fc4-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="44fc4-189">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="44fc4-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="44fc4-190">аппсдефаултпермиссионполици</span><span class="sxs-lookup"><span data-stu-id="44fc4-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="44fc4-191">андроиддевицеовнердефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="44fc4-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="44fc4-192">Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом.</span><span class="sxs-lookup"><span data-stu-id="44fc4-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="44fc4-193">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="44fc4-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="44fc4-194">аппсрекоммендскиппингфирстусехинтс</span><span class="sxs-lookup"><span data-stu-id="44fc4-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="44fc4-195">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-195">Boolean</span></span>|<span data-ttu-id="44fc4-196">Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.</span><span class="sxs-lookup"><span data-stu-id="44fc4-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="44fc4-197">блуетусблоккконфигуратион</span><span class="sxs-lookup"><span data-stu-id="44fc4-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="44fc4-198">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-198">Boolean</span></span>|<span data-ttu-id="44fc4-199">Указывает, следует ли запретить пользователю настраивать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="44fc4-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="44fc4-200">блуетусблоккконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="44fc4-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="44fc4-201">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-201">Boolean</span></span>|<span data-ttu-id="44fc4-202">Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="44fc4-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="44fc4-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="44fc4-203">cameraBlocked</span></span>|<span data-ttu-id="44fc4-204">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-204">Boolean</span></span>|<span data-ttu-id="44fc4-205">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="44fc4-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="44fc4-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="44fc4-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="44fc4-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="44fc4-207">Boolean</span></span>|<span data-ttu-id="44fc4-208">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="44fc4-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="44fc4-209">цертификатекредентиалконфигуратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="44fc4-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="44fc4-210">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-210">Boolean</span></span>|<span data-ttu-id="44fc4-211">Указывает, следует ли запретить пользователям настраивать учетные данные сертификатов.</span><span class="sxs-lookup"><span data-stu-id="44fc4-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="44fc4-212">микрософтлаунчерконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="44fc4-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="44fc4-213">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-213">Boolean</span></span>|<span data-ttu-id="44fc4-214">Указывает, следует ли настроить средство запуска Microsoft.</span><span class="sxs-lookup"><span data-stu-id="44fc4-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="44fc4-215">микрософтлаунчеркустомваллпаперенаблед</span><span class="sxs-lookup"><span data-stu-id="44fc4-215">microsoftLauncherCustomWallpaperEnabled</span></span>|<span data-ttu-id="44fc4-216">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-216">Boolean</span></span>|<span data-ttu-id="44fc4-217">Указывает, следует ли настраивать фоновый рисунок на целевых устройствах.</span><span class="sxs-lookup"><span data-stu-id="44fc4-217">Indicates whether or not to configure the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="44fc4-218">микрософтлаунчеркустомваллпаперимажеурл</span><span class="sxs-lookup"><span data-stu-id="44fc4-218">microsoftLauncherCustomWallpaperImageUrl</span></span>|<span data-ttu-id="44fc4-219">String</span><span class="sxs-lookup"><span data-stu-id="44fc4-219">String</span></span>|<span data-ttu-id="44fc4-220">Указывает URL-адрес для файла изображения, который будет использоваться в качестве фонового рисунка на целевых устройствах.</span><span class="sxs-lookup"><span data-stu-id="44fc4-220">Indicates the URL for the image file to use as the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="44fc4-221">микрософтлаунчеркустомваллпапералловусермодификатион</span><span class="sxs-lookup"><span data-stu-id="44fc4-221">microsoftLauncherCustomWallpaperAllowUserModification</span></span>|<span data-ttu-id="44fc4-222">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-222">Boolean</span></span>|<span data-ttu-id="44fc4-223">Указывает, может ли пользователь изменять фоновый рисунок для персонализации своего устройства.</span><span class="sxs-lookup"><span data-stu-id="44fc4-223">Indicates whether or not the user can modify the wallpaper to personalize their device.</span></span>|
|<span data-ttu-id="44fc4-224">микрософтлаунчерфиденаблед</span><span class="sxs-lookup"><span data-stu-id="44fc4-224">microsoftLauncherFeedEnabled</span></span>|<span data-ttu-id="44fc4-225">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-225">Boolean</span></span>|<span data-ttu-id="44fc4-226">Указывает, следует ли включить веб-канал запуска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="44fc4-226">Indicates whether or not you want to enable the launcher feed on the device.</span></span>|
|<span data-ttu-id="44fc4-227">микрософтлаунчерфидалловусермодификатион</span><span class="sxs-lookup"><span data-stu-id="44fc4-227">microsoftLauncherFeedAllowUserModification</span></span>|<span data-ttu-id="44fc4-228">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-228">Boolean</span></span>|<span data-ttu-id="44fc4-229">Указывает, может ли пользователь изменять веб-канал запуска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="44fc4-229">Indicates whether or not the user can modify the launcher feed on the device.</span></span>|
|<span data-ttu-id="44fc4-230">микрософтлаунчердоккпресенцеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="44fc4-230">microsoftLauncherDockPresenceConfiguration</span></span>|[<span data-ttu-id="44fc4-231">microsoftLauncherDockPresence</span><span class="sxs-lookup"><span data-stu-id="44fc4-231">microsoftLauncherDockPresence</span></span>](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|<span data-ttu-id="44fc4-232">Указывает, следует ли настроить закрепление устройства.</span><span class="sxs-lookup"><span data-stu-id="44fc4-232">Indicates whether or not you want to configure the device dock.</span></span> <span data-ttu-id="44fc4-233">Возможные значения: `notConfigured`, `show`, `hide`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="44fc4-233">Possible values are: `notConfigured`, `show`, `hide`, `disabled`.</span></span>|
|<span data-ttu-id="44fc4-234">микрософтлаунчердоккпресенцеалловусермодификатион</span><span class="sxs-lookup"><span data-stu-id="44fc4-234">microsoftLauncherDockPresenceAllowUserModification</span></span>|<span data-ttu-id="44fc4-235">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-235">Boolean</span></span>|<span data-ttu-id="44fc4-236">Указывает, может ли пользователь изменять конфигурацию закрепления устройств на устройстве.</span><span class="sxs-lookup"><span data-stu-id="44fc4-236">Indicates whether or not the user can modify the device dock configuration on the device.</span></span>|
|<span data-ttu-id="44fc4-237">микрософтлаунчерсеарчбарплацементконфигуратион</span><span class="sxs-lookup"><span data-stu-id="44fc4-237">microsoftLauncherSearchBarPlacementConfiguration</span></span>|[<span data-ttu-id="44fc4-238">microsoftLauncherSearchBarPlacement</span><span class="sxs-lookup"><span data-stu-id="44fc4-238">microsoftLauncherSearchBarPlacement</span></span>](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|<span data-ttu-id="44fc4-239">Указывает конфигурацию размещения панели поиска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="44fc4-239">Indicates the search bar placement configuration on the device.</span></span> <span data-ttu-id="44fc4-240">Возможные значения: `notConfigured`, `top`, `bottom`, `hide`.</span><span class="sxs-lookup"><span data-stu-id="44fc4-240">Possible values are: `notConfigured`, `top`, `bottom`, `hide`.</span></span>|
|<span data-ttu-id="44fc4-241">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="44fc4-241">enrollmentProfile</span></span>|[<span data-ttu-id="44fc4-242">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="44fc4-242">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="44fc4-243">Указывает, какой профиль регистрации вы хотите настроить.</span><span class="sxs-lookup"><span data-stu-id="44fc4-243">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="44fc4-244">Возможные значения: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span><span class="sxs-lookup"><span data-stu-id="44fc4-244">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="44fc4-245">датароамингблоккед</span><span class="sxs-lookup"><span data-stu-id="44fc4-245">dataRoamingBlocked</span></span>|<span data-ttu-id="44fc4-246">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-246">Boolean</span></span>|<span data-ttu-id="44fc4-247">Указывает, следует ли запретить пользователю перемещать данные.</span><span class="sxs-lookup"><span data-stu-id="44fc4-247">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="44fc4-248">датетимеконфигуратионблоккед</span><span class="sxs-lookup"><span data-stu-id="44fc4-248">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="44fc4-249">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-249">Boolean</span></span>|<span data-ttu-id="44fc4-250">Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.</span><span class="sxs-lookup"><span data-stu-id="44fc4-250">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="44fc4-251">факториресетдевицеадминистраторемаилс</span><span class="sxs-lookup"><span data-stu-id="44fc4-251">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="44fc4-252">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="44fc4-252">String collection</span></span>|<span data-ttu-id="44fc4-253">Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.</span><span class="sxs-lookup"><span data-stu-id="44fc4-253">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="44fc4-254">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="44fc4-254">factoryResetBlocked</span></span>|<span data-ttu-id="44fc4-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="44fc4-255">Boolean</span></span>|<span data-ttu-id="44fc4-256">Указывает, отключен ли параметр Reset фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="44fc4-256">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="44fc4-257">глобалпрокси</span><span class="sxs-lookup"><span data-stu-id="44fc4-257">globalProxy</span></span>|[<span data-ttu-id="44fc4-258">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="44fc4-258">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="44fc4-259">Прокси-сервер настраивается напрямую с узлом, портом и исключенными узлами.</span><span class="sxs-lookup"><span data-stu-id="44fc4-259">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="44fc4-260">гуглеаккаунтсблоккед</span><span class="sxs-lookup"><span data-stu-id="44fc4-260">googleAccountsBlocked</span></span>|<span data-ttu-id="44fc4-261">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-261">Boolean</span></span>|<span data-ttu-id="44fc4-262">Указывает, будут ли блокироваться учетные записи Google.</span><span class="sxs-lookup"><span data-stu-id="44fc4-262">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="44fc4-263">киоскмодескринсаверконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="44fc4-263">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="44fc4-264">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-264">Boolean</span></span>|<span data-ttu-id="44fc4-265">Указывает, следует ли включить режим экранной заставки или не в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-265">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="44fc4-266">киоскмодескринсаверимажеурл</span><span class="sxs-lookup"><span data-stu-id="44fc4-266">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="44fc4-267">String</span><span class="sxs-lookup"><span data-stu-id="44fc4-267">String</span></span>|<span data-ttu-id="44fc4-268">URL-адрес изображения, которое будет экранной заставкой устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-268">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="44fc4-269">киоскмодескринсавердисплайтимеинсекондс</span><span class="sxs-lookup"><span data-stu-id="44fc4-269">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="44fc4-270">Int32</span><span class="sxs-lookup"><span data-stu-id="44fc4-270">Int32</span></span>|<span data-ttu-id="44fc4-271">Время (в секундах), в течение которого устройство будет отображать экранную заставку в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-271">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="44fc4-272">Допустимые значения — от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="44fc4-272">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="44fc4-273">киоскмодескринсаверстартделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="44fc4-273">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="44fc4-274">Int32</span><span class="sxs-lookup"><span data-stu-id="44fc4-274">Int32</span></span>|<span data-ttu-id="44fc4-275">Время (в секундах), в течение которого устройство должно быть неактивным, чтобы экранная заставка отображалась в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-275">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="44fc4-276">Допустимые значения — от 1 до 9999999</span><span class="sxs-lookup"><span data-stu-id="44fc4-276">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="44fc4-277">киоскмодескринсавердетектмедиадисаблед</span><span class="sxs-lookup"><span data-stu-id="44fc4-277">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="44fc4-278">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-278">Boolean</span></span>|<span data-ttu-id="44fc4-279">Указывает, должно ли устройство отображать экранную заставку при воспроизведении аудио-и видеоконференций в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="44fc4-279">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="44fc4-280">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="44fc4-280">kioskModeApps</span></span>|<span data-ttu-id="44fc4-281">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="44fc4-281">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="44fc4-282">Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-282">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="44fc4-283">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="44fc4-283">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="44fc4-284">киоскмодеваллпаперурл</span><span class="sxs-lookup"><span data-stu-id="44fc4-284">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="44fc4-285">String</span><span class="sxs-lookup"><span data-stu-id="44fc4-285">String</span></span>|<span data-ttu-id="44fc4-286">URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-286">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="44fc4-287">киоскмодикситкоде</span><span class="sxs-lookup"><span data-stu-id="44fc4-287">kioskModeExitCode</span></span>|<span data-ttu-id="44fc4-288">String</span><span class="sxs-lookup"><span data-stu-id="44fc4-288">String</span></span>|<span data-ttu-id="44fc4-289">Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-289">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="44fc4-290">киоскмодевиртуалхомебуттоненаблед</span><span class="sxs-lookup"><span data-stu-id="44fc4-290">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="44fc4-291">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-291">Boolean</span></span>|<span data-ttu-id="44fc4-292">Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-292">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="44fc4-293">киоскмодевиртуалхомебуттонтипе</span><span class="sxs-lookup"><span data-stu-id="44fc4-293">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="44fc4-294">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="44fc4-294">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="44fc4-295">Указывает, является ли кнопка "Виртуальная Домашняя страница" кнопкой "Прокрутка вверх" или плавающей кнопкой "домой".</span><span class="sxs-lookup"><span data-stu-id="44fc4-295">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="44fc4-296">Возможные значения: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="44fc4-296">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="44fc4-297">киоскмодеблуетусконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="44fc4-297">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="44fc4-298">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-298">Boolean</span></span>|<span data-ttu-id="44fc4-299">Указывает, следует ли запретить пользователю настраивать параметры Bluetooth в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-299">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="44fc4-300">киоскмодевификонфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="44fc4-300">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="44fc4-301">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-301">Boolean</span></span>|<span data-ttu-id="44fc4-302">Указывает, следует ли разрешить пользователю настраивать параметры Wi/Fi в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-302">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="44fc4-303">киоскмодефлашлигхтконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="44fc4-303">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="44fc4-304">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-304">Boolean</span></span>|<span data-ttu-id="44fc4-305">Указывает, следует ли разрешить пользователю использовать флашлигхт в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-305">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="44fc4-306">киоскмодемедиаволумеконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="44fc4-306">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="44fc4-307">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-307">Boolean</span></span>|<span data-ttu-id="44fc4-308">Указывает, следует ли запретить пользователю изменять громкость мультимедиа в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-308">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="44fc4-309">киоскмодешовдевицеинфо</span><span class="sxs-lookup"><span data-stu-id="44fc4-309">kioskModeShowDeviceInfo</span></span>|<span data-ttu-id="44fc4-310">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-310">Boolean</span></span>|<span data-ttu-id="44fc4-311">Указывает, следует ли разрешить пользователю доступ к сведениям о базовом устройстве.</span><span class="sxs-lookup"><span data-stu-id="44fc4-311">Whether or not to allow a user to access basic device information.</span></span>|
|<span data-ttu-id="44fc4-312">киоскмодеманажедсеттингсентридисаблед</span><span class="sxs-lookup"><span data-stu-id="44fc4-312">kioskModeManagedSettingsEntryDisabled</span></span>|<span data-ttu-id="44fc4-313">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-313">Boolean</span></span>|<span data-ttu-id="44fc4-314">Указывает, следует ли отображать точку входа управляемых параметров на управляемом домашнем экране в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-314">Whether or not to display the Managed Settings entry point on the managed home screen in Kiosk Mode.</span></span>|
|<span data-ttu-id="44fc4-315">киоскмодедебугменуеасякцессенаблед</span><span class="sxs-lookup"><span data-stu-id="44fc4-315">kioskModeDebugMenuEasyAccessEnabled</span></span>|<span data-ttu-id="44fc4-316">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-316">Boolean</span></span>|<span data-ttu-id="44fc4-317">Указывает, следует ли запретить пользователю простой доступ к меню Отладка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-317">Whether or not to allow a user to easy access to the debug menu in Kiosk Mode.</span></span>|
|<span data-ttu-id="44fc4-318">киоскмодешоваппнотификатионбадже</span><span class="sxs-lookup"><span data-stu-id="44fc4-318">kioskModeShowAppNotificationBadge</span></span>|<span data-ttu-id="44fc4-319">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-319">Boolean</span></span>|<span data-ttu-id="44fc4-320">Указывает, следует ли отображать эмблемы уведомлений приложений в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-320">Whether or not to display application notification badges in Kiosk Mode.</span></span>|
|<span data-ttu-id="44fc4-321">киоскмодескринориентатион</span><span class="sxs-lookup"><span data-stu-id="44fc4-321">kioskModeScreenOrientation</span></span>|[<span data-ttu-id="44fc4-322">андроиддевицеовнеркиоскмодескринориентатион</span><span class="sxs-lookup"><span data-stu-id="44fc4-322">androidDeviceOwnerKioskModeScreenOrientation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|<span data-ttu-id="44fc4-323">Конфигурация ориентации экрана для управляемого экрана дома в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-323">Screen orientation configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="44fc4-324">Возможные значения: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span><span class="sxs-lookup"><span data-stu-id="44fc4-324">Possible values are: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span></span>|
|<span data-ttu-id="44fc4-325">киоскмодеиконсизе</span><span class="sxs-lookup"><span data-stu-id="44fc4-325">kioskModeIconSize</span></span>|[<span data-ttu-id="44fc4-326">андроиддевицеовнеркиоскмодеиконсизе</span><span class="sxs-lookup"><span data-stu-id="44fc4-326">androidDeviceOwnerKioskModeIconSize</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|<span data-ttu-id="44fc4-327">Конфигурация размера значков для управляемого экрана дома в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-327">Icon size configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="44fc4-328">Возможные значения: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span><span class="sxs-lookup"><span data-stu-id="44fc4-328">Possible values are: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span></span>|
|<span data-ttu-id="44fc4-329">киоскмодефолдерикон</span><span class="sxs-lookup"><span data-stu-id="44fc4-329">kioskModeFolderIcon</span></span>|[<span data-ttu-id="44fc4-330">андроиддевицеовнеркиоскмодефолдерикон</span><span class="sxs-lookup"><span data-stu-id="44fc4-330">androidDeviceOwnerKioskModeFolderIcon</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|<span data-ttu-id="44fc4-331">Конфигурация значков папок для управляемого экрана дома в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-331">Folder icon configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="44fc4-332">Возможные значения: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span><span class="sxs-lookup"><span data-stu-id="44fc4-332">Possible values are: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span></span>|
|<span data-ttu-id="44fc4-333">киоскмодевифиалловедссидс</span><span class="sxs-lookup"><span data-stu-id="44fc4-333">kioskModeWifiAllowedSsids</span></span>|<span data-ttu-id="44fc4-334">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="44fc4-334">String collection</span></span>|<span data-ttu-id="44fc4-335">Ограниченный набор подключений WIFI SSID, доступных пользователю для настройки в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44fc4-335">The restricted set of WIFI SSIDs available for the user to configure in Kiosk Mode.</span></span> <span data-ttu-id="44fc4-336">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="44fc4-336">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="44fc4-337">микрофонефорцемуте</span><span class="sxs-lookup"><span data-stu-id="44fc4-337">microphoneForceMute</span></span>|<span data-ttu-id="44fc4-338">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-338">Boolean</span></span>|<span data-ttu-id="44fc4-339">Указывает, следует ли запретить разблокирование микрофона устройства.</span><span class="sxs-lookup"><span data-stu-id="44fc4-339">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="44fc4-340">нетворкескапехатчалловед</span><span class="sxs-lookup"><span data-stu-id="44fc4-340">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="44fc4-341">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-341">Boolean</span></span>|<span data-ttu-id="44fc4-342">Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="44fc4-342">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="44fc4-343">нфкблоккаутгоингбеам</span><span class="sxs-lookup"><span data-stu-id="44fc4-343">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="44fc4-344">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-344">Boolean</span></span>|<span data-ttu-id="44fc4-345">Указывает, следует ли заблокировать исходящую форму NFC.</span><span class="sxs-lookup"><span data-stu-id="44fc4-345">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="44fc4-346">пассвордблокккэйгуард</span><span class="sxs-lookup"><span data-stu-id="44fc4-346">passwordBlockKeyguard</span></span>|<span data-ttu-id="44fc4-347">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-347">Boolean</span></span>|<span data-ttu-id="44fc4-348">Указывает, отключен ли кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="44fc4-348">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="44fc4-349">пассвордблокккэйгуардфеатурес</span><span class="sxs-lookup"><span data-stu-id="44fc4-349">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="44fc4-350">Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="44fc4-350">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="44fc4-351">Список компонентов кэйгуард устройств, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="44fc4-351">List of device keyguard features to block.</span></span> <span data-ttu-id="44fc4-352">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="44fc4-352">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="44fc4-353">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="44fc4-353">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="44fc4-354">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="44fc4-354">passwordExpirationDays</span></span>|<span data-ttu-id="44fc4-355">Int32</span><span class="sxs-lookup"><span data-stu-id="44fc4-355">Int32</span></span>|<span data-ttu-id="44fc4-356">Указывает время в секундах, в течение которого можно задать пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="44fc4-356">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="44fc4-357">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="44fc4-357">Valid values 1 to 365</span></span>|
|<span data-ttu-id="44fc4-358">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="44fc4-358">passwordMinimumLength</span></span>|<span data-ttu-id="44fc4-359">Int32</span><span class="sxs-lookup"><span data-stu-id="44fc4-359">Int32</span></span>|<span data-ttu-id="44fc4-360">Указывает минимальную длину пароля, необходимого для устройства.</span><span class="sxs-lookup"><span data-stu-id="44fc4-360">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="44fc4-361">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="44fc4-361">Valid values 4 to 16</span></span>|
|<span data-ttu-id="44fc4-362">пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="44fc4-362">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="44fc4-363">Int32</span><span class="sxs-lookup"><span data-stu-id="44fc4-363">Int32</span></span>|<span data-ttu-id="44fc4-364">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="44fc4-364">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="44fc4-365">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="44fc4-365">Valid values 1 to 16</span></span>|
|<span data-ttu-id="44fc4-366">пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="44fc4-366">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="44fc4-367">Int32</span><span class="sxs-lookup"><span data-stu-id="44fc4-367">Int32</span></span>|<span data-ttu-id="44fc4-368">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="44fc4-368">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="44fc4-369">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="44fc4-369">Valid values 1 to 16</span></span>|
|<span data-ttu-id="44fc4-370">пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="44fc4-370">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="44fc4-371">Int32</span><span class="sxs-lookup"><span data-stu-id="44fc4-371">Int32</span></span>|<span data-ttu-id="44fc4-372">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="44fc4-372">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="44fc4-373">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="44fc4-373">Valid values 1 to 16</span></span>|
|<span data-ttu-id="44fc4-374">пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="44fc4-374">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="44fc4-375">Int32</span><span class="sxs-lookup"><span data-stu-id="44fc4-375">Int32</span></span>|<span data-ttu-id="44fc4-376">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="44fc4-376">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="44fc4-377">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="44fc4-377">Valid values 1 to 16</span></span>|
|<span data-ttu-id="44fc4-378">пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="44fc4-378">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="44fc4-379">Int32</span><span class="sxs-lookup"><span data-stu-id="44fc4-379">Int32</span></span>|<span data-ttu-id="44fc4-380">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="44fc4-380">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="44fc4-381">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="44fc4-381">Valid values 1 to 16</span></span>|
|<span data-ttu-id="44fc4-382">пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="44fc4-382">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="44fc4-383">Int32</span><span class="sxs-lookup"><span data-stu-id="44fc4-383">Int32</span></span>|<span data-ttu-id="44fc4-384">Указывает минимальное число символов верхнего каселеттер, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="44fc4-384">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="44fc4-385">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="44fc4-385">Valid values 1 to 16</span></span>|
|<span data-ttu-id="44fc4-386">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="44fc4-386">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="44fc4-387">Int32</span><span class="sxs-lookup"><span data-stu-id="44fc4-387">Int32</span></span>|<span data-ttu-id="44fc4-388">Миллисекунды бездействия до истечения времени ожидания экрана.</span><span class="sxs-lookup"><span data-stu-id="44fc4-388">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="44fc4-389">пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="44fc4-389">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="44fc4-390">Int32</span><span class="sxs-lookup"><span data-stu-id="44fc4-390">Int32</span></span>|<span data-ttu-id="44fc4-391">Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале.</span><span class="sxs-lookup"><span data-stu-id="44fc4-391">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="44fc4-392">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="44fc4-392">Valid values 0 to 24</span></span>|
|<span data-ttu-id="44fc4-393">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="44fc4-393">passwordRequiredType</span></span>|[<span data-ttu-id="44fc4-394">андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="44fc4-394">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="44fc4-395">Указывает минимальное качество пароля, необходимое для устройства.</span><span class="sxs-lookup"><span data-stu-id="44fc4-395">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="44fc4-396">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="44fc4-396">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="44fc4-397">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="44fc4-397">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="44fc4-398">Int32</span><span class="sxs-lookup"><span data-stu-id="44fc4-398">Int32</span></span>|<span data-ttu-id="44fc4-399">Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="44fc4-399">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="44fc4-400">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="44fc4-400">Valid values 4 to 11</span></span>|
|<span data-ttu-id="44fc4-401">плайсторемоде</span><span class="sxs-lookup"><span data-stu-id="44fc4-401">playStoreMode</span></span>|[<span data-ttu-id="44fc4-402">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="44fc4-402">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="44fc4-403">Указывает режим проигрывания устройства в хранилище.</span><span class="sxs-lookup"><span data-stu-id="44fc4-403">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="44fc4-404">Возможные значения: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="44fc4-404">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="44fc4-405">сафебутблоккед</span><span class="sxs-lookup"><span data-stu-id="44fc4-405">safeBootBlocked</span></span>|<span data-ttu-id="44fc4-406">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-406">Boolean</span></span>|<span data-ttu-id="44fc4-407">Указывает, отключена ли загрузка устройства в "безопасная загрузка".</span><span class="sxs-lookup"><span data-stu-id="44fc4-407">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="44fc4-408">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="44fc4-408">screenCaptureBlocked</span></span>|<span data-ttu-id="44fc4-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="44fc4-409">Boolean</span></span>|<span data-ttu-id="44fc4-410">Указывает, следует ли отключить возможность использования снимков экрана.</span><span class="sxs-lookup"><span data-stu-id="44fc4-410">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="44fc4-411">секуритялловдебуггингфеатурес</span><span class="sxs-lookup"><span data-stu-id="44fc4-411">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="44fc4-412">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-412">Boolean</span></span>|<span data-ttu-id="44fc4-413">Указывает, следует ли запретить пользователю включать функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="44fc4-413">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="44fc4-414">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="44fc4-414">securityRequireVerifyApps</span></span>|<span data-ttu-id="44fc4-415">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-415">Boolean</span></span>|<span data-ttu-id="44fc4-416">Указывает, требуется ли проверка приложений.</span><span class="sxs-lookup"><span data-stu-id="44fc4-416">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="44fc4-417">статусбарблоккед</span><span class="sxs-lookup"><span data-stu-id="44fc4-417">statusBarBlocked</span></span>|<span data-ttu-id="44fc4-418">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-418">Boolean</span></span>|<span data-ttu-id="44fc4-419">Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.</span><span class="sxs-lookup"><span data-stu-id="44fc4-419">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="44fc4-420">стайонмодес</span><span class="sxs-lookup"><span data-stu-id="44fc4-420">stayOnModes</span></span>|<span data-ttu-id="44fc4-421">Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="44fc4-421">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="44fc4-422">Список режимов, в которых дисплей устройства остается включенным.</span><span class="sxs-lookup"><span data-stu-id="44fc4-422">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="44fc4-423">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="44fc4-423">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="44fc4-424">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="44fc4-424">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="44fc4-425">сторажеалловусб</span><span class="sxs-lookup"><span data-stu-id="44fc4-425">storageAllowUsb</span></span>|<span data-ttu-id="44fc4-426">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-426">Boolean</span></span>|<span data-ttu-id="44fc4-427">Указывает, следует ли разрешить запоминающее устройство USB.</span><span class="sxs-lookup"><span data-stu-id="44fc4-427">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="44fc4-428">сторажеблоккекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="44fc4-428">storageBlockExternalMedia</span></span>|<span data-ttu-id="44fc4-429">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-429">Boolean</span></span>|<span data-ttu-id="44fc4-430">Указывает, следует ли заблокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="44fc4-430">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="44fc4-431">сторажеблоккусбфилетрансфер</span><span class="sxs-lookup"><span data-stu-id="44fc4-431">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="44fc4-432">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-432">Boolean</span></span>|<span data-ttu-id="44fc4-433">Указывает, следует ли запретить передачу файлов через USB.</span><span class="sxs-lookup"><span data-stu-id="44fc4-433">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="44fc4-434">системупдатевиндовстартминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="44fc4-434">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="44fc4-435">Int32</span><span class="sxs-lookup"><span data-stu-id="44fc4-435">Int32</span></span>|<span data-ttu-id="44fc4-436">Указывает количество минут после полуночи, когда запустится окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="44fc4-436">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="44fc4-437">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="44fc4-437">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="44fc4-438">системупдатевиндовендминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="44fc4-438">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="44fc4-439">Int32</span><span class="sxs-lookup"><span data-stu-id="44fc4-439">Int32</span></span>|<span data-ttu-id="44fc4-440">Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="44fc4-440">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="44fc4-441">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="44fc4-441">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="44fc4-442">системупдатеинсталлтипе</span><span class="sxs-lookup"><span data-stu-id="44fc4-442">systemUpdateInstallType</span></span>|[<span data-ttu-id="44fc4-443">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="44fc4-443">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="44fc4-444">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="44fc4-444">The type of system update configuration.</span></span> <span data-ttu-id="44fc4-445">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="44fc4-445">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="44fc4-446">системвиндовсблоккед</span><span class="sxs-lookup"><span data-stu-id="44fc4-446">systemWindowsBlocked</span></span>|<span data-ttu-id="44fc4-447">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-447">Boolean</span></span>|<span data-ttu-id="44fc4-448">Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="44fc4-448">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="44fc4-449">усерсблоккадд</span><span class="sxs-lookup"><span data-stu-id="44fc4-449">usersBlockAdd</span></span>|<span data-ttu-id="44fc4-450">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-450">Boolean</span></span>|<span data-ttu-id="44fc4-451">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="44fc4-451">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="44fc4-452">усерсблоккремове</span><span class="sxs-lookup"><span data-stu-id="44fc4-452">usersBlockRemove</span></span>|<span data-ttu-id="44fc4-453">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-453">Boolean</span></span>|<span data-ttu-id="44fc4-454">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="44fc4-454">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="44fc4-455">волумеблоккаджустмент</span><span class="sxs-lookup"><span data-stu-id="44fc4-455">volumeBlockAdjustment</span></span>|<span data-ttu-id="44fc4-456">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-456">Boolean</span></span>|<span data-ttu-id="44fc4-457">Указывает, отключена ли настройка главного тома.</span><span class="sxs-lookup"><span data-stu-id="44fc4-457">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="44fc4-458">впналвайсонлоккдовнмоде</span><span class="sxs-lookup"><span data-stu-id="44fc4-458">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="44fc4-459">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-459">Boolean</span></span>|<span data-ttu-id="44fc4-460">Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="44fc4-460">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="44fc4-461">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="44fc4-461">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="44fc4-462">String</span><span class="sxs-lookup"><span data-stu-id="44fc4-462">String</span></span>|<span data-ttu-id="44fc4-463">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="44fc4-463">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="44fc4-464">вифиблоккедитконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="44fc4-464">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="44fc4-465">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-465">Boolean</span></span>|<span data-ttu-id="44fc4-466">Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="44fc4-466">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="44fc4-467">вифиблоккедитполицидефинедконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="44fc4-467">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="44fc4-468">Логический</span><span class="sxs-lookup"><span data-stu-id="44fc4-468">Boolean</span></span>|<span data-ttu-id="44fc4-469">Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="44fc4-469">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="44fc4-470">Отклик</span><span class="sxs-lookup"><span data-stu-id="44fc4-470">Response</span></span>
<span data-ttu-id="44fc4-471">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44fc4-471">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44fc4-472">Пример</span><span class="sxs-lookup"><span data-stu-id="44fc4-472">Example</span></span>

### <a name="request"></a><span data-ttu-id="44fc4-473">Запрос</span><span class="sxs-lookup"><span data-stu-id="44fc4-473">Request</span></span>
<span data-ttu-id="44fc4-474">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44fc4-474">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 5359

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
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "show",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "top",
  "enrollmentProfile": "dedicatedDevice",
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
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "portrait",
  "kioskModeIconSize": "smallest",
  "kioskModeFolderIcon": "darkSquare",
  "kioskModeWifiAllowedSsids": [
    "Kiosk Mode Wifi Allowed Ssids value"
  ],
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

### <a name="response"></a><span data-ttu-id="44fc4-475">Отклик</span><span class="sxs-lookup"><span data-stu-id="44fc4-475">Response</span></span>
<span data-ttu-id="44fc4-p143">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44fc4-p143">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5531

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
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "show",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "top",
  "enrollmentProfile": "dedicatedDevice",
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
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "portrait",
  "kioskModeIconSize": "smallest",
  "kioskModeFolderIcon": "darkSquare",
  "kioskModeWifiAllowedSsids": [
    "Kiosk Mode Wifi Allowed Ssids value"
  ],
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



