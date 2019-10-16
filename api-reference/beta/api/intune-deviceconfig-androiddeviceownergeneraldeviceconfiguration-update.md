---
title: Обновление androidDeviceOwnerGeneralDeviceConfiguration
description: Обновление свойств объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 431a2809b72e780c379a7dbcc7b678a5a4a4b78d
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534808"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="70c26-103">Обновление androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="70c26-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="70c26-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70c26-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70c26-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70c26-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70c26-106">Обновление свойств объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="70c26-106">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70c26-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="70c26-107">Prerequisites</span></span>
<span data-ttu-id="70c26-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70c26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70c26-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70c26-110">Permission type</span></span>|<span data-ttu-id="70c26-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="70c26-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70c26-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70c26-112">Delegated (work or school account)</span></span>|<span data-ttu-id="70c26-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70c26-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="70c26-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70c26-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70c26-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70c26-115">Not supported.</span></span>|
|<span data-ttu-id="70c26-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="70c26-116">Application</span></span>|<span data-ttu-id="70c26-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70c26-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="70c26-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70c26-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="70c26-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70c26-119">Request headers</span></span>
|<span data-ttu-id="70c26-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70c26-120">Header</span></span>|<span data-ttu-id="70c26-121">Значение</span><span class="sxs-lookup"><span data-stu-id="70c26-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70c26-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70c26-122">Authorization</span></span>|<span data-ttu-id="70c26-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70c26-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70c26-124">Accept</span><span class="sxs-lookup"><span data-stu-id="70c26-124">Accept</span></span>|<span data-ttu-id="70c26-125">application/json</span><span class="sxs-lookup"><span data-stu-id="70c26-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70c26-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70c26-126">Request body</span></span>
<span data-ttu-id="70c26-127">В тексте запроса добавьте представление объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70c26-127">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="70c26-128">В следующей таблице приведены свойства, необходимые при создании [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70c26-128">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="70c26-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="70c26-129">Property</span></span>|<span data-ttu-id="70c26-130">Тип</span><span class="sxs-lookup"><span data-stu-id="70c26-130">Type</span></span>|<span data-ttu-id="70c26-131">Описание</span><span class="sxs-lookup"><span data-stu-id="70c26-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70c26-132">id</span><span class="sxs-lookup"><span data-stu-id="70c26-132">id</span></span>|<span data-ttu-id="70c26-133">String</span><span class="sxs-lookup"><span data-stu-id="70c26-133">String</span></span>|<span data-ttu-id="70c26-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="70c26-134">Key of the entity.</span></span> <span data-ttu-id="70c26-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70c26-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70c26-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70c26-136">lastModifiedDateTime</span></span>|<span data-ttu-id="70c26-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70c26-137">DateTimeOffset</span></span>|<span data-ttu-id="70c26-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="70c26-138">DateTime the object was last modified.</span></span> <span data-ttu-id="70c26-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70c26-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70c26-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="70c26-140">roleScopeTagIds</span></span>|<span data-ttu-id="70c26-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="70c26-141">String collection</span></span>|<span data-ttu-id="70c26-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="70c26-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="70c26-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70c26-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70c26-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="70c26-144">supportsScopeTags</span></span>|<span data-ttu-id="70c26-145">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-145">Boolean</span></span>|<span data-ttu-id="70c26-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="70c26-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="70c26-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="70c26-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="70c26-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="70c26-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="70c26-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="70c26-149">This property is read-only.</span></span> <span data-ttu-id="70c26-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70c26-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70c26-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="70c26-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="70c26-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="70c26-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="70c26-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="70c26-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="70c26-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70c26-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70c26-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="70c26-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="70c26-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="70c26-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="70c26-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="70c26-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="70c26-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70c26-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70c26-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="70c26-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="70c26-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="70c26-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="70c26-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="70c26-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="70c26-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70c26-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70c26-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70c26-163">createdDateTime</span></span>|<span data-ttu-id="70c26-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70c26-164">DateTimeOffset</span></span>|<span data-ttu-id="70c26-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="70c26-165">DateTime the object was created.</span></span> <span data-ttu-id="70c26-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70c26-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70c26-167">description</span><span class="sxs-lookup"><span data-stu-id="70c26-167">description</span></span>|<span data-ttu-id="70c26-168">String</span><span class="sxs-lookup"><span data-stu-id="70c26-168">String</span></span>|<span data-ttu-id="70c26-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="70c26-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="70c26-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70c26-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70c26-171">displayName</span><span class="sxs-lookup"><span data-stu-id="70c26-171">displayName</span></span>|<span data-ttu-id="70c26-172">Строка</span><span class="sxs-lookup"><span data-stu-id="70c26-172">String</span></span>|<span data-ttu-id="70c26-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="70c26-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="70c26-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70c26-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70c26-175">version</span><span class="sxs-lookup"><span data-stu-id="70c26-175">version</span></span>|<span data-ttu-id="70c26-176">Int32</span><span class="sxs-lookup"><span data-stu-id="70c26-176">Int32</span></span>|<span data-ttu-id="70c26-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="70c26-177">Version of the device configuration.</span></span> <span data-ttu-id="70c26-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="70c26-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="70c26-179">аккаунтсблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="70c26-179">accountsBlockModification</span></span>|<span data-ttu-id="70c26-180">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-180">Boolean</span></span>|<span data-ttu-id="70c26-181">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="70c26-181">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="70c26-182">аппсалловинсталлфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="70c26-182">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="70c26-183">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-183">Boolean</span></span>|<span data-ttu-id="70c26-184">Указывает, может ли пользователь включить параметр "неизвестные источники".</span><span class="sxs-lookup"><span data-stu-id="70c26-184">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="70c26-185">аппсаутаупдатеполици</span><span class="sxs-lookup"><span data-stu-id="70c26-185">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="70c26-186">андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="70c26-186">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="70c26-187">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="70c26-187">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="70c26-188">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="70c26-188">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="70c26-189">аппсдефаултпермиссионполици</span><span class="sxs-lookup"><span data-stu-id="70c26-189">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="70c26-190">андроиддевицеовнердефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="70c26-190">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="70c26-191">Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом.</span><span class="sxs-lookup"><span data-stu-id="70c26-191">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="70c26-192">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="70c26-192">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="70c26-193">аппсрекоммендскиппингфирстусехинтс</span><span class="sxs-lookup"><span data-stu-id="70c26-193">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="70c26-194">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-194">Boolean</span></span>|<span data-ttu-id="70c26-195">Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.</span><span class="sxs-lookup"><span data-stu-id="70c26-195">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="70c26-196">блуетусблоккконфигуратион</span><span class="sxs-lookup"><span data-stu-id="70c26-196">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="70c26-197">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-197">Boolean</span></span>|<span data-ttu-id="70c26-198">Указывает, следует ли запретить пользователю настраивать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="70c26-198">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="70c26-199">блуетусблоккконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="70c26-199">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="70c26-200">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-200">Boolean</span></span>|<span data-ttu-id="70c26-201">Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="70c26-201">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="70c26-202">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="70c26-202">cameraBlocked</span></span>|<span data-ttu-id="70c26-203">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-203">Boolean</span></span>|<span data-ttu-id="70c26-204">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="70c26-204">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="70c26-205">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="70c26-205">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="70c26-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="70c26-206">Boolean</span></span>|<span data-ttu-id="70c26-207">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="70c26-207">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="70c26-208">датароамингблоккед</span><span class="sxs-lookup"><span data-stu-id="70c26-208">dataRoamingBlocked</span></span>|<span data-ttu-id="70c26-209">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-209">Boolean</span></span>|<span data-ttu-id="70c26-210">Указывает, следует ли запретить пользователю перемещать данные.</span><span class="sxs-lookup"><span data-stu-id="70c26-210">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="70c26-211">датетимеконфигуратионблоккед</span><span class="sxs-lookup"><span data-stu-id="70c26-211">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="70c26-212">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-212">Boolean</span></span>|<span data-ttu-id="70c26-213">Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.</span><span class="sxs-lookup"><span data-stu-id="70c26-213">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="70c26-214">факториресетдевицеадминистраторемаилс</span><span class="sxs-lookup"><span data-stu-id="70c26-214">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="70c26-215">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="70c26-215">String collection</span></span>|<span data-ttu-id="70c26-216">Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.</span><span class="sxs-lookup"><span data-stu-id="70c26-216">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="70c26-217">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="70c26-217">factoryResetBlocked</span></span>|<span data-ttu-id="70c26-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="70c26-218">Boolean</span></span>|<span data-ttu-id="70c26-219">Указывает, отключен ли параметр Reset фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="70c26-219">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="70c26-220">глобалпрокси</span><span class="sxs-lookup"><span data-stu-id="70c26-220">globalProxy</span></span>|[<span data-ttu-id="70c26-221">андроиддевицеовнерглобалпрокси</span><span class="sxs-lookup"><span data-stu-id="70c26-221">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="70c26-222">Прокси-сервер настраивается напрямую с узлом, портом и исключенными узлами.</span><span class="sxs-lookup"><span data-stu-id="70c26-222">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="70c26-223">киоскмодескринсаверконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="70c26-223">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="70c26-224">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-224">Boolean</span></span>|<span data-ttu-id="70c26-225">Указывает, следует ли включить режим экранной заставки или не в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="70c26-225">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="70c26-226">киоскмодескринсаверимажеурл</span><span class="sxs-lookup"><span data-stu-id="70c26-226">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="70c26-227">String</span><span class="sxs-lookup"><span data-stu-id="70c26-227">String</span></span>|<span data-ttu-id="70c26-228">URL-адрес изображения, которое будет экранной заставкой устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="70c26-228">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="70c26-229">киоскмодескринсавердисплайтимеинсекондс</span><span class="sxs-lookup"><span data-stu-id="70c26-229">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="70c26-230">Int32</span><span class="sxs-lookup"><span data-stu-id="70c26-230">Int32</span></span>|<span data-ttu-id="70c26-231">Время (в секундах), в течение которого устройство будет отображать экранную заставку в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="70c26-231">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="70c26-232">Допустимые значения — от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="70c26-232">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="70c26-233">киоскмодескринсаверстартделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="70c26-233">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="70c26-234">Int32</span><span class="sxs-lookup"><span data-stu-id="70c26-234">Int32</span></span>|<span data-ttu-id="70c26-235">Время (в секундах), в течение которого устройство должно быть неактивным, чтобы экранная заставка отображалась в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="70c26-235">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="70c26-236">Допустимые значения — от 1 до 9999999</span><span class="sxs-lookup"><span data-stu-id="70c26-236">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="70c26-237">киоскмодескринсавердетектмедиадисаблед</span><span class="sxs-lookup"><span data-stu-id="70c26-237">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="70c26-238">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-238">Boolean</span></span>|<span data-ttu-id="70c26-239">Указывает, должно ли устройство отображать экранную заставку при воспроизведении аудио-и видеоконференций в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="70c26-239">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="70c26-240">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="70c26-240">kioskModeApps</span></span>|<span data-ttu-id="70c26-241">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="70c26-241">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="70c26-242">Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="70c26-242">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="70c26-243">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="70c26-243">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="70c26-244">киоскмодеваллпаперурл</span><span class="sxs-lookup"><span data-stu-id="70c26-244">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="70c26-245">String</span><span class="sxs-lookup"><span data-stu-id="70c26-245">String</span></span>|<span data-ttu-id="70c26-246">URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="70c26-246">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="70c26-247">киоскмодикситкоде</span><span class="sxs-lookup"><span data-stu-id="70c26-247">kioskModeExitCode</span></span>|<span data-ttu-id="70c26-248">String</span><span class="sxs-lookup"><span data-stu-id="70c26-248">String</span></span>|<span data-ttu-id="70c26-249">Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="70c26-249">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="70c26-250">киоскмодевиртуалхомебуттоненаблед</span><span class="sxs-lookup"><span data-stu-id="70c26-250">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="70c26-251">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-251">Boolean</span></span>|<span data-ttu-id="70c26-252">Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="70c26-252">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="70c26-253">киоскмодевиртуалхомебуттонтипе</span><span class="sxs-lookup"><span data-stu-id="70c26-253">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="70c26-254">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="70c26-254">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="70c26-255">Указывает, является ли кнопка "Виртуальная Домашняя страница" кнопкой "Прокрутка вверх" или плавающей кнопкой "домой".</span><span class="sxs-lookup"><span data-stu-id="70c26-255">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="70c26-256">Возможные значения: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="70c26-256">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="70c26-257">киоскмодеблуетусконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="70c26-257">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="70c26-258">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-258">Boolean</span></span>|<span data-ttu-id="70c26-259">Указывает, следует ли запретить пользователю настраивать параметры Bluetooth в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="70c26-259">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="70c26-260">киоскмодевификонфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="70c26-260">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="70c26-261">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-261">Boolean</span></span>|<span data-ttu-id="70c26-262">Указывает, следует ли разрешить пользователю настраивать параметры Wi/Fi в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="70c26-262">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="70c26-263">киоскмодефлашлигхтконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="70c26-263">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="70c26-264">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-264">Boolean</span></span>|<span data-ttu-id="70c26-265">Указывает, следует ли разрешить пользователю использовать флашлигхт в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="70c26-265">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="70c26-266">киоскмодемедиаволумеконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="70c26-266">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="70c26-267">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-267">Boolean</span></span>|<span data-ttu-id="70c26-268">Указывает, следует ли запретить пользователю изменять громкость мультимедиа в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="70c26-268">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="70c26-269">микрофонефорцемуте</span><span class="sxs-lookup"><span data-stu-id="70c26-269">microphoneForceMute</span></span>|<span data-ttu-id="70c26-270">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-270">Boolean</span></span>|<span data-ttu-id="70c26-271">Указывает, следует ли запретить разблокирование микрофона устройства.</span><span class="sxs-lookup"><span data-stu-id="70c26-271">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="70c26-272">нетворкескапехатчалловед</span><span class="sxs-lookup"><span data-stu-id="70c26-272">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="70c26-273">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-273">Boolean</span></span>|<span data-ttu-id="70c26-274">Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="70c26-274">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="70c26-275">нфкблоккаутгоингбеам</span><span class="sxs-lookup"><span data-stu-id="70c26-275">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="70c26-276">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-276">Boolean</span></span>|<span data-ttu-id="70c26-277">Указывает, следует ли заблокировать исходящую форму NFC.</span><span class="sxs-lookup"><span data-stu-id="70c26-277">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="70c26-278">пассвордблокккэйгуард</span><span class="sxs-lookup"><span data-stu-id="70c26-278">passwordBlockKeyguard</span></span>|<span data-ttu-id="70c26-279">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-279">Boolean</span></span>|<span data-ttu-id="70c26-280">Указывает, отключен ли кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="70c26-280">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="70c26-281">пассвордблокккэйгуардфеатурес</span><span class="sxs-lookup"><span data-stu-id="70c26-281">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="70c26-282">Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="70c26-282">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="70c26-283">Список компонентов кэйгуард устройств, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="70c26-283">List of device keyguard features to block.</span></span> <span data-ttu-id="70c26-284">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="70c26-284">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="70c26-285">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="70c26-285">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="70c26-286">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="70c26-286">passwordExpirationDays</span></span>|<span data-ttu-id="70c26-287">Int32</span><span class="sxs-lookup"><span data-stu-id="70c26-287">Int32</span></span>|<span data-ttu-id="70c26-288">Указывает время в секундах, в течение которого можно задать пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="70c26-288">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="70c26-289">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="70c26-289">Valid values 1 to 365</span></span>|
|<span data-ttu-id="70c26-290">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="70c26-290">passwordMinimumLength</span></span>|<span data-ttu-id="70c26-291">Int32</span><span class="sxs-lookup"><span data-stu-id="70c26-291">Int32</span></span>|<span data-ttu-id="70c26-292">Указывает минимальную длину пароля, необходимого для устройства.</span><span class="sxs-lookup"><span data-stu-id="70c26-292">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="70c26-293">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="70c26-293">Valid values 4 to 16</span></span>|
|<span data-ttu-id="70c26-294">пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="70c26-294">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="70c26-295">Int32</span><span class="sxs-lookup"><span data-stu-id="70c26-295">Int32</span></span>|<span data-ttu-id="70c26-296">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="70c26-296">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="70c26-297">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="70c26-297">Valid values 1 to 16</span></span>|
|<span data-ttu-id="70c26-298">пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="70c26-298">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="70c26-299">Int32</span><span class="sxs-lookup"><span data-stu-id="70c26-299">Int32</span></span>|<span data-ttu-id="70c26-300">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="70c26-300">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="70c26-301">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="70c26-301">Valid values 1 to 16</span></span>|
|<span data-ttu-id="70c26-302">пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="70c26-302">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="70c26-303">Int32</span><span class="sxs-lookup"><span data-stu-id="70c26-303">Int32</span></span>|<span data-ttu-id="70c26-304">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="70c26-304">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="70c26-305">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="70c26-305">Valid values 1 to 16</span></span>|
|<span data-ttu-id="70c26-306">пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="70c26-306">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="70c26-307">Int32</span><span class="sxs-lookup"><span data-stu-id="70c26-307">Int32</span></span>|<span data-ttu-id="70c26-308">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="70c26-308">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="70c26-309">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="70c26-309">Valid values 1 to 16</span></span>|
|<span data-ttu-id="70c26-310">пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="70c26-310">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="70c26-311">Int32</span><span class="sxs-lookup"><span data-stu-id="70c26-311">Int32</span></span>|<span data-ttu-id="70c26-312">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="70c26-312">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="70c26-313">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="70c26-313">Valid values 1 to 16</span></span>|
|<span data-ttu-id="70c26-314">пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="70c26-314">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="70c26-315">Int32</span><span class="sxs-lookup"><span data-stu-id="70c26-315">Int32</span></span>|<span data-ttu-id="70c26-316">Указывает минимальное число символов верхнего каселеттер, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="70c26-316">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="70c26-317">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="70c26-317">Valid values 1 to 16</span></span>|
|<span data-ttu-id="70c26-318">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="70c26-318">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="70c26-319">Int32</span><span class="sxs-lookup"><span data-stu-id="70c26-319">Int32</span></span>|<span data-ttu-id="70c26-320">Миллисекунды бездействия до истечения времени ожидания экрана.</span><span class="sxs-lookup"><span data-stu-id="70c26-320">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="70c26-321">пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="70c26-321">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="70c26-322">Int32</span><span class="sxs-lookup"><span data-stu-id="70c26-322">Int32</span></span>|<span data-ttu-id="70c26-323">Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале.</span><span class="sxs-lookup"><span data-stu-id="70c26-323">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="70c26-324">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="70c26-324">Valid values 0 to 24</span></span>|
|<span data-ttu-id="70c26-325">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="70c26-325">passwordRequiredType</span></span>|[<span data-ttu-id="70c26-326">андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="70c26-326">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="70c26-327">Указывает минимальное качество пароля, необходимое для устройства.</span><span class="sxs-lookup"><span data-stu-id="70c26-327">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="70c26-328">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="70c26-328">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="70c26-329">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="70c26-329">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="70c26-330">Int32</span><span class="sxs-lookup"><span data-stu-id="70c26-330">Int32</span></span>|<span data-ttu-id="70c26-331">Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="70c26-331">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="70c26-332">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="70c26-332">Valid values 4 to 11</span></span>|
|<span data-ttu-id="70c26-333">плайсторемоде</span><span class="sxs-lookup"><span data-stu-id="70c26-333">playStoreMode</span></span>|[<span data-ttu-id="70c26-334">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="70c26-334">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="70c26-335">Указывает режим проигрывания устройства в хранилище.</span><span class="sxs-lookup"><span data-stu-id="70c26-335">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="70c26-336">Возможные значения: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="70c26-336">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="70c26-337">сафебутблоккед</span><span class="sxs-lookup"><span data-stu-id="70c26-337">safeBootBlocked</span></span>|<span data-ttu-id="70c26-338">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-338">Boolean</span></span>|<span data-ttu-id="70c26-339">Указывает, отключена ли загрузка устройства в "безопасная загрузка".</span><span class="sxs-lookup"><span data-stu-id="70c26-339">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="70c26-340">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="70c26-340">screenCaptureBlocked</span></span>|<span data-ttu-id="70c26-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="70c26-341">Boolean</span></span>|<span data-ttu-id="70c26-342">Указывает, следует ли отключить возможность использования снимков экрана.</span><span class="sxs-lookup"><span data-stu-id="70c26-342">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="70c26-343">секуритялловдебуггингфеатурес</span><span class="sxs-lookup"><span data-stu-id="70c26-343">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="70c26-344">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-344">Boolean</span></span>|<span data-ttu-id="70c26-345">Указывает, следует ли запретить пользователю включать функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="70c26-345">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="70c26-346">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="70c26-346">securityRequireVerifyApps</span></span>|<span data-ttu-id="70c26-347">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-347">Boolean</span></span>|<span data-ttu-id="70c26-348">Указывает, требуется ли проверка приложений.</span><span class="sxs-lookup"><span data-stu-id="70c26-348">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="70c26-349">статусбарблоккед</span><span class="sxs-lookup"><span data-stu-id="70c26-349">statusBarBlocked</span></span>|<span data-ttu-id="70c26-350">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-350">Boolean</span></span>|<span data-ttu-id="70c26-351">Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.</span><span class="sxs-lookup"><span data-stu-id="70c26-351">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="70c26-352">стайонмодес</span><span class="sxs-lookup"><span data-stu-id="70c26-352">stayOnModes</span></span>|<span data-ttu-id="70c26-353">Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="70c26-353">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="70c26-354">Список режимов, в которых дисплей устройства остается включенным.</span><span class="sxs-lookup"><span data-stu-id="70c26-354">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="70c26-355">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="70c26-355">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="70c26-356">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="70c26-356">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="70c26-357">сторажеалловусб</span><span class="sxs-lookup"><span data-stu-id="70c26-357">storageAllowUsb</span></span>|<span data-ttu-id="70c26-358">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-358">Boolean</span></span>|<span data-ttu-id="70c26-359">Указывает, следует ли разрешить запоминающее устройство USB.</span><span class="sxs-lookup"><span data-stu-id="70c26-359">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="70c26-360">сторажеблоккекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="70c26-360">storageBlockExternalMedia</span></span>|<span data-ttu-id="70c26-361">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-361">Boolean</span></span>|<span data-ttu-id="70c26-362">Указывает, следует ли заблокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="70c26-362">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="70c26-363">сторажеблоккусбфилетрансфер</span><span class="sxs-lookup"><span data-stu-id="70c26-363">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="70c26-364">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-364">Boolean</span></span>|<span data-ttu-id="70c26-365">Указывает, следует ли запретить передачу файлов через USB.</span><span class="sxs-lookup"><span data-stu-id="70c26-365">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="70c26-366">системупдатевиндовстартминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="70c26-366">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="70c26-367">Int32</span><span class="sxs-lookup"><span data-stu-id="70c26-367">Int32</span></span>|<span data-ttu-id="70c26-368">Указывает количество минут после полуночи, когда запустится окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="70c26-368">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="70c26-369">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="70c26-369">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="70c26-370">системупдатевиндовендминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="70c26-370">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="70c26-371">Int32</span><span class="sxs-lookup"><span data-stu-id="70c26-371">Int32</span></span>|<span data-ttu-id="70c26-372">Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="70c26-372">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="70c26-373">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="70c26-373">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="70c26-374">системупдатеинсталлтипе</span><span class="sxs-lookup"><span data-stu-id="70c26-374">systemUpdateInstallType</span></span>|[<span data-ttu-id="70c26-375">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="70c26-375">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="70c26-376">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="70c26-376">The type of system update configuration.</span></span> <span data-ttu-id="70c26-377">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="70c26-377">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="70c26-378">системвиндовсблоккед</span><span class="sxs-lookup"><span data-stu-id="70c26-378">systemWindowsBlocked</span></span>|<span data-ttu-id="70c26-379">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-379">Boolean</span></span>|<span data-ttu-id="70c26-380">Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="70c26-380">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="70c26-381">усерсблоккадд</span><span class="sxs-lookup"><span data-stu-id="70c26-381">usersBlockAdd</span></span>|<span data-ttu-id="70c26-382">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-382">Boolean</span></span>|<span data-ttu-id="70c26-383">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="70c26-383">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="70c26-384">усерсблоккремове</span><span class="sxs-lookup"><span data-stu-id="70c26-384">usersBlockRemove</span></span>|<span data-ttu-id="70c26-385">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-385">Boolean</span></span>|<span data-ttu-id="70c26-386">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="70c26-386">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="70c26-387">волумеблоккаджустмент</span><span class="sxs-lookup"><span data-stu-id="70c26-387">volumeBlockAdjustment</span></span>|<span data-ttu-id="70c26-388">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-388">Boolean</span></span>|<span data-ttu-id="70c26-389">Указывает, отключена ли настройка главного тома.</span><span class="sxs-lookup"><span data-stu-id="70c26-389">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="70c26-390">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="70c26-390">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="70c26-391">String</span><span class="sxs-lookup"><span data-stu-id="70c26-391">String</span></span>|<span data-ttu-id="70c26-392">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="70c26-392">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="70c26-393">впналвайсонлоккдовнмоде</span><span class="sxs-lookup"><span data-stu-id="70c26-393">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="70c26-394">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-394">Boolean</span></span>|<span data-ttu-id="70c26-395">Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="70c26-395">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="70c26-396">вифиблоккедитконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="70c26-396">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="70c26-397">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-397">Boolean</span></span>|<span data-ttu-id="70c26-398">Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="70c26-398">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="70c26-399">вифиблоккедитполицидефинедконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="70c26-399">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="70c26-400">Логический</span><span class="sxs-lookup"><span data-stu-id="70c26-400">Boolean</span></span>|<span data-ttu-id="70c26-401">Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="70c26-401">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="70c26-402">Отклик</span><span class="sxs-lookup"><span data-stu-id="70c26-402">Response</span></span>
<span data-ttu-id="70c26-403">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70c26-403">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70c26-404">Пример</span><span class="sxs-lookup"><span data-stu-id="70c26-404">Example</span></span>

### <a name="request"></a><span data-ttu-id="70c26-405">Запрос</span><span class="sxs-lookup"><span data-stu-id="70c26-405">Request</span></span>
<span data-ttu-id="70c26-406">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70c26-406">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="70c26-407">Отклик</span><span class="sxs-lookup"><span data-stu-id="70c26-407">Response</span></span>
<span data-ttu-id="70c26-p136">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70c26-p136">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






