---
title: Создание androidDeviceOwnerGeneralDeviceConfiguration
description: Создание нового объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 06e2bae6e729fa76fef88be33b30b5de0c6cb4fa
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49240938"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="af3ef-103">Создание androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="af3ef-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="af3ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af3ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af3ef-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af3ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af3ef-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af3ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af3ef-107">Создание нового объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="af3ef-107">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af3ef-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="af3ef-108">Prerequisites</span></span>
<span data-ttu-id="af3ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af3ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af3ef-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af3ef-111">Permission type</span></span>|<span data-ttu-id="af3ef-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af3ef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af3ef-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af3ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af3ef-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af3ef-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="af3ef-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af3ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af3ef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af3ef-116">Not supported.</span></span>|
|<span data-ttu-id="af3ef-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="af3ef-117">Application</span></span>|<span data-ttu-id="af3ef-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af3ef-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af3ef-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af3ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="af3ef-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="af3ef-120">Request headers</span></span>
|<span data-ttu-id="af3ef-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af3ef-121">Header</span></span>|<span data-ttu-id="af3ef-122">Значение</span><span class="sxs-lookup"><span data-stu-id="af3ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af3ef-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af3ef-123">Authorization</span></span>|<span data-ttu-id="af3ef-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af3ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af3ef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="af3ef-125">Accept</span></span>|<span data-ttu-id="af3ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af3ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af3ef-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af3ef-127">Request body</span></span>
<span data-ttu-id="af3ef-128">В тексте запроса добавьте представление объекта androidDeviceOwnerGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af3ef-128">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="af3ef-129">В следующей таблице приведены свойства, необходимые при создании androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="af3ef-129">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="af3ef-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="af3ef-130">Property</span></span>|<span data-ttu-id="af3ef-131">Тип</span><span class="sxs-lookup"><span data-stu-id="af3ef-131">Type</span></span>|<span data-ttu-id="af3ef-132">Описание</span><span class="sxs-lookup"><span data-stu-id="af3ef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af3ef-133">id</span><span class="sxs-lookup"><span data-stu-id="af3ef-133">id</span></span>|<span data-ttu-id="af3ef-134">String</span><span class="sxs-lookup"><span data-stu-id="af3ef-134">String</span></span>|<span data-ttu-id="af3ef-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="af3ef-135">Key of the entity.</span></span> <span data-ttu-id="af3ef-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af3ef-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af3ef-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af3ef-137">lastModifiedDateTime</span></span>|<span data-ttu-id="af3ef-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af3ef-138">DateTimeOffset</span></span>|<span data-ttu-id="af3ef-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="af3ef-139">DateTime the object was last modified.</span></span> <span data-ttu-id="af3ef-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af3ef-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af3ef-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="af3ef-141">roleScopeTagIds</span></span>|<span data-ttu-id="af3ef-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="af3ef-142">String collection</span></span>|<span data-ttu-id="af3ef-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="af3ef-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="af3ef-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af3ef-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af3ef-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="af3ef-145">supportsScopeTags</span></span>|<span data-ttu-id="af3ef-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-146">Boolean</span></span>|<span data-ttu-id="af3ef-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="af3ef-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="af3ef-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="af3ef-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="af3ef-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="af3ef-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="af3ef-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="af3ef-150">This property is read-only.</span></span> <span data-ttu-id="af3ef-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af3ef-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af3ef-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="af3ef-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="af3ef-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="af3ef-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="af3ef-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="af3ef-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="af3ef-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af3ef-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af3ef-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="af3ef-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="af3ef-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="af3ef-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="af3ef-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="af3ef-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="af3ef-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af3ef-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af3ef-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="af3ef-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="af3ef-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="af3ef-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="af3ef-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="af3ef-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="af3ef-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af3ef-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af3ef-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af3ef-164">createdDateTime</span></span>|<span data-ttu-id="af3ef-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af3ef-165">DateTimeOffset</span></span>|<span data-ttu-id="af3ef-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="af3ef-166">DateTime the object was created.</span></span> <span data-ttu-id="af3ef-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af3ef-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af3ef-168">description</span><span class="sxs-lookup"><span data-stu-id="af3ef-168">description</span></span>|<span data-ttu-id="af3ef-169">String</span><span class="sxs-lookup"><span data-stu-id="af3ef-169">String</span></span>|<span data-ttu-id="af3ef-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="af3ef-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="af3ef-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af3ef-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af3ef-172">displayName</span><span class="sxs-lookup"><span data-stu-id="af3ef-172">displayName</span></span>|<span data-ttu-id="af3ef-173">String</span><span class="sxs-lookup"><span data-stu-id="af3ef-173">String</span></span>|<span data-ttu-id="af3ef-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="af3ef-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="af3ef-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af3ef-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af3ef-176">version</span><span class="sxs-lookup"><span data-stu-id="af3ef-176">version</span></span>|<span data-ttu-id="af3ef-177">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-177">Int32</span></span>|<span data-ttu-id="af3ef-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="af3ef-178">Version of the device configuration.</span></span> <span data-ttu-id="af3ef-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="af3ef-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="af3ef-180">аккаунтсблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="af3ef-180">accountsBlockModification</span></span>|<span data-ttu-id="af3ef-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-181">Boolean</span></span>|<span data-ttu-id="af3ef-182">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="af3ef-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="af3ef-183">аппсалловинсталлфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="af3ef-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="af3ef-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-184">Boolean</span></span>|<span data-ttu-id="af3ef-185">Указывает, может ли пользователь включить параметр "неизвестные источники".</span><span class="sxs-lookup"><span data-stu-id="af3ef-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="af3ef-186">аппсаутаупдатеполици</span><span class="sxs-lookup"><span data-stu-id="af3ef-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="af3ef-187">андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="af3ef-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="af3ef-188">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="af3ef-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="af3ef-189">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="af3ef-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="af3ef-190">аппсдефаултпермиссионполици</span><span class="sxs-lookup"><span data-stu-id="af3ef-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="af3ef-191">андроиддевицеовнердефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="af3ef-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="af3ef-192">Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом.</span><span class="sxs-lookup"><span data-stu-id="af3ef-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="af3ef-193">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="af3ef-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="af3ef-194">аппсрекоммендскиппингфирстусехинтс</span><span class="sxs-lookup"><span data-stu-id="af3ef-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="af3ef-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-195">Boolean</span></span>|<span data-ttu-id="af3ef-196">Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.</span><span class="sxs-lookup"><span data-stu-id="af3ef-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="af3ef-197">блуетусблоккконфигуратион</span><span class="sxs-lookup"><span data-stu-id="af3ef-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="af3ef-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-198">Boolean</span></span>|<span data-ttu-id="af3ef-199">Указывает, следует ли запретить пользователю настраивать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="af3ef-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="af3ef-200">блуетусблоккконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="af3ef-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="af3ef-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-201">Boolean</span></span>|<span data-ttu-id="af3ef-202">Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="af3ef-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="af3ef-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="af3ef-203">cameraBlocked</span></span>|<span data-ttu-id="af3ef-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-204">Boolean</span></span>|<span data-ttu-id="af3ef-205">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="af3ef-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="af3ef-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="af3ef-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="af3ef-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-207">Boolean</span></span>|<span data-ttu-id="af3ef-208">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="af3ef-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="af3ef-209">цертификатекредентиалконфигуратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="af3ef-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="af3ef-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-210">Boolean</span></span>|<span data-ttu-id="af3ef-211">Указывает, следует ли запретить пользователям настраивать учетные данные сертификатов.</span><span class="sxs-lookup"><span data-stu-id="af3ef-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="af3ef-212">микрософтлаунчерконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="af3ef-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="af3ef-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-213">Boolean</span></span>|<span data-ttu-id="af3ef-214">Указывает, следует ли настроить средство запуска Microsoft.</span><span class="sxs-lookup"><span data-stu-id="af3ef-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="af3ef-215">микрософтлаунчеркустомваллпаперенаблед</span><span class="sxs-lookup"><span data-stu-id="af3ef-215">microsoftLauncherCustomWallpaperEnabled</span></span>|<span data-ttu-id="af3ef-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-216">Boolean</span></span>|<span data-ttu-id="af3ef-217">Указывает, следует ли настраивать фоновый рисунок на целевых устройствах.</span><span class="sxs-lookup"><span data-stu-id="af3ef-217">Indicates whether or not to configure the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="af3ef-218">микрософтлаунчеркустомваллпаперимажеурл</span><span class="sxs-lookup"><span data-stu-id="af3ef-218">microsoftLauncherCustomWallpaperImageUrl</span></span>|<span data-ttu-id="af3ef-219">String</span><span class="sxs-lookup"><span data-stu-id="af3ef-219">String</span></span>|<span data-ttu-id="af3ef-220">Указывает URL-адрес для файла изображения, который будет использоваться в качестве фонового рисунка на целевых устройствах.</span><span class="sxs-lookup"><span data-stu-id="af3ef-220">Indicates the URL for the image file to use as the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="af3ef-221">микрософтлаунчеркустомваллпапералловусермодификатион</span><span class="sxs-lookup"><span data-stu-id="af3ef-221">microsoftLauncherCustomWallpaperAllowUserModification</span></span>|<span data-ttu-id="af3ef-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-222">Boolean</span></span>|<span data-ttu-id="af3ef-223">Указывает, может ли пользователь изменять фоновый рисунок для персонализации своего устройства.</span><span class="sxs-lookup"><span data-stu-id="af3ef-223">Indicates whether or not the user can modify the wallpaper to personalize their device.</span></span>|
|<span data-ttu-id="af3ef-224">микрософтлаунчерфиденаблед</span><span class="sxs-lookup"><span data-stu-id="af3ef-224">microsoftLauncherFeedEnabled</span></span>|<span data-ttu-id="af3ef-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-225">Boolean</span></span>|<span data-ttu-id="af3ef-226">Указывает, следует ли включить веб-канал запуска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="af3ef-226">Indicates whether or not you want to enable the launcher feed on the device.</span></span>|
|<span data-ttu-id="af3ef-227">микрософтлаунчерфидалловусермодификатион</span><span class="sxs-lookup"><span data-stu-id="af3ef-227">microsoftLauncherFeedAllowUserModification</span></span>|<span data-ttu-id="af3ef-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-228">Boolean</span></span>|<span data-ttu-id="af3ef-229">Указывает, может ли пользователь изменять веб-канал запуска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="af3ef-229">Indicates whether or not the user can modify the launcher feed on the device.</span></span>|
|<span data-ttu-id="af3ef-230">микрософтлаунчердоккпресенцеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="af3ef-230">microsoftLauncherDockPresenceConfiguration</span></span>|[<span data-ttu-id="af3ef-231">microsoftLauncherDockPresence</span><span class="sxs-lookup"><span data-stu-id="af3ef-231">microsoftLauncherDockPresence</span></span>](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|<span data-ttu-id="af3ef-232">Указывает, следует ли настроить закрепление устройства.</span><span class="sxs-lookup"><span data-stu-id="af3ef-232">Indicates whether or not you want to configure the device dock.</span></span> <span data-ttu-id="af3ef-233">Возможные значения: `notConfigured`, `show`, `hide`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="af3ef-233">Possible values are: `notConfigured`, `show`, `hide`, `disabled`.</span></span>|
|<span data-ttu-id="af3ef-234">микрософтлаунчердоккпресенцеалловусермодификатион</span><span class="sxs-lookup"><span data-stu-id="af3ef-234">microsoftLauncherDockPresenceAllowUserModification</span></span>|<span data-ttu-id="af3ef-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-235">Boolean</span></span>|<span data-ttu-id="af3ef-236">Указывает, может ли пользователь изменять конфигурацию закрепления устройств на устройстве.</span><span class="sxs-lookup"><span data-stu-id="af3ef-236">Indicates whether or not the user can modify the device dock configuration on the device.</span></span>|
|<span data-ttu-id="af3ef-237">микрософтлаунчерсеарчбарплацементконфигуратион</span><span class="sxs-lookup"><span data-stu-id="af3ef-237">microsoftLauncherSearchBarPlacementConfiguration</span></span>|[<span data-ttu-id="af3ef-238">microsoftLauncherSearchBarPlacement</span><span class="sxs-lookup"><span data-stu-id="af3ef-238">microsoftLauncherSearchBarPlacement</span></span>](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|<span data-ttu-id="af3ef-239">Указывает конфигурацию размещения панели поиска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="af3ef-239">Indicates the search bar placement configuration on the device.</span></span> <span data-ttu-id="af3ef-240">Возможные значения: `notConfigured`, `top`, `bottom`, `hide`.</span><span class="sxs-lookup"><span data-stu-id="af3ef-240">Possible values are: `notConfigured`, `top`, `bottom`, `hide`.</span></span>|
|<span data-ttu-id="af3ef-241">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="af3ef-241">enrollmentProfile</span></span>|[<span data-ttu-id="af3ef-242">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="af3ef-242">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="af3ef-243">Указывает, какой профиль регистрации вы хотите настроить.</span><span class="sxs-lookup"><span data-stu-id="af3ef-243">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="af3ef-244">Возможные значения: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span><span class="sxs-lookup"><span data-stu-id="af3ef-244">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="af3ef-245">датароамингблоккед</span><span class="sxs-lookup"><span data-stu-id="af3ef-245">dataRoamingBlocked</span></span>|<span data-ttu-id="af3ef-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-246">Boolean</span></span>|<span data-ttu-id="af3ef-247">Указывает, следует ли запретить пользователю перемещать данные.</span><span class="sxs-lookup"><span data-stu-id="af3ef-247">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="af3ef-248">датетимеконфигуратионблоккед</span><span class="sxs-lookup"><span data-stu-id="af3ef-248">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="af3ef-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-249">Boolean</span></span>|<span data-ttu-id="af3ef-250">Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.</span><span class="sxs-lookup"><span data-stu-id="af3ef-250">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="af3ef-251">факториресетдевицеадминистраторемаилс</span><span class="sxs-lookup"><span data-stu-id="af3ef-251">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="af3ef-252">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="af3ef-252">String collection</span></span>|<span data-ttu-id="af3ef-253">Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.</span><span class="sxs-lookup"><span data-stu-id="af3ef-253">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="af3ef-254">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="af3ef-254">factoryResetBlocked</span></span>|<span data-ttu-id="af3ef-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-255">Boolean</span></span>|<span data-ttu-id="af3ef-256">Указывает, отключен ли параметр Reset фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="af3ef-256">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="af3ef-257">глобалпрокси</span><span class="sxs-lookup"><span data-stu-id="af3ef-257">globalProxy</span></span>|[<span data-ttu-id="af3ef-258">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="af3ef-258">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="af3ef-259">Прокси-сервер настраивается напрямую с узлом, портом и исключенными узлами.</span><span class="sxs-lookup"><span data-stu-id="af3ef-259">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="af3ef-260">гуглеаккаунтсблоккед</span><span class="sxs-lookup"><span data-stu-id="af3ef-260">googleAccountsBlocked</span></span>|<span data-ttu-id="af3ef-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-261">Boolean</span></span>|<span data-ttu-id="af3ef-262">Указывает, будут ли блокироваться учетные записи Google.</span><span class="sxs-lookup"><span data-stu-id="af3ef-262">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="af3ef-263">киосккустомизатиондевицесеттингсблоккед</span><span class="sxs-lookup"><span data-stu-id="af3ef-263">kioskCustomizationDeviceSettingsBlocked</span></span>|<span data-ttu-id="af3ef-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-264">Boolean</span></span>|<span data-ttu-id="af3ef-265">Указывает, может ли пользователь получить доступ к приложению параметров устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-265">Indicates whether a user can access the device's Settings app while in Kiosk Mode.</span></span>|
|<span data-ttu-id="af3ef-266">киосккустомизатионповербуттонактионсблоккед</span><span class="sxs-lookup"><span data-stu-id="af3ef-266">kioskCustomizationPowerButtonActionsBlocked</span></span>|<span data-ttu-id="af3ef-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-267">Boolean</span></span>|<span data-ttu-id="af3ef-268">Отображается ли меню "Электропитание", когда пользователь нажимает кнопку Power на устройстве в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-268">Whether the power menu is shown when a user long presses the Power button of a device in Kiosk Mode.</span></span>|
|<span data-ttu-id="af3ef-269">киосккустомизатионстатусбар</span><span class="sxs-lookup"><span data-stu-id="af3ef-269">kioskCustomizationStatusBar</span></span>|[<span data-ttu-id="af3ef-270">андроиддевицеовнеркиосккустомизатионстатусбар</span><span class="sxs-lookup"><span data-stu-id="af3ef-270">androidDeviceOwnerKioskCustomizationStatusBar</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|<span data-ttu-id="af3ef-271">Указывает, отключаются ли сведения о системе и уведомления в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-271">Indicates whether system info and notifications are disabled in Kiosk Mode.</span></span> <span data-ttu-id="af3ef-272">Возможные значения: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.</span><span class="sxs-lookup"><span data-stu-id="af3ef-272">Possible values are: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.</span></span>|
|<span data-ttu-id="af3ef-273">киосккустомизатионсистемеррорварнингс</span><span class="sxs-lookup"><span data-stu-id="af3ef-273">kioskCustomizationSystemErrorWarnings</span></span>|<span data-ttu-id="af3ef-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-274">Boolean</span></span>|<span data-ttu-id="af3ef-275">Указывает, отображаются ли диалоговые окна системных ошибок для аварийных или не реагирующих приложений в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-275">Indicates whether system error dialogs for crashed or unresponsive apps are shown in Kiosk Mode.</span></span>|
|<span data-ttu-id="af3ef-276">киосккустомизатионсистемнавигатион</span><span class="sxs-lookup"><span data-stu-id="af3ef-276">kioskCustomizationSystemNavigation</span></span>|[<span data-ttu-id="af3ef-277">андроиддевицеовнеркиосккустомизатионсистемнавигатион</span><span class="sxs-lookup"><span data-stu-id="af3ef-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|<span data-ttu-id="af3ef-278">Указывает, какие функции навигации включены в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-278">Indicates which navigation features are enabled in Kiosk Mode.</span></span> <span data-ttu-id="af3ef-279">Возможные значения: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.</span><span class="sxs-lookup"><span data-stu-id="af3ef-279">Possible values are: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.</span></span>|
|<span data-ttu-id="af3ef-280">киоскмодескринсаверконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="af3ef-280">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="af3ef-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-281">Boolean</span></span>|<span data-ttu-id="af3ef-282">Указывает, следует ли включить режим экранной заставки или не в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-282">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="af3ef-283">киоскмодескринсаверимажеурл</span><span class="sxs-lookup"><span data-stu-id="af3ef-283">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="af3ef-284">String</span><span class="sxs-lookup"><span data-stu-id="af3ef-284">String</span></span>|<span data-ttu-id="af3ef-285">URL-адрес изображения, которое будет экранной заставкой устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-285">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="af3ef-286">киоскмодескринсавердисплайтимеинсекондс</span><span class="sxs-lookup"><span data-stu-id="af3ef-286">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="af3ef-287">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-287">Int32</span></span>|<span data-ttu-id="af3ef-288">Время (в секундах), в течение которого устройство будет отображать экранную заставку в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-288">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="af3ef-289">Допустимые значения — от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="af3ef-289">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="af3ef-290">киоскмодескринсаверстартделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="af3ef-290">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="af3ef-291">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-291">Int32</span></span>|<span data-ttu-id="af3ef-292">Время (в секундах), в течение которого устройство должно быть неактивным, чтобы экранная заставка отображалась в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-292">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="af3ef-293">Допустимые значения — от 1 до 9999999</span><span class="sxs-lookup"><span data-stu-id="af3ef-293">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="af3ef-294">киоскмодескринсавердетектмедиадисаблед</span><span class="sxs-lookup"><span data-stu-id="af3ef-294">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="af3ef-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-295">Boolean</span></span>|<span data-ttu-id="af3ef-296">Указывает, должно ли устройство отображать экранную заставку при воспроизведении аудио-и видеоконференций в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="af3ef-296">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="af3ef-297">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="af3ef-297">kioskModeApps</span></span>|<span data-ttu-id="af3ef-298">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="af3ef-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="af3ef-299">Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-299">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="af3ef-300">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="af3ef-300">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="af3ef-301">киоскмодеваллпаперурл</span><span class="sxs-lookup"><span data-stu-id="af3ef-301">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="af3ef-302">String</span><span class="sxs-lookup"><span data-stu-id="af3ef-302">String</span></span>|<span data-ttu-id="af3ef-303">URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-303">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="af3ef-304">киоскмодикситкоде</span><span class="sxs-lookup"><span data-stu-id="af3ef-304">kioskModeExitCode</span></span>|<span data-ttu-id="af3ef-305">String</span><span class="sxs-lookup"><span data-stu-id="af3ef-305">String</span></span>|<span data-ttu-id="af3ef-306">Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-306">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="af3ef-307">киоскмодевиртуалхомебуттоненаблед</span><span class="sxs-lookup"><span data-stu-id="af3ef-307">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="af3ef-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-308">Boolean</span></span>|<span data-ttu-id="af3ef-309">Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-309">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="af3ef-310">киоскмодевиртуалхомебуттонтипе</span><span class="sxs-lookup"><span data-stu-id="af3ef-310">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="af3ef-311">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="af3ef-311">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="af3ef-312">Указывает, является ли кнопка "Виртуальная Домашняя страница" кнопкой "Прокрутка вверх" или плавающей кнопкой "домой".</span><span class="sxs-lookup"><span data-stu-id="af3ef-312">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="af3ef-313">Возможные значения: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="af3ef-313">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="af3ef-314">киоскмодеблуетусконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="af3ef-314">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="af3ef-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-315">Boolean</span></span>|<span data-ttu-id="af3ef-316">Указывает, следует ли запретить пользователю настраивать параметры Bluetooth в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-316">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="af3ef-317">киоскмодевификонфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="af3ef-317">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="af3ef-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-318">Boolean</span></span>|<span data-ttu-id="af3ef-319">Указывает, следует ли запретить пользователю настраивать параметры Wi-Fi в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-319">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="af3ef-320">киоскмодефлашлигхтконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="af3ef-320">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="af3ef-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-321">Boolean</span></span>|<span data-ttu-id="af3ef-322">Указывает, следует ли разрешить пользователю использовать флашлигхт в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-322">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="af3ef-323">киоскмодемедиаволумеконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="af3ef-323">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="af3ef-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-324">Boolean</span></span>|<span data-ttu-id="af3ef-325">Указывает, следует ли запретить пользователю изменять громкость мультимедиа в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-325">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="af3ef-326">киоскмодешовдевицеинфо</span><span class="sxs-lookup"><span data-stu-id="af3ef-326">kioskModeShowDeviceInfo</span></span>|<span data-ttu-id="af3ef-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-327">Boolean</span></span>|<span data-ttu-id="af3ef-328">Указывает, следует ли разрешить пользователю доступ к сведениям о базовом устройстве.</span><span class="sxs-lookup"><span data-stu-id="af3ef-328">Whether or not to allow a user to access basic device information.</span></span>|
|<span data-ttu-id="af3ef-329">киоскмодеманажедсеттингсентридисаблед</span><span class="sxs-lookup"><span data-stu-id="af3ef-329">kioskModeManagedSettingsEntryDisabled</span></span>|<span data-ttu-id="af3ef-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-330">Boolean</span></span>|<span data-ttu-id="af3ef-331">Указывает, следует ли отображать точку входа управляемых параметров на управляемом домашнем экране в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-331">Whether or not to display the Managed Settings entry point on the managed home screen in Kiosk Mode.</span></span>|
|<span data-ttu-id="af3ef-332">киоскмодедебугменуеасякцессенаблед</span><span class="sxs-lookup"><span data-stu-id="af3ef-332">kioskModeDebugMenuEasyAccessEnabled</span></span>|<span data-ttu-id="af3ef-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-333">Boolean</span></span>|<span data-ttu-id="af3ef-334">Указывает, следует ли запретить пользователю простой доступ к меню Отладка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-334">Whether or not to allow a user to easy access to the debug menu in Kiosk Mode.</span></span>|
|<span data-ttu-id="af3ef-335">киоскмодешоваппнотификатионбадже</span><span class="sxs-lookup"><span data-stu-id="af3ef-335">kioskModeShowAppNotificationBadge</span></span>|<span data-ttu-id="af3ef-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-336">Boolean</span></span>|<span data-ttu-id="af3ef-337">Указывает, следует ли отображать эмблемы уведомлений приложений в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-337">Whether or not to display application notification badges in Kiosk Mode.</span></span>|
|<span data-ttu-id="af3ef-338">киоскмодескринориентатион</span><span class="sxs-lookup"><span data-stu-id="af3ef-338">kioskModeScreenOrientation</span></span>|[<span data-ttu-id="af3ef-339">androidDeviceOwnerKioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="af3ef-339">androidDeviceOwnerKioskModeScreenOrientation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|<span data-ttu-id="af3ef-340">Конфигурация ориентации экрана для управляемого экрана дома в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-340">Screen orientation configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="af3ef-341">Возможные значения: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span><span class="sxs-lookup"><span data-stu-id="af3ef-341">Possible values are: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span></span>|
|<span data-ttu-id="af3ef-342">киоскмодеиконсизе</span><span class="sxs-lookup"><span data-stu-id="af3ef-342">kioskModeIconSize</span></span>|[<span data-ttu-id="af3ef-343">androidDeviceOwnerKioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="af3ef-343">androidDeviceOwnerKioskModeIconSize</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|<span data-ttu-id="af3ef-344">Конфигурация размера значков для управляемого экрана дома в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-344">Icon size configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="af3ef-345">Возможные значения: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span><span class="sxs-lookup"><span data-stu-id="af3ef-345">Possible values are: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span></span>|
|<span data-ttu-id="af3ef-346">киоскмодефолдерикон</span><span class="sxs-lookup"><span data-stu-id="af3ef-346">kioskModeFolderIcon</span></span>|[<span data-ttu-id="af3ef-347">androidDeviceOwnerKioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="af3ef-347">androidDeviceOwnerKioskModeFolderIcon</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|<span data-ttu-id="af3ef-348">Конфигурация значков папок для управляемого экрана дома в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-348">Folder icon configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="af3ef-349">Возможные значения: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span><span class="sxs-lookup"><span data-stu-id="af3ef-349">Possible values are: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span></span>|
|<span data-ttu-id="af3ef-350">киоскмодевифиалловедссидс</span><span class="sxs-lookup"><span data-stu-id="af3ef-350">kioskModeWifiAllowedSsids</span></span>|<span data-ttu-id="af3ef-351">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="af3ef-351">String collection</span></span>|<span data-ttu-id="af3ef-352">Ограниченный набор подключений WIFI SSID, доступных пользователю для настройки в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="af3ef-352">The restricted set of WIFI SSIDs available for the user to configure in Kiosk Mode.</span></span> <span data-ttu-id="af3ef-353">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="af3ef-353">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="af3ef-354">микрофонефорцемуте</span><span class="sxs-lookup"><span data-stu-id="af3ef-354">microphoneForceMute</span></span>|<span data-ttu-id="af3ef-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-355">Boolean</span></span>|<span data-ttu-id="af3ef-356">Указывает, следует ли запретить разблокирование микрофона устройства.</span><span class="sxs-lookup"><span data-stu-id="af3ef-356">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="af3ef-357">нетворкескапехатчалловед</span><span class="sxs-lookup"><span data-stu-id="af3ef-357">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="af3ef-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-358">Boolean</span></span>|<span data-ttu-id="af3ef-359">Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="af3ef-359">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="af3ef-360">нфкблоккаутгоингбеам</span><span class="sxs-lookup"><span data-stu-id="af3ef-360">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="af3ef-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-361">Boolean</span></span>|<span data-ttu-id="af3ef-362">Указывает, следует ли заблокировать исходящую форму NFC.</span><span class="sxs-lookup"><span data-stu-id="af3ef-362">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="af3ef-363">пассвордблокккэйгуард</span><span class="sxs-lookup"><span data-stu-id="af3ef-363">passwordBlockKeyguard</span></span>|<span data-ttu-id="af3ef-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-364">Boolean</span></span>|<span data-ttu-id="af3ef-365">Указывает, отключен ли кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="af3ef-365">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="af3ef-366">пассвордблокккэйгуардфеатурес</span><span class="sxs-lookup"><span data-stu-id="af3ef-366">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="af3ef-367">Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="af3ef-367">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="af3ef-368">Список компонентов кэйгуард устройств, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="af3ef-368">List of device keyguard features to block.</span></span> <span data-ttu-id="af3ef-369">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="af3ef-369">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="af3ef-370">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="af3ef-370">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="af3ef-371">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="af3ef-371">passwordExpirationDays</span></span>|<span data-ttu-id="af3ef-372">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-372">Int32</span></span>|<span data-ttu-id="af3ef-373">Указывает период времени, в течение которого можно задать пароль до истечения срока его действия, а также потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="af3ef-373">Indicates the amount of time that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="af3ef-374">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="af3ef-374">Valid values 1 to 365</span></span>|
|<span data-ttu-id="af3ef-375">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="af3ef-375">passwordMinimumLength</span></span>|<span data-ttu-id="af3ef-376">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-376">Int32</span></span>|<span data-ttu-id="af3ef-377">Указывает минимальную длину пароля, необходимого для устройства.</span><span class="sxs-lookup"><span data-stu-id="af3ef-377">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="af3ef-378">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="af3ef-378">Valid values 4 to 16</span></span>|
|<span data-ttu-id="af3ef-379">пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="af3ef-379">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="af3ef-380">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-380">Int32</span></span>|<span data-ttu-id="af3ef-381">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="af3ef-381">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="af3ef-382">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="af3ef-382">Valid values 1 to 16</span></span>|
|<span data-ttu-id="af3ef-383">пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="af3ef-383">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="af3ef-384">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-384">Int32</span></span>|<span data-ttu-id="af3ef-385">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="af3ef-385">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="af3ef-386">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="af3ef-386">Valid values 1 to 16</span></span>|
|<span data-ttu-id="af3ef-387">пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="af3ef-387">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="af3ef-388">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-388">Int32</span></span>|<span data-ttu-id="af3ef-389">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="af3ef-389">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="af3ef-390">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="af3ef-390">Valid values 1 to 16</span></span>|
|<span data-ttu-id="af3ef-391">пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="af3ef-391">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="af3ef-392">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-392">Int32</span></span>|<span data-ttu-id="af3ef-393">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="af3ef-393">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="af3ef-394">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="af3ef-394">Valid values 1 to 16</span></span>|
|<span data-ttu-id="af3ef-395">пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="af3ef-395">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="af3ef-396">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-396">Int32</span></span>|<span data-ttu-id="af3ef-397">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="af3ef-397">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="af3ef-398">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="af3ef-398">Valid values 1 to 16</span></span>|
|<span data-ttu-id="af3ef-399">пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="af3ef-399">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="af3ef-400">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-400">Int32</span></span>|<span data-ttu-id="af3ef-401">Указывает минимальное количество символов в верхнем регистре, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="af3ef-401">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="af3ef-402">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="af3ef-402">Valid values 1 to 16</span></span>|
|<span data-ttu-id="af3ef-403">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="af3ef-403">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="af3ef-404">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-404">Int32</span></span>|<span data-ttu-id="af3ef-405">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="af3ef-405">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="af3ef-406">пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="af3ef-406">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="af3ef-407">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-407">Int32</span></span>|<span data-ttu-id="af3ef-408">Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале.</span><span class="sxs-lookup"><span data-stu-id="af3ef-408">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="af3ef-409">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="af3ef-409">Valid values 0 to 24</span></span>|
|<span data-ttu-id="af3ef-410">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="af3ef-410">passwordRequiredType</span></span>|[<span data-ttu-id="af3ef-411">андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="af3ef-411">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="af3ef-412">Указывает минимальное качество пароля, необходимое для устройства.</span><span class="sxs-lookup"><span data-stu-id="af3ef-412">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="af3ef-413">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="af3ef-413">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="af3ef-414">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="af3ef-414">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="af3ef-415">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-415">Int32</span></span>|<span data-ttu-id="af3ef-416">Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="af3ef-416">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="af3ef-417">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="af3ef-417">Valid values 4 to 11</span></span>|
|<span data-ttu-id="af3ef-418">плайсторемоде</span><span class="sxs-lookup"><span data-stu-id="af3ef-418">playStoreMode</span></span>|[<span data-ttu-id="af3ef-419">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="af3ef-419">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="af3ef-420">Указывает режим проигрывания устройства в хранилище.</span><span class="sxs-lookup"><span data-stu-id="af3ef-420">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="af3ef-421">Возможные значения: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="af3ef-421">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="af3ef-422">сафебутблоккед</span><span class="sxs-lookup"><span data-stu-id="af3ef-422">safeBootBlocked</span></span>|<span data-ttu-id="af3ef-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-423">Boolean</span></span>|<span data-ttu-id="af3ef-424">Указывает, отключена ли загрузка устройства в "безопасная загрузка".</span><span class="sxs-lookup"><span data-stu-id="af3ef-424">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="af3ef-425">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="af3ef-425">screenCaptureBlocked</span></span>|<span data-ttu-id="af3ef-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-426">Boolean</span></span>|<span data-ttu-id="af3ef-427">Указывает, следует ли отключить возможность использования снимков экрана.</span><span class="sxs-lookup"><span data-stu-id="af3ef-427">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="af3ef-428">секуритялловдебуггингфеатурес</span><span class="sxs-lookup"><span data-stu-id="af3ef-428">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="af3ef-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-429">Boolean</span></span>|<span data-ttu-id="af3ef-430">Указывает, следует ли запретить пользователю включать функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="af3ef-430">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="af3ef-431">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="af3ef-431">securityRequireVerifyApps</span></span>|<span data-ttu-id="af3ef-432">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-432">Boolean</span></span>|<span data-ttu-id="af3ef-433">Указывает, требуется ли проверка приложений.</span><span class="sxs-lookup"><span data-stu-id="af3ef-433">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="af3ef-434">статусбарблоккед</span><span class="sxs-lookup"><span data-stu-id="af3ef-434">statusBarBlocked</span></span>|<span data-ttu-id="af3ef-435">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-435">Boolean</span></span>|<span data-ttu-id="af3ef-436">Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.</span><span class="sxs-lookup"><span data-stu-id="af3ef-436">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="af3ef-437">стайонмодес</span><span class="sxs-lookup"><span data-stu-id="af3ef-437">stayOnModes</span></span>|<span data-ttu-id="af3ef-438">Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="af3ef-438">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="af3ef-439">Список режимов, в которых дисплей устройства остается включенным.</span><span class="sxs-lookup"><span data-stu-id="af3ef-439">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="af3ef-440">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="af3ef-440">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="af3ef-441">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="af3ef-441">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="af3ef-442">сторажеалловусб</span><span class="sxs-lookup"><span data-stu-id="af3ef-442">storageAllowUsb</span></span>|<span data-ttu-id="af3ef-443">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-443">Boolean</span></span>|<span data-ttu-id="af3ef-444">Указывает, следует ли разрешить запоминающее устройство USB.</span><span class="sxs-lookup"><span data-stu-id="af3ef-444">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="af3ef-445">сторажеблоккекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="af3ef-445">storageBlockExternalMedia</span></span>|<span data-ttu-id="af3ef-446">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-446">Boolean</span></span>|<span data-ttu-id="af3ef-447">Указывает, следует ли заблокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="af3ef-447">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="af3ef-448">сторажеблоккусбфилетрансфер</span><span class="sxs-lookup"><span data-stu-id="af3ef-448">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="af3ef-449">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-449">Boolean</span></span>|<span data-ttu-id="af3ef-450">Указывает, следует ли запретить передачу файлов через USB.</span><span class="sxs-lookup"><span data-stu-id="af3ef-450">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="af3ef-451">системупдатевиндовстартминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="af3ef-451">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="af3ef-452">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-452">Int32</span></span>|<span data-ttu-id="af3ef-453">Указывает количество минут после полуночи, когда запустится окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="af3ef-453">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="af3ef-454">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="af3ef-454">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="af3ef-455">системупдатевиндовендминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="af3ef-455">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="af3ef-456">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-456">Int32</span></span>|<span data-ttu-id="af3ef-457">Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="af3ef-457">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="af3ef-458">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="af3ef-458">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="af3ef-459">системупдатеинсталлтипе</span><span class="sxs-lookup"><span data-stu-id="af3ef-459">systemUpdateInstallType</span></span>|[<span data-ttu-id="af3ef-460">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="af3ef-460">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="af3ef-461">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="af3ef-461">The type of system update configuration.</span></span> <span data-ttu-id="af3ef-462">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="af3ef-462">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="af3ef-463">системвиндовсблоккед</span><span class="sxs-lookup"><span data-stu-id="af3ef-463">systemWindowsBlocked</span></span>|<span data-ttu-id="af3ef-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-464">Boolean</span></span>|<span data-ttu-id="af3ef-465">Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="af3ef-465">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="af3ef-466">усерсблоккадд</span><span class="sxs-lookup"><span data-stu-id="af3ef-466">usersBlockAdd</span></span>|<span data-ttu-id="af3ef-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-467">Boolean</span></span>|<span data-ttu-id="af3ef-468">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="af3ef-468">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="af3ef-469">усерсблоккремове</span><span class="sxs-lookup"><span data-stu-id="af3ef-469">usersBlockRemove</span></span>|<span data-ttu-id="af3ef-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-470">Boolean</span></span>|<span data-ttu-id="af3ef-471">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="af3ef-471">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="af3ef-472">волумеблоккаджустмент</span><span class="sxs-lookup"><span data-stu-id="af3ef-472">volumeBlockAdjustment</span></span>|<span data-ttu-id="af3ef-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-473">Boolean</span></span>|<span data-ttu-id="af3ef-474">Указывает, отключена ли настройка главного тома.</span><span class="sxs-lookup"><span data-stu-id="af3ef-474">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="af3ef-475">впналвайсонлоккдовнмоде</span><span class="sxs-lookup"><span data-stu-id="af3ef-475">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="af3ef-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-476">Boolean</span></span>|<span data-ttu-id="af3ef-477">Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="af3ef-477">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="af3ef-478">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="af3ef-478">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="af3ef-479">String</span><span class="sxs-lookup"><span data-stu-id="af3ef-479">String</span></span>|<span data-ttu-id="af3ef-480">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="af3ef-480">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="af3ef-481">вифиблоккедитконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="af3ef-481">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="af3ef-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-482">Boolean</span></span>|<span data-ttu-id="af3ef-483">Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="af3ef-483">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="af3ef-484">вифиблоккедитполицидефинедконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="af3ef-484">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="af3ef-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-485">Boolean</span></span>|<span data-ttu-id="af3ef-486">Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="af3ef-486">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|
|<span data-ttu-id="af3ef-487">персоналпрофилеаппсалловинсталлфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="af3ef-487">personalProfileAppsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="af3ef-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-488">Boolean</span></span>|<span data-ttu-id="af3ef-489">Указывает, может ли пользователь устанавливать приложения из неизвестных источников в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="af3ef-489">Indicates whether the user can install apps from unknown sources on the personal profile.</span></span>|
|<span data-ttu-id="af3ef-490">персоналпрофилекамераблоккед</span><span class="sxs-lookup"><span data-stu-id="af3ef-490">personalProfileCameraBlocked</span></span>|<span data-ttu-id="af3ef-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-491">Boolean</span></span>|<span data-ttu-id="af3ef-492">Указывает, следует ли отключить использование камеры в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="af3ef-492">Indicates whether to disable the use of the camera on the personal profile.</span></span>|
|<span data-ttu-id="af3ef-493">персоналпрофилескринкаптуреблоккед</span><span class="sxs-lookup"><span data-stu-id="af3ef-493">personalProfileScreenCaptureBlocked</span></span>|<span data-ttu-id="af3ef-494">Boolean</span><span class="sxs-lookup"><span data-stu-id="af3ef-494">Boolean</span></span>|<span data-ttu-id="af3ef-495">Указывает, следует ли отключить возможность делать снимки экрана в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="af3ef-495">Indicates whether to disable the capability to take screenshots on the personal profile.</span></span>|
|<span data-ttu-id="af3ef-496">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="af3ef-496">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="af3ef-497">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-497">Int32</span></span>|<span data-ttu-id="af3ef-498">Указывает количество дней, в течение которых может быть установлен пароль рабочего профиля до истечения срока действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="af3ef-498">Indicates the number of days that a work profile password can be set before it expires and a new password will be required.</span></span> <span data-ttu-id="af3ef-499">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="af3ef-499">Valid values 1 to 365</span></span>|
|<span data-ttu-id="af3ef-500">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="af3ef-500">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="af3ef-501">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-501">Int32</span></span>|<span data-ttu-id="af3ef-502">Указывает минимальную длину пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="af3ef-502">Indicates the minimum length of the work profile password.</span></span> <span data-ttu-id="af3ef-503">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="af3ef-503">Valid values 4 to 16</span></span>|
|<span data-ttu-id="af3ef-504">воркпрофилепассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="af3ef-504">workProfilePasswordMinimumNumericCharacters</span></span>|<span data-ttu-id="af3ef-505">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-505">Int32</span></span>|<span data-ttu-id="af3ef-506">Указывает минимальное количество числовых символов, необходимое для пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="af3ef-506">Indicates the minimum number of numeric characters required for the work profile password.</span></span> <span data-ttu-id="af3ef-507">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="af3ef-507">Valid values 1 to 16</span></span>|
|<span data-ttu-id="af3ef-508">воркпрофилепассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="af3ef-508">workProfilePasswordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="af3ef-509">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-509">Int32</span></span>|<span data-ttu-id="af3ef-510">Указывает минимальное количество небуквенных символов, необходимых для пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="af3ef-510">Indicates the minimum number of non-letter characters required for the work profile password.</span></span> <span data-ttu-id="af3ef-511">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="af3ef-511">Valid values 1 to 16</span></span>|
|<span data-ttu-id="af3ef-512">воркпрофилепассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="af3ef-512">workProfilePasswordMinimumLetterCharacters</span></span>|<span data-ttu-id="af3ef-513">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-513">Int32</span></span>|<span data-ttu-id="af3ef-514">Указывает минимальное число символов, необходимых для пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="af3ef-514">Indicates the minimum number of letter characters required for the work profile password.</span></span> <span data-ttu-id="af3ef-515">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="af3ef-515">Valid values 1 to 16</span></span>|
|<span data-ttu-id="af3ef-516">воркпрофилепассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="af3ef-516">workProfilePasswordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="af3ef-517">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-517">Int32</span></span>|<span data-ttu-id="af3ef-518">Указывает минимальное количество символов нижнего регистра, необходимых для пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="af3ef-518">Indicates the minimum number of lower-case characters required for the work profile password.</span></span> <span data-ttu-id="af3ef-519">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="af3ef-519">Valid values 1 to 16</span></span>|
|<span data-ttu-id="af3ef-520">воркпрофилепассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="af3ef-520">workProfilePasswordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="af3ef-521">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-521">Int32</span></span>|<span data-ttu-id="af3ef-522">Указывает минимальное количество символов в верхнем регистре, необходимое для пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="af3ef-522">Indicates the minimum number of upper-case letter characters required for the work profile password.</span></span> <span data-ttu-id="af3ef-523">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="af3ef-523">Valid values 1 to 16</span></span>|
|<span data-ttu-id="af3ef-524">воркпрофилепассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="af3ef-524">workProfilePasswordMinimumSymbolCharacters</span></span>|<span data-ttu-id="af3ef-525">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-525">Int32</span></span>|<span data-ttu-id="af3ef-526">Указывает минимальное число символов, необходимых для пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="af3ef-526">Indicates the minimum number of symbol characters required for the work profile password.</span></span> <span data-ttu-id="af3ef-527">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="af3ef-527">Valid values 1 to 16</span></span>|
|<span data-ttu-id="af3ef-528">воркпрофилепассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="af3ef-528">workProfilePasswordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="af3ef-529">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-529">Int32</span></span>|<span data-ttu-id="af3ef-530">Указывает длину журнала паролей рабочего профиля, в котором пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале.</span><span class="sxs-lookup"><span data-stu-id="af3ef-530">Indicates the length of the work profile password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="af3ef-531">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="af3ef-531">Valid values 0 to 24</span></span>|
|<span data-ttu-id="af3ef-532">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="af3ef-532">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="af3ef-533">Int32</span><span class="sxs-lookup"><span data-stu-id="af3ef-533">Int32</span></span>|<span data-ttu-id="af3ef-534">Указывает, сколько раз пользователь может ввести неправильный пароль рабочего профиля, прежде чем устройство будет очищено.</span><span class="sxs-lookup"><span data-stu-id="af3ef-534">Indicates the number of times a user can enter an incorrect work profile password before the device is wiped.</span></span> <span data-ttu-id="af3ef-535">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="af3ef-535">Valid values 4 to 11</span></span>|
|<span data-ttu-id="af3ef-536">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="af3ef-536">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="af3ef-537">андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="af3ef-537">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="af3ef-538">Указывает минимальное качество пароля, необходимое для пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="af3ef-538">Indicates the minimum password quality required on the work profile password.</span></span> <span data-ttu-id="af3ef-539">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="af3ef-539">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="af3ef-540">Отклик</span><span class="sxs-lookup"><span data-stu-id="af3ef-540">Response</span></span>
<span data-ttu-id="af3ef-541">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="af3ef-541">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af3ef-542">Пример</span><span class="sxs-lookup"><span data-stu-id="af3ef-542">Example</span></span>

### <a name="request"></a><span data-ttu-id="af3ef-543">Запрос</span><span class="sxs-lookup"><span data-stu-id="af3ef-543">Request</span></span>
<span data-ttu-id="af3ef-544">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af3ef-544">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 6387

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
  "kioskCustomizationDeviceSettingsBlocked": true,
  "kioskCustomizationPowerButtonActionsBlocked": true,
  "kioskCustomizationStatusBar": "notificationsAndSystemInfoEnabled",
  "kioskCustomizationSystemErrorWarnings": true,
  "kioskCustomizationSystemNavigation": "navigationEnabled",
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
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinimumNumericCharacters": 11,
  "workProfilePasswordMinimumNonLetterCharacters": 13,
  "workProfilePasswordMinimumLetterCharacters": 10,
  "workProfilePasswordMinimumLowerCaseCharacters": 13,
  "workProfilePasswordMinimumUpperCaseCharacters": 13,
  "workProfilePasswordMinimumSymbolCharacters": 10,
  "workProfilePasswordPreviousPasswordCountToBlock": 15,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "required"
}
```

### <a name="response"></a><span data-ttu-id="af3ef-545">Отклик</span><span class="sxs-lookup"><span data-stu-id="af3ef-545">Response</span></span>
<span data-ttu-id="af3ef-p156">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af3ef-p156">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 6559

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
  "kioskCustomizationDeviceSettingsBlocked": true,
  "kioskCustomizationPowerButtonActionsBlocked": true,
  "kioskCustomizationStatusBar": "notificationsAndSystemInfoEnabled",
  "kioskCustomizationSystemErrorWarnings": true,
  "kioskCustomizationSystemNavigation": "navigationEnabled",
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
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinimumNumericCharacters": 11,
  "workProfilePasswordMinimumNonLetterCharacters": 13,
  "workProfilePasswordMinimumLetterCharacters": 10,
  "workProfilePasswordMinimumLowerCaseCharacters": 13,
  "workProfilePasswordMinimumUpperCaseCharacters": 13,
  "workProfilePasswordMinimumSymbolCharacters": 10,
  "workProfilePasswordPreviousPasswordCountToBlock": 15,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "required"
}
```




