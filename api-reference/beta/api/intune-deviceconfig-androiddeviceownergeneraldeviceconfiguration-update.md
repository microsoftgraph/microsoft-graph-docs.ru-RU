---
title: Обновление androidDeviceOwnerGeneralDeviceConfiguration
description: Обновление свойств объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc6746dca524394be358d1a4c31fc5cfe53c001b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793117"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="e0ad3-103">Обновление androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0ad3-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="e0ad3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0ad3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0ad3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0ad3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0ad3-107">Обновление свойств объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e0ad3-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0ad3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e0ad3-108">Prerequisites</span></span>
<span data-ttu-id="e0ad3-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e0ad3-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0ad3-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0ad3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0ad3-111">Permission type</span></span>|<span data-ttu-id="e0ad3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0ad3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0ad3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0ad3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0ad3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0ad3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e0ad3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0ad3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0ad3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-116">Not supported.</span></span>|
|<span data-ttu-id="e0ad3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0ad3-117">Application</span></span>|<span data-ttu-id="e0ad3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0ad3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0ad3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0ad3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e0ad3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e0ad3-120">Request headers</span></span>
|<span data-ttu-id="e0ad3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0ad3-121">Header</span></span>|<span data-ttu-id="e0ad3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e0ad3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0ad3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0ad3-123">Authorization</span></span>|<span data-ttu-id="e0ad3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0ad3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e0ad3-125">Accept</span></span>|<span data-ttu-id="e0ad3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0ad3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0ad3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e0ad3-127">Request body</span></span>
<span data-ttu-id="e0ad3-128">В тексте запроса добавьте представление объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="e0ad3-129">В следующей таблице приведены свойства, необходимые при создании [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0ad3-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="e0ad3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0ad3-130">Property</span></span>|<span data-ttu-id="e0ad3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e0ad3-131">Type</span></span>|<span data-ttu-id="e0ad3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e0ad3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0ad3-133">id</span><span class="sxs-lookup"><span data-stu-id="e0ad3-133">id</span></span>|<span data-ttu-id="e0ad3-134">String</span><span class="sxs-lookup"><span data-stu-id="e0ad3-134">String</span></span>|<span data-ttu-id="e0ad3-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-135">Key of the entity.</span></span> <span data-ttu-id="e0ad3-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0ad3-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0ad3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0ad3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e0ad3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0ad3-138">DateTimeOffset</span></span>|<span data-ttu-id="e0ad3-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e0ad3-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0ad3-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0ad3-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e0ad3-141">roleScopeTagIds</span></span>|<span data-ttu-id="e0ad3-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e0ad3-142">String collection</span></span>|<span data-ttu-id="e0ad3-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e0ad3-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0ad3-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0ad3-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e0ad3-145">supportsScopeTags</span></span>|<span data-ttu-id="e0ad3-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-146">Boolean</span></span>|<span data-ttu-id="e0ad3-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e0ad3-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e0ad3-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e0ad3-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-150">This property is read-only.</span></span> <span data-ttu-id="e0ad3-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0ad3-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0ad3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e0ad3-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e0ad3-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e0ad3-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e0ad3-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e0ad3-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0ad3-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0ad3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e0ad3-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e0ad3-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e0ad3-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e0ad3-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e0ad3-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0ad3-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0ad3-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e0ad3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e0ad3-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e0ad3-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e0ad3-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e0ad3-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0ad3-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0ad3-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0ad3-164">createdDateTime</span></span>|<span data-ttu-id="e0ad3-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0ad3-165">DateTimeOffset</span></span>|<span data-ttu-id="e0ad3-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-166">DateTime the object was created.</span></span> <span data-ttu-id="e0ad3-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0ad3-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0ad3-168">description</span><span class="sxs-lookup"><span data-stu-id="e0ad3-168">description</span></span>|<span data-ttu-id="e0ad3-169">String</span><span class="sxs-lookup"><span data-stu-id="e0ad3-169">String</span></span>|<span data-ttu-id="e0ad3-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e0ad3-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0ad3-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0ad3-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e0ad3-172">displayName</span></span>|<span data-ttu-id="e0ad3-173">Строка</span><span class="sxs-lookup"><span data-stu-id="e0ad3-173">String</span></span>|<span data-ttu-id="e0ad3-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e0ad3-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0ad3-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0ad3-176">version</span><span class="sxs-lookup"><span data-stu-id="e0ad3-176">version</span></span>|<span data-ttu-id="e0ad3-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ad3-177">Int32</span></span>|<span data-ttu-id="e0ad3-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-178">Version of the device configuration.</span></span> <span data-ttu-id="e0ad3-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0ad3-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0ad3-180">аккаунтсблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="e0ad3-180">accountsBlockModification</span></span>|<span data-ttu-id="e0ad3-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-181">Boolean</span></span>|<span data-ttu-id="e0ad3-182">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="e0ad3-183">аппсалловинсталлфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="e0ad3-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="e0ad3-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-184">Boolean</span></span>|<span data-ttu-id="e0ad3-185">Указывает, может ли пользователь включить параметр "неизвестные источники".</span><span class="sxs-lookup"><span data-stu-id="e0ad3-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="e0ad3-186">аппсаутаупдатеполици</span><span class="sxs-lookup"><span data-stu-id="e0ad3-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="e0ad3-187">андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="e0ad3-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="e0ad3-188">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="e0ad3-189">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="e0ad3-190">аппсдефаултпермиссионполици</span><span class="sxs-lookup"><span data-stu-id="e0ad3-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="e0ad3-191">андроиддевицеовнердефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="e0ad3-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="e0ad3-192">Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="e0ad3-193">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="e0ad3-194">аппсрекоммендскиппингфирстусехинтс</span><span class="sxs-lookup"><span data-stu-id="e0ad3-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="e0ad3-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-195">Boolean</span></span>|<span data-ttu-id="e0ad3-196">Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="e0ad3-197">блуетусблоккконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e0ad3-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="e0ad3-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-198">Boolean</span></span>|<span data-ttu-id="e0ad3-199">Указывает, следует ли запретить пользователю настраивать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="e0ad3-200">блуетусблоккконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="e0ad3-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="e0ad3-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-201">Boolean</span></span>|<span data-ttu-id="e0ad3-202">Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="e0ad3-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="e0ad3-203">cameraBlocked</span></span>|<span data-ttu-id="e0ad3-204">Логический</span><span class="sxs-lookup"><span data-stu-id="e0ad3-204">Boolean</span></span>|<span data-ttu-id="e0ad3-205">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="e0ad3-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="e0ad3-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="e0ad3-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-207">Boolean</span></span>|<span data-ttu-id="e0ad3-208">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="e0ad3-209">цертификатекредентиалконфигуратиондисаблед</span><span class="sxs-lookup"><span data-stu-id="e0ad3-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="e0ad3-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-210">Boolean</span></span>|<span data-ttu-id="e0ad3-211">Указывает, следует ли запретить пользователям настраивать учетные данные сертификатов.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="e0ad3-212">микрософтлаунчерконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="e0ad3-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="e0ad3-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-213">Boolean</span></span>|<span data-ttu-id="e0ad3-214">Указывает, следует ли настроить средство запуска Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="e0ad3-215">микрософтлаунчеркустомваллпаперенаблед</span><span class="sxs-lookup"><span data-stu-id="e0ad3-215">microsoftLauncherCustomWallpaperEnabled</span></span>|<span data-ttu-id="e0ad3-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-216">Boolean</span></span>|<span data-ttu-id="e0ad3-217">Указывает, следует ли настраивать фоновый рисунок на целевых устройствах.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-217">Indicates whether or not to configure the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="e0ad3-218">микрософтлаунчеркустомваллпаперимажеурл</span><span class="sxs-lookup"><span data-stu-id="e0ad3-218">microsoftLauncherCustomWallpaperImageUrl</span></span>|<span data-ttu-id="e0ad3-219">String</span><span class="sxs-lookup"><span data-stu-id="e0ad3-219">String</span></span>|<span data-ttu-id="e0ad3-220">Указывает URL-адрес для файла изображения, который будет использоваться в качестве фонового рисунка на целевых устройствах.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-220">Indicates the URL for the image file to use as the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="e0ad3-221">микрософтлаунчеркустомваллпапералловусермодификатион</span><span class="sxs-lookup"><span data-stu-id="e0ad3-221">microsoftLauncherCustomWallpaperAllowUserModification</span></span>|<span data-ttu-id="e0ad3-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-222">Boolean</span></span>|<span data-ttu-id="e0ad3-223">Указывает, может ли пользователь изменять фоновый рисунок для персонализации своего устройства.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-223">Indicates whether or not the user can modify the wallpaper to personalize their device.</span></span>|
|<span data-ttu-id="e0ad3-224">микрософтлаунчерфиденаблед</span><span class="sxs-lookup"><span data-stu-id="e0ad3-224">microsoftLauncherFeedEnabled</span></span>|<span data-ttu-id="e0ad3-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-225">Boolean</span></span>|<span data-ttu-id="e0ad3-226">Указывает, следует ли включить веб-канал запуска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-226">Indicates whether or not you want to enable the launcher feed on the device.</span></span>|
|<span data-ttu-id="e0ad3-227">микрософтлаунчерфидалловусермодификатион</span><span class="sxs-lookup"><span data-stu-id="e0ad3-227">microsoftLauncherFeedAllowUserModification</span></span>|<span data-ttu-id="e0ad3-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-228">Boolean</span></span>|<span data-ttu-id="e0ad3-229">Указывает, может ли пользователь изменять веб-канал запуска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-229">Indicates whether or not the user can modify the launcher feed on the device.</span></span>|
|<span data-ttu-id="e0ad3-230">микрософтлаунчердоккпресенцеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e0ad3-230">microsoftLauncherDockPresenceConfiguration</span></span>|[<span data-ttu-id="e0ad3-231">микрософтлаунчердоккпресенце</span><span class="sxs-lookup"><span data-stu-id="e0ad3-231">microsoftLauncherDockPresence</span></span>](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|<span data-ttu-id="e0ad3-232">Указывает, следует ли настроить закрепление устройства.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-232">Indicates whether or not you want to configure the device dock.</span></span> <span data-ttu-id="e0ad3-233">Возможные значения: `notConfigured`, `show`, `hide`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-233">Possible values are: `notConfigured`, `show`, `hide`, `disabled`.</span></span>|
|<span data-ttu-id="e0ad3-234">микрософтлаунчердоккпресенцеалловусермодификатион</span><span class="sxs-lookup"><span data-stu-id="e0ad3-234">microsoftLauncherDockPresenceAllowUserModification</span></span>|<span data-ttu-id="e0ad3-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-235">Boolean</span></span>|<span data-ttu-id="e0ad3-236">Указывает, может ли пользователь изменять конфигурацию закрепления устройств на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-236">Indicates whether or not the user can modify the device dock configuration on the device.</span></span>|
|<span data-ttu-id="e0ad3-237">микрософтлаунчерсеарчбарплацементконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e0ad3-237">microsoftLauncherSearchBarPlacementConfiguration</span></span>|[<span data-ttu-id="e0ad3-238">микрософтлаунчерсеарчбарплацемент</span><span class="sxs-lookup"><span data-stu-id="e0ad3-238">microsoftLauncherSearchBarPlacement</span></span>](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|<span data-ttu-id="e0ad3-239">Указывает конфигурацию размещения панели поиска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-239">Indicates the search bar placement configuration on the device.</span></span> <span data-ttu-id="e0ad3-240">Возможные значения: `notConfigured`, `top`, `bottom`, `hide`.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-240">Possible values are: `notConfigured`, `top`, `bottom`, `hide`.</span></span>|
|<span data-ttu-id="e0ad3-241">микрософтлаунчерсеарчбарплацементалловусермодификатион</span><span class="sxs-lookup"><span data-stu-id="e0ad3-241">microsoftLauncherSearchBarPlacementAllowUserModification</span></span>|<span data-ttu-id="e0ad3-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-242">Boolean</span></span>|<span data-ttu-id="e0ad3-243">Указывает, может ли пользователь изменять расположение панели поиска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-243">Indicates whether the user can modify the search bar placement on the device.</span></span>|
|<span data-ttu-id="e0ad3-244">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e0ad3-244">enrollmentProfile</span></span>|[<span data-ttu-id="e0ad3-245">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="e0ad3-245">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="e0ad3-246">Указывает, какой профиль регистрации вы хотите настроить.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-246">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="e0ad3-247">Возможные значения: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-247">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="e0ad3-248">датароамингблоккед</span><span class="sxs-lookup"><span data-stu-id="e0ad3-248">dataRoamingBlocked</span></span>|<span data-ttu-id="e0ad3-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-249">Boolean</span></span>|<span data-ttu-id="e0ad3-250">Указывает, следует ли запретить пользователю перемещать данные.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-250">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="e0ad3-251">датетимеконфигуратионблоккед</span><span class="sxs-lookup"><span data-stu-id="e0ad3-251">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="e0ad3-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-252">Boolean</span></span>|<span data-ttu-id="e0ad3-253">Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-253">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="e0ad3-254">факториресетдевицеадминистраторемаилс</span><span class="sxs-lookup"><span data-stu-id="e0ad3-254">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="e0ad3-255">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e0ad3-255">String collection</span></span>|<span data-ttu-id="e0ad3-256">Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-256">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="e0ad3-257">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="e0ad3-257">factoryResetBlocked</span></span>|<span data-ttu-id="e0ad3-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-258">Boolean</span></span>|<span data-ttu-id="e0ad3-259">Указывает, отключен ли параметр Reset фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-259">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="e0ad3-260">глобалпрокси</span><span class="sxs-lookup"><span data-stu-id="e0ad3-260">globalProxy</span></span>|[<span data-ttu-id="e0ad3-261">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="e0ad3-261">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="e0ad3-262">Прокси-сервер настраивается напрямую с узлом, портом и исключенными узлами.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-262">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="e0ad3-263">гуглеаккаунтсблоккед</span><span class="sxs-lookup"><span data-stu-id="e0ad3-263">googleAccountsBlocked</span></span>|<span data-ttu-id="e0ad3-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-264">Boolean</span></span>|<span data-ttu-id="e0ad3-265">Указывает, будут ли блокироваться учетные записи Google.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-265">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="e0ad3-266">киоскмодескринсаверконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="e0ad3-266">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="e0ad3-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-267">Boolean</span></span>|<span data-ttu-id="e0ad3-268">Указывает, следует ли включить режим экранной заставки или не в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-268">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="e0ad3-269">киоскмодескринсаверимажеурл</span><span class="sxs-lookup"><span data-stu-id="e0ad3-269">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="e0ad3-270">String</span><span class="sxs-lookup"><span data-stu-id="e0ad3-270">String</span></span>|<span data-ttu-id="e0ad3-271">URL-адрес изображения, которое будет экранной заставкой устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-271">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="e0ad3-272">киоскмодескринсавердисплайтимеинсекондс</span><span class="sxs-lookup"><span data-stu-id="e0ad3-272">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="e0ad3-273">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ad3-273">Int32</span></span>|<span data-ttu-id="e0ad3-274">Время (в секундах), в течение которого устройство будет отображать экранную заставку в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-274">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="e0ad3-275">Допустимые значения — от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="e0ad3-275">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="e0ad3-276">киоскмодескринсаверстартделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="e0ad3-276">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="e0ad3-277">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ad3-277">Int32</span></span>|<span data-ttu-id="e0ad3-278">Время (в секундах), в течение которого устройство должно быть неактивным, чтобы экранная заставка отображалась в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-278">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="e0ad3-279">Допустимые значения — от 1 до 9999999</span><span class="sxs-lookup"><span data-stu-id="e0ad3-279">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="e0ad3-280">киоскмодескринсавердетектмедиадисаблед</span><span class="sxs-lookup"><span data-stu-id="e0ad3-280">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="e0ad3-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-281">Boolean</span></span>|<span data-ttu-id="e0ad3-282">Указывает, должно ли устройство отображать экранную заставку при воспроизведении аудио-и видеоконференций в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-282">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="e0ad3-283">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="e0ad3-283">kioskModeApps</span></span>|<span data-ttu-id="e0ad3-284">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="e0ad3-284">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e0ad3-285">Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-285">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="e0ad3-286">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-286">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e0ad3-287">киоскмодеваллпаперурл</span><span class="sxs-lookup"><span data-stu-id="e0ad3-287">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="e0ad3-288">String</span><span class="sxs-lookup"><span data-stu-id="e0ad3-288">String</span></span>|<span data-ttu-id="e0ad3-289">URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-289">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="e0ad3-290">киоскмодикситкоде</span><span class="sxs-lookup"><span data-stu-id="e0ad3-290">kioskModeExitCode</span></span>|<span data-ttu-id="e0ad3-291">String</span><span class="sxs-lookup"><span data-stu-id="e0ad3-291">String</span></span>|<span data-ttu-id="e0ad3-292">Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-292">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="e0ad3-293">киоскмодевиртуалхомебуттоненаблед</span><span class="sxs-lookup"><span data-stu-id="e0ad3-293">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="e0ad3-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-294">Boolean</span></span>|<span data-ttu-id="e0ad3-295">Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-295">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="e0ad3-296">киоскмодевиртуалхомебуттонтипе</span><span class="sxs-lookup"><span data-stu-id="e0ad3-296">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="e0ad3-297">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="e0ad3-297">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="e0ad3-298">Указывает, является ли кнопка "Виртуальная Домашняя страница" кнопкой "Прокрутка вверх" или плавающей кнопкой "домой".</span><span class="sxs-lookup"><span data-stu-id="e0ad3-298">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="e0ad3-299">Возможные значения: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-299">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="e0ad3-300">киоскмодеблуетусконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="e0ad3-300">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="e0ad3-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-301">Boolean</span></span>|<span data-ttu-id="e0ad3-302">Указывает, следует ли запретить пользователю настраивать параметры Bluetooth в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-302">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="e0ad3-303">киоскмодевификонфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="e0ad3-303">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="e0ad3-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-304">Boolean</span></span>|<span data-ttu-id="e0ad3-305">Указывает, следует ли разрешить пользователю настраивать параметры Wi/Fi в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-305">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="e0ad3-306">киоскмодефлашлигхтконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="e0ad3-306">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="e0ad3-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-307">Boolean</span></span>|<span data-ttu-id="e0ad3-308">Указывает, следует ли разрешить пользователю использовать флашлигхт в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-308">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="e0ad3-309">киоскмодемедиаволумеконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="e0ad3-309">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="e0ad3-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-310">Boolean</span></span>|<span data-ttu-id="e0ad3-311">Указывает, следует ли запретить пользователю изменять громкость мультимедиа в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-311">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="e0ad3-312">микрофонефорцемуте</span><span class="sxs-lookup"><span data-stu-id="e0ad3-312">microphoneForceMute</span></span>|<span data-ttu-id="e0ad3-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-313">Boolean</span></span>|<span data-ttu-id="e0ad3-314">Указывает, следует ли запретить разблокирование микрофона устройства.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-314">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="e0ad3-315">нетворкескапехатчалловед</span><span class="sxs-lookup"><span data-stu-id="e0ad3-315">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="e0ad3-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-316">Boolean</span></span>|<span data-ttu-id="e0ad3-317">Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-317">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="e0ad3-318">нфкблоккаутгоингбеам</span><span class="sxs-lookup"><span data-stu-id="e0ad3-318">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="e0ad3-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-319">Boolean</span></span>|<span data-ttu-id="e0ad3-320">Указывает, следует ли заблокировать исходящую форму NFC.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-320">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="e0ad3-321">пассвордблокккэйгуард</span><span class="sxs-lookup"><span data-stu-id="e0ad3-321">passwordBlockKeyguard</span></span>|<span data-ttu-id="e0ad3-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-322">Boolean</span></span>|<span data-ttu-id="e0ad3-323">Указывает, отключен ли кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-323">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="e0ad3-324">пассвордблокккэйгуардфеатурес</span><span class="sxs-lookup"><span data-stu-id="e0ad3-324">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="e0ad3-325">Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="e0ad3-325">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="e0ad3-326">Список компонентов кэйгуард устройств, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-326">List of device keyguard features to block.</span></span> <span data-ttu-id="e0ad3-327">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-327">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="e0ad3-328">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-328">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="e0ad3-329">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e0ad3-329">passwordExpirationDays</span></span>|<span data-ttu-id="e0ad3-330">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ad3-330">Int32</span></span>|<span data-ttu-id="e0ad3-331">Указывает время в секундах, в течение которого можно задать пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-331">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="e0ad3-332">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-332">Valid values 1 to 365</span></span>|
|<span data-ttu-id="e0ad3-333">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e0ad3-333">passwordMinimumLength</span></span>|<span data-ttu-id="e0ad3-334">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ad3-334">Int32</span></span>|<span data-ttu-id="e0ad3-335">Указывает минимальную длину пароля, необходимого для устройства.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-335">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="e0ad3-336">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-336">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e0ad3-337">пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="e0ad3-337">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="e0ad3-338">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ad3-338">Int32</span></span>|<span data-ttu-id="e0ad3-339">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-339">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="e0ad3-340">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-340">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e0ad3-341">пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="e0ad3-341">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="e0ad3-342">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ad3-342">Int32</span></span>|<span data-ttu-id="e0ad3-343">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-343">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="e0ad3-344">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-344">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e0ad3-345">пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="e0ad3-345">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="e0ad3-346">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ad3-346">Int32</span></span>|<span data-ttu-id="e0ad3-347">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-347">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="e0ad3-348">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-348">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e0ad3-349">пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="e0ad3-349">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="e0ad3-350">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ad3-350">Int32</span></span>|<span data-ttu-id="e0ad3-351">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-351">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="e0ad3-352">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-352">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e0ad3-353">пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="e0ad3-353">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="e0ad3-354">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ad3-354">Int32</span></span>|<span data-ttu-id="e0ad3-355">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-355">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="e0ad3-356">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-356">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e0ad3-357">пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="e0ad3-357">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="e0ad3-358">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ad3-358">Int32</span></span>|<span data-ttu-id="e0ad3-359">Указывает минимальное число символов верхнего каселеттер, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-359">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="e0ad3-360">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-360">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e0ad3-361">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e0ad3-361">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e0ad3-362">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ad3-362">Int32</span></span>|<span data-ttu-id="e0ad3-363">Миллисекунды бездействия до истечения времени ожидания экрана.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-363">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e0ad3-364">пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="e0ad3-364">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="e0ad3-365">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ad3-365">Int32</span></span>|<span data-ttu-id="e0ad3-366">Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-366">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="e0ad3-367">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-367">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e0ad3-368">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e0ad3-368">passwordRequiredType</span></span>|[<span data-ttu-id="e0ad3-369">андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="e0ad3-369">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="e0ad3-370">Указывает минимальное качество пароля, необходимое для устройства.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-370">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="e0ad3-371">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-371">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="e0ad3-372">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e0ad3-372">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e0ad3-373">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ad3-373">Int32</span></span>|<span data-ttu-id="e0ad3-374">Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-374">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="e0ad3-375">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-375">Valid values 4 to 11</span></span>|
|<span data-ttu-id="e0ad3-376">плайсторемоде</span><span class="sxs-lookup"><span data-stu-id="e0ad3-376">playStoreMode</span></span>|[<span data-ttu-id="e0ad3-377">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="e0ad3-377">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="e0ad3-378">Указывает режим проигрывания устройства в хранилище.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-378">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="e0ad3-379">Возможные значения: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-379">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="e0ad3-380">сафебутблоккед</span><span class="sxs-lookup"><span data-stu-id="e0ad3-380">safeBootBlocked</span></span>|<span data-ttu-id="e0ad3-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-381">Boolean</span></span>|<span data-ttu-id="e0ad3-382">Указывает, отключена ли загрузка устройства в "безопасная загрузка".</span><span class="sxs-lookup"><span data-stu-id="e0ad3-382">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="e0ad3-383">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="e0ad3-383">screenCaptureBlocked</span></span>|<span data-ttu-id="e0ad3-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-384">Boolean</span></span>|<span data-ttu-id="e0ad3-385">Указывает, следует ли отключить возможность использования снимков экрана.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-385">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="e0ad3-386">секуритялловдебуггингфеатурес</span><span class="sxs-lookup"><span data-stu-id="e0ad3-386">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="e0ad3-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-387">Boolean</span></span>|<span data-ttu-id="e0ad3-388">Указывает, следует ли запретить пользователю включать функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-388">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="e0ad3-389">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="e0ad3-389">securityRequireVerifyApps</span></span>|<span data-ttu-id="e0ad3-390">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-390">Boolean</span></span>|<span data-ttu-id="e0ad3-391">Указывает, требуется ли проверка приложений.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-391">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="e0ad3-392">статусбарблоккед</span><span class="sxs-lookup"><span data-stu-id="e0ad3-392">statusBarBlocked</span></span>|<span data-ttu-id="e0ad3-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-393">Boolean</span></span>|<span data-ttu-id="e0ad3-394">Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-394">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="e0ad3-395">стайонмодес</span><span class="sxs-lookup"><span data-stu-id="e0ad3-395">stayOnModes</span></span>|<span data-ttu-id="e0ad3-396">Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="e0ad3-396">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="e0ad3-397">Список режимов, в которых дисплей устройства остается включенным.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-397">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="e0ad3-398">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-398">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="e0ad3-399">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-399">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="e0ad3-400">сторажеалловусб</span><span class="sxs-lookup"><span data-stu-id="e0ad3-400">storageAllowUsb</span></span>|<span data-ttu-id="e0ad3-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-401">Boolean</span></span>|<span data-ttu-id="e0ad3-402">Указывает, следует ли разрешить запоминающее устройство USB.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-402">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="e0ad3-403">сторажеблоккекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="e0ad3-403">storageBlockExternalMedia</span></span>|<span data-ttu-id="e0ad3-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-404">Boolean</span></span>|<span data-ttu-id="e0ad3-405">Указывает, следует ли заблокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-405">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="e0ad3-406">сторажеблоккусбфилетрансфер</span><span class="sxs-lookup"><span data-stu-id="e0ad3-406">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="e0ad3-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-407">Boolean</span></span>|<span data-ttu-id="e0ad3-408">Указывает, следует ли запретить передачу файлов через USB.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-408">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="e0ad3-409">системупдатевиндовстартминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="e0ad3-409">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="e0ad3-410">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ad3-410">Int32</span></span>|<span data-ttu-id="e0ad3-411">Указывает количество минут после полуночи, когда запустится окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-411">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="e0ad3-412">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="e0ad3-412">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="e0ad3-413">системупдатевиндовендминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="e0ad3-413">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="e0ad3-414">Int32</span><span class="sxs-lookup"><span data-stu-id="e0ad3-414">Int32</span></span>|<span data-ttu-id="e0ad3-415">Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-415">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="e0ad3-416">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="e0ad3-416">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="e0ad3-417">системупдатеинсталлтипе</span><span class="sxs-lookup"><span data-stu-id="e0ad3-417">systemUpdateInstallType</span></span>|[<span data-ttu-id="e0ad3-418">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="e0ad3-418">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="e0ad3-419">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-419">The type of system update configuration.</span></span> <span data-ttu-id="e0ad3-420">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-420">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="e0ad3-421">системвиндовсблоккед</span><span class="sxs-lookup"><span data-stu-id="e0ad3-421">systemWindowsBlocked</span></span>|<span data-ttu-id="e0ad3-422">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-422">Boolean</span></span>|<span data-ttu-id="e0ad3-423">Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-423">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="e0ad3-424">усерсблоккадд</span><span class="sxs-lookup"><span data-stu-id="e0ad3-424">usersBlockAdd</span></span>|<span data-ttu-id="e0ad3-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-425">Boolean</span></span>|<span data-ttu-id="e0ad3-426">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-426">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="e0ad3-427">усерсблоккремове</span><span class="sxs-lookup"><span data-stu-id="e0ad3-427">usersBlockRemove</span></span>|<span data-ttu-id="e0ad3-428">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-428">Boolean</span></span>|<span data-ttu-id="e0ad3-429">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-429">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="e0ad3-430">волумеблоккаджустмент</span><span class="sxs-lookup"><span data-stu-id="e0ad3-430">volumeBlockAdjustment</span></span>|<span data-ttu-id="e0ad3-431">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-431">Boolean</span></span>|<span data-ttu-id="e0ad3-432">Указывает, отключена ли настройка главного тома.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-432">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="e0ad3-433">впналвайсонлоккдовнмоде</span><span class="sxs-lookup"><span data-stu-id="e0ad3-433">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="e0ad3-434">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-434">Boolean</span></span>|<span data-ttu-id="e0ad3-435">Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-435">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="e0ad3-436">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="e0ad3-436">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="e0ad3-437">String</span><span class="sxs-lookup"><span data-stu-id="e0ad3-437">String</span></span>|<span data-ttu-id="e0ad3-438">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-438">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="e0ad3-439">вифиблоккедитконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="e0ad3-439">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="e0ad3-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-440">Boolean</span></span>|<span data-ttu-id="e0ad3-441">Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-441">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="e0ad3-442">вифиблоккедитполицидефинедконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="e0ad3-442">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="e0ad3-443">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0ad3-443">Boolean</span></span>|<span data-ttu-id="e0ad3-444">Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-444">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="e0ad3-445">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0ad3-445">Response</span></span>
<span data-ttu-id="e0ad3-446">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-446">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0ad3-447">Пример</span><span class="sxs-lookup"><span data-stu-id="e0ad3-447">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0ad3-448">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0ad3-448">Request</span></span>
<span data-ttu-id="e0ad3-449">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-449">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 5044

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
  "microsoftLauncherSearchBarPlacementAllowUserModification": true,
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

### <a name="response"></a><span data-ttu-id="e0ad3-450">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0ad3-450">Response</span></span>
<span data-ttu-id="e0ad3-451">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-451">Here is an example of the response.</span></span> <span data-ttu-id="e0ad3-452">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-452">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e0ad3-453">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e0ad3-453">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5216

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
  "microsoftLauncherSearchBarPlacementAllowUserModification": true,
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



