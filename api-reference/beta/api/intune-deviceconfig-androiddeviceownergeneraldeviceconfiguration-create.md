---
title: Создание androidDeviceOwnerGeneralDeviceConfiguration
description: Создание нового объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 91b30037e9d8ca1141b9a4610f390cad248ff081
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36312616"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="4b66c-103">Создание androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b66c-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="4b66c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b66c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b66c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b66c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b66c-106">Создание нового объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4b66c-106">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b66c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4b66c-107">Prerequisites</span></span>
<span data-ttu-id="4b66c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b66c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b66c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b66c-110">Permission type</span></span>|<span data-ttu-id="4b66c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b66c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b66c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b66c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b66c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b66c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b66c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b66c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b66c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b66c-115">Not supported.</span></span>|
|<span data-ttu-id="4b66c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b66c-116">Application</span></span>|<span data-ttu-id="4b66c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b66c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b66c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b66c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4b66c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b66c-119">Request headers</span></span>
|<span data-ttu-id="4b66c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b66c-120">Header</span></span>|<span data-ttu-id="4b66c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4b66c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b66c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b66c-122">Authorization</span></span>|<span data-ttu-id="4b66c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b66c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b66c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4b66c-124">Accept</span></span>|<span data-ttu-id="4b66c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4b66c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b66c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4b66c-126">Request body</span></span>
<span data-ttu-id="4b66c-127">В тексте запроса добавьте представление объекта androidDeviceOwnerGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b66c-127">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="4b66c-128">В следующей таблице приведены свойства, необходимые при создании androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4b66c-128">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="4b66c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b66c-129">Property</span></span>|<span data-ttu-id="4b66c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4b66c-130">Type</span></span>|<span data-ttu-id="4b66c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4b66c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b66c-132">id</span><span class="sxs-lookup"><span data-stu-id="4b66c-132">id</span></span>|<span data-ttu-id="4b66c-133">String</span><span class="sxs-lookup"><span data-stu-id="4b66c-133">String</span></span>|<span data-ttu-id="4b66c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4b66c-134">Key of the entity.</span></span> <span data-ttu-id="4b66c-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b66c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b66c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b66c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4b66c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b66c-137">DateTimeOffset</span></span>|<span data-ttu-id="4b66c-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4b66c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4b66c-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b66c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b66c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4b66c-140">roleScopeTagIds</span></span>|<span data-ttu-id="4b66c-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4b66c-141">String collection</span></span>|<span data-ttu-id="4b66c-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4b66c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4b66c-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b66c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b66c-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4b66c-144">supportsScopeTags</span></span>|<span data-ttu-id="4b66c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-145">Boolean</span></span>|<span data-ttu-id="4b66c-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4b66c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4b66c-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4b66c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4b66c-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4b66c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4b66c-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4b66c-149">This property is read-only.</span></span> <span data-ttu-id="4b66c-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b66c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b66c-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4b66c-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4b66c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4b66c-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4b66c-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4b66c-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4b66c-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b66c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b66c-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4b66c-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4b66c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4b66c-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4b66c-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4b66c-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4b66c-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b66c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b66c-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="4b66c-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4b66c-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="4b66c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4b66c-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4b66c-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4b66c-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b66c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b66c-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b66c-163">createdDateTime</span></span>|<span data-ttu-id="4b66c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b66c-164">DateTimeOffset</span></span>|<span data-ttu-id="4b66c-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4b66c-165">DateTime the object was created.</span></span> <span data-ttu-id="4b66c-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b66c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b66c-167">description</span><span class="sxs-lookup"><span data-stu-id="4b66c-167">description</span></span>|<span data-ttu-id="4b66c-168">String</span><span class="sxs-lookup"><span data-stu-id="4b66c-168">String</span></span>|<span data-ttu-id="4b66c-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b66c-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4b66c-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b66c-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b66c-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4b66c-171">displayName</span></span>|<span data-ttu-id="4b66c-172">Строка</span><span class="sxs-lookup"><span data-stu-id="4b66c-172">String</span></span>|<span data-ttu-id="4b66c-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b66c-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4b66c-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b66c-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b66c-175">version</span><span class="sxs-lookup"><span data-stu-id="4b66c-175">version</span></span>|<span data-ttu-id="4b66c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4b66c-176">Int32</span></span>|<span data-ttu-id="4b66c-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b66c-177">Version of the device configuration.</span></span> <span data-ttu-id="4b66c-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b66c-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b66c-179">аккаунтсблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="4b66c-179">accountsBlockModification</span></span>|<span data-ttu-id="4b66c-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-180">Boolean</span></span>|<span data-ttu-id="4b66c-181">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="4b66c-181">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="4b66c-182">аппсалловинсталлфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="4b66c-182">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="4b66c-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-183">Boolean</span></span>|<span data-ttu-id="4b66c-184">Указывает, может ли пользователь включить параметр "неизвестные источники".</span><span class="sxs-lookup"><span data-stu-id="4b66c-184">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="4b66c-185">аппсаутаупдатеполици</span><span class="sxs-lookup"><span data-stu-id="4b66c-185">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="4b66c-186">андроиддевицеовнераппаутаупдатеполицитипе</span><span class="sxs-lookup"><span data-stu-id="4b66c-186">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="4b66c-187">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="4b66c-187">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="4b66c-188">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="4b66c-188">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="4b66c-189">аппсдефаултпермиссионполици</span><span class="sxs-lookup"><span data-stu-id="4b66c-189">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="4b66c-190">андроиддевицеовнердефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="4b66c-190">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="4b66c-191">Указывает политику разрешений для запросов для разрешений среды выполнения, если она не определена для приложения особым образом.</span><span class="sxs-lookup"><span data-stu-id="4b66c-191">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="4b66c-192">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="4b66c-192">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="4b66c-193">аппсрекоммендскиппингфирстусехинтс</span><span class="sxs-lookup"><span data-stu-id="4b66c-193">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="4b66c-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-194">Boolean</span></span>|<span data-ttu-id="4b66c-195">Указывает, следует ли запретить всем приложениям пропускать все подсказок по первому использованию, которые они могли добавить.</span><span class="sxs-lookup"><span data-stu-id="4b66c-195">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="4b66c-196">блуетусблоккконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4b66c-196">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="4b66c-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-197">Boolean</span></span>|<span data-ttu-id="4b66c-198">Указывает, следует ли запретить пользователю настраивать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="4b66c-198">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="4b66c-199">блуетусблоккконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="4b66c-199">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="4b66c-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-200">Boolean</span></span>|<span data-ttu-id="4b66c-201">Указывает, следует ли запретить пользователю предоставлять общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="4b66c-201">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="4b66c-202">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="4b66c-202">cameraBlocked</span></span>|<span data-ttu-id="4b66c-203">Логический</span><span class="sxs-lookup"><span data-stu-id="4b66c-203">Boolean</span></span>|<span data-ttu-id="4b66c-204">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="4b66c-204">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="4b66c-205">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="4b66c-205">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="4b66c-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-206">Boolean</span></span>|<span data-ttu-id="4b66c-207">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="4b66c-207">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="4b66c-208">датароамингблоккед</span><span class="sxs-lookup"><span data-stu-id="4b66c-208">dataRoamingBlocked</span></span>|<span data-ttu-id="4b66c-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-209">Boolean</span></span>|<span data-ttu-id="4b66c-210">Указывает, следует ли запретить пользователю перемещать данные.</span><span class="sxs-lookup"><span data-stu-id="4b66c-210">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="4b66c-211">датетимеконфигуратионблоккед</span><span class="sxs-lookup"><span data-stu-id="4b66c-211">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="4b66c-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-212">Boolean</span></span>|<span data-ttu-id="4b66c-213">Указывает, следует ли запретить пользователю вручную изменять дату или время на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4b66c-213">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="4b66c-214">факториресетдевицеадминистраторемаилс</span><span class="sxs-lookup"><span data-stu-id="4b66c-214">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="4b66c-215">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4b66c-215">String collection</span></span>|<span data-ttu-id="4b66c-216">Список сообщений учетных записей Google, которые потребуются для проверки подлинности после завершения фабричного сброса устройства перед его настройкой.</span><span class="sxs-lookup"><span data-stu-id="4b66c-216">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="4b66c-217">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="4b66c-217">factoryResetBlocked</span></span>|<span data-ttu-id="4b66c-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-218">Boolean</span></span>|<span data-ttu-id="4b66c-219">Указывает, отключен ли параметр Reset фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="4b66c-219">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="4b66c-220">киоскмодескринсаверконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="4b66c-220">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="4b66c-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-221">Boolean</span></span>|<span data-ttu-id="4b66c-222">Указывает, следует ли включить режим экранной заставки или не в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4b66c-222">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="4b66c-223">киоскмодескринсаверимажеурл</span><span class="sxs-lookup"><span data-stu-id="4b66c-223">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="4b66c-224">String</span><span class="sxs-lookup"><span data-stu-id="4b66c-224">String</span></span>|<span data-ttu-id="4b66c-225">URL-адрес изображения, которое будет экранной заставкой устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4b66c-225">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="4b66c-226">киоскмодескринсавердисплайтимеинсекондс</span><span class="sxs-lookup"><span data-stu-id="4b66c-226">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="4b66c-227">Int32</span><span class="sxs-lookup"><span data-stu-id="4b66c-227">Int32</span></span>|<span data-ttu-id="4b66c-228">Время (в секундах), в течение которого устройство будет отображать экранную заставку в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4b66c-228">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="4b66c-229">Допустимые значения — от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="4b66c-229">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="4b66c-230">киоскмодескринсаверстартделайинсекондс</span><span class="sxs-lookup"><span data-stu-id="4b66c-230">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="4b66c-231">Int32</span><span class="sxs-lookup"><span data-stu-id="4b66c-231">Int32</span></span>|<span data-ttu-id="4b66c-232">Время (в секундах), в течение которого устройство должно быть неактивным, чтобы экранная заставка отображалась в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4b66c-232">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="4b66c-233">Допустимые значения — от 1 до 9999999</span><span class="sxs-lookup"><span data-stu-id="4b66c-233">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="4b66c-234">киоскмодескринсавердетектмедиадисаблед</span><span class="sxs-lookup"><span data-stu-id="4b66c-234">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="4b66c-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-235">Boolean</span></span>|<span data-ttu-id="4b66c-236">Указывает, должно ли устройство отображать экранную заставку при воспроизведении аудио-и видеоконференций в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="4b66c-236">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="4b66c-237">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="4b66c-237">kioskModeApps</span></span>|<span data-ttu-id="4b66c-238">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="4b66c-238">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4b66c-239">Список управляемых приложений, которые будут отображаться, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4b66c-239">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="4b66c-240">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4b66c-240">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4b66c-241">киоскмодеваллпаперурл</span><span class="sxs-lookup"><span data-stu-id="4b66c-241">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="4b66c-242">String</span><span class="sxs-lookup"><span data-stu-id="4b66c-242">String</span></span>|<span data-ttu-id="4b66c-243">URL-адрес общедоступного изображения, которое будет использоваться для фонового рисунка, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4b66c-243">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="4b66c-244">киоскмодикситкоде</span><span class="sxs-lookup"><span data-stu-id="4b66c-244">kioskModeExitCode</span></span>|<span data-ttu-id="4b66c-245">String</span><span class="sxs-lookup"><span data-stu-id="4b66c-245">String</span></span>|<span data-ttu-id="4b66c-246">Код выхода, позволяющий пользователю выходить из режима киоска, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4b66c-246">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="4b66c-247">киоскмодевиртуалхомебуттоненаблед</span><span class="sxs-lookup"><span data-stu-id="4b66c-247">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="4b66c-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-248">Boolean</span></span>|<span data-ttu-id="4b66c-249">Указывает, следует ли отображать кнопку виртуальной домашней страницы, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4b66c-249">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="4b66c-250">киоскмодевиртуалхомебуттонтипе</span><span class="sxs-lookup"><span data-stu-id="4b66c-250">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="4b66c-251">андроиддевицеовнервиртуалхомебуттонтипе</span><span class="sxs-lookup"><span data-stu-id="4b66c-251">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="4b66c-252">Указывает, является ли кнопка "Виртуальная Домашняя страница" кнопкой "Прокрутка вверх" или плавающей кнопкой "домой".</span><span class="sxs-lookup"><span data-stu-id="4b66c-252">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="4b66c-253">Возможные значения: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="4b66c-253">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="4b66c-254">киоскмодеблуетусконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="4b66c-254">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="4b66c-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-255">Boolean</span></span>|<span data-ttu-id="4b66c-256">Указывает, следует ли запретить пользователю настраивать параметры Bluetooth в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4b66c-256">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="4b66c-257">киоскмодевификонфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="4b66c-257">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="4b66c-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-258">Boolean</span></span>|<span data-ttu-id="4b66c-259">Указывает, следует ли разрешить пользователю настраивать параметры Wi/Fi в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4b66c-259">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="4b66c-260">киоскмодефлашлигхтконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="4b66c-260">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="4b66c-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-261">Boolean</span></span>|<span data-ttu-id="4b66c-262">Указывает, следует ли разрешить пользователю использовать флашлигхт в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4b66c-262">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="4b66c-263">киоскмодемедиаволумеконфигуратионенаблед</span><span class="sxs-lookup"><span data-stu-id="4b66c-263">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="4b66c-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-264">Boolean</span></span>|<span data-ttu-id="4b66c-265">Указывает, следует ли запретить пользователю изменять громкость мультимедиа в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="4b66c-265">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="4b66c-266">микрофонефорцемуте</span><span class="sxs-lookup"><span data-stu-id="4b66c-266">microphoneForceMute</span></span>|<span data-ttu-id="4b66c-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-267">Boolean</span></span>|<span data-ttu-id="4b66c-268">Указывает, следует ли запретить разблокирование микрофона устройства.</span><span class="sxs-lookup"><span data-stu-id="4b66c-268">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="4b66c-269">нетворкескапехатчалловед</span><span class="sxs-lookup"><span data-stu-id="4b66c-269">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="4b66c-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-270">Boolean</span></span>|<span data-ttu-id="4b66c-271">Указывает, будет ли устройство разрешать подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="4b66c-271">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="4b66c-272">нфкблоккаутгоингбеам</span><span class="sxs-lookup"><span data-stu-id="4b66c-272">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="4b66c-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-273">Boolean</span></span>|<span data-ttu-id="4b66c-274">Указывает, следует ли заблокировать исходящую форму NFC.</span><span class="sxs-lookup"><span data-stu-id="4b66c-274">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="4b66c-275">пассвордблокккэйгуард</span><span class="sxs-lookup"><span data-stu-id="4b66c-275">passwordBlockKeyguard</span></span>|<span data-ttu-id="4b66c-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-276">Boolean</span></span>|<span data-ttu-id="4b66c-277">Указывает, отключен ли кэйгуард.</span><span class="sxs-lookup"><span data-stu-id="4b66c-277">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="4b66c-278">пассвордблокккэйгуардфеатурес</span><span class="sxs-lookup"><span data-stu-id="4b66c-278">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="4b66c-279">Коллекция [андроидкэйгуардфеатуре](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="4b66c-279">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="4b66c-280">Список компонентов кэйгуард устройств, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="4b66c-280">List of device keyguard features to block.</span></span> <span data-ttu-id="4b66c-281">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="4b66c-281">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="4b66c-282">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="4b66c-282">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="4b66c-283">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4b66c-283">passwordExpirationDays</span></span>|<span data-ttu-id="4b66c-284">Int32</span><span class="sxs-lookup"><span data-stu-id="4b66c-284">Int32</span></span>|<span data-ttu-id="4b66c-285">Указывает время в секундах, в течение которого можно задать пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="4b66c-285">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="4b66c-286">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="4b66c-286">Valid values 1 to 365</span></span>|
|<span data-ttu-id="4b66c-287">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4b66c-287">passwordMinimumLength</span></span>|<span data-ttu-id="4b66c-288">Int32</span><span class="sxs-lookup"><span data-stu-id="4b66c-288">Int32</span></span>|<span data-ttu-id="4b66c-289">Указывает минимальную длину пароля, необходимого для устройства.</span><span class="sxs-lookup"><span data-stu-id="4b66c-289">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="4b66c-290">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="4b66c-290">Valid values 4 to 16</span></span>|
|<span data-ttu-id="4b66c-291">пассвордминимумлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="4b66c-291">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="4b66c-292">Int32</span><span class="sxs-lookup"><span data-stu-id="4b66c-292">Int32</span></span>|<span data-ttu-id="4b66c-293">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="4b66c-293">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="4b66c-294">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="4b66c-294">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4b66c-295">пассвордминимумловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="4b66c-295">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="4b66c-296">Int32</span><span class="sxs-lookup"><span data-stu-id="4b66c-296">Int32</span></span>|<span data-ttu-id="4b66c-297">Указывает минимальное число символов нижнего регистра, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="4b66c-297">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="4b66c-298">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="4b66c-298">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4b66c-299">пассвордминимумнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="4b66c-299">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="4b66c-300">Int32</span><span class="sxs-lookup"><span data-stu-id="4b66c-300">Int32</span></span>|<span data-ttu-id="4b66c-301">Указывает минимальное количество небуквенных символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="4b66c-301">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="4b66c-302">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="4b66c-302">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4b66c-303">пассвордминимумнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="4b66c-303">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="4b66c-304">Int32</span><span class="sxs-lookup"><span data-stu-id="4b66c-304">Int32</span></span>|<span data-ttu-id="4b66c-305">Указывает минимальное количество числовых символов, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="4b66c-305">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="4b66c-306">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="4b66c-306">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4b66c-307">пассвордминимумсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="4b66c-307">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="4b66c-308">Int32</span><span class="sxs-lookup"><span data-stu-id="4b66c-308">Int32</span></span>|<span data-ttu-id="4b66c-309">Указывает минимальное число символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="4b66c-309">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="4b66c-310">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="4b66c-310">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4b66c-311">пассвордминимумупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="4b66c-311">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="4b66c-312">Int32</span><span class="sxs-lookup"><span data-stu-id="4b66c-312">Int32</span></span>|<span data-ttu-id="4b66c-313">Указывает минимальное число символов верхнего каселеттер, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="4b66c-313">Indicates the minimum number of upper caseletter characters required for device password.</span></span> <span data-ttu-id="4b66c-314">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="4b66c-314">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4b66c-315">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4b66c-315">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4b66c-316">Int32</span><span class="sxs-lookup"><span data-stu-id="4b66c-316">Int32</span></span>|<span data-ttu-id="4b66c-317">Миллисекунды бездействия до истечения времени ожидания экрана.</span><span class="sxs-lookup"><span data-stu-id="4b66c-317">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="4b66c-318">пассвордпревиауспассвордкаунттоблокк</span><span class="sxs-lookup"><span data-stu-id="4b66c-318">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="4b66c-319">Int32</span><span class="sxs-lookup"><span data-stu-id="4b66c-319">Int32</span></span>|<span data-ttu-id="4b66c-320">Указывает продолжительность истории паролей, в которой пользователь не сможет ввести новый пароль, который совпадает с любым паролем в журнале.</span><span class="sxs-lookup"><span data-stu-id="4b66c-320">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="4b66c-321">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="4b66c-321">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4b66c-322">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4b66c-322">passwordRequiredType</span></span>|[<span data-ttu-id="4b66c-323">андроиддевицеовнеррекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="4b66c-323">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="4b66c-324">Указывает минимальное качество пароля, необходимое для устройства.</span><span class="sxs-lookup"><span data-stu-id="4b66c-324">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="4b66c-325">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="4b66c-325">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="4b66c-326">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4b66c-326">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4b66c-327">Int32</span><span class="sxs-lookup"><span data-stu-id="4b66c-327">Int32</span></span>|<span data-ttu-id="4b66c-328">Указывает, сколько раз пользователь может ввести неправильный пароль до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="4b66c-328">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="4b66c-329">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="4b66c-329">Valid values 4 to 11</span></span>|
|<span data-ttu-id="4b66c-330">плайсторемоде</span><span class="sxs-lookup"><span data-stu-id="4b66c-330">playStoreMode</span></span>|[<span data-ttu-id="4b66c-331">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="4b66c-331">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="4b66c-332">Указывает режим проигрывания устройства в хранилище.</span><span class="sxs-lookup"><span data-stu-id="4b66c-332">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="4b66c-333">Возможные значения: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="4b66c-333">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="4b66c-334">сафебутблоккед</span><span class="sxs-lookup"><span data-stu-id="4b66c-334">safeBootBlocked</span></span>|<span data-ttu-id="4b66c-335">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-335">Boolean</span></span>|<span data-ttu-id="4b66c-336">Указывает, отключена ли загрузка устройства в "безопасная загрузка".</span><span class="sxs-lookup"><span data-stu-id="4b66c-336">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="4b66c-337">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="4b66c-337">screenCaptureBlocked</span></span>|<span data-ttu-id="4b66c-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-338">Boolean</span></span>|<span data-ttu-id="4b66c-339">Указывает, следует ли отключить возможность использования снимков экрана.</span><span class="sxs-lookup"><span data-stu-id="4b66c-339">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="4b66c-340">секуритялловдебуггингфеатурес</span><span class="sxs-lookup"><span data-stu-id="4b66c-340">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="4b66c-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-341">Boolean</span></span>|<span data-ttu-id="4b66c-342">Указывает, следует ли запретить пользователю включать функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4b66c-342">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="4b66c-343">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="4b66c-343">securityRequireVerifyApps</span></span>|<span data-ttu-id="4b66c-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-344">Boolean</span></span>|<span data-ttu-id="4b66c-345">Указывает, требуется ли проверка приложений.</span><span class="sxs-lookup"><span data-stu-id="4b66c-345">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="4b66c-346">статусбарблоккед</span><span class="sxs-lookup"><span data-stu-id="4b66c-346">statusBarBlocked</span></span>|<span data-ttu-id="4b66c-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-347">Boolean</span></span>|<span data-ttu-id="4b66c-348">Указывает, отключена ли строка состояния, в том числе уведомления, быстрые параметры и другие наложение экрана.</span><span class="sxs-lookup"><span data-stu-id="4b66c-348">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="4b66c-349">стайонмодес</span><span class="sxs-lookup"><span data-stu-id="4b66c-349">stayOnModes</span></span>|<span data-ttu-id="4b66c-350">Коллекция [андроиддевицеовнербаттериплугжедмоде](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="4b66c-350">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="4b66c-351">Список режимов, в которых дисплей устройства остается включенным.</span><span class="sxs-lookup"><span data-stu-id="4b66c-351">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="4b66c-352">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="4b66c-352">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="4b66c-353">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="4b66c-353">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="4b66c-354">сторажеалловусб</span><span class="sxs-lookup"><span data-stu-id="4b66c-354">storageAllowUsb</span></span>|<span data-ttu-id="4b66c-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-355">Boolean</span></span>|<span data-ttu-id="4b66c-356">Указывает, следует ли разрешить запоминающее устройство USB.</span><span class="sxs-lookup"><span data-stu-id="4b66c-356">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="4b66c-357">сторажеблоккекстерналмедиа</span><span class="sxs-lookup"><span data-stu-id="4b66c-357">storageBlockExternalMedia</span></span>|<span data-ttu-id="4b66c-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-358">Boolean</span></span>|<span data-ttu-id="4b66c-359">Указывает, следует ли заблокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="4b66c-359">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="4b66c-360">сторажеблоккусбфилетрансфер</span><span class="sxs-lookup"><span data-stu-id="4b66c-360">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="4b66c-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-361">Boolean</span></span>|<span data-ttu-id="4b66c-362">Указывает, следует ли запретить передачу файлов через USB.</span><span class="sxs-lookup"><span data-stu-id="4b66c-362">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="4b66c-363">системупдатевиндовстартминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="4b66c-363">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="4b66c-364">Int32</span><span class="sxs-lookup"><span data-stu-id="4b66c-364">Int32</span></span>|<span data-ttu-id="4b66c-365">Указывает количество минут после полуночи, когда запустится окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="4b66c-365">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="4b66c-366">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="4b66c-366">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="4b66c-367">системупдатевиндовендминутесафтермиднигхт</span><span class="sxs-lookup"><span data-stu-id="4b66c-367">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="4b66c-368">Int32</span><span class="sxs-lookup"><span data-stu-id="4b66c-368">Int32</span></span>|<span data-ttu-id="4b66c-369">Указывает количество минут после полуночи, в течение которого будет завершено окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="4b66c-369">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="4b66c-370">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="4b66c-370">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="4b66c-371">системупдатеинсталлтипе</span><span class="sxs-lookup"><span data-stu-id="4b66c-371">systemUpdateInstallType</span></span>|[<span data-ttu-id="4b66c-372">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="4b66c-372">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="4b66c-373">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="4b66c-373">The type of system update configuration.</span></span> <span data-ttu-id="4b66c-374">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="4b66c-374">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="4b66c-375">системвиндовсблоккед</span><span class="sxs-lookup"><span data-stu-id="4b66c-375">systemWindowsBlocked</span></span>|<span data-ttu-id="4b66c-376">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-376">Boolean</span></span>|<span data-ttu-id="4b66c-377">Указывает, следует ли заблокировать окна командной строки системы Android, например, уведомления, телефонные действия и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="4b66c-377">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="4b66c-378">усерсблоккадд</span><span class="sxs-lookup"><span data-stu-id="4b66c-378">usersBlockAdd</span></span>|<span data-ttu-id="4b66c-379">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-379">Boolean</span></span>|<span data-ttu-id="4b66c-380">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="4b66c-380">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="4b66c-381">усерсблоккремове</span><span class="sxs-lookup"><span data-stu-id="4b66c-381">usersBlockRemove</span></span>|<span data-ttu-id="4b66c-382">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-382">Boolean</span></span>|<span data-ttu-id="4b66c-383">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="4b66c-383">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="4b66c-384">волумеблоккаджустмент</span><span class="sxs-lookup"><span data-stu-id="4b66c-384">volumeBlockAdjustment</span></span>|<span data-ttu-id="4b66c-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-385">Boolean</span></span>|<span data-ttu-id="4b66c-386">Указывает, отключена ли настройка главного тома.</span><span class="sxs-lookup"><span data-stu-id="4b66c-386">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="4b66c-387">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="4b66c-387">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="4b66c-388">String</span><span class="sxs-lookup"><span data-stu-id="4b66c-388">String</span></span>|<span data-ttu-id="4b66c-389">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="4b66c-389">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="4b66c-390">впналвайсонлоккдовнмоде</span><span class="sxs-lookup"><span data-stu-id="4b66c-390">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="4b66c-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-391">Boolean</span></span>|<span data-ttu-id="4b66c-392">Указывает, следует ли блокировать сетевой трафик при отключении VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="4b66c-392">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="4b66c-393">вифиблоккедитконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="4b66c-393">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="4b66c-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-394">Boolean</span></span>|<span data-ttu-id="4b66c-395">Указывает, следует ли запретить пользователю редактировать параметры подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="4b66c-395">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="4b66c-396">вифиблоккедитполицидефинедконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="4b66c-396">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="4b66c-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b66c-397">Boolean</span></span>|<span data-ttu-id="4b66c-398">Указывает, следует ли запретить пользователю редактировать только сети, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="4b66c-398">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="4b66c-399">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b66c-399">Response</span></span>
<span data-ttu-id="4b66c-400">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b66c-400">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b66c-401">Пример</span><span class="sxs-lookup"><span data-stu-id="4b66c-401">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b66c-402">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b66c-402">Request</span></span>
<span data-ttu-id="4b66c-403">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b66c-403">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4123

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

### <a name="response"></a><span data-ttu-id="4b66c-404">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b66c-404">Response</span></span>
<span data-ttu-id="4b66c-p136">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b66c-p136">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4295

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






