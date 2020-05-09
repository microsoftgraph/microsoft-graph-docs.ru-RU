---
title: Обновление androidDeviceOwnerGeneralDeviceConfiguration
description: Обновление свойств объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ec76020364ee73e173804a47acd29c5225af17cf
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178726"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="060ac-103">Обновление androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="060ac-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="060ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="060ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="060ac-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="060ac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="060ac-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="060ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="060ac-107">Обновление свойств объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="060ac-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="060ac-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="060ac-108">Prerequisites</span></span>
<span data-ttu-id="060ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="060ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="060ac-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="060ac-111">Permission type</span></span>|<span data-ttu-id="060ac-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="060ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="060ac-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="060ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="060ac-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="060ac-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="060ac-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="060ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="060ac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="060ac-116">Not supported.</span></span>|
|<span data-ttu-id="060ac-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="060ac-117">Application</span></span>|<span data-ttu-id="060ac-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="060ac-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="060ac-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="060ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="060ac-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="060ac-120">Request headers</span></span>
|<span data-ttu-id="060ac-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="060ac-121">Header</span></span>|<span data-ttu-id="060ac-122">Значение</span><span class="sxs-lookup"><span data-stu-id="060ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="060ac-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="060ac-123">Authorization</span></span>|<span data-ttu-id="060ac-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="060ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="060ac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="060ac-125">Accept</span></span>|<span data-ttu-id="060ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="060ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="060ac-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="060ac-127">Request body</span></span>
<span data-ttu-id="060ac-128">В тексте запроса добавьте представление объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="060ac-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="060ac-129">В следующей таблице приведены свойства, необходимые при создании [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060ac-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="060ac-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="060ac-130">Property</span></span>|<span data-ttu-id="060ac-131">Тип</span><span class="sxs-lookup"><span data-stu-id="060ac-131">Type</span></span>|<span data-ttu-id="060ac-132">Описание</span><span class="sxs-lookup"><span data-stu-id="060ac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="060ac-133">id</span><span class="sxs-lookup"><span data-stu-id="060ac-133">id</span></span>|<span data-ttu-id="060ac-134">String</span><span class="sxs-lookup"><span data-stu-id="060ac-134">String</span></span>|<span data-ttu-id="060ac-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="060ac-135">Key of the entity.</span></span> <span data-ttu-id="060ac-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060ac-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060ac-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="060ac-137">lastModifiedDateTime</span></span>|<span data-ttu-id="060ac-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="060ac-138">DateTimeOffset</span></span>|<span data-ttu-id="060ac-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="060ac-139">DateTime the object was last modified.</span></span> <span data-ttu-id="060ac-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060ac-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060ac-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="060ac-141">roleScopeTagIds</span></span>|<span data-ttu-id="060ac-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="060ac-142">String collection</span></span>|<span data-ttu-id="060ac-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="060ac-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="060ac-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060ac-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060ac-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="060ac-145">supportsScopeTags</span></span>|<span data-ttu-id="060ac-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-146">Boolean</span></span>|<span data-ttu-id="060ac-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="060ac-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="060ac-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="060ac-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="060ac-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="060ac-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="060ac-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="060ac-150">This property is read-only.</span></span> <span data-ttu-id="060ac-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060ac-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060ac-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="060ac-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="060ac-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="060ac-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="060ac-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="060ac-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="060ac-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060ac-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060ac-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="060ac-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="060ac-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="060ac-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="060ac-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="060ac-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="060ac-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060ac-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060ac-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="060ac-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="060ac-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="060ac-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="060ac-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="060ac-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="060ac-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060ac-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060ac-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="060ac-164">createdDateTime</span></span>|<span data-ttu-id="060ac-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="060ac-165">DateTimeOffset</span></span>|<span data-ttu-id="060ac-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="060ac-166">DateTime the object was created.</span></span> <span data-ttu-id="060ac-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060ac-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060ac-168">description</span><span class="sxs-lookup"><span data-stu-id="060ac-168">description</span></span>|<span data-ttu-id="060ac-169">String</span><span class="sxs-lookup"><span data-stu-id="060ac-169">String</span></span>|<span data-ttu-id="060ac-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="060ac-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="060ac-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060ac-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060ac-172">displayName</span><span class="sxs-lookup"><span data-stu-id="060ac-172">displayName</span></span>|<span data-ttu-id="060ac-173">Строка</span><span class="sxs-lookup"><span data-stu-id="060ac-173">String</span></span>|<span data-ttu-id="060ac-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="060ac-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="060ac-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060ac-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060ac-176">version</span><span class="sxs-lookup"><span data-stu-id="060ac-176">version</span></span>|<span data-ttu-id="060ac-177">Int32</span><span class="sxs-lookup"><span data-stu-id="060ac-177">Int32</span></span>|<span data-ttu-id="060ac-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="060ac-178">Version of the device configuration.</span></span> <span data-ttu-id="060ac-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="060ac-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="060ac-180">аккаунтсблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="060ac-180">accountsBlockModification</span></span>|<span data-ttu-id="060ac-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-181">Boolean</span></span>|<span data-ttu-id="060ac-182">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="060ac-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="060ac-183">аппсалловинсталлфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="060ac-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="060ac-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-184">Boolean</span></span>|<span data-ttu-id="060ac-185">Указывает, может ли пользователь включить параметр "неизвестные источники".</span><span class="sxs-lookup"><span data-stu-id="060ac-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="060ac-186">аппсаутаупдатеполици</span><span class="sxs-lookup"><span data-stu-id="060ac-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="060ac-187">андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="060ac-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="060ac-188">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="060ac-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="060ac-189">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="060ac-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="060ac-190">аппсдефаултпермиссионполици</span><span class="sxs-lookup"><span data-stu-id="060ac-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="060ac-191">андроиддевицеовнердефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="060ac-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="060ac-192">Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом.</span><span class="sxs-lookup"><span data-stu-id="060ac-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="060ac-193">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="060ac-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="060ac-194">аппсрекоммендскиппингфирстусехинтс</span><span class="sxs-lookup"><span data-stu-id="060ac-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="060ac-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-195">Boolean</span></span>|<span data-ttu-id="060ac-196">Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.</span><span class="sxs-lookup"><span data-stu-id="060ac-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="060ac-197">блуетусблоккконфигуратион</span><span class="sxs-lookup"><span data-stu-id="060ac-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="060ac-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-198">Boolean</span></span>|<span data-ttu-id="060ac-199">Указывает, следует ли запретить пользователю настраивать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="060ac-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="060ac-200">блуетусблоккконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="060ac-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="060ac-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-201">Boolean</span></span>|<span data-ttu-id="060ac-202">Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="060ac-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="060ac-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="060ac-203">cameraBlocked</span></span>|<span data-ttu-id="060ac-204">Логический</span><span class="sxs-lookup"><span data-stu-id="060ac-204">Boolean</span></span>|<span data-ttu-id="060ac-205">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="060ac-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="060ac-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="060ac-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="060ac-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-207">Boolean</span></span>|<span data-ttu-id="060ac-208">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="060ac-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="060ac-209">цертификатекредентиалконфигуратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="060ac-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="060ac-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-210">Boolean</span></span>|<span data-ttu-id="060ac-211">Указывает, следует ли запретить пользователям настраивать учетные данные сертификатов.</span><span class="sxs-lookup"><span data-stu-id="060ac-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="060ac-212">микрософтлаунчерконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="060ac-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="060ac-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-213">Boolean</span></span>|<span data-ttu-id="060ac-214">Указывает, следует ли настроить средство запуска Microsoft.</span><span class="sxs-lookup"><span data-stu-id="060ac-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="060ac-215">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="060ac-215">enrollmentProfile</span></span>|[<span data-ttu-id="060ac-216">андроиддевицеовнеренроллментпрофилетипе</span><span class="sxs-lookup"><span data-stu-id="060ac-216">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="060ac-217">Указывает, какой профиль регистрации вы хотите настроить.</span><span class="sxs-lookup"><span data-stu-id="060ac-217">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="060ac-218">Возможные значения: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span><span class="sxs-lookup"><span data-stu-id="060ac-218">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="060ac-219">датароамингблоккед</span><span class="sxs-lookup"><span data-stu-id="060ac-219">dataRoamingBlocked</span></span>|<span data-ttu-id="060ac-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-220">Boolean</span></span>|<span data-ttu-id="060ac-221">Указывает, следует ли запретить пользователю перемещать данные.</span><span class="sxs-lookup"><span data-stu-id="060ac-221">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="060ac-222">датетимеконфигуратионблоккед</span><span class="sxs-lookup"><span data-stu-id="060ac-222">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="060ac-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-223">Boolean</span></span>|<span data-ttu-id="060ac-224">Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.</span><span class="sxs-lookup"><span data-stu-id="060ac-224">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="060ac-225">факториресетдевицеадминистраторемаилс</span><span class="sxs-lookup"><span data-stu-id="060ac-225">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="060ac-226">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="060ac-226">String collection</span></span>|<span data-ttu-id="060ac-227">Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.</span><span class="sxs-lookup"><span data-stu-id="060ac-227">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="060ac-228">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="060ac-228">factoryResetBlocked</span></span>|<span data-ttu-id="060ac-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-229">Boolean</span></span>|<span data-ttu-id="060ac-230">Указывает, отключен ли параметр Reset фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="060ac-230">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="060ac-231">глобалпрокси</span><span class="sxs-lookup"><span data-stu-id="060ac-231">globalProxy</span></span>|[<span data-ttu-id="060ac-232">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="060ac-232">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="060ac-233">Прокси-сервер настраивается напрямую с узлом, портом и исключенными узлами.</span><span class="sxs-lookup"><span data-stu-id="060ac-233">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="060ac-234">гуглеаккаунтсблоккед</span><span class="sxs-lookup"><span data-stu-id="060ac-234">googleAccountsBlocked</span></span>|<span data-ttu-id="060ac-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-235">Boolean</span></span>|<span data-ttu-id="060ac-236">Указывает, будут ли блокироваться учетные записи Google.</span><span class="sxs-lookup"><span data-stu-id="060ac-236">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="060ac-237">киоскмодескринсаверконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="060ac-237">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="060ac-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-238">Boolean</span></span>|<span data-ttu-id="060ac-239">Указывает, следует ли включить режим экранной заставки или не в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="060ac-239">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="060ac-240">киоскмодескринсаверимажеурл</span><span class="sxs-lookup"><span data-stu-id="060ac-240">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="060ac-241">Строка</span><span class="sxs-lookup"><span data-stu-id="060ac-241">String</span></span>|<span data-ttu-id="060ac-242">URL-адрес изображения, которое будет экранной заставкой устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="060ac-242">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="060ac-243">киоскмодескринсавердисплайтимеинсекондс</span><span class="sxs-lookup"><span data-stu-id="060ac-243">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="060ac-244">Int32</span><span class="sxs-lookup"><span data-stu-id="060ac-244">Int32</span></span>|<span data-ttu-id="060ac-245">Время (в секундах), в течение которого устройство будет отображать экранную заставку в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="060ac-245">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="060ac-246">Допустимые значения — от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="060ac-246">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="060ac-247">киоскмодескринсаверстартделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="060ac-247">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="060ac-248">Int32</span><span class="sxs-lookup"><span data-stu-id="060ac-248">Int32</span></span>|<span data-ttu-id="060ac-249">Время (в секундах), в течение которого устройство должно быть неактивным, чтобы экранная заставка отображалась в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="060ac-249">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="060ac-250">Допустимые значения — от 1 до 9999999</span><span class="sxs-lookup"><span data-stu-id="060ac-250">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="060ac-251">киоскмодескринсавердетектмедиадисаблед</span><span class="sxs-lookup"><span data-stu-id="060ac-251">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="060ac-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-252">Boolean</span></span>|<span data-ttu-id="060ac-253">Указывает, должно ли устройство отображать экранную заставку при воспроизведении аудио-и видеоконференций в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="060ac-253">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="060ac-254">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="060ac-254">kioskModeApps</span></span>|<span data-ttu-id="060ac-255">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="060ac-255">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="060ac-256">Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="060ac-256">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="060ac-257">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="060ac-257">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="060ac-258">киоскмодеваллпаперурл</span><span class="sxs-lookup"><span data-stu-id="060ac-258">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="060ac-259">Строка</span><span class="sxs-lookup"><span data-stu-id="060ac-259">String</span></span>|<span data-ttu-id="060ac-260">URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="060ac-260">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="060ac-261">киоскмодикситкоде</span><span class="sxs-lookup"><span data-stu-id="060ac-261">kioskModeExitCode</span></span>|<span data-ttu-id="060ac-262">Строка</span><span class="sxs-lookup"><span data-stu-id="060ac-262">String</span></span>|<span data-ttu-id="060ac-263">Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="060ac-263">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="060ac-264">киоскмодевиртуалхомебуттоненаблед</span><span class="sxs-lookup"><span data-stu-id="060ac-264">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="060ac-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-265">Boolean</span></span>|<span data-ttu-id="060ac-266">Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="060ac-266">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="060ac-267">киоскмодевиртуалхомебуттонтипе</span><span class="sxs-lookup"><span data-stu-id="060ac-267">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="060ac-268">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="060ac-268">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="060ac-269">Указывает, является ли кнопка "Виртуальная Домашняя страница" кнопкой "Прокрутка вверх" или плавающей кнопкой "домой".</span><span class="sxs-lookup"><span data-stu-id="060ac-269">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="060ac-270">Возможные значения: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="060ac-270">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="060ac-271">киоскмодеблуетусконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="060ac-271">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="060ac-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-272">Boolean</span></span>|<span data-ttu-id="060ac-273">Указывает, следует ли запретить пользователю настраивать параметры Bluetooth в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="060ac-273">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="060ac-274">киоскмодевификонфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="060ac-274">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="060ac-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-275">Boolean</span></span>|<span data-ttu-id="060ac-276">Указывает, следует ли разрешить пользователю настраивать параметры Wi/Fi в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="060ac-276">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="060ac-277">киоскмодефлашлигхтконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="060ac-277">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="060ac-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-278">Boolean</span></span>|<span data-ttu-id="060ac-279">Указывает, следует ли разрешить пользователю использовать флашлигхт в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="060ac-279">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="060ac-280">киоскмодемедиаволумеконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="060ac-280">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="060ac-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-281">Boolean</span></span>|<span data-ttu-id="060ac-282">Указывает, следует ли запретить пользователю изменять громкость мультимедиа в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="060ac-282">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="060ac-283">микрофонефорцемуте</span><span class="sxs-lookup"><span data-stu-id="060ac-283">microphoneForceMute</span></span>|<span data-ttu-id="060ac-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-284">Boolean</span></span>|<span data-ttu-id="060ac-285">Указывает, следует ли запретить разблокирование микрофона устройства.</span><span class="sxs-lookup"><span data-stu-id="060ac-285">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="060ac-286">нетворкескапехатчалловед</span><span class="sxs-lookup"><span data-stu-id="060ac-286">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="060ac-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-287">Boolean</span></span>|<span data-ttu-id="060ac-288">Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="060ac-288">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="060ac-289">нфкблоккаутгоингбеам</span><span class="sxs-lookup"><span data-stu-id="060ac-289">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="060ac-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-290">Boolean</span></span>|<span data-ttu-id="060ac-291">Указывает, следует ли заблокировать исходящую форму NFC.</span><span class="sxs-lookup"><span data-stu-id="060ac-291">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="060ac-292">пассвордблокккэйгуард</span><span class="sxs-lookup"><span data-stu-id="060ac-292">passwordBlockKeyguard</span></span>|<span data-ttu-id="060ac-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-293">Boolean</span></span>|<span data-ttu-id="060ac-294">Указывает, отключен ли кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="060ac-294">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="060ac-295">пассвордблокккэйгуардфеатурес</span><span class="sxs-lookup"><span data-stu-id="060ac-295">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="060ac-296">Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="060ac-296">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="060ac-297">Список компонентов кэйгуард устройств, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="060ac-297">List of device keyguard features to block.</span></span> <span data-ttu-id="060ac-298">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="060ac-298">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="060ac-299">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="060ac-299">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="060ac-300">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="060ac-300">passwordExpirationDays</span></span>|<span data-ttu-id="060ac-301">Int32</span><span class="sxs-lookup"><span data-stu-id="060ac-301">Int32</span></span>|<span data-ttu-id="060ac-302">Указывает время в секундах, в течение которого можно задать пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="060ac-302">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="060ac-303">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="060ac-303">Valid values 1 to 365</span></span>|
|<span data-ttu-id="060ac-304">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="060ac-304">passwordMinimumLength</span></span>|<span data-ttu-id="060ac-305">Int32</span><span class="sxs-lookup"><span data-stu-id="060ac-305">Int32</span></span>|<span data-ttu-id="060ac-306">Указывает минимальную длину пароля, необходимого для устройства.</span><span class="sxs-lookup"><span data-stu-id="060ac-306">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="060ac-307">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="060ac-307">Valid values 4 to 16</span></span>|
|<span data-ttu-id="060ac-308">пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="060ac-308">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="060ac-309">Int32</span><span class="sxs-lookup"><span data-stu-id="060ac-309">Int32</span></span>|<span data-ttu-id="060ac-310">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="060ac-310">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="060ac-311">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="060ac-311">Valid values 1 to 16</span></span>|
|<span data-ttu-id="060ac-312">пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="060ac-312">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="060ac-313">Int32</span><span class="sxs-lookup"><span data-stu-id="060ac-313">Int32</span></span>|<span data-ttu-id="060ac-314">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="060ac-314">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="060ac-315">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="060ac-315">Valid values 1 to 16</span></span>|
|<span data-ttu-id="060ac-316">пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="060ac-316">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="060ac-317">Int32</span><span class="sxs-lookup"><span data-stu-id="060ac-317">Int32</span></span>|<span data-ttu-id="060ac-318">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="060ac-318">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="060ac-319">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="060ac-319">Valid values 1 to 16</span></span>|
|<span data-ttu-id="060ac-320">пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="060ac-320">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="060ac-321">Int32</span><span class="sxs-lookup"><span data-stu-id="060ac-321">Int32</span></span>|<span data-ttu-id="060ac-322">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="060ac-322">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="060ac-323">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="060ac-323">Valid values 1 to 16</span></span>|
|<span data-ttu-id="060ac-324">пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="060ac-324">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="060ac-325">Int32</span><span class="sxs-lookup"><span data-stu-id="060ac-325">Int32</span></span>|<span data-ttu-id="060ac-326">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="060ac-326">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="060ac-327">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="060ac-327">Valid values 1 to 16</span></span>|
|<span data-ttu-id="060ac-328">пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="060ac-328">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="060ac-329">Int32</span><span class="sxs-lookup"><span data-stu-id="060ac-329">Int32</span></span>|<span data-ttu-id="060ac-330">Указывает минимальное число символов верхнего каселеттер, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="060ac-330">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="060ac-331">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="060ac-331">Valid values 1 to 16</span></span>|
|<span data-ttu-id="060ac-332">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="060ac-332">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="060ac-333">Int32</span><span class="sxs-lookup"><span data-stu-id="060ac-333">Int32</span></span>|<span data-ttu-id="060ac-334">Миллисекунды бездействия до истечения времени ожидания экрана.</span><span class="sxs-lookup"><span data-stu-id="060ac-334">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="060ac-335">пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="060ac-335">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="060ac-336">Int32</span><span class="sxs-lookup"><span data-stu-id="060ac-336">Int32</span></span>|<span data-ttu-id="060ac-337">Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале.</span><span class="sxs-lookup"><span data-stu-id="060ac-337">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="060ac-338">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="060ac-338">Valid values 0 to 24</span></span>|
|<span data-ttu-id="060ac-339">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="060ac-339">passwordRequiredType</span></span>|[<span data-ttu-id="060ac-340">андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="060ac-340">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="060ac-341">Указывает минимальное качество пароля, необходимое для устройства.</span><span class="sxs-lookup"><span data-stu-id="060ac-341">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="060ac-342">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="060ac-342">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="060ac-343">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="060ac-343">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="060ac-344">Int32</span><span class="sxs-lookup"><span data-stu-id="060ac-344">Int32</span></span>|<span data-ttu-id="060ac-345">Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="060ac-345">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="060ac-346">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="060ac-346">Valid values 4 to 11</span></span>|
|<span data-ttu-id="060ac-347">плайсторемоде</span><span class="sxs-lookup"><span data-stu-id="060ac-347">playStoreMode</span></span>|[<span data-ttu-id="060ac-348">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="060ac-348">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="060ac-349">Указывает режим проигрывания устройства в хранилище.</span><span class="sxs-lookup"><span data-stu-id="060ac-349">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="060ac-350">Возможные значения: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="060ac-350">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="060ac-351">сафебутблоккед</span><span class="sxs-lookup"><span data-stu-id="060ac-351">safeBootBlocked</span></span>|<span data-ttu-id="060ac-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-352">Boolean</span></span>|<span data-ttu-id="060ac-353">Указывает, отключена ли загрузка устройства в "безопасная загрузка".</span><span class="sxs-lookup"><span data-stu-id="060ac-353">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="060ac-354">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="060ac-354">screenCaptureBlocked</span></span>|<span data-ttu-id="060ac-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-355">Boolean</span></span>|<span data-ttu-id="060ac-356">Указывает, следует ли отключить возможность использования снимков экрана.</span><span class="sxs-lookup"><span data-stu-id="060ac-356">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="060ac-357">секуритялловдебуггингфеатурес</span><span class="sxs-lookup"><span data-stu-id="060ac-357">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="060ac-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-358">Boolean</span></span>|<span data-ttu-id="060ac-359">Указывает, следует ли запретить пользователю включать функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="060ac-359">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="060ac-360">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="060ac-360">securityRequireVerifyApps</span></span>|<span data-ttu-id="060ac-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-361">Boolean</span></span>|<span data-ttu-id="060ac-362">Указывает, требуется ли проверка приложений.</span><span class="sxs-lookup"><span data-stu-id="060ac-362">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="060ac-363">статусбарблоккед</span><span class="sxs-lookup"><span data-stu-id="060ac-363">statusBarBlocked</span></span>|<span data-ttu-id="060ac-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-364">Boolean</span></span>|<span data-ttu-id="060ac-365">Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.</span><span class="sxs-lookup"><span data-stu-id="060ac-365">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="060ac-366">стайонмодес</span><span class="sxs-lookup"><span data-stu-id="060ac-366">stayOnModes</span></span>|<span data-ttu-id="060ac-367">Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="060ac-367">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="060ac-368">Список режимов, в которых дисплей устройства остается включенным.</span><span class="sxs-lookup"><span data-stu-id="060ac-368">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="060ac-369">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="060ac-369">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="060ac-370">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="060ac-370">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="060ac-371">сторажеалловусб</span><span class="sxs-lookup"><span data-stu-id="060ac-371">storageAllowUsb</span></span>|<span data-ttu-id="060ac-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-372">Boolean</span></span>|<span data-ttu-id="060ac-373">Указывает, следует ли разрешить запоминающее устройство USB.</span><span class="sxs-lookup"><span data-stu-id="060ac-373">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="060ac-374">сторажеблоккекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="060ac-374">storageBlockExternalMedia</span></span>|<span data-ttu-id="060ac-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-375">Boolean</span></span>|<span data-ttu-id="060ac-376">Указывает, следует ли заблокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="060ac-376">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="060ac-377">сторажеблоккусбфилетрансфер</span><span class="sxs-lookup"><span data-stu-id="060ac-377">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="060ac-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-378">Boolean</span></span>|<span data-ttu-id="060ac-379">Указывает, следует ли запретить передачу файлов через USB.</span><span class="sxs-lookup"><span data-stu-id="060ac-379">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="060ac-380">системупдатевиндовстартминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="060ac-380">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="060ac-381">Int32</span><span class="sxs-lookup"><span data-stu-id="060ac-381">Int32</span></span>|<span data-ttu-id="060ac-382">Указывает количество минут после полуночи, когда запустится окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="060ac-382">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="060ac-383">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="060ac-383">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="060ac-384">системупдатевиндовендминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="060ac-384">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="060ac-385">Int32</span><span class="sxs-lookup"><span data-stu-id="060ac-385">Int32</span></span>|<span data-ttu-id="060ac-386">Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="060ac-386">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="060ac-387">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="060ac-387">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="060ac-388">системупдатеинсталлтипе</span><span class="sxs-lookup"><span data-stu-id="060ac-388">systemUpdateInstallType</span></span>|[<span data-ttu-id="060ac-389">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="060ac-389">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="060ac-390">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="060ac-390">The type of system update configuration.</span></span> <span data-ttu-id="060ac-391">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="060ac-391">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="060ac-392">системвиндовсблоккед</span><span class="sxs-lookup"><span data-stu-id="060ac-392">systemWindowsBlocked</span></span>|<span data-ttu-id="060ac-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-393">Boolean</span></span>|<span data-ttu-id="060ac-394">Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="060ac-394">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="060ac-395">усерсблоккадд</span><span class="sxs-lookup"><span data-stu-id="060ac-395">usersBlockAdd</span></span>|<span data-ttu-id="060ac-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-396">Boolean</span></span>|<span data-ttu-id="060ac-397">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="060ac-397">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="060ac-398">усерсблоккремове</span><span class="sxs-lookup"><span data-stu-id="060ac-398">usersBlockRemove</span></span>|<span data-ttu-id="060ac-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-399">Boolean</span></span>|<span data-ttu-id="060ac-400">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="060ac-400">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="060ac-401">волумеблоккаджустмент</span><span class="sxs-lookup"><span data-stu-id="060ac-401">volumeBlockAdjustment</span></span>|<span data-ttu-id="060ac-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-402">Boolean</span></span>|<span data-ttu-id="060ac-403">Указывает, отключена ли настройка главного тома.</span><span class="sxs-lookup"><span data-stu-id="060ac-403">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="060ac-404">впналвайсонлоккдовнмоде</span><span class="sxs-lookup"><span data-stu-id="060ac-404">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="060ac-405">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-405">Boolean</span></span>|<span data-ttu-id="060ac-406">Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="060ac-406">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="060ac-407">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="060ac-407">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="060ac-408">Строка</span><span class="sxs-lookup"><span data-stu-id="060ac-408">String</span></span>|<span data-ttu-id="060ac-409">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="060ac-409">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="060ac-410">вифиблоккедитконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="060ac-410">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="060ac-411">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-411">Boolean</span></span>|<span data-ttu-id="060ac-412">Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="060ac-412">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="060ac-413">вифиблоккедитполицидефинедконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="060ac-413">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="060ac-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="060ac-414">Boolean</span></span>|<span data-ttu-id="060ac-415">Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="060ac-415">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="060ac-416">Ответ</span><span class="sxs-lookup"><span data-stu-id="060ac-416">Response</span></span>
<span data-ttu-id="060ac-417">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="060ac-417">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="060ac-418">Пример</span><span class="sxs-lookup"><span data-stu-id="060ac-418">Example</span></span>

### <a name="request"></a><span data-ttu-id="060ac-419">Запрос</span><span class="sxs-lookup"><span data-stu-id="060ac-419">Request</span></span>
<span data-ttu-id="060ac-420">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="060ac-420">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4467

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

### <a name="response"></a><span data-ttu-id="060ac-421">Отклик</span><span class="sxs-lookup"><span data-stu-id="060ac-421">Response</span></span>
<span data-ttu-id="060ac-p137">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="060ac-p137">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4639

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



