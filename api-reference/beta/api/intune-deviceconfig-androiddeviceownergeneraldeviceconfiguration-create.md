---
title: Создание androidDeviceOwnerGeneralDeviceConfiguration
description: Создание нового объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: be9f2b0fd08f09cfa96d227d879c0f9cb6931358
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178747"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="22345-103">Создание androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="22345-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="22345-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22345-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22345-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22345-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22345-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22345-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22345-107">Создание нового объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="22345-107">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22345-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="22345-108">Prerequisites</span></span>
<span data-ttu-id="22345-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22345-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22345-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22345-111">Permission type</span></span>|<span data-ttu-id="22345-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="22345-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22345-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22345-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22345-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22345-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22345-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22345-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22345-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22345-116">Not supported.</span></span>|
|<span data-ttu-id="22345-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22345-117">Application</span></span>|<span data-ttu-id="22345-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22345-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22345-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22345-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="22345-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="22345-120">Request headers</span></span>
|<span data-ttu-id="22345-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22345-121">Header</span></span>|<span data-ttu-id="22345-122">Значение</span><span class="sxs-lookup"><span data-stu-id="22345-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22345-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22345-123">Authorization</span></span>|<span data-ttu-id="22345-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22345-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22345-125">Accept</span><span class="sxs-lookup"><span data-stu-id="22345-125">Accept</span></span>|<span data-ttu-id="22345-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22345-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22345-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22345-127">Request body</span></span>
<span data-ttu-id="22345-128">В тексте запроса добавьте представление объекта androidDeviceOwnerGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22345-128">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="22345-129">В следующей таблице приведены свойства, необходимые при создании androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="22345-129">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="22345-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="22345-130">Property</span></span>|<span data-ttu-id="22345-131">Тип</span><span class="sxs-lookup"><span data-stu-id="22345-131">Type</span></span>|<span data-ttu-id="22345-132">Описание</span><span class="sxs-lookup"><span data-stu-id="22345-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22345-133">id</span><span class="sxs-lookup"><span data-stu-id="22345-133">id</span></span>|<span data-ttu-id="22345-134">String</span><span class="sxs-lookup"><span data-stu-id="22345-134">String</span></span>|<span data-ttu-id="22345-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="22345-135">Key of the entity.</span></span> <span data-ttu-id="22345-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22345-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22345-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22345-137">lastModifiedDateTime</span></span>|<span data-ttu-id="22345-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22345-138">DateTimeOffset</span></span>|<span data-ttu-id="22345-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="22345-139">DateTime the object was last modified.</span></span> <span data-ttu-id="22345-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22345-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22345-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="22345-141">roleScopeTagIds</span></span>|<span data-ttu-id="22345-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="22345-142">String collection</span></span>|<span data-ttu-id="22345-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="22345-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="22345-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22345-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22345-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="22345-145">supportsScopeTags</span></span>|<span data-ttu-id="22345-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-146">Boolean</span></span>|<span data-ttu-id="22345-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="22345-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="22345-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="22345-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="22345-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="22345-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="22345-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="22345-150">This property is read-only.</span></span> <span data-ttu-id="22345-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22345-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22345-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="22345-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="22345-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="22345-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="22345-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="22345-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="22345-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22345-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22345-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="22345-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="22345-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="22345-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="22345-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="22345-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="22345-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22345-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22345-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="22345-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="22345-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="22345-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="22345-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="22345-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="22345-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22345-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22345-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22345-164">createdDateTime</span></span>|<span data-ttu-id="22345-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22345-165">DateTimeOffset</span></span>|<span data-ttu-id="22345-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="22345-166">DateTime the object was created.</span></span> <span data-ttu-id="22345-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22345-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22345-168">description</span><span class="sxs-lookup"><span data-stu-id="22345-168">description</span></span>|<span data-ttu-id="22345-169">String</span><span class="sxs-lookup"><span data-stu-id="22345-169">String</span></span>|<span data-ttu-id="22345-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="22345-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="22345-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22345-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22345-172">displayName</span><span class="sxs-lookup"><span data-stu-id="22345-172">displayName</span></span>|<span data-ttu-id="22345-173">Строка</span><span class="sxs-lookup"><span data-stu-id="22345-173">String</span></span>|<span data-ttu-id="22345-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="22345-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="22345-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22345-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22345-176">version</span><span class="sxs-lookup"><span data-stu-id="22345-176">version</span></span>|<span data-ttu-id="22345-177">Int32</span><span class="sxs-lookup"><span data-stu-id="22345-177">Int32</span></span>|<span data-ttu-id="22345-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="22345-178">Version of the device configuration.</span></span> <span data-ttu-id="22345-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22345-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22345-180">аккаунтсблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="22345-180">accountsBlockModification</span></span>|<span data-ttu-id="22345-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-181">Boolean</span></span>|<span data-ttu-id="22345-182">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="22345-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="22345-183">аппсалловинсталлфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="22345-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="22345-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-184">Boolean</span></span>|<span data-ttu-id="22345-185">Указывает, может ли пользователь включить параметр "неизвестные источники".</span><span class="sxs-lookup"><span data-stu-id="22345-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="22345-186">аппсаутаупдатеполици</span><span class="sxs-lookup"><span data-stu-id="22345-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="22345-187">андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="22345-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="22345-188">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="22345-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="22345-189">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="22345-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="22345-190">аппсдефаултпермиссионполици</span><span class="sxs-lookup"><span data-stu-id="22345-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="22345-191">андроиддевицеовнердефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="22345-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="22345-192">Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом.</span><span class="sxs-lookup"><span data-stu-id="22345-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="22345-193">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="22345-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="22345-194">аппсрекоммендскиппингфирстусехинтс</span><span class="sxs-lookup"><span data-stu-id="22345-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="22345-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-195">Boolean</span></span>|<span data-ttu-id="22345-196">Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.</span><span class="sxs-lookup"><span data-stu-id="22345-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="22345-197">блуетусблоккконфигуратион</span><span class="sxs-lookup"><span data-stu-id="22345-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="22345-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-198">Boolean</span></span>|<span data-ttu-id="22345-199">Указывает, следует ли запретить пользователю настраивать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="22345-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="22345-200">блуетусблоккконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="22345-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="22345-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-201">Boolean</span></span>|<span data-ttu-id="22345-202">Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="22345-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="22345-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="22345-203">cameraBlocked</span></span>|<span data-ttu-id="22345-204">Логический</span><span class="sxs-lookup"><span data-stu-id="22345-204">Boolean</span></span>|<span data-ttu-id="22345-205">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="22345-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="22345-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="22345-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="22345-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-207">Boolean</span></span>|<span data-ttu-id="22345-208">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="22345-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="22345-209">цертификатекредентиалконфигуратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="22345-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="22345-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-210">Boolean</span></span>|<span data-ttu-id="22345-211">Указывает, следует ли запретить пользователям настраивать учетные данные сертификатов.</span><span class="sxs-lookup"><span data-stu-id="22345-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="22345-212">микрософтлаунчерконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="22345-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="22345-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-213">Boolean</span></span>|<span data-ttu-id="22345-214">Указывает, следует ли настроить средство запуска Microsoft.</span><span class="sxs-lookup"><span data-stu-id="22345-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="22345-215">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="22345-215">enrollmentProfile</span></span>|[<span data-ttu-id="22345-216">андроиддевицеовнеренроллментпрофилетипе</span><span class="sxs-lookup"><span data-stu-id="22345-216">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="22345-217">Указывает, какой профиль регистрации вы хотите настроить.</span><span class="sxs-lookup"><span data-stu-id="22345-217">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="22345-218">Возможные значения: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span><span class="sxs-lookup"><span data-stu-id="22345-218">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="22345-219">датароамингблоккед</span><span class="sxs-lookup"><span data-stu-id="22345-219">dataRoamingBlocked</span></span>|<span data-ttu-id="22345-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-220">Boolean</span></span>|<span data-ttu-id="22345-221">Указывает, следует ли запретить пользователю перемещать данные.</span><span class="sxs-lookup"><span data-stu-id="22345-221">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="22345-222">датетимеконфигуратионблоккед</span><span class="sxs-lookup"><span data-stu-id="22345-222">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="22345-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-223">Boolean</span></span>|<span data-ttu-id="22345-224">Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.</span><span class="sxs-lookup"><span data-stu-id="22345-224">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="22345-225">факториресетдевицеадминистраторемаилс</span><span class="sxs-lookup"><span data-stu-id="22345-225">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="22345-226">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="22345-226">String collection</span></span>|<span data-ttu-id="22345-227">Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.</span><span class="sxs-lookup"><span data-stu-id="22345-227">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="22345-228">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="22345-228">factoryResetBlocked</span></span>|<span data-ttu-id="22345-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-229">Boolean</span></span>|<span data-ttu-id="22345-230">Указывает, отключен ли параметр Reset фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="22345-230">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="22345-231">глобалпрокси</span><span class="sxs-lookup"><span data-stu-id="22345-231">globalProxy</span></span>|[<span data-ttu-id="22345-232">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="22345-232">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="22345-233">Прокси-сервер настраивается напрямую с узлом, портом и исключенными узлами.</span><span class="sxs-lookup"><span data-stu-id="22345-233">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="22345-234">гуглеаккаунтсблоккед</span><span class="sxs-lookup"><span data-stu-id="22345-234">googleAccountsBlocked</span></span>|<span data-ttu-id="22345-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-235">Boolean</span></span>|<span data-ttu-id="22345-236">Указывает, будут ли блокироваться учетные записи Google.</span><span class="sxs-lookup"><span data-stu-id="22345-236">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="22345-237">киоскмодескринсаверконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="22345-237">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="22345-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-238">Boolean</span></span>|<span data-ttu-id="22345-239">Указывает, следует ли включить режим экранной заставки или не в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="22345-239">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="22345-240">киоскмодескринсаверимажеурл</span><span class="sxs-lookup"><span data-stu-id="22345-240">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="22345-241">Строка</span><span class="sxs-lookup"><span data-stu-id="22345-241">String</span></span>|<span data-ttu-id="22345-242">URL-адрес изображения, которое будет экранной заставкой устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="22345-242">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="22345-243">киоскмодескринсавердисплайтимеинсекондс</span><span class="sxs-lookup"><span data-stu-id="22345-243">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="22345-244">Int32</span><span class="sxs-lookup"><span data-stu-id="22345-244">Int32</span></span>|<span data-ttu-id="22345-245">Время (в секундах), в течение которого устройство будет отображать экранную заставку в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="22345-245">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="22345-246">Допустимые значения — от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="22345-246">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="22345-247">киоскмодескринсаверстартделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="22345-247">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="22345-248">Int32</span><span class="sxs-lookup"><span data-stu-id="22345-248">Int32</span></span>|<span data-ttu-id="22345-249">Время (в секундах), в течение которого устройство должно быть неактивным, чтобы экранная заставка отображалась в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="22345-249">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="22345-250">Допустимые значения — от 1 до 9999999</span><span class="sxs-lookup"><span data-stu-id="22345-250">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="22345-251">киоскмодескринсавердетектмедиадисаблед</span><span class="sxs-lookup"><span data-stu-id="22345-251">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="22345-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-252">Boolean</span></span>|<span data-ttu-id="22345-253">Указывает, должно ли устройство отображать экранную заставку при воспроизведении аудио-и видеоконференций в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="22345-253">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="22345-254">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="22345-254">kioskModeApps</span></span>|<span data-ttu-id="22345-255">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="22345-255">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="22345-256">Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="22345-256">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="22345-257">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="22345-257">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="22345-258">киоскмодеваллпаперурл</span><span class="sxs-lookup"><span data-stu-id="22345-258">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="22345-259">Строка</span><span class="sxs-lookup"><span data-stu-id="22345-259">String</span></span>|<span data-ttu-id="22345-260">URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="22345-260">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="22345-261">киоскмодикситкоде</span><span class="sxs-lookup"><span data-stu-id="22345-261">kioskModeExitCode</span></span>|<span data-ttu-id="22345-262">Строка</span><span class="sxs-lookup"><span data-stu-id="22345-262">String</span></span>|<span data-ttu-id="22345-263">Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="22345-263">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="22345-264">киоскмодевиртуалхомебуттоненаблед</span><span class="sxs-lookup"><span data-stu-id="22345-264">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="22345-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-265">Boolean</span></span>|<span data-ttu-id="22345-266">Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="22345-266">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="22345-267">киоскмодевиртуалхомебуттонтипе</span><span class="sxs-lookup"><span data-stu-id="22345-267">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="22345-268">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="22345-268">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="22345-269">Указывает, является ли кнопка "Виртуальная Домашняя страница" кнопкой "Прокрутка вверх" или плавающей кнопкой "домой".</span><span class="sxs-lookup"><span data-stu-id="22345-269">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="22345-270">Возможные значения: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="22345-270">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="22345-271">киоскмодеблуетусконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="22345-271">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="22345-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-272">Boolean</span></span>|<span data-ttu-id="22345-273">Указывает, следует ли запретить пользователю настраивать параметры Bluetooth в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="22345-273">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="22345-274">киоскмодевификонфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="22345-274">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="22345-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-275">Boolean</span></span>|<span data-ttu-id="22345-276">Указывает, следует ли разрешить пользователю настраивать параметры Wi/Fi в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="22345-276">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="22345-277">киоскмодефлашлигхтконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="22345-277">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="22345-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-278">Boolean</span></span>|<span data-ttu-id="22345-279">Указывает, следует ли разрешить пользователю использовать флашлигхт в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="22345-279">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="22345-280">киоскмодемедиаволумеконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="22345-280">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="22345-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-281">Boolean</span></span>|<span data-ttu-id="22345-282">Указывает, следует ли запретить пользователю изменять громкость мультимедиа в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="22345-282">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="22345-283">микрофонефорцемуте</span><span class="sxs-lookup"><span data-stu-id="22345-283">microphoneForceMute</span></span>|<span data-ttu-id="22345-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-284">Boolean</span></span>|<span data-ttu-id="22345-285">Указывает, следует ли запретить разблокирование микрофона устройства.</span><span class="sxs-lookup"><span data-stu-id="22345-285">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="22345-286">нетворкескапехатчалловед</span><span class="sxs-lookup"><span data-stu-id="22345-286">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="22345-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-287">Boolean</span></span>|<span data-ttu-id="22345-288">Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="22345-288">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="22345-289">нфкблоккаутгоингбеам</span><span class="sxs-lookup"><span data-stu-id="22345-289">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="22345-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-290">Boolean</span></span>|<span data-ttu-id="22345-291">Указывает, следует ли заблокировать исходящую форму NFC.</span><span class="sxs-lookup"><span data-stu-id="22345-291">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="22345-292">пассвордблокккэйгуард</span><span class="sxs-lookup"><span data-stu-id="22345-292">passwordBlockKeyguard</span></span>|<span data-ttu-id="22345-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-293">Boolean</span></span>|<span data-ttu-id="22345-294">Указывает, отключен ли кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="22345-294">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="22345-295">пассвордблокккэйгуардфеатурес</span><span class="sxs-lookup"><span data-stu-id="22345-295">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="22345-296">Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="22345-296">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="22345-297">Список компонентов кэйгуард устройств, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="22345-297">List of device keyguard features to block.</span></span> <span data-ttu-id="22345-298">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="22345-298">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="22345-299">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="22345-299">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="22345-300">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="22345-300">passwordExpirationDays</span></span>|<span data-ttu-id="22345-301">Int32</span><span class="sxs-lookup"><span data-stu-id="22345-301">Int32</span></span>|<span data-ttu-id="22345-302">Указывает время в секундах, в течение которого можно задать пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="22345-302">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="22345-303">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="22345-303">Valid values 1 to 365</span></span>|
|<span data-ttu-id="22345-304">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="22345-304">passwordMinimumLength</span></span>|<span data-ttu-id="22345-305">Int32</span><span class="sxs-lookup"><span data-stu-id="22345-305">Int32</span></span>|<span data-ttu-id="22345-306">Указывает минимальную длину пароля, необходимого для устройства.</span><span class="sxs-lookup"><span data-stu-id="22345-306">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="22345-307">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="22345-307">Valid values 4 to 16</span></span>|
|<span data-ttu-id="22345-308">пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="22345-308">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="22345-309">Int32</span><span class="sxs-lookup"><span data-stu-id="22345-309">Int32</span></span>|<span data-ttu-id="22345-310">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="22345-310">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="22345-311">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="22345-311">Valid values 1 to 16</span></span>|
|<span data-ttu-id="22345-312">пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="22345-312">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="22345-313">Int32</span><span class="sxs-lookup"><span data-stu-id="22345-313">Int32</span></span>|<span data-ttu-id="22345-314">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="22345-314">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="22345-315">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="22345-315">Valid values 1 to 16</span></span>|
|<span data-ttu-id="22345-316">пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="22345-316">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="22345-317">Int32</span><span class="sxs-lookup"><span data-stu-id="22345-317">Int32</span></span>|<span data-ttu-id="22345-318">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="22345-318">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="22345-319">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="22345-319">Valid values 1 to 16</span></span>|
|<span data-ttu-id="22345-320">пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="22345-320">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="22345-321">Int32</span><span class="sxs-lookup"><span data-stu-id="22345-321">Int32</span></span>|<span data-ttu-id="22345-322">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="22345-322">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="22345-323">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="22345-323">Valid values 1 to 16</span></span>|
|<span data-ttu-id="22345-324">пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="22345-324">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="22345-325">Int32</span><span class="sxs-lookup"><span data-stu-id="22345-325">Int32</span></span>|<span data-ttu-id="22345-326">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="22345-326">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="22345-327">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="22345-327">Valid values 1 to 16</span></span>|
|<span data-ttu-id="22345-328">пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="22345-328">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="22345-329">Int32</span><span class="sxs-lookup"><span data-stu-id="22345-329">Int32</span></span>|<span data-ttu-id="22345-330">Указывает минимальное число символов верхнего каселеттер, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="22345-330">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="22345-331">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="22345-331">Valid values 1 to 16</span></span>|
|<span data-ttu-id="22345-332">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="22345-332">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="22345-333">Int32</span><span class="sxs-lookup"><span data-stu-id="22345-333">Int32</span></span>|<span data-ttu-id="22345-334">Миллисекунды бездействия до истечения времени ожидания экрана.</span><span class="sxs-lookup"><span data-stu-id="22345-334">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="22345-335">пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="22345-335">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="22345-336">Int32</span><span class="sxs-lookup"><span data-stu-id="22345-336">Int32</span></span>|<span data-ttu-id="22345-337">Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале.</span><span class="sxs-lookup"><span data-stu-id="22345-337">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="22345-338">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="22345-338">Valid values 0 to 24</span></span>|
|<span data-ttu-id="22345-339">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="22345-339">passwordRequiredType</span></span>|[<span data-ttu-id="22345-340">андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="22345-340">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="22345-341">Указывает минимальное качество пароля, необходимое для устройства.</span><span class="sxs-lookup"><span data-stu-id="22345-341">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="22345-342">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="22345-342">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="22345-343">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="22345-343">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="22345-344">Int32</span><span class="sxs-lookup"><span data-stu-id="22345-344">Int32</span></span>|<span data-ttu-id="22345-345">Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="22345-345">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="22345-346">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="22345-346">Valid values 4 to 11</span></span>|
|<span data-ttu-id="22345-347">плайсторемоде</span><span class="sxs-lookup"><span data-stu-id="22345-347">playStoreMode</span></span>|[<span data-ttu-id="22345-348">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="22345-348">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="22345-349">Указывает режим проигрывания устройства в хранилище.</span><span class="sxs-lookup"><span data-stu-id="22345-349">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="22345-350">Возможные значения: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="22345-350">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="22345-351">сафебутблоккед</span><span class="sxs-lookup"><span data-stu-id="22345-351">safeBootBlocked</span></span>|<span data-ttu-id="22345-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-352">Boolean</span></span>|<span data-ttu-id="22345-353">Указывает, отключена ли загрузка устройства в "безопасная загрузка".</span><span class="sxs-lookup"><span data-stu-id="22345-353">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="22345-354">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="22345-354">screenCaptureBlocked</span></span>|<span data-ttu-id="22345-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-355">Boolean</span></span>|<span data-ttu-id="22345-356">Указывает, следует ли отключить возможность использования снимков экрана.</span><span class="sxs-lookup"><span data-stu-id="22345-356">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="22345-357">секуритялловдебуггингфеатурес</span><span class="sxs-lookup"><span data-stu-id="22345-357">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="22345-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-358">Boolean</span></span>|<span data-ttu-id="22345-359">Указывает, следует ли запретить пользователю включать функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="22345-359">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="22345-360">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="22345-360">securityRequireVerifyApps</span></span>|<span data-ttu-id="22345-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-361">Boolean</span></span>|<span data-ttu-id="22345-362">Указывает, требуется ли проверка приложений.</span><span class="sxs-lookup"><span data-stu-id="22345-362">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="22345-363">статусбарблоккед</span><span class="sxs-lookup"><span data-stu-id="22345-363">statusBarBlocked</span></span>|<span data-ttu-id="22345-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-364">Boolean</span></span>|<span data-ttu-id="22345-365">Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.</span><span class="sxs-lookup"><span data-stu-id="22345-365">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="22345-366">стайонмодес</span><span class="sxs-lookup"><span data-stu-id="22345-366">stayOnModes</span></span>|<span data-ttu-id="22345-367">Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="22345-367">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="22345-368">Список режимов, в которых дисплей устройства остается включенным.</span><span class="sxs-lookup"><span data-stu-id="22345-368">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="22345-369">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="22345-369">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="22345-370">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="22345-370">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="22345-371">сторажеалловусб</span><span class="sxs-lookup"><span data-stu-id="22345-371">storageAllowUsb</span></span>|<span data-ttu-id="22345-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-372">Boolean</span></span>|<span data-ttu-id="22345-373">Указывает, следует ли разрешить запоминающее устройство USB.</span><span class="sxs-lookup"><span data-stu-id="22345-373">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="22345-374">сторажеблоккекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="22345-374">storageBlockExternalMedia</span></span>|<span data-ttu-id="22345-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-375">Boolean</span></span>|<span data-ttu-id="22345-376">Указывает, следует ли заблокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="22345-376">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="22345-377">сторажеблоккусбфилетрансфер</span><span class="sxs-lookup"><span data-stu-id="22345-377">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="22345-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-378">Boolean</span></span>|<span data-ttu-id="22345-379">Указывает, следует ли запретить передачу файлов через USB.</span><span class="sxs-lookup"><span data-stu-id="22345-379">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="22345-380">системупдатевиндовстартминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="22345-380">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="22345-381">Int32</span><span class="sxs-lookup"><span data-stu-id="22345-381">Int32</span></span>|<span data-ttu-id="22345-382">Указывает количество минут после полуночи, когда запустится окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="22345-382">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="22345-383">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="22345-383">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="22345-384">системупдатевиндовендминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="22345-384">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="22345-385">Int32</span><span class="sxs-lookup"><span data-stu-id="22345-385">Int32</span></span>|<span data-ttu-id="22345-386">Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="22345-386">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="22345-387">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="22345-387">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="22345-388">системупдатеинсталлтипе</span><span class="sxs-lookup"><span data-stu-id="22345-388">systemUpdateInstallType</span></span>|[<span data-ttu-id="22345-389">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="22345-389">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="22345-390">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="22345-390">The type of system update configuration.</span></span> <span data-ttu-id="22345-391">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="22345-391">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="22345-392">системвиндовсблоккед</span><span class="sxs-lookup"><span data-stu-id="22345-392">systemWindowsBlocked</span></span>|<span data-ttu-id="22345-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-393">Boolean</span></span>|<span data-ttu-id="22345-394">Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="22345-394">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="22345-395">усерсблоккадд</span><span class="sxs-lookup"><span data-stu-id="22345-395">usersBlockAdd</span></span>|<span data-ttu-id="22345-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-396">Boolean</span></span>|<span data-ttu-id="22345-397">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="22345-397">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="22345-398">усерсблоккремове</span><span class="sxs-lookup"><span data-stu-id="22345-398">usersBlockRemove</span></span>|<span data-ttu-id="22345-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-399">Boolean</span></span>|<span data-ttu-id="22345-400">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="22345-400">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="22345-401">волумеблоккаджустмент</span><span class="sxs-lookup"><span data-stu-id="22345-401">volumeBlockAdjustment</span></span>|<span data-ttu-id="22345-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-402">Boolean</span></span>|<span data-ttu-id="22345-403">Указывает, отключена ли настройка главного тома.</span><span class="sxs-lookup"><span data-stu-id="22345-403">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="22345-404">впналвайсонлоккдовнмоде</span><span class="sxs-lookup"><span data-stu-id="22345-404">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="22345-405">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-405">Boolean</span></span>|<span data-ttu-id="22345-406">Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="22345-406">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="22345-407">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="22345-407">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="22345-408">Строка</span><span class="sxs-lookup"><span data-stu-id="22345-408">String</span></span>|<span data-ttu-id="22345-409">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="22345-409">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="22345-410">вифиблоккедитконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="22345-410">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="22345-411">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-411">Boolean</span></span>|<span data-ttu-id="22345-412">Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="22345-412">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="22345-413">вифиблоккедитполицидефинедконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="22345-413">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="22345-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="22345-414">Boolean</span></span>|<span data-ttu-id="22345-415">Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="22345-415">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="22345-416">Ответ</span><span class="sxs-lookup"><span data-stu-id="22345-416">Response</span></span>
<span data-ttu-id="22345-417">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="22345-417">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22345-418">Пример</span><span class="sxs-lookup"><span data-stu-id="22345-418">Example</span></span>

### <a name="request"></a><span data-ttu-id="22345-419">Запрос</span><span class="sxs-lookup"><span data-stu-id="22345-419">Request</span></span>
<span data-ttu-id="22345-420">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22345-420">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="22345-421">Отклик</span><span class="sxs-lookup"><span data-stu-id="22345-421">Response</span></span>
<span data-ttu-id="22345-p137">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22345-p137">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



