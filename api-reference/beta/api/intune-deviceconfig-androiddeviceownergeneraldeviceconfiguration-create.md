---
title: Создание androidDeviceOwnerGeneralDeviceConfiguration
description: Создание нового объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 16ba295955cc32f932612c5d2d4007ffedca46af
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34971432"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="44157-103">Создание androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="44157-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="44157-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44157-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44157-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44157-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44157-106">Создание нового объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="44157-106">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44157-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="44157-107">Prerequisites</span></span>
<span data-ttu-id="44157-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44157-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44157-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44157-110">Permission type</span></span>|<span data-ttu-id="44157-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44157-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44157-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44157-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44157-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44157-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44157-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44157-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44157-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44157-115">Not supported.</span></span>|
|<span data-ttu-id="44157-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44157-116">Application</span></span>|<span data-ttu-id="44157-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44157-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44157-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44157-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="44157-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44157-119">Request headers</span></span>
|<span data-ttu-id="44157-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44157-120">Header</span></span>|<span data-ttu-id="44157-121">Значение</span><span class="sxs-lookup"><span data-stu-id="44157-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44157-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44157-122">Authorization</span></span>|<span data-ttu-id="44157-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44157-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44157-124">Accept</span><span class="sxs-lookup"><span data-stu-id="44157-124">Accept</span></span>|<span data-ttu-id="44157-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44157-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44157-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="44157-126">Request body</span></span>
<span data-ttu-id="44157-127">В тексте запроса добавьте представление объекта androidDeviceOwnerGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44157-127">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="44157-128">В следующей таблице приведены свойства, необходимые при создании androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="44157-128">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="44157-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="44157-129">Property</span></span>|<span data-ttu-id="44157-130">Тип</span><span class="sxs-lookup"><span data-stu-id="44157-130">Type</span></span>|<span data-ttu-id="44157-131">Описание</span><span class="sxs-lookup"><span data-stu-id="44157-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44157-132">id</span><span class="sxs-lookup"><span data-stu-id="44157-132">id</span></span>|<span data-ttu-id="44157-133">String</span><span class="sxs-lookup"><span data-stu-id="44157-133">String</span></span>|<span data-ttu-id="44157-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="44157-134">Key of the entity.</span></span> <span data-ttu-id="44157-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44157-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44157-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44157-136">lastModifiedDateTime</span></span>|<span data-ttu-id="44157-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44157-137">DateTimeOffset</span></span>|<span data-ttu-id="44157-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="44157-138">DateTime the object was last modified.</span></span> <span data-ttu-id="44157-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44157-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44157-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="44157-140">roleScopeTagIds</span></span>|<span data-ttu-id="44157-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="44157-141">String collection</span></span>|<span data-ttu-id="44157-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="44157-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="44157-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44157-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44157-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="44157-144">supportsScopeTags</span></span>|<span data-ttu-id="44157-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-145">Boolean</span></span>|<span data-ttu-id="44157-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="44157-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="44157-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="44157-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="44157-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="44157-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="44157-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="44157-149">This property is read-only.</span></span> <span data-ttu-id="44157-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44157-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44157-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="44157-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="44157-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="44157-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="44157-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="44157-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="44157-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44157-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44157-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="44157-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="44157-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="44157-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="44157-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="44157-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="44157-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44157-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44157-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="44157-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="44157-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="44157-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="44157-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="44157-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="44157-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44157-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44157-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44157-163">createdDateTime</span></span>|<span data-ttu-id="44157-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44157-164">DateTimeOffset</span></span>|<span data-ttu-id="44157-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="44157-165">DateTime the object was created.</span></span> <span data-ttu-id="44157-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44157-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44157-167">description</span><span class="sxs-lookup"><span data-stu-id="44157-167">description</span></span>|<span data-ttu-id="44157-168">String</span><span class="sxs-lookup"><span data-stu-id="44157-168">String</span></span>|<span data-ttu-id="44157-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="44157-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="44157-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44157-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44157-171">displayName</span><span class="sxs-lookup"><span data-stu-id="44157-171">displayName</span></span>|<span data-ttu-id="44157-172">Строка</span><span class="sxs-lookup"><span data-stu-id="44157-172">String</span></span>|<span data-ttu-id="44157-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="44157-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="44157-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44157-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44157-175">version</span><span class="sxs-lookup"><span data-stu-id="44157-175">version</span></span>|<span data-ttu-id="44157-176">Int32</span><span class="sxs-lookup"><span data-stu-id="44157-176">Int32</span></span>|<span data-ttu-id="44157-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="44157-177">Version of the device configuration.</span></span> <span data-ttu-id="44157-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44157-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44157-179">Аккаунтсблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="44157-179">accountsBlockModification</span></span>|<span data-ttu-id="44157-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-180">Boolean</span></span>|<span data-ttu-id="44157-181">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="44157-181">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="44157-182">Аппсалловинсталлфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="44157-182">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="44157-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-183">Boolean</span></span>|<span data-ttu-id="44157-184">Указывает, может ли пользователь включить параметр "неизвестные источники".</span><span class="sxs-lookup"><span data-stu-id="44157-184">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="44157-185">Аппсаутаупдатеполици</span><span class="sxs-lookup"><span data-stu-id="44157-185">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="44157-186">Андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="44157-186">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="44157-187">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="44157-187">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="44157-188">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="44157-188">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="44157-189">Аппсдефаултпермиссионполици</span><span class="sxs-lookup"><span data-stu-id="44157-189">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="44157-190">Андроиддевицеовнердефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="44157-190">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="44157-191">Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом.</span><span class="sxs-lookup"><span data-stu-id="44157-191">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="44157-192">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="44157-192">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="44157-193">Аппсрекоммендскиппингфирстусехинтс</span><span class="sxs-lookup"><span data-stu-id="44157-193">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="44157-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-194">Boolean</span></span>|<span data-ttu-id="44157-195">Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.</span><span class="sxs-lookup"><span data-stu-id="44157-195">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="44157-196">Блуетусблоккконфигуратион</span><span class="sxs-lookup"><span data-stu-id="44157-196">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="44157-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-197">Boolean</span></span>|<span data-ttu-id="44157-198">Указывает, следует ли запретить пользователю настраивать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="44157-198">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="44157-199">Блуетусблоккконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="44157-199">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="44157-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-200">Boolean</span></span>|<span data-ttu-id="44157-201">Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="44157-201">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="44157-202">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="44157-202">cameraBlocked</span></span>|<span data-ttu-id="44157-203">Логический</span><span class="sxs-lookup"><span data-stu-id="44157-203">Boolean</span></span>|<span data-ttu-id="44157-204">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="44157-204">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="44157-205">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="44157-205">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="44157-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-206">Boolean</span></span>|<span data-ttu-id="44157-207">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="44157-207">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="44157-208">Датароамингблоккед</span><span class="sxs-lookup"><span data-stu-id="44157-208">dataRoamingBlocked</span></span>|<span data-ttu-id="44157-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-209">Boolean</span></span>|<span data-ttu-id="44157-210">Указывает, следует ли запретить пользователю перемещать данные.</span><span class="sxs-lookup"><span data-stu-id="44157-210">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="44157-211">Датетимеконфигуратионблоккед</span><span class="sxs-lookup"><span data-stu-id="44157-211">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="44157-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-212">Boolean</span></span>|<span data-ttu-id="44157-213">Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.</span><span class="sxs-lookup"><span data-stu-id="44157-213">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="44157-214">Факториресетдевицеадминистраторемаилс</span><span class="sxs-lookup"><span data-stu-id="44157-214">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="44157-215">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="44157-215">String collection</span></span>|<span data-ttu-id="44157-216">Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.</span><span class="sxs-lookup"><span data-stu-id="44157-216">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="44157-217">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="44157-217">factoryResetBlocked</span></span>|<span data-ttu-id="44157-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-218">Boolean</span></span>|<span data-ttu-id="44157-219">Указывает, отключен ли параметр Reset фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="44157-219">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="44157-220">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="44157-220">kioskModeApps</span></span>|<span data-ttu-id="44157-221">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="44157-221">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="44157-222">Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44157-222">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="44157-223">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="44157-223">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="44157-224">Киоскмодеваллпаперурл</span><span class="sxs-lookup"><span data-stu-id="44157-224">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="44157-225">String</span><span class="sxs-lookup"><span data-stu-id="44157-225">String</span></span>|<span data-ttu-id="44157-226">URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44157-226">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="44157-227">Киоскмодикситкоде</span><span class="sxs-lookup"><span data-stu-id="44157-227">kioskModeExitCode</span></span>|<span data-ttu-id="44157-228">String</span><span class="sxs-lookup"><span data-stu-id="44157-228">String</span></span>|<span data-ttu-id="44157-229">Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44157-229">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="44157-230">Киоскмодевиртуалхомебуттоненаблед</span><span class="sxs-lookup"><span data-stu-id="44157-230">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="44157-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-231">Boolean</span></span>|<span data-ttu-id="44157-232">Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44157-232">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="44157-233">Киоскмодеблуетусконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="44157-233">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="44157-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-234">Boolean</span></span>|<span data-ttu-id="44157-235">Указывает, следует ли запретить пользователю настраивать параметры Bluetooth в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44157-235">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="44157-236">Киоскмодевификонфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="44157-236">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="44157-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-237">Boolean</span></span>|<span data-ttu-id="44157-238">Указывает, следует ли разрешить пользователю настраивать параметры Wi/Fi в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="44157-238">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="44157-239">Микрофонефорцемуте</span><span class="sxs-lookup"><span data-stu-id="44157-239">microphoneForceMute</span></span>|<span data-ttu-id="44157-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-240">Boolean</span></span>|<span data-ttu-id="44157-241">Указывает, следует ли запретить разблокирование микрофона устройства.</span><span class="sxs-lookup"><span data-stu-id="44157-241">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="44157-242">Нетворкескапехатчалловед</span><span class="sxs-lookup"><span data-stu-id="44157-242">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="44157-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-243">Boolean</span></span>|<span data-ttu-id="44157-244">Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="44157-244">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="44157-245">Нфкблоккаутгоингбеам</span><span class="sxs-lookup"><span data-stu-id="44157-245">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="44157-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-246">Boolean</span></span>|<span data-ttu-id="44157-247">Указывает, следует ли заблокировать исходящую форму NFC.</span><span class="sxs-lookup"><span data-stu-id="44157-247">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="44157-248">Пассвордблокккэйгуард</span><span class="sxs-lookup"><span data-stu-id="44157-248">passwordBlockKeyguard</span></span>|<span data-ttu-id="44157-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-249">Boolean</span></span>|<span data-ttu-id="44157-250">Указывает, отключен ли кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="44157-250">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="44157-251">Пассвордблокккэйгуардфеатурес</span><span class="sxs-lookup"><span data-stu-id="44157-251">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="44157-252">Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="44157-252">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="44157-253">Список компонентов кэйгуард устройств, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="44157-253">List of device keyguard features to block.</span></span> <span data-ttu-id="44157-254">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="44157-254">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="44157-255">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="44157-255">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="44157-256">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="44157-256">passwordExpirationDays</span></span>|<span data-ttu-id="44157-257">Int32</span><span class="sxs-lookup"><span data-stu-id="44157-257">Int32</span></span>|<span data-ttu-id="44157-258">Указывает время в секундах, в течение которого можно задать пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="44157-258">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="44157-259">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="44157-259">Valid values 1 to 365</span></span>|
|<span data-ttu-id="44157-260">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="44157-260">passwordMinimumLength</span></span>|<span data-ttu-id="44157-261">Int32</span><span class="sxs-lookup"><span data-stu-id="44157-261">Int32</span></span>|<span data-ttu-id="44157-262">Указывает минимальную длину пароля, необходимого для устройства.</span><span class="sxs-lookup"><span data-stu-id="44157-262">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="44157-263">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="44157-263">Valid values 4 to 16</span></span>|
|<span data-ttu-id="44157-264">Пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="44157-264">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="44157-265">Int32</span><span class="sxs-lookup"><span data-stu-id="44157-265">Int32</span></span>|<span data-ttu-id="44157-266">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="44157-266">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="44157-267">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="44157-267">Valid values 1 to 16</span></span>|
|<span data-ttu-id="44157-268">Пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="44157-268">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="44157-269">Int32</span><span class="sxs-lookup"><span data-stu-id="44157-269">Int32</span></span>|<span data-ttu-id="44157-270">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="44157-270">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="44157-271">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="44157-271">Valid values 1 to 16</span></span>|
|<span data-ttu-id="44157-272">Пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="44157-272">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="44157-273">Int32</span><span class="sxs-lookup"><span data-stu-id="44157-273">Int32</span></span>|<span data-ttu-id="44157-274">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="44157-274">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="44157-275">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="44157-275">Valid values 1 to 16</span></span>|
|<span data-ttu-id="44157-276">Пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="44157-276">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="44157-277">Int32</span><span class="sxs-lookup"><span data-stu-id="44157-277">Int32</span></span>|<span data-ttu-id="44157-278">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="44157-278">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="44157-279">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="44157-279">Valid values 1 to 16</span></span>|
|<span data-ttu-id="44157-280">Пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="44157-280">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="44157-281">Int32</span><span class="sxs-lookup"><span data-stu-id="44157-281">Int32</span></span>|<span data-ttu-id="44157-282">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="44157-282">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="44157-283">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="44157-283">Valid values 1 to 16</span></span>|
|<span data-ttu-id="44157-284">Пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="44157-284">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="44157-285">Int32</span><span class="sxs-lookup"><span data-stu-id="44157-285">Int32</span></span>|<span data-ttu-id="44157-286">Указывает минимальное число символов верхнего каселеттер, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="44157-286">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="44157-287">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="44157-287">Valid values 1 to 16</span></span>|
|<span data-ttu-id="44157-288">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="44157-288">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="44157-289">Int32</span><span class="sxs-lookup"><span data-stu-id="44157-289">Int32</span></span>|<span data-ttu-id="44157-290">Миллисекунды бездействия до истечения времени ожидания экрана.</span><span class="sxs-lookup"><span data-stu-id="44157-290">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="44157-291">Пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="44157-291">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="44157-292">Int32</span><span class="sxs-lookup"><span data-stu-id="44157-292">Int32</span></span>|<span data-ttu-id="44157-293">Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале.</span><span class="sxs-lookup"><span data-stu-id="44157-293">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="44157-294">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="44157-294">Valid values 0 to 24</span></span>|
|<span data-ttu-id="44157-295">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="44157-295">passwordRequiredType</span></span>|[<span data-ttu-id="44157-296">Андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="44157-296">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="44157-297">Указывает минимальное качество пароля, необходимое для устройства.</span><span class="sxs-lookup"><span data-stu-id="44157-297">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="44157-298">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="44157-298">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="44157-299">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="44157-299">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="44157-300">Int32</span><span class="sxs-lookup"><span data-stu-id="44157-300">Int32</span></span>|<span data-ttu-id="44157-301">Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="44157-301">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="44157-302">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="44157-302">Valid values 4 to 11</span></span>|
|<span data-ttu-id="44157-303">Плайсторемоде</span><span class="sxs-lookup"><span data-stu-id="44157-303">playStoreMode</span></span>|[<span data-ttu-id="44157-304">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="44157-304">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="44157-305">Указывает режим проигрывания устройства в хранилище.</span><span class="sxs-lookup"><span data-stu-id="44157-305">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="44157-306">Возможные значения: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="44157-306">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="44157-307">Сафебутблоккед</span><span class="sxs-lookup"><span data-stu-id="44157-307">safeBootBlocked</span></span>|<span data-ttu-id="44157-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-308">Boolean</span></span>|<span data-ttu-id="44157-309">Указывает, отключена ли загрузка устройства в "безопасная загрузка".</span><span class="sxs-lookup"><span data-stu-id="44157-309">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="44157-310">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="44157-310">screenCaptureBlocked</span></span>|<span data-ttu-id="44157-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-311">Boolean</span></span>|<span data-ttu-id="44157-312">Указывает, следует ли отключить возможность использования снимков экрана.</span><span class="sxs-lookup"><span data-stu-id="44157-312">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="44157-313">Секуритялловдебуггингфеатурес</span><span class="sxs-lookup"><span data-stu-id="44157-313">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="44157-314">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-314">Boolean</span></span>|<span data-ttu-id="44157-315">Указывает, следует ли запретить пользователю включать функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="44157-315">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="44157-316">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="44157-316">securityRequireVerifyApps</span></span>|<span data-ttu-id="44157-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-317">Boolean</span></span>|<span data-ttu-id="44157-318">Указывает, требуется ли проверка приложений.</span><span class="sxs-lookup"><span data-stu-id="44157-318">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="44157-319">Статусбарблоккед</span><span class="sxs-lookup"><span data-stu-id="44157-319">statusBarBlocked</span></span>|<span data-ttu-id="44157-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-320">Boolean</span></span>|<span data-ttu-id="44157-321">Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.</span><span class="sxs-lookup"><span data-stu-id="44157-321">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="44157-322">Стайонмодес</span><span class="sxs-lookup"><span data-stu-id="44157-322">stayOnModes</span></span>|<span data-ttu-id="44157-323">Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="44157-323">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="44157-324">Список режимов, в которых дисплей устройства остается включенным.</span><span class="sxs-lookup"><span data-stu-id="44157-324">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="44157-325">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="44157-325">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="44157-326">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="44157-326">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="44157-327">Сторажеалловусб</span><span class="sxs-lookup"><span data-stu-id="44157-327">storageAllowUsb</span></span>|<span data-ttu-id="44157-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-328">Boolean</span></span>|<span data-ttu-id="44157-329">Указывает, следует ли разрешить запоминающее устройство USB.</span><span class="sxs-lookup"><span data-stu-id="44157-329">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="44157-330">Сторажеблоккекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="44157-330">storageBlockExternalMedia</span></span>|<span data-ttu-id="44157-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-331">Boolean</span></span>|<span data-ttu-id="44157-332">Указывает, следует ли заблокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="44157-332">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="44157-333">Сторажеблоккусбфилетрансфер</span><span class="sxs-lookup"><span data-stu-id="44157-333">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="44157-334">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-334">Boolean</span></span>|<span data-ttu-id="44157-335">Указывает, следует ли запретить передачу файлов через USB.</span><span class="sxs-lookup"><span data-stu-id="44157-335">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="44157-336">Системупдатевиндовстартминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="44157-336">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="44157-337">Int32</span><span class="sxs-lookup"><span data-stu-id="44157-337">Int32</span></span>|<span data-ttu-id="44157-338">Указывает количество минут после полуночи, когда запустится окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="44157-338">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="44157-339">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="44157-339">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="44157-340">Системупдатевиндовендминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="44157-340">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="44157-341">Int32</span><span class="sxs-lookup"><span data-stu-id="44157-341">Int32</span></span>|<span data-ttu-id="44157-342">Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="44157-342">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="44157-343">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="44157-343">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="44157-344">Системупдатеинсталлтипе</span><span class="sxs-lookup"><span data-stu-id="44157-344">systemUpdateInstallType</span></span>|[<span data-ttu-id="44157-345">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="44157-345">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="44157-346">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="44157-346">The type of system update configuration.</span></span> <span data-ttu-id="44157-347">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="44157-347">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="44157-348">Системвиндовсблоккед</span><span class="sxs-lookup"><span data-stu-id="44157-348">systemWindowsBlocked</span></span>|<span data-ttu-id="44157-349">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-349">Boolean</span></span>|<span data-ttu-id="44157-350">Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="44157-350">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="44157-351">Усерсблоккадд</span><span class="sxs-lookup"><span data-stu-id="44157-351">usersBlockAdd</span></span>|<span data-ttu-id="44157-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-352">Boolean</span></span>|<span data-ttu-id="44157-353">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="44157-353">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="44157-354">Усерсблоккремове</span><span class="sxs-lookup"><span data-stu-id="44157-354">usersBlockRemove</span></span>|<span data-ttu-id="44157-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-355">Boolean</span></span>|<span data-ttu-id="44157-356">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="44157-356">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="44157-357">Волумеблоккаджустмент</span><span class="sxs-lookup"><span data-stu-id="44157-357">volumeBlockAdjustment</span></span>|<span data-ttu-id="44157-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-358">Boolean</span></span>|<span data-ttu-id="44157-359">Указывает, отключена ли настройка главного тома.</span><span class="sxs-lookup"><span data-stu-id="44157-359">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="44157-360">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="44157-360">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="44157-361">String</span><span class="sxs-lookup"><span data-stu-id="44157-361">String</span></span>|<span data-ttu-id="44157-362">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="44157-362">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="44157-363">Впналвайсонлоккдовнмоде</span><span class="sxs-lookup"><span data-stu-id="44157-363">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="44157-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-364">Boolean</span></span>|<span data-ttu-id="44157-365">Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="44157-365">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="44157-366">Вифиблоккедитконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="44157-366">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="44157-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-367">Boolean</span></span>|<span data-ttu-id="44157-368">Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="44157-368">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="44157-369">Вифиблоккедитполицидефинедконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="44157-369">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="44157-370">Boolean</span><span class="sxs-lookup"><span data-stu-id="44157-370">Boolean</span></span>|<span data-ttu-id="44157-371">Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="44157-371">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="44157-372">Отклик</span><span class="sxs-lookup"><span data-stu-id="44157-372">Response</span></span>
<span data-ttu-id="44157-373">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44157-373">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44157-374">Пример</span><span class="sxs-lookup"><span data-stu-id="44157-374">Example</span></span>

### <a name="request"></a><span data-ttu-id="44157-375">Запрос</span><span class="sxs-lookup"><span data-stu-id="44157-375">Request</span></span>
<span data-ttu-id="44157-376">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44157-376">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3678

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
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
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

### <a name="response"></a><span data-ttu-id="44157-377">Отклик</span><span class="sxs-lookup"><span data-stu-id="44157-377">Response</span></span>
<span data-ttu-id="44157-p133">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44157-p133">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3850

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
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
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





