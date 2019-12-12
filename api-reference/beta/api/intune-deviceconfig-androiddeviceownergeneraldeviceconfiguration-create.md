---
title: Создание androidDeviceOwnerGeneralDeviceConfiguration
description: Создание нового объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fb1d5e49d61abc4481e9b6dfec17d28ec18ba115
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39953868"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="4ab73-103">Создание androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ab73-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="4ab73-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ab73-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ab73-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ab73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ab73-106">Создание нового объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4ab73-106">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ab73-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4ab73-107">Prerequisites</span></span>
<span data-ttu-id="4ab73-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ab73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ab73-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ab73-110">Permission type</span></span>|<span data-ttu-id="4ab73-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ab73-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ab73-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ab73-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ab73-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ab73-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ab73-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ab73-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ab73-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ab73-115">Not supported.</span></span>|
|<span data-ttu-id="4ab73-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ab73-116">Application</span></span>|<span data-ttu-id="4ab73-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ab73-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ab73-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ab73-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4ab73-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4ab73-119">Request headers</span></span>
|<span data-ttu-id="4ab73-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ab73-120">Header</span></span>|<span data-ttu-id="4ab73-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4ab73-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ab73-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ab73-122">Authorization</span></span>|<span data-ttu-id="4ab73-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ab73-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ab73-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4ab73-124">Accept</span></span>|<span data-ttu-id="4ab73-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ab73-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ab73-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4ab73-126">Request body</span></span>
<span data-ttu-id="4ab73-127">В тексте запроса добавьте представление объекта androidDeviceOwnerGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ab73-127">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="4ab73-128">В следующей таблице приведены свойства, необходимые при создании androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4ab73-128">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="4ab73-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ab73-129">Property</span></span>|<span data-ttu-id="4ab73-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4ab73-130">Type</span></span>|<span data-ttu-id="4ab73-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4ab73-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ab73-132">id</span><span class="sxs-lookup"><span data-stu-id="4ab73-132">id</span></span>|<span data-ttu-id="4ab73-133">String</span><span class="sxs-lookup"><span data-stu-id="4ab73-133">String</span></span>|<span data-ttu-id="4ab73-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4ab73-134">Key of the entity.</span></span> <span data-ttu-id="4ab73-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ab73-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ab73-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ab73-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4ab73-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ab73-137">DateTimeOffset</span></span>|<span data-ttu-id="4ab73-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4ab73-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4ab73-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ab73-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ab73-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4ab73-140">roleScopeTagIds</span></span>|<span data-ttu-id="4ab73-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4ab73-141">String collection</span></span>|<span data-ttu-id="4ab73-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4ab73-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4ab73-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ab73-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ab73-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4ab73-144">supportsScopeTags</span></span>|<span data-ttu-id="4ab73-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-145">Boolean</span></span>|<span data-ttu-id="4ab73-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4ab73-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4ab73-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4ab73-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4ab73-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4ab73-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4ab73-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ab73-149">This property is read-only.</span></span> <span data-ttu-id="4ab73-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ab73-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ab73-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4ab73-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4ab73-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4ab73-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4ab73-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4ab73-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4ab73-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ab73-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ab73-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4ab73-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4ab73-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4ab73-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4ab73-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4ab73-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4ab73-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ab73-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ab73-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4ab73-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4ab73-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4ab73-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4ab73-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4ab73-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4ab73-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ab73-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ab73-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ab73-163">createdDateTime</span></span>|<span data-ttu-id="4ab73-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ab73-164">DateTimeOffset</span></span>|<span data-ttu-id="4ab73-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4ab73-165">DateTime the object was created.</span></span> <span data-ttu-id="4ab73-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ab73-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ab73-167">description</span><span class="sxs-lookup"><span data-stu-id="4ab73-167">description</span></span>|<span data-ttu-id="4ab73-168">String</span><span class="sxs-lookup"><span data-stu-id="4ab73-168">String</span></span>|<span data-ttu-id="4ab73-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4ab73-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4ab73-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ab73-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ab73-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4ab73-171">displayName</span></span>|<span data-ttu-id="4ab73-172">Строка</span><span class="sxs-lookup"><span data-stu-id="4ab73-172">String</span></span>|<span data-ttu-id="4ab73-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4ab73-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4ab73-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ab73-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ab73-175">version</span><span class="sxs-lookup"><span data-stu-id="4ab73-175">version</span></span>|<span data-ttu-id="4ab73-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab73-176">Int32</span></span>|<span data-ttu-id="4ab73-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4ab73-177">Version of the device configuration.</span></span> <span data-ttu-id="4ab73-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ab73-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ab73-179">аккаунтсблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="4ab73-179">accountsBlockModification</span></span>|<span data-ttu-id="4ab73-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-180">Boolean</span></span>|<span data-ttu-id="4ab73-181">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="4ab73-181">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="4ab73-182">аппсалловинсталлфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="4ab73-182">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="4ab73-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-183">Boolean</span></span>|<span data-ttu-id="4ab73-184">Указывает, может ли пользователь включить параметр "неизвестные источники".</span><span class="sxs-lookup"><span data-stu-id="4ab73-184">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="4ab73-185">аппсаутаупдатеполици</span><span class="sxs-lookup"><span data-stu-id="4ab73-185">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="4ab73-186">андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="4ab73-186">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="4ab73-187">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="4ab73-187">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="4ab73-188">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="4ab73-188">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="4ab73-189">аппсдефаултпермиссионполици</span><span class="sxs-lookup"><span data-stu-id="4ab73-189">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="4ab73-190">андроиддевицеовнердефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="4ab73-190">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="4ab73-191">Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом.</span><span class="sxs-lookup"><span data-stu-id="4ab73-191">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="4ab73-192">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="4ab73-192">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="4ab73-193">аппсрекоммендскиппингфирстусехинтс</span><span class="sxs-lookup"><span data-stu-id="4ab73-193">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="4ab73-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-194">Boolean</span></span>|<span data-ttu-id="4ab73-195">Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.</span><span class="sxs-lookup"><span data-stu-id="4ab73-195">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="4ab73-196">блуетусблоккконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4ab73-196">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="4ab73-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-197">Boolean</span></span>|<span data-ttu-id="4ab73-198">Указывает, следует ли запретить пользователю настраивать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="4ab73-198">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="4ab73-199">блуетусблоккконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="4ab73-199">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="4ab73-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-200">Boolean</span></span>|<span data-ttu-id="4ab73-201">Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="4ab73-201">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="4ab73-202">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="4ab73-202">cameraBlocked</span></span>|<span data-ttu-id="4ab73-203">Логический</span><span class="sxs-lookup"><span data-stu-id="4ab73-203">Boolean</span></span>|<span data-ttu-id="4ab73-204">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="4ab73-204">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="4ab73-205">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="4ab73-205">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="4ab73-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-206">Boolean</span></span>|<span data-ttu-id="4ab73-207">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="4ab73-207">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="4ab73-208">цертификатекредентиалконфигуратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="4ab73-208">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="4ab73-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-209">Boolean</span></span>|<span data-ttu-id="4ab73-210">Указывает, следует ли запретить пользователям настраивать учетные данные сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4ab73-210">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="4ab73-211">датароамингблоккед</span><span class="sxs-lookup"><span data-stu-id="4ab73-211">dataRoamingBlocked</span></span>|<span data-ttu-id="4ab73-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-212">Boolean</span></span>|<span data-ttu-id="4ab73-213">Указывает, следует ли запретить пользователю перемещать данные.</span><span class="sxs-lookup"><span data-stu-id="4ab73-213">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="4ab73-214">датетимеконфигуратионблоккед</span><span class="sxs-lookup"><span data-stu-id="4ab73-214">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="4ab73-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-215">Boolean</span></span>|<span data-ttu-id="4ab73-216">Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4ab73-216">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="4ab73-217">факториресетдевицеадминистраторемаилс</span><span class="sxs-lookup"><span data-stu-id="4ab73-217">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="4ab73-218">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4ab73-218">String collection</span></span>|<span data-ttu-id="4ab73-219">Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.</span><span class="sxs-lookup"><span data-stu-id="4ab73-219">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="4ab73-220">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="4ab73-220">factoryResetBlocked</span></span>|<span data-ttu-id="4ab73-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-221">Boolean</span></span>|<span data-ttu-id="4ab73-222">Указывает, отключен ли параметр Reset фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="4ab73-222">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="4ab73-223">глобалпрокси</span><span class="sxs-lookup"><span data-stu-id="4ab73-223">globalProxy</span></span>|[<span data-ttu-id="4ab73-224">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="4ab73-224">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="4ab73-225">Прокси-сервер настраивается напрямую с узлом, портом и исключенными узлами.</span><span class="sxs-lookup"><span data-stu-id="4ab73-225">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="4ab73-226">гуглеаккаунтсблоккед</span><span class="sxs-lookup"><span data-stu-id="4ab73-226">googleAccountsBlocked</span></span>|<span data-ttu-id="4ab73-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-227">Boolean</span></span>|<span data-ttu-id="4ab73-228">Указывает, будут ли блокироваться учетные записи Google.</span><span class="sxs-lookup"><span data-stu-id="4ab73-228">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="4ab73-229">киоскмодескринсаверконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="4ab73-229">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="4ab73-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-230">Boolean</span></span>|<span data-ttu-id="4ab73-231">Указывает, следует ли включить режим экранной заставки или не в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4ab73-231">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="4ab73-232">киоскмодескринсаверимажеурл</span><span class="sxs-lookup"><span data-stu-id="4ab73-232">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="4ab73-233">Строка</span><span class="sxs-lookup"><span data-stu-id="4ab73-233">String</span></span>|<span data-ttu-id="4ab73-234">URL-адрес изображения, которое будет экранной заставкой устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4ab73-234">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="4ab73-235">киоскмодескринсавердисплайтимеинсекондс</span><span class="sxs-lookup"><span data-stu-id="4ab73-235">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="4ab73-236">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab73-236">Int32</span></span>|<span data-ttu-id="4ab73-237">Время (в секундах), в течение которого устройство будет отображать экранную заставку в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4ab73-237">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="4ab73-238">Допустимые значения — от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="4ab73-238">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="4ab73-239">киоскмодескринсаверстартделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="4ab73-239">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="4ab73-240">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab73-240">Int32</span></span>|<span data-ttu-id="4ab73-241">Время (в секундах), в течение которого устройство должно быть неактивным, чтобы экранная заставка отображалась в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4ab73-241">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="4ab73-242">Допустимые значения — от 1 до 9999999</span><span class="sxs-lookup"><span data-stu-id="4ab73-242">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="4ab73-243">киоскмодескринсавердетектмедиадисаблед</span><span class="sxs-lookup"><span data-stu-id="4ab73-243">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="4ab73-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-244">Boolean</span></span>|<span data-ttu-id="4ab73-245">Указывает, должно ли устройство отображать экранную заставку при воспроизведении аудио-и видеоконференций в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="4ab73-245">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="4ab73-246">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="4ab73-246">kioskModeApps</span></span>|<span data-ttu-id="4ab73-247">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="4ab73-247">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4ab73-248">Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4ab73-248">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="4ab73-249">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4ab73-249">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4ab73-250">киоскмодеваллпаперурл</span><span class="sxs-lookup"><span data-stu-id="4ab73-250">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="4ab73-251">Строка</span><span class="sxs-lookup"><span data-stu-id="4ab73-251">String</span></span>|<span data-ttu-id="4ab73-252">URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4ab73-252">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="4ab73-253">киоскмодикситкоде</span><span class="sxs-lookup"><span data-stu-id="4ab73-253">kioskModeExitCode</span></span>|<span data-ttu-id="4ab73-254">Строка</span><span class="sxs-lookup"><span data-stu-id="4ab73-254">String</span></span>|<span data-ttu-id="4ab73-255">Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4ab73-255">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="4ab73-256">киоскмодевиртуалхомебуттоненаблед</span><span class="sxs-lookup"><span data-stu-id="4ab73-256">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="4ab73-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-257">Boolean</span></span>|<span data-ttu-id="4ab73-258">Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4ab73-258">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="4ab73-259">киоскмодевиртуалхомебуттонтипе</span><span class="sxs-lookup"><span data-stu-id="4ab73-259">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="4ab73-260">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="4ab73-260">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="4ab73-261">Указывает, является ли кнопка "Виртуальная Домашняя страница" кнопкой "Прокрутка вверх" или плавающей кнопкой "домой".</span><span class="sxs-lookup"><span data-stu-id="4ab73-261">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="4ab73-262">Возможные значения: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="4ab73-262">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="4ab73-263">киоскмодеблуетусконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="4ab73-263">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="4ab73-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-264">Boolean</span></span>|<span data-ttu-id="4ab73-265">Указывает, следует ли запретить пользователю настраивать параметры Bluetooth в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4ab73-265">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="4ab73-266">киоскмодевификонфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="4ab73-266">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="4ab73-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-267">Boolean</span></span>|<span data-ttu-id="4ab73-268">Указывает, следует ли разрешить пользователю настраивать параметры Wi/Fi в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4ab73-268">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="4ab73-269">киоскмодефлашлигхтконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="4ab73-269">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="4ab73-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-270">Boolean</span></span>|<span data-ttu-id="4ab73-271">Указывает, следует ли разрешить пользователю использовать флашлигхт в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4ab73-271">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="4ab73-272">киоскмодемедиаволумеконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="4ab73-272">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="4ab73-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-273">Boolean</span></span>|<span data-ttu-id="4ab73-274">Указывает, следует ли запретить пользователю изменять громкость мультимедиа в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4ab73-274">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="4ab73-275">микрофонефорцемуте</span><span class="sxs-lookup"><span data-stu-id="4ab73-275">microphoneForceMute</span></span>|<span data-ttu-id="4ab73-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-276">Boolean</span></span>|<span data-ttu-id="4ab73-277">Указывает, следует ли запретить разблокирование микрофона устройства.</span><span class="sxs-lookup"><span data-stu-id="4ab73-277">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="4ab73-278">нетворкескапехатчалловед</span><span class="sxs-lookup"><span data-stu-id="4ab73-278">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="4ab73-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-279">Boolean</span></span>|<span data-ttu-id="4ab73-280">Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="4ab73-280">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="4ab73-281">нфкблоккаутгоингбеам</span><span class="sxs-lookup"><span data-stu-id="4ab73-281">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="4ab73-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-282">Boolean</span></span>|<span data-ttu-id="4ab73-283">Указывает, следует ли заблокировать исходящую форму NFC.</span><span class="sxs-lookup"><span data-stu-id="4ab73-283">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="4ab73-284">пассвордблокккэйгуард</span><span class="sxs-lookup"><span data-stu-id="4ab73-284">passwordBlockKeyguard</span></span>|<span data-ttu-id="4ab73-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-285">Boolean</span></span>|<span data-ttu-id="4ab73-286">Указывает, отключен ли кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="4ab73-286">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="4ab73-287">пассвордблокккэйгуардфеатурес</span><span class="sxs-lookup"><span data-stu-id="4ab73-287">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="4ab73-288">Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="4ab73-288">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="4ab73-289">Список компонентов кэйгуард устройств, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="4ab73-289">List of device keyguard features to block.</span></span> <span data-ttu-id="4ab73-290">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="4ab73-290">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="4ab73-291">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="4ab73-291">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="4ab73-292">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4ab73-292">passwordExpirationDays</span></span>|<span data-ttu-id="4ab73-293">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab73-293">Int32</span></span>|<span data-ttu-id="4ab73-294">Указывает время в секундах, в течение которого можно задать пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="4ab73-294">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="4ab73-295">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="4ab73-295">Valid values 1 to 365</span></span>|
|<span data-ttu-id="4ab73-296">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4ab73-296">passwordMinimumLength</span></span>|<span data-ttu-id="4ab73-297">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab73-297">Int32</span></span>|<span data-ttu-id="4ab73-298">Указывает минимальную длину пароля, необходимого для устройства.</span><span class="sxs-lookup"><span data-stu-id="4ab73-298">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="4ab73-299">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="4ab73-299">Valid values 4 to 16</span></span>|
|<span data-ttu-id="4ab73-300">пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="4ab73-300">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="4ab73-301">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab73-301">Int32</span></span>|<span data-ttu-id="4ab73-302">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="4ab73-302">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="4ab73-303">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="4ab73-303">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4ab73-304">пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="4ab73-304">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="4ab73-305">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab73-305">Int32</span></span>|<span data-ttu-id="4ab73-306">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="4ab73-306">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="4ab73-307">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="4ab73-307">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4ab73-308">пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="4ab73-308">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="4ab73-309">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab73-309">Int32</span></span>|<span data-ttu-id="4ab73-310">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="4ab73-310">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="4ab73-311">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="4ab73-311">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4ab73-312">пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="4ab73-312">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="4ab73-313">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab73-313">Int32</span></span>|<span data-ttu-id="4ab73-314">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="4ab73-314">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="4ab73-315">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="4ab73-315">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4ab73-316">пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="4ab73-316">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="4ab73-317">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab73-317">Int32</span></span>|<span data-ttu-id="4ab73-318">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="4ab73-318">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="4ab73-319">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="4ab73-319">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4ab73-320">пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="4ab73-320">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="4ab73-321">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab73-321">Int32</span></span>|<span data-ttu-id="4ab73-322">Указывает минимальное число символов верхнего каселеттер, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="4ab73-322">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="4ab73-323">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="4ab73-323">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4ab73-324">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4ab73-324">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4ab73-325">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab73-325">Int32</span></span>|<span data-ttu-id="4ab73-326">Миллисекунды бездействия до истечения времени ожидания экрана.</span><span class="sxs-lookup"><span data-stu-id="4ab73-326">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="4ab73-327">пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="4ab73-327">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="4ab73-328">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab73-328">Int32</span></span>|<span data-ttu-id="4ab73-329">Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале.</span><span class="sxs-lookup"><span data-stu-id="4ab73-329">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="4ab73-330">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="4ab73-330">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4ab73-331">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4ab73-331">passwordRequiredType</span></span>|[<span data-ttu-id="4ab73-332">андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="4ab73-332">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="4ab73-333">Указывает минимальное качество пароля, необходимое для устройства.</span><span class="sxs-lookup"><span data-stu-id="4ab73-333">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="4ab73-334">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="4ab73-334">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="4ab73-335">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4ab73-335">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4ab73-336">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab73-336">Int32</span></span>|<span data-ttu-id="4ab73-337">Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="4ab73-337">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="4ab73-338">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="4ab73-338">Valid values 4 to 11</span></span>|
|<span data-ttu-id="4ab73-339">плайсторемоде</span><span class="sxs-lookup"><span data-stu-id="4ab73-339">playStoreMode</span></span>|[<span data-ttu-id="4ab73-340">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="4ab73-340">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="4ab73-341">Указывает режим проигрывания устройства в хранилище.</span><span class="sxs-lookup"><span data-stu-id="4ab73-341">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="4ab73-342">Возможные значения: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="4ab73-342">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="4ab73-343">сафебутблоккед</span><span class="sxs-lookup"><span data-stu-id="4ab73-343">safeBootBlocked</span></span>|<span data-ttu-id="4ab73-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-344">Boolean</span></span>|<span data-ttu-id="4ab73-345">Указывает, отключена ли загрузка устройства в "безопасная загрузка".</span><span class="sxs-lookup"><span data-stu-id="4ab73-345">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="4ab73-346">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="4ab73-346">screenCaptureBlocked</span></span>|<span data-ttu-id="4ab73-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-347">Boolean</span></span>|<span data-ttu-id="4ab73-348">Указывает, следует ли отключить возможность использования снимков экрана.</span><span class="sxs-lookup"><span data-stu-id="4ab73-348">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="4ab73-349">секуритялловдебуггингфеатурес</span><span class="sxs-lookup"><span data-stu-id="4ab73-349">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="4ab73-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-350">Boolean</span></span>|<span data-ttu-id="4ab73-351">Указывает, следует ли запретить пользователю включать функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4ab73-351">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="4ab73-352">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="4ab73-352">securityRequireVerifyApps</span></span>|<span data-ttu-id="4ab73-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-353">Boolean</span></span>|<span data-ttu-id="4ab73-354">Указывает, требуется ли проверка приложений.</span><span class="sxs-lookup"><span data-stu-id="4ab73-354">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="4ab73-355">статусбарблоккед</span><span class="sxs-lookup"><span data-stu-id="4ab73-355">statusBarBlocked</span></span>|<span data-ttu-id="4ab73-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-356">Boolean</span></span>|<span data-ttu-id="4ab73-357">Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.</span><span class="sxs-lookup"><span data-stu-id="4ab73-357">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="4ab73-358">стайонмодес</span><span class="sxs-lookup"><span data-stu-id="4ab73-358">stayOnModes</span></span>|<span data-ttu-id="4ab73-359">Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="4ab73-359">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="4ab73-360">Список режимов, в которых дисплей устройства остается включенным.</span><span class="sxs-lookup"><span data-stu-id="4ab73-360">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="4ab73-361">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="4ab73-361">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="4ab73-362">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="4ab73-362">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="4ab73-363">сторажеалловусб</span><span class="sxs-lookup"><span data-stu-id="4ab73-363">storageAllowUsb</span></span>|<span data-ttu-id="4ab73-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-364">Boolean</span></span>|<span data-ttu-id="4ab73-365">Указывает, следует ли разрешить запоминающее устройство USB.</span><span class="sxs-lookup"><span data-stu-id="4ab73-365">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="4ab73-366">сторажеблоккекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="4ab73-366">storageBlockExternalMedia</span></span>|<span data-ttu-id="4ab73-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-367">Boolean</span></span>|<span data-ttu-id="4ab73-368">Указывает, следует ли заблокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="4ab73-368">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="4ab73-369">сторажеблоккусбфилетрансфер</span><span class="sxs-lookup"><span data-stu-id="4ab73-369">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="4ab73-370">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-370">Boolean</span></span>|<span data-ttu-id="4ab73-371">Указывает, следует ли запретить передачу файлов через USB.</span><span class="sxs-lookup"><span data-stu-id="4ab73-371">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="4ab73-372">системупдатевиндовстартминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="4ab73-372">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="4ab73-373">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab73-373">Int32</span></span>|<span data-ttu-id="4ab73-374">Указывает количество минут после полуночи, когда запустится окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="4ab73-374">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="4ab73-375">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="4ab73-375">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="4ab73-376">системупдатевиндовендминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="4ab73-376">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="4ab73-377">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab73-377">Int32</span></span>|<span data-ttu-id="4ab73-378">Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="4ab73-378">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="4ab73-379">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="4ab73-379">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="4ab73-380">системупдатеинсталлтипе</span><span class="sxs-lookup"><span data-stu-id="4ab73-380">systemUpdateInstallType</span></span>|[<span data-ttu-id="4ab73-381">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="4ab73-381">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="4ab73-382">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="4ab73-382">The type of system update configuration.</span></span> <span data-ttu-id="4ab73-383">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="4ab73-383">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="4ab73-384">системвиндовсблоккед</span><span class="sxs-lookup"><span data-stu-id="4ab73-384">systemWindowsBlocked</span></span>|<span data-ttu-id="4ab73-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-385">Boolean</span></span>|<span data-ttu-id="4ab73-386">Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="4ab73-386">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="4ab73-387">усерсблоккадд</span><span class="sxs-lookup"><span data-stu-id="4ab73-387">usersBlockAdd</span></span>|<span data-ttu-id="4ab73-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-388">Boolean</span></span>|<span data-ttu-id="4ab73-389">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="4ab73-389">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="4ab73-390">усерсблоккремове</span><span class="sxs-lookup"><span data-stu-id="4ab73-390">usersBlockRemove</span></span>|<span data-ttu-id="4ab73-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-391">Boolean</span></span>|<span data-ttu-id="4ab73-392">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="4ab73-392">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="4ab73-393">волумеблоккаджустмент</span><span class="sxs-lookup"><span data-stu-id="4ab73-393">volumeBlockAdjustment</span></span>|<span data-ttu-id="4ab73-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-394">Boolean</span></span>|<span data-ttu-id="4ab73-395">Указывает, отключена ли настройка главного тома.</span><span class="sxs-lookup"><span data-stu-id="4ab73-395">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="4ab73-396">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="4ab73-396">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="4ab73-397">Строка</span><span class="sxs-lookup"><span data-stu-id="4ab73-397">String</span></span>|<span data-ttu-id="4ab73-398">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="4ab73-398">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="4ab73-399">впналвайсонлоккдовнмоде</span><span class="sxs-lookup"><span data-stu-id="4ab73-399">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="4ab73-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-400">Boolean</span></span>|<span data-ttu-id="4ab73-401">Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="4ab73-401">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="4ab73-402">вифиблоккедитконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="4ab73-402">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="4ab73-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-403">Boolean</span></span>|<span data-ttu-id="4ab73-404">Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="4ab73-404">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="4ab73-405">вифиблоккедитполицидефинедконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="4ab73-405">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="4ab73-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ab73-406">Boolean</span></span>|<span data-ttu-id="4ab73-407">Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="4ab73-407">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="4ab73-408">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ab73-408">Response</span></span>
<span data-ttu-id="4ab73-409">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4ab73-409">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ab73-410">Пример</span><span class="sxs-lookup"><span data-stu-id="4ab73-410">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ab73-411">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ab73-411">Request</span></span>
<span data-ttu-id="4ab73-412">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ab73-412">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="4ab73-413">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ab73-413">Response</span></span>
<span data-ttu-id="4ab73-p136">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ab73-p136">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```





