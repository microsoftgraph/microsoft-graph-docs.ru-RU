---
title: Создание androidDeviceOwnerGeneralDeviceConfiguration
description: Создание нового объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 353fca8ebede19287151369fc2cbe59c74670e4f
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534829"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="8e1ac-103">Создание androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8e1ac-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="8e1ac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e1ac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e1ac-106">Создание нового объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8e1ac-106">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e1ac-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8e1ac-107">Prerequisites</span></span>
<span data-ttu-id="8e1ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e1ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e1ac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e1ac-110">Permission type</span></span>|<span data-ttu-id="8e1ac-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e1ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e1ac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e1ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8e1ac-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e1ac-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e1ac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e1ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e1ac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-115">Not supported.</span></span>|
|<span data-ttu-id="8e1ac-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8e1ac-116">Application</span></span>|<span data-ttu-id="8e1ac-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e1ac-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e1ac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e1ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8e1ac-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e1ac-119">Request headers</span></span>
|<span data-ttu-id="8e1ac-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e1ac-120">Header</span></span>|<span data-ttu-id="8e1ac-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8e1ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e1ac-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e1ac-122">Authorization</span></span>|<span data-ttu-id="8e1ac-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e1ac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8e1ac-124">Accept</span></span>|<span data-ttu-id="8e1ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8e1ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e1ac-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e1ac-126">Request body</span></span>
<span data-ttu-id="8e1ac-127">В тексте запроса добавьте представление объекта androidDeviceOwnerGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-127">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="8e1ac-128">В следующей таблице приведены свойства, необходимые при создании androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-128">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="8e1ac-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e1ac-129">Property</span></span>|<span data-ttu-id="8e1ac-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8e1ac-130">Type</span></span>|<span data-ttu-id="8e1ac-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8e1ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e1ac-132">id</span><span class="sxs-lookup"><span data-stu-id="8e1ac-132">id</span></span>|<span data-ttu-id="8e1ac-133">String</span><span class="sxs-lookup"><span data-stu-id="8e1ac-133">String</span></span>|<span data-ttu-id="8e1ac-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-134">Key of the entity.</span></span> <span data-ttu-id="8e1ac-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e1ac-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e1ac-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e1ac-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8e1ac-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e1ac-137">DateTimeOffset</span></span>|<span data-ttu-id="8e1ac-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8e1ac-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e1ac-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e1ac-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8e1ac-140">roleScopeTagIds</span></span>|<span data-ttu-id="8e1ac-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8e1ac-141">String collection</span></span>|<span data-ttu-id="8e1ac-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8e1ac-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e1ac-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e1ac-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="8e1ac-144">supportsScopeTags</span></span>|<span data-ttu-id="8e1ac-145">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-145">Boolean</span></span>|<span data-ttu-id="8e1ac-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8e1ac-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8e1ac-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8e1ac-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-149">This property is read-only.</span></span> <span data-ttu-id="8e1ac-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e1ac-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e1ac-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8e1ac-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8e1ac-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8e1ac-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8e1ac-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8e1ac-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e1ac-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e1ac-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8e1ac-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8e1ac-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8e1ac-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8e1ac-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8e1ac-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e1ac-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e1ac-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8e1ac-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8e1ac-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8e1ac-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8e1ac-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8e1ac-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e1ac-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e1ac-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e1ac-163">createdDateTime</span></span>|<span data-ttu-id="8e1ac-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e1ac-164">DateTimeOffset</span></span>|<span data-ttu-id="8e1ac-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-165">DateTime the object was created.</span></span> <span data-ttu-id="8e1ac-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e1ac-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e1ac-167">description</span><span class="sxs-lookup"><span data-stu-id="8e1ac-167">description</span></span>|<span data-ttu-id="8e1ac-168">String</span><span class="sxs-lookup"><span data-stu-id="8e1ac-168">String</span></span>|<span data-ttu-id="8e1ac-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8e1ac-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e1ac-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e1ac-171">displayName</span><span class="sxs-lookup"><span data-stu-id="8e1ac-171">displayName</span></span>|<span data-ttu-id="8e1ac-172">Строка</span><span class="sxs-lookup"><span data-stu-id="8e1ac-172">String</span></span>|<span data-ttu-id="8e1ac-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8e1ac-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e1ac-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e1ac-175">version</span><span class="sxs-lookup"><span data-stu-id="8e1ac-175">version</span></span>|<span data-ttu-id="8e1ac-176">Int32</span><span class="sxs-lookup"><span data-stu-id="8e1ac-176">Int32</span></span>|<span data-ttu-id="8e1ac-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-177">Version of the device configuration.</span></span> <span data-ttu-id="8e1ac-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e1ac-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e1ac-179">аккаунтсблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="8e1ac-179">accountsBlockModification</span></span>|<span data-ttu-id="8e1ac-180">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-180">Boolean</span></span>|<span data-ttu-id="8e1ac-181">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-181">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="8e1ac-182">аппсалловинсталлфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="8e1ac-182">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="8e1ac-183">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-183">Boolean</span></span>|<span data-ttu-id="8e1ac-184">Указывает, может ли пользователь включить параметр "неизвестные источники".</span><span class="sxs-lookup"><span data-stu-id="8e1ac-184">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="8e1ac-185">аппсаутаупдатеполици</span><span class="sxs-lookup"><span data-stu-id="8e1ac-185">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="8e1ac-186">андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="8e1ac-186">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="8e1ac-187">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-187">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="8e1ac-188">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-188">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="8e1ac-189">аппсдефаултпермиссионполици</span><span class="sxs-lookup"><span data-stu-id="8e1ac-189">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="8e1ac-190">андроиддевицеовнердефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="8e1ac-190">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="8e1ac-191">Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-191">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="8e1ac-192">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-192">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="8e1ac-193">аппсрекоммендскиппингфирстусехинтс</span><span class="sxs-lookup"><span data-stu-id="8e1ac-193">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="8e1ac-194">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-194">Boolean</span></span>|<span data-ttu-id="8e1ac-195">Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-195">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="8e1ac-196">блуетусблоккконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8e1ac-196">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="8e1ac-197">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-197">Boolean</span></span>|<span data-ttu-id="8e1ac-198">Указывает, следует ли запретить пользователю настраивать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-198">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="8e1ac-199">блуетусблоккконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="8e1ac-199">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="8e1ac-200">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-200">Boolean</span></span>|<span data-ttu-id="8e1ac-201">Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-201">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="8e1ac-202">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="8e1ac-202">cameraBlocked</span></span>|<span data-ttu-id="8e1ac-203">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-203">Boolean</span></span>|<span data-ttu-id="8e1ac-204">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-204">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="8e1ac-205">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="8e1ac-205">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="8e1ac-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e1ac-206">Boolean</span></span>|<span data-ttu-id="8e1ac-207">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-207">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="8e1ac-208">датароамингблоккед</span><span class="sxs-lookup"><span data-stu-id="8e1ac-208">dataRoamingBlocked</span></span>|<span data-ttu-id="8e1ac-209">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-209">Boolean</span></span>|<span data-ttu-id="8e1ac-210">Указывает, следует ли запретить пользователю перемещать данные.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-210">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="8e1ac-211">датетимеконфигуратионблоккед</span><span class="sxs-lookup"><span data-stu-id="8e1ac-211">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="8e1ac-212">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-212">Boolean</span></span>|<span data-ttu-id="8e1ac-213">Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-213">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="8e1ac-214">факториресетдевицеадминистраторемаилс</span><span class="sxs-lookup"><span data-stu-id="8e1ac-214">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="8e1ac-215">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8e1ac-215">String collection</span></span>|<span data-ttu-id="8e1ac-216">Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-216">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="8e1ac-217">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="8e1ac-217">factoryResetBlocked</span></span>|<span data-ttu-id="8e1ac-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e1ac-218">Boolean</span></span>|<span data-ttu-id="8e1ac-219">Указывает, отключен ли параметр Reset фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-219">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="8e1ac-220">глобалпрокси</span><span class="sxs-lookup"><span data-stu-id="8e1ac-220">globalProxy</span></span>|[<span data-ttu-id="8e1ac-221">андроиддевицеовнерглобалпрокси</span><span class="sxs-lookup"><span data-stu-id="8e1ac-221">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="8e1ac-222">Прокси-сервер настраивается напрямую с узлом, портом и исключенными узлами.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-222">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="8e1ac-223">киоскмодескринсаверконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="8e1ac-223">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="8e1ac-224">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-224">Boolean</span></span>|<span data-ttu-id="8e1ac-225">Указывает, следует ли включить режим экранной заставки или не в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-225">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="8e1ac-226">киоскмодескринсаверимажеурл</span><span class="sxs-lookup"><span data-stu-id="8e1ac-226">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="8e1ac-227">String</span><span class="sxs-lookup"><span data-stu-id="8e1ac-227">String</span></span>|<span data-ttu-id="8e1ac-228">URL-адрес изображения, которое будет экранной заставкой устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-228">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="8e1ac-229">киоскмодескринсавердисплайтимеинсекондс</span><span class="sxs-lookup"><span data-stu-id="8e1ac-229">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="8e1ac-230">Int32</span><span class="sxs-lookup"><span data-stu-id="8e1ac-230">Int32</span></span>|<span data-ttu-id="8e1ac-231">Время (в секундах), в течение которого устройство будет отображать экранную заставку в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-231">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="8e1ac-232">Допустимые значения — от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="8e1ac-232">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="8e1ac-233">киоскмодескринсаверстартделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="8e1ac-233">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="8e1ac-234">Int32</span><span class="sxs-lookup"><span data-stu-id="8e1ac-234">Int32</span></span>|<span data-ttu-id="8e1ac-235">Время (в секундах), в течение которого устройство должно быть неактивным, чтобы экранная заставка отображалась в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-235">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="8e1ac-236">Допустимые значения — от 1 до 9999999</span><span class="sxs-lookup"><span data-stu-id="8e1ac-236">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="8e1ac-237">киоскмодескринсавердетектмедиадисаблед</span><span class="sxs-lookup"><span data-stu-id="8e1ac-237">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="8e1ac-238">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-238">Boolean</span></span>|<span data-ttu-id="8e1ac-239">Указывает, должно ли устройство отображать экранную заставку при воспроизведении аудио-и видеоконференций в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-239">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="8e1ac-240">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="8e1ac-240">kioskModeApps</span></span>|<span data-ttu-id="8e1ac-241">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="8e1ac-241">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="8e1ac-242">Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-242">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="8e1ac-243">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-243">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8e1ac-244">киоскмодеваллпаперурл</span><span class="sxs-lookup"><span data-stu-id="8e1ac-244">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="8e1ac-245">String</span><span class="sxs-lookup"><span data-stu-id="8e1ac-245">String</span></span>|<span data-ttu-id="8e1ac-246">URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-246">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="8e1ac-247">киоскмодикситкоде</span><span class="sxs-lookup"><span data-stu-id="8e1ac-247">kioskModeExitCode</span></span>|<span data-ttu-id="8e1ac-248">String</span><span class="sxs-lookup"><span data-stu-id="8e1ac-248">String</span></span>|<span data-ttu-id="8e1ac-249">Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-249">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="8e1ac-250">киоскмодевиртуалхомебуттоненаблед</span><span class="sxs-lookup"><span data-stu-id="8e1ac-250">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="8e1ac-251">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-251">Boolean</span></span>|<span data-ttu-id="8e1ac-252">Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-252">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="8e1ac-253">киоскмодевиртуалхомебуттонтипе</span><span class="sxs-lookup"><span data-stu-id="8e1ac-253">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="8e1ac-254">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="8e1ac-254">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="8e1ac-255">Указывает, является ли кнопка "Виртуальная Домашняя страница" кнопкой "Прокрутка вверх" или плавающей кнопкой "домой".</span><span class="sxs-lookup"><span data-stu-id="8e1ac-255">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="8e1ac-256">Возможные значения: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-256">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="8e1ac-257">киоскмодеблуетусконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="8e1ac-257">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="8e1ac-258">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-258">Boolean</span></span>|<span data-ttu-id="8e1ac-259">Указывает, следует ли запретить пользователю настраивать параметры Bluetooth в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-259">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="8e1ac-260">киоскмодевификонфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="8e1ac-260">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="8e1ac-261">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-261">Boolean</span></span>|<span data-ttu-id="8e1ac-262">Указывает, следует ли разрешить пользователю настраивать параметры Wi/Fi в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-262">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="8e1ac-263">киоскмодефлашлигхтконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="8e1ac-263">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="8e1ac-264">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-264">Boolean</span></span>|<span data-ttu-id="8e1ac-265">Указывает, следует ли разрешить пользователю использовать флашлигхт в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-265">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="8e1ac-266">киоскмодемедиаволумеконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="8e1ac-266">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="8e1ac-267">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-267">Boolean</span></span>|<span data-ttu-id="8e1ac-268">Указывает, следует ли запретить пользователю изменять громкость мультимедиа в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-268">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="8e1ac-269">микрофонефорцемуте</span><span class="sxs-lookup"><span data-stu-id="8e1ac-269">microphoneForceMute</span></span>|<span data-ttu-id="8e1ac-270">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-270">Boolean</span></span>|<span data-ttu-id="8e1ac-271">Указывает, следует ли запретить разблокирование микрофона устройства.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-271">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="8e1ac-272">нетворкескапехатчалловед</span><span class="sxs-lookup"><span data-stu-id="8e1ac-272">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="8e1ac-273">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-273">Boolean</span></span>|<span data-ttu-id="8e1ac-274">Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-274">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="8e1ac-275">нфкблоккаутгоингбеам</span><span class="sxs-lookup"><span data-stu-id="8e1ac-275">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="8e1ac-276">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-276">Boolean</span></span>|<span data-ttu-id="8e1ac-277">Указывает, следует ли заблокировать исходящую форму NFC.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-277">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="8e1ac-278">пассвордблокккэйгуард</span><span class="sxs-lookup"><span data-stu-id="8e1ac-278">passwordBlockKeyguard</span></span>|<span data-ttu-id="8e1ac-279">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-279">Boolean</span></span>|<span data-ttu-id="8e1ac-280">Указывает, отключен ли кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-280">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="8e1ac-281">пассвордблокккэйгуардфеатурес</span><span class="sxs-lookup"><span data-stu-id="8e1ac-281">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="8e1ac-282">Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="8e1ac-282">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="8e1ac-283">Список компонентов кэйгуард устройств, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-283">List of device keyguard features to block.</span></span> <span data-ttu-id="8e1ac-284">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-284">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="8e1ac-285">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-285">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="8e1ac-286">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8e1ac-286">passwordExpirationDays</span></span>|<span data-ttu-id="8e1ac-287">Int32</span><span class="sxs-lookup"><span data-stu-id="8e1ac-287">Int32</span></span>|<span data-ttu-id="8e1ac-288">Указывает время в секундах, в течение которого можно задать пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-288">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="8e1ac-289">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-289">Valid values 1 to 365</span></span>|
|<span data-ttu-id="8e1ac-290">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8e1ac-290">passwordMinimumLength</span></span>|<span data-ttu-id="8e1ac-291">Int32</span><span class="sxs-lookup"><span data-stu-id="8e1ac-291">Int32</span></span>|<span data-ttu-id="8e1ac-292">Указывает минимальную длину пароля, необходимого для устройства.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-292">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="8e1ac-293">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-293">Valid values 4 to 16</span></span>|
|<span data-ttu-id="8e1ac-294">пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="8e1ac-294">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="8e1ac-295">Int32</span><span class="sxs-lookup"><span data-stu-id="8e1ac-295">Int32</span></span>|<span data-ttu-id="8e1ac-296">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-296">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="8e1ac-297">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-297">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8e1ac-298">пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="8e1ac-298">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="8e1ac-299">Int32</span><span class="sxs-lookup"><span data-stu-id="8e1ac-299">Int32</span></span>|<span data-ttu-id="8e1ac-300">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-300">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="8e1ac-301">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-301">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8e1ac-302">пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="8e1ac-302">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="8e1ac-303">Int32</span><span class="sxs-lookup"><span data-stu-id="8e1ac-303">Int32</span></span>|<span data-ttu-id="8e1ac-304">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-304">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="8e1ac-305">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-305">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8e1ac-306">пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="8e1ac-306">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="8e1ac-307">Int32</span><span class="sxs-lookup"><span data-stu-id="8e1ac-307">Int32</span></span>|<span data-ttu-id="8e1ac-308">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-308">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="8e1ac-309">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-309">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8e1ac-310">пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="8e1ac-310">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="8e1ac-311">Int32</span><span class="sxs-lookup"><span data-stu-id="8e1ac-311">Int32</span></span>|<span data-ttu-id="8e1ac-312">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-312">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="8e1ac-313">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-313">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8e1ac-314">пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="8e1ac-314">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="8e1ac-315">Int32</span><span class="sxs-lookup"><span data-stu-id="8e1ac-315">Int32</span></span>|<span data-ttu-id="8e1ac-316">Указывает минимальное число символов верхнего каселеттер, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-316">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="8e1ac-317">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-317">Valid values 1 to 16</span></span>|
|<span data-ttu-id="8e1ac-318">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="8e1ac-318">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="8e1ac-319">Int32</span><span class="sxs-lookup"><span data-stu-id="8e1ac-319">Int32</span></span>|<span data-ttu-id="8e1ac-320">Миллисекунды бездействия до истечения времени ожидания экрана.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-320">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="8e1ac-321">пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="8e1ac-321">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="8e1ac-322">Int32</span><span class="sxs-lookup"><span data-stu-id="8e1ac-322">Int32</span></span>|<span data-ttu-id="8e1ac-323">Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-323">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="8e1ac-324">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-324">Valid values 0 to 24</span></span>|
|<span data-ttu-id="8e1ac-325">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8e1ac-325">passwordRequiredType</span></span>|[<span data-ttu-id="8e1ac-326">андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="8e1ac-326">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="8e1ac-327">Указывает минимальное качество пароля, необходимое для устройства.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-327">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="8e1ac-328">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-328">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="8e1ac-329">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="8e1ac-329">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="8e1ac-330">Int32</span><span class="sxs-lookup"><span data-stu-id="8e1ac-330">Int32</span></span>|<span data-ttu-id="8e1ac-331">Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-331">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="8e1ac-332">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-332">Valid values 4 to 11</span></span>|
|<span data-ttu-id="8e1ac-333">плайсторемоде</span><span class="sxs-lookup"><span data-stu-id="8e1ac-333">playStoreMode</span></span>|[<span data-ttu-id="8e1ac-334">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="8e1ac-334">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="8e1ac-335">Указывает режим проигрывания устройства в хранилище.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-335">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="8e1ac-336">Возможные значения: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-336">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="8e1ac-337">сафебутблоккед</span><span class="sxs-lookup"><span data-stu-id="8e1ac-337">safeBootBlocked</span></span>|<span data-ttu-id="8e1ac-338">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-338">Boolean</span></span>|<span data-ttu-id="8e1ac-339">Указывает, отключена ли загрузка устройства в "безопасная загрузка".</span><span class="sxs-lookup"><span data-stu-id="8e1ac-339">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="8e1ac-340">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="8e1ac-340">screenCaptureBlocked</span></span>|<span data-ttu-id="8e1ac-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e1ac-341">Boolean</span></span>|<span data-ttu-id="8e1ac-342">Указывает, следует ли отключить возможность использования снимков экрана.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-342">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="8e1ac-343">секуритялловдебуггингфеатурес</span><span class="sxs-lookup"><span data-stu-id="8e1ac-343">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="8e1ac-344">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-344">Boolean</span></span>|<span data-ttu-id="8e1ac-345">Указывает, следует ли запретить пользователю включать функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-345">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="8e1ac-346">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="8e1ac-346">securityRequireVerifyApps</span></span>|<span data-ttu-id="8e1ac-347">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-347">Boolean</span></span>|<span data-ttu-id="8e1ac-348">Указывает, требуется ли проверка приложений.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-348">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="8e1ac-349">статусбарблоккед</span><span class="sxs-lookup"><span data-stu-id="8e1ac-349">statusBarBlocked</span></span>|<span data-ttu-id="8e1ac-350">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-350">Boolean</span></span>|<span data-ttu-id="8e1ac-351">Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-351">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="8e1ac-352">стайонмодес</span><span class="sxs-lookup"><span data-stu-id="8e1ac-352">stayOnModes</span></span>|<span data-ttu-id="8e1ac-353">Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="8e1ac-353">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="8e1ac-354">Список режимов, в которых дисплей устройства остается включенным.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-354">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="8e1ac-355">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-355">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="8e1ac-356">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-356">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="8e1ac-357">сторажеалловусб</span><span class="sxs-lookup"><span data-stu-id="8e1ac-357">storageAllowUsb</span></span>|<span data-ttu-id="8e1ac-358">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-358">Boolean</span></span>|<span data-ttu-id="8e1ac-359">Указывает, следует ли разрешить запоминающее устройство USB.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-359">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="8e1ac-360">сторажеблоккекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="8e1ac-360">storageBlockExternalMedia</span></span>|<span data-ttu-id="8e1ac-361">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-361">Boolean</span></span>|<span data-ttu-id="8e1ac-362">Указывает, следует ли заблокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-362">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="8e1ac-363">сторажеблоккусбфилетрансфер</span><span class="sxs-lookup"><span data-stu-id="8e1ac-363">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="8e1ac-364">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-364">Boolean</span></span>|<span data-ttu-id="8e1ac-365">Указывает, следует ли запретить передачу файлов через USB.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-365">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="8e1ac-366">системупдатевиндовстартминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="8e1ac-366">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="8e1ac-367">Int32</span><span class="sxs-lookup"><span data-stu-id="8e1ac-367">Int32</span></span>|<span data-ttu-id="8e1ac-368">Указывает количество минут после полуночи, когда запустится окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-368">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="8e1ac-369">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="8e1ac-369">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="8e1ac-370">системупдатевиндовендминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="8e1ac-370">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="8e1ac-371">Int32</span><span class="sxs-lookup"><span data-stu-id="8e1ac-371">Int32</span></span>|<span data-ttu-id="8e1ac-372">Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-372">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="8e1ac-373">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="8e1ac-373">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="8e1ac-374">системупдатеинсталлтипе</span><span class="sxs-lookup"><span data-stu-id="8e1ac-374">systemUpdateInstallType</span></span>|[<span data-ttu-id="8e1ac-375">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="8e1ac-375">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="8e1ac-376">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-376">The type of system update configuration.</span></span> <span data-ttu-id="8e1ac-377">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-377">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="8e1ac-378">системвиндовсблоккед</span><span class="sxs-lookup"><span data-stu-id="8e1ac-378">systemWindowsBlocked</span></span>|<span data-ttu-id="8e1ac-379">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-379">Boolean</span></span>|<span data-ttu-id="8e1ac-380">Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-380">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="8e1ac-381">усерсблоккадд</span><span class="sxs-lookup"><span data-stu-id="8e1ac-381">usersBlockAdd</span></span>|<span data-ttu-id="8e1ac-382">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-382">Boolean</span></span>|<span data-ttu-id="8e1ac-383">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-383">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="8e1ac-384">усерсблоккремове</span><span class="sxs-lookup"><span data-stu-id="8e1ac-384">usersBlockRemove</span></span>|<span data-ttu-id="8e1ac-385">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-385">Boolean</span></span>|<span data-ttu-id="8e1ac-386">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-386">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="8e1ac-387">волумеблоккаджустмент</span><span class="sxs-lookup"><span data-stu-id="8e1ac-387">volumeBlockAdjustment</span></span>|<span data-ttu-id="8e1ac-388">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-388">Boolean</span></span>|<span data-ttu-id="8e1ac-389">Указывает, отключена ли настройка главного тома.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-389">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="8e1ac-390">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="8e1ac-390">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="8e1ac-391">String</span><span class="sxs-lookup"><span data-stu-id="8e1ac-391">String</span></span>|<span data-ttu-id="8e1ac-392">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-392">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="8e1ac-393">впналвайсонлоккдовнмоде</span><span class="sxs-lookup"><span data-stu-id="8e1ac-393">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="8e1ac-394">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-394">Boolean</span></span>|<span data-ttu-id="8e1ac-395">Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-395">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="8e1ac-396">вифиблоккедитконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="8e1ac-396">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="8e1ac-397">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-397">Boolean</span></span>|<span data-ttu-id="8e1ac-398">Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-398">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="8e1ac-399">вифиблоккедитполицидефинедконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="8e1ac-399">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="8e1ac-400">Логический</span><span class="sxs-lookup"><span data-stu-id="8e1ac-400">Boolean</span></span>|<span data-ttu-id="8e1ac-401">Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-401">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="8e1ac-402">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e1ac-402">Response</span></span>
<span data-ttu-id="8e1ac-403">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-403">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e1ac-404">Пример</span><span class="sxs-lookup"><span data-stu-id="8e1ac-404">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e1ac-405">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e1ac-405">Request</span></span>
<span data-ttu-id="8e1ac-406">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-406">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4285

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

### <a name="response"></a><span data-ttu-id="8e1ac-407">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e1ac-407">Response</span></span>
<span data-ttu-id="8e1ac-p136">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e1ac-p136">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4457

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






