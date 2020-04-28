---
title: Создание androidDeviceOwnerGeneralDeviceConfiguration
description: Создание нового объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6ab466aca2100d4151ceedee5f95931014cebd28
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43350762"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="3f04e-103">Создание androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3f04e-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="3f04e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f04e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f04e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f04e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f04e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f04e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f04e-107">Создание нового объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3f04e-107">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f04e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3f04e-108">Prerequisites</span></span>
<span data-ttu-id="3f04e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f04e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f04e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f04e-111">Permission type</span></span>|<span data-ttu-id="3f04e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f04e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f04e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f04e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f04e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f04e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3f04e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f04e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f04e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f04e-116">Not supported.</span></span>|
|<span data-ttu-id="3f04e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f04e-117">Application</span></span>|<span data-ttu-id="3f04e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f04e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f04e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f04e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3f04e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3f04e-120">Request headers</span></span>
|<span data-ttu-id="3f04e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f04e-121">Header</span></span>|<span data-ttu-id="3f04e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3f04e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f04e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f04e-123">Authorization</span></span>|<span data-ttu-id="3f04e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f04e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f04e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3f04e-125">Accept</span></span>|<span data-ttu-id="3f04e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f04e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f04e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3f04e-127">Request body</span></span>
<span data-ttu-id="3f04e-128">В тексте запроса добавьте представление объекта androidDeviceOwnerGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f04e-128">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="3f04e-129">В следующей таблице приведены свойства, необходимые при создании androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3f04e-129">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="3f04e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f04e-130">Property</span></span>|<span data-ttu-id="3f04e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3f04e-131">Type</span></span>|<span data-ttu-id="3f04e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3f04e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f04e-133">id</span><span class="sxs-lookup"><span data-stu-id="3f04e-133">id</span></span>|<span data-ttu-id="3f04e-134">String</span><span class="sxs-lookup"><span data-stu-id="3f04e-134">String</span></span>|<span data-ttu-id="3f04e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3f04e-135">Key of the entity.</span></span> <span data-ttu-id="3f04e-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f04e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f04e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f04e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3f04e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f04e-138">DateTimeOffset</span></span>|<span data-ttu-id="3f04e-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3f04e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3f04e-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f04e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f04e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3f04e-141">roleScopeTagIds</span></span>|<span data-ttu-id="3f04e-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="3f04e-142">String collection</span></span>|<span data-ttu-id="3f04e-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3f04e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3f04e-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f04e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f04e-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="3f04e-145">supportsScopeTags</span></span>|<span data-ttu-id="3f04e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-146">Boolean</span></span>|<span data-ttu-id="3f04e-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="3f04e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3f04e-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="3f04e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3f04e-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3f04e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3f04e-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f04e-150">This property is read-only.</span></span> <span data-ttu-id="3f04e-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f04e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f04e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3f04e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3f04e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3f04e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3f04e-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3f04e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3f04e-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f04e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f04e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3f04e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3f04e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3f04e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3f04e-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3f04e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3f04e-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f04e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f04e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3f04e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3f04e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3f04e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3f04e-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3f04e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3f04e-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f04e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f04e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f04e-164">createdDateTime</span></span>|<span data-ttu-id="3f04e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f04e-165">DateTimeOffset</span></span>|<span data-ttu-id="3f04e-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3f04e-166">DateTime the object was created.</span></span> <span data-ttu-id="3f04e-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f04e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f04e-168">description</span><span class="sxs-lookup"><span data-stu-id="3f04e-168">description</span></span>|<span data-ttu-id="3f04e-169">String</span><span class="sxs-lookup"><span data-stu-id="3f04e-169">String</span></span>|<span data-ttu-id="3f04e-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3f04e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3f04e-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f04e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f04e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3f04e-172">displayName</span></span>|<span data-ttu-id="3f04e-173">Строка</span><span class="sxs-lookup"><span data-stu-id="3f04e-173">String</span></span>|<span data-ttu-id="3f04e-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3f04e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3f04e-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f04e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f04e-176">version</span><span class="sxs-lookup"><span data-stu-id="3f04e-176">version</span></span>|<span data-ttu-id="3f04e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3f04e-177">Int32</span></span>|<span data-ttu-id="3f04e-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3f04e-178">Version of the device configuration.</span></span> <span data-ttu-id="3f04e-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f04e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f04e-180">аккаунтсблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="3f04e-180">accountsBlockModification</span></span>|<span data-ttu-id="3f04e-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-181">Boolean</span></span>|<span data-ttu-id="3f04e-182">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="3f04e-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="3f04e-183">аппсалловинсталлфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="3f04e-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="3f04e-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-184">Boolean</span></span>|<span data-ttu-id="3f04e-185">Указывает, может ли пользователь включить параметр "неизвестные источники".</span><span class="sxs-lookup"><span data-stu-id="3f04e-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="3f04e-186">аппсаутаупдатеполици</span><span class="sxs-lookup"><span data-stu-id="3f04e-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="3f04e-187">андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="3f04e-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="3f04e-188">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="3f04e-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="3f04e-189">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="3f04e-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="3f04e-190">аппсдефаултпермиссионполици</span><span class="sxs-lookup"><span data-stu-id="3f04e-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="3f04e-191">андроиддевицеовнердефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="3f04e-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="3f04e-192">Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом.</span><span class="sxs-lookup"><span data-stu-id="3f04e-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="3f04e-193">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="3f04e-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="3f04e-194">аппсрекоммендскиппингфирстусехинтс</span><span class="sxs-lookup"><span data-stu-id="3f04e-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="3f04e-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-195">Boolean</span></span>|<span data-ttu-id="3f04e-196">Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.</span><span class="sxs-lookup"><span data-stu-id="3f04e-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="3f04e-197">блуетусблоккконфигуратион</span><span class="sxs-lookup"><span data-stu-id="3f04e-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="3f04e-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-198">Boolean</span></span>|<span data-ttu-id="3f04e-199">Указывает, следует ли запретить пользователю настраивать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="3f04e-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="3f04e-200">блуетусблоккконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="3f04e-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="3f04e-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-201">Boolean</span></span>|<span data-ttu-id="3f04e-202">Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="3f04e-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="3f04e-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="3f04e-203">cameraBlocked</span></span>|<span data-ttu-id="3f04e-204">Логический</span><span class="sxs-lookup"><span data-stu-id="3f04e-204">Boolean</span></span>|<span data-ttu-id="3f04e-205">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="3f04e-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="3f04e-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="3f04e-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="3f04e-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-207">Boolean</span></span>|<span data-ttu-id="3f04e-208">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="3f04e-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="3f04e-209">цертификатекредентиалконфигуратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="3f04e-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="3f04e-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-210">Boolean</span></span>|<span data-ttu-id="3f04e-211">Указывает, следует ли запретить пользователям настраивать учетные данные сертификатов.</span><span class="sxs-lookup"><span data-stu-id="3f04e-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="3f04e-212">датароамингблоккед</span><span class="sxs-lookup"><span data-stu-id="3f04e-212">dataRoamingBlocked</span></span>|<span data-ttu-id="3f04e-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-213">Boolean</span></span>|<span data-ttu-id="3f04e-214">Указывает, следует ли запретить пользователю перемещать данные.</span><span class="sxs-lookup"><span data-stu-id="3f04e-214">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="3f04e-215">датетимеконфигуратионблоккед</span><span class="sxs-lookup"><span data-stu-id="3f04e-215">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="3f04e-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-216">Boolean</span></span>|<span data-ttu-id="3f04e-217">Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.</span><span class="sxs-lookup"><span data-stu-id="3f04e-217">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="3f04e-218">факториресетдевицеадминистраторемаилс</span><span class="sxs-lookup"><span data-stu-id="3f04e-218">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="3f04e-219">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="3f04e-219">String collection</span></span>|<span data-ttu-id="3f04e-220">Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.</span><span class="sxs-lookup"><span data-stu-id="3f04e-220">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="3f04e-221">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="3f04e-221">factoryResetBlocked</span></span>|<span data-ttu-id="3f04e-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-222">Boolean</span></span>|<span data-ttu-id="3f04e-223">Указывает, отключен ли параметр Reset фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="3f04e-223">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="3f04e-224">глобалпрокси</span><span class="sxs-lookup"><span data-stu-id="3f04e-224">globalProxy</span></span>|[<span data-ttu-id="3f04e-225">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="3f04e-225">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="3f04e-226">Прокси-сервер настраивается напрямую с узлом, портом и исключенными узлами.</span><span class="sxs-lookup"><span data-stu-id="3f04e-226">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="3f04e-227">гуглеаккаунтсблоккед</span><span class="sxs-lookup"><span data-stu-id="3f04e-227">googleAccountsBlocked</span></span>|<span data-ttu-id="3f04e-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-228">Boolean</span></span>|<span data-ttu-id="3f04e-229">Указывает, будут ли блокироваться учетные записи Google.</span><span class="sxs-lookup"><span data-stu-id="3f04e-229">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="3f04e-230">киоскмодескринсаверконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="3f04e-230">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="3f04e-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-231">Boolean</span></span>|<span data-ttu-id="3f04e-232">Указывает, следует ли включить режим экранной заставки или не в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="3f04e-232">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="3f04e-233">киоскмодескринсаверимажеурл</span><span class="sxs-lookup"><span data-stu-id="3f04e-233">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="3f04e-234">String</span><span class="sxs-lookup"><span data-stu-id="3f04e-234">String</span></span>|<span data-ttu-id="3f04e-235">URL-адрес изображения, которое будет экранной заставкой устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="3f04e-235">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="3f04e-236">киоскмодескринсавердисплайтимеинсекондс</span><span class="sxs-lookup"><span data-stu-id="3f04e-236">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="3f04e-237">Int32</span><span class="sxs-lookup"><span data-stu-id="3f04e-237">Int32</span></span>|<span data-ttu-id="3f04e-238">Время (в секундах), в течение которого устройство будет отображать экранную заставку в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="3f04e-238">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="3f04e-239">Допустимые значения — от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="3f04e-239">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="3f04e-240">киоскмодескринсаверстартделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="3f04e-240">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="3f04e-241">Int32</span><span class="sxs-lookup"><span data-stu-id="3f04e-241">Int32</span></span>|<span data-ttu-id="3f04e-242">Время (в секундах), в течение которого устройство должно быть неактивным, чтобы экранная заставка отображалась в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="3f04e-242">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="3f04e-243">Допустимые значения — от 1 до 9999999</span><span class="sxs-lookup"><span data-stu-id="3f04e-243">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="3f04e-244">киоскмодескринсавердетектмедиадисаблед</span><span class="sxs-lookup"><span data-stu-id="3f04e-244">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="3f04e-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-245">Boolean</span></span>|<span data-ttu-id="3f04e-246">Указывает, должно ли устройство отображать экранную заставку при воспроизведении аудио-и видеоконференций в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="3f04e-246">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="3f04e-247">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="3f04e-247">kioskModeApps</span></span>|<span data-ttu-id="3f04e-248">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="3f04e-248">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="3f04e-249">Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="3f04e-249">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="3f04e-250">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3f04e-250">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3f04e-251">киоскмодеваллпаперурл</span><span class="sxs-lookup"><span data-stu-id="3f04e-251">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="3f04e-252">String</span><span class="sxs-lookup"><span data-stu-id="3f04e-252">String</span></span>|<span data-ttu-id="3f04e-253">URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="3f04e-253">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="3f04e-254">киоскмодикситкоде</span><span class="sxs-lookup"><span data-stu-id="3f04e-254">kioskModeExitCode</span></span>|<span data-ttu-id="3f04e-255">String</span><span class="sxs-lookup"><span data-stu-id="3f04e-255">String</span></span>|<span data-ttu-id="3f04e-256">Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="3f04e-256">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="3f04e-257">киоскмодевиртуалхомебуттоненаблед</span><span class="sxs-lookup"><span data-stu-id="3f04e-257">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="3f04e-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-258">Boolean</span></span>|<span data-ttu-id="3f04e-259">Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="3f04e-259">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="3f04e-260">киоскмодевиртуалхомебуттонтипе</span><span class="sxs-lookup"><span data-stu-id="3f04e-260">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="3f04e-261">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="3f04e-261">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="3f04e-262">Указывает, является ли кнопка "Виртуальная Домашняя страница" кнопкой "Прокрутка вверх" или плавающей кнопкой "домой".</span><span class="sxs-lookup"><span data-stu-id="3f04e-262">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="3f04e-263">Возможные значения: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="3f04e-263">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="3f04e-264">киоскмодеблуетусконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="3f04e-264">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="3f04e-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-265">Boolean</span></span>|<span data-ttu-id="3f04e-266">Указывает, следует ли запретить пользователю настраивать параметры Bluetooth в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="3f04e-266">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="3f04e-267">киоскмодевификонфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="3f04e-267">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="3f04e-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-268">Boolean</span></span>|<span data-ttu-id="3f04e-269">Указывает, следует ли разрешить пользователю настраивать параметры Wi/Fi в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="3f04e-269">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="3f04e-270">киоскмодефлашлигхтконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="3f04e-270">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="3f04e-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-271">Boolean</span></span>|<span data-ttu-id="3f04e-272">Указывает, следует ли разрешить пользователю использовать флашлигхт в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="3f04e-272">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="3f04e-273">киоскмодемедиаволумеконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="3f04e-273">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="3f04e-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-274">Boolean</span></span>|<span data-ttu-id="3f04e-275">Указывает, следует ли запретить пользователю изменять громкость мультимедиа в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="3f04e-275">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="3f04e-276">микрофонефорцемуте</span><span class="sxs-lookup"><span data-stu-id="3f04e-276">microphoneForceMute</span></span>|<span data-ttu-id="3f04e-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-277">Boolean</span></span>|<span data-ttu-id="3f04e-278">Указывает, следует ли запретить разблокирование микрофона устройства.</span><span class="sxs-lookup"><span data-stu-id="3f04e-278">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="3f04e-279">нетворкескапехатчалловед</span><span class="sxs-lookup"><span data-stu-id="3f04e-279">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="3f04e-280">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-280">Boolean</span></span>|<span data-ttu-id="3f04e-281">Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="3f04e-281">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="3f04e-282">нфкблоккаутгоингбеам</span><span class="sxs-lookup"><span data-stu-id="3f04e-282">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="3f04e-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-283">Boolean</span></span>|<span data-ttu-id="3f04e-284">Указывает, следует ли заблокировать исходящую форму NFC.</span><span class="sxs-lookup"><span data-stu-id="3f04e-284">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="3f04e-285">пассвордблокккэйгуард</span><span class="sxs-lookup"><span data-stu-id="3f04e-285">passwordBlockKeyguard</span></span>|<span data-ttu-id="3f04e-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-286">Boolean</span></span>|<span data-ttu-id="3f04e-287">Указывает, отключен ли кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="3f04e-287">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="3f04e-288">пассвордблокккэйгуардфеатурес</span><span class="sxs-lookup"><span data-stu-id="3f04e-288">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="3f04e-289">Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="3f04e-289">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="3f04e-290">Список компонентов кэйгуард устройств, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="3f04e-290">List of device keyguard features to block.</span></span> <span data-ttu-id="3f04e-291">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="3f04e-291">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="3f04e-292">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="3f04e-292">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="3f04e-293">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3f04e-293">passwordExpirationDays</span></span>|<span data-ttu-id="3f04e-294">Int32</span><span class="sxs-lookup"><span data-stu-id="3f04e-294">Int32</span></span>|<span data-ttu-id="3f04e-295">Указывает время в секундах, в течение которого можно задать пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="3f04e-295">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="3f04e-296">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="3f04e-296">Valid values 1 to 365</span></span>|
|<span data-ttu-id="3f04e-297">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3f04e-297">passwordMinimumLength</span></span>|<span data-ttu-id="3f04e-298">Int32</span><span class="sxs-lookup"><span data-stu-id="3f04e-298">Int32</span></span>|<span data-ttu-id="3f04e-299">Указывает минимальную длину пароля, необходимого для устройства.</span><span class="sxs-lookup"><span data-stu-id="3f04e-299">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="3f04e-300">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="3f04e-300">Valid values 4 to 16</span></span>|
|<span data-ttu-id="3f04e-301">пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="3f04e-301">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="3f04e-302">Int32</span><span class="sxs-lookup"><span data-stu-id="3f04e-302">Int32</span></span>|<span data-ttu-id="3f04e-303">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="3f04e-303">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="3f04e-304">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="3f04e-304">Valid values 1 to 16</span></span>|
|<span data-ttu-id="3f04e-305">пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="3f04e-305">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="3f04e-306">Int32</span><span class="sxs-lookup"><span data-stu-id="3f04e-306">Int32</span></span>|<span data-ttu-id="3f04e-307">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="3f04e-307">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="3f04e-308">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="3f04e-308">Valid values 1 to 16</span></span>|
|<span data-ttu-id="3f04e-309">пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="3f04e-309">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="3f04e-310">Int32</span><span class="sxs-lookup"><span data-stu-id="3f04e-310">Int32</span></span>|<span data-ttu-id="3f04e-311">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="3f04e-311">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="3f04e-312">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="3f04e-312">Valid values 1 to 16</span></span>|
|<span data-ttu-id="3f04e-313">пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="3f04e-313">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="3f04e-314">Int32</span><span class="sxs-lookup"><span data-stu-id="3f04e-314">Int32</span></span>|<span data-ttu-id="3f04e-315">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="3f04e-315">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="3f04e-316">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="3f04e-316">Valid values 1 to 16</span></span>|
|<span data-ttu-id="3f04e-317">пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="3f04e-317">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="3f04e-318">Int32</span><span class="sxs-lookup"><span data-stu-id="3f04e-318">Int32</span></span>|<span data-ttu-id="3f04e-319">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="3f04e-319">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="3f04e-320">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="3f04e-320">Valid values 1 to 16</span></span>|
|<span data-ttu-id="3f04e-321">пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="3f04e-321">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="3f04e-322">Int32</span><span class="sxs-lookup"><span data-stu-id="3f04e-322">Int32</span></span>|<span data-ttu-id="3f04e-323">Указывает минимальное число символов верхнего каселеттер, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="3f04e-323">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="3f04e-324">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="3f04e-324">Valid values 1 to 16</span></span>|
|<span data-ttu-id="3f04e-325">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="3f04e-325">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="3f04e-326">Int32</span><span class="sxs-lookup"><span data-stu-id="3f04e-326">Int32</span></span>|<span data-ttu-id="3f04e-327">Миллисекунды бездействия до истечения времени ожидания экрана.</span><span class="sxs-lookup"><span data-stu-id="3f04e-327">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="3f04e-328">пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="3f04e-328">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="3f04e-329">Int32</span><span class="sxs-lookup"><span data-stu-id="3f04e-329">Int32</span></span>|<span data-ttu-id="3f04e-330">Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале.</span><span class="sxs-lookup"><span data-stu-id="3f04e-330">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="3f04e-331">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="3f04e-331">Valid values 0 to 24</span></span>|
|<span data-ttu-id="3f04e-332">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3f04e-332">passwordRequiredType</span></span>|[<span data-ttu-id="3f04e-333">андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="3f04e-333">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="3f04e-334">Указывает минимальное качество пароля, необходимое для устройства.</span><span class="sxs-lookup"><span data-stu-id="3f04e-334">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="3f04e-335">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="3f04e-335">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="3f04e-336">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="3f04e-336">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="3f04e-337">Int32</span><span class="sxs-lookup"><span data-stu-id="3f04e-337">Int32</span></span>|<span data-ttu-id="3f04e-338">Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="3f04e-338">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="3f04e-339">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="3f04e-339">Valid values 4 to 11</span></span>|
|<span data-ttu-id="3f04e-340">плайсторемоде</span><span class="sxs-lookup"><span data-stu-id="3f04e-340">playStoreMode</span></span>|[<span data-ttu-id="3f04e-341">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="3f04e-341">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="3f04e-342">Указывает режим проигрывания устройства в хранилище.</span><span class="sxs-lookup"><span data-stu-id="3f04e-342">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="3f04e-343">Возможные значения: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="3f04e-343">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="3f04e-344">сафебутблоккед</span><span class="sxs-lookup"><span data-stu-id="3f04e-344">safeBootBlocked</span></span>|<span data-ttu-id="3f04e-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-345">Boolean</span></span>|<span data-ttu-id="3f04e-346">Указывает, отключена ли загрузка устройства в "безопасная загрузка".</span><span class="sxs-lookup"><span data-stu-id="3f04e-346">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="3f04e-347">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="3f04e-347">screenCaptureBlocked</span></span>|<span data-ttu-id="3f04e-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-348">Boolean</span></span>|<span data-ttu-id="3f04e-349">Указывает, следует ли отключить возможность использования снимков экрана.</span><span class="sxs-lookup"><span data-stu-id="3f04e-349">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="3f04e-350">секуритялловдебуггингфеатурес</span><span class="sxs-lookup"><span data-stu-id="3f04e-350">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="3f04e-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-351">Boolean</span></span>|<span data-ttu-id="3f04e-352">Указывает, следует ли запретить пользователю включать функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="3f04e-352">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="3f04e-353">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="3f04e-353">securityRequireVerifyApps</span></span>|<span data-ttu-id="3f04e-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-354">Boolean</span></span>|<span data-ttu-id="3f04e-355">Указывает, требуется ли проверка приложений.</span><span class="sxs-lookup"><span data-stu-id="3f04e-355">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="3f04e-356">статусбарблоккед</span><span class="sxs-lookup"><span data-stu-id="3f04e-356">statusBarBlocked</span></span>|<span data-ttu-id="3f04e-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-357">Boolean</span></span>|<span data-ttu-id="3f04e-358">Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.</span><span class="sxs-lookup"><span data-stu-id="3f04e-358">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="3f04e-359">стайонмодес</span><span class="sxs-lookup"><span data-stu-id="3f04e-359">stayOnModes</span></span>|<span data-ttu-id="3f04e-360">Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="3f04e-360">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="3f04e-361">Список режимов, в которых дисплей устройства остается включенным.</span><span class="sxs-lookup"><span data-stu-id="3f04e-361">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="3f04e-362">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="3f04e-362">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="3f04e-363">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="3f04e-363">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="3f04e-364">сторажеалловусб</span><span class="sxs-lookup"><span data-stu-id="3f04e-364">storageAllowUsb</span></span>|<span data-ttu-id="3f04e-365">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-365">Boolean</span></span>|<span data-ttu-id="3f04e-366">Указывает, следует ли разрешить запоминающее устройство USB.</span><span class="sxs-lookup"><span data-stu-id="3f04e-366">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="3f04e-367">сторажеблоккекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="3f04e-367">storageBlockExternalMedia</span></span>|<span data-ttu-id="3f04e-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-368">Boolean</span></span>|<span data-ttu-id="3f04e-369">Указывает, следует ли заблокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="3f04e-369">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="3f04e-370">сторажеблоккусбфилетрансфер</span><span class="sxs-lookup"><span data-stu-id="3f04e-370">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="3f04e-371">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-371">Boolean</span></span>|<span data-ttu-id="3f04e-372">Указывает, следует ли запретить передачу файлов через USB.</span><span class="sxs-lookup"><span data-stu-id="3f04e-372">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="3f04e-373">системупдатевиндовстартминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="3f04e-373">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="3f04e-374">Int32</span><span class="sxs-lookup"><span data-stu-id="3f04e-374">Int32</span></span>|<span data-ttu-id="3f04e-375">Указывает количество минут после полуночи, когда запустится окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="3f04e-375">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="3f04e-376">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="3f04e-376">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="3f04e-377">системупдатевиндовендминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="3f04e-377">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="3f04e-378">Int32</span><span class="sxs-lookup"><span data-stu-id="3f04e-378">Int32</span></span>|<span data-ttu-id="3f04e-379">Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="3f04e-379">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="3f04e-380">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="3f04e-380">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="3f04e-381">системупдатеинсталлтипе</span><span class="sxs-lookup"><span data-stu-id="3f04e-381">systemUpdateInstallType</span></span>|[<span data-ttu-id="3f04e-382">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="3f04e-382">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="3f04e-383">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="3f04e-383">The type of system update configuration.</span></span> <span data-ttu-id="3f04e-384">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="3f04e-384">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="3f04e-385">системвиндовсблоккед</span><span class="sxs-lookup"><span data-stu-id="3f04e-385">systemWindowsBlocked</span></span>|<span data-ttu-id="3f04e-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-386">Boolean</span></span>|<span data-ttu-id="3f04e-387">Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="3f04e-387">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="3f04e-388">усерсблоккадд</span><span class="sxs-lookup"><span data-stu-id="3f04e-388">usersBlockAdd</span></span>|<span data-ttu-id="3f04e-389">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-389">Boolean</span></span>|<span data-ttu-id="3f04e-390">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="3f04e-390">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="3f04e-391">усерсблоккремове</span><span class="sxs-lookup"><span data-stu-id="3f04e-391">usersBlockRemove</span></span>|<span data-ttu-id="3f04e-392">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-392">Boolean</span></span>|<span data-ttu-id="3f04e-393">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="3f04e-393">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="3f04e-394">волумеблоккаджустмент</span><span class="sxs-lookup"><span data-stu-id="3f04e-394">volumeBlockAdjustment</span></span>|<span data-ttu-id="3f04e-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-395">Boolean</span></span>|<span data-ttu-id="3f04e-396">Указывает, отключена ли настройка главного тома.</span><span class="sxs-lookup"><span data-stu-id="3f04e-396">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="3f04e-397">впналвайсонлоккдовнмоде</span><span class="sxs-lookup"><span data-stu-id="3f04e-397">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="3f04e-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-398">Boolean</span></span>|<span data-ttu-id="3f04e-399">Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="3f04e-399">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="3f04e-400">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="3f04e-400">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="3f04e-401">String</span><span class="sxs-lookup"><span data-stu-id="3f04e-401">String</span></span>|<span data-ttu-id="3f04e-402">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="3f04e-402">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="3f04e-403">вифиблоккедитконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="3f04e-403">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="3f04e-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-404">Boolean</span></span>|<span data-ttu-id="3f04e-405">Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="3f04e-405">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="3f04e-406">вифиблоккедитполицидефинедконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="3f04e-406">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="3f04e-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f04e-407">Boolean</span></span>|<span data-ttu-id="3f04e-408">Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="3f04e-408">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="3f04e-409">Ответ</span><span class="sxs-lookup"><span data-stu-id="3f04e-409">Response</span></span>
<span data-ttu-id="3f04e-410">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3f04e-410">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f04e-411">Пример</span><span class="sxs-lookup"><span data-stu-id="3f04e-411">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f04e-412">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f04e-412">Request</span></span>
<span data-ttu-id="3f04e-413">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f04e-413">Here is an example of the request.</span></span>
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
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="3f04e-414">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f04e-414">Response</span></span>
<span data-ttu-id="3f04e-p136">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3f04e-p136">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```



