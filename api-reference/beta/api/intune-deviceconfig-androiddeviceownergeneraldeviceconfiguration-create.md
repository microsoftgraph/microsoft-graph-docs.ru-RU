---
title: Создание androidDeviceOwnerGeneralDeviceConfiguration
description: Создание объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a3076636b8961a93bd6a9313070514942fbfb3a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156170"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="731db-103">Создание androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="731db-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="731db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="731db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="731db-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="731db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="731db-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="731db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="731db-107">Создание объекта [androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="731db-107">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="731db-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="731db-108">Prerequisites</span></span>
<span data-ttu-id="731db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="731db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="731db-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="731db-111">Permission type</span></span>|<span data-ttu-id="731db-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="731db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="731db-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="731db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="731db-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="731db-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="731db-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="731db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="731db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="731db-116">Not supported.</span></span>|
|<span data-ttu-id="731db-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="731db-117">Application</span></span>|<span data-ttu-id="731db-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="731db-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="731db-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="731db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="731db-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="731db-120">Request headers</span></span>
|<span data-ttu-id="731db-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="731db-121">Header</span></span>|<span data-ttu-id="731db-122">Значение</span><span class="sxs-lookup"><span data-stu-id="731db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="731db-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="731db-123">Authorization</span></span>|<span data-ttu-id="731db-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="731db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="731db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="731db-125">Accept</span></span>|<span data-ttu-id="731db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="731db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="731db-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="731db-127">Request body</span></span>
<span data-ttu-id="731db-128">В теле запроса предоставляем представление объекта androidDeviceOwnerGeneralDeviceConfiguration в JSON.</span><span class="sxs-lookup"><span data-stu-id="731db-128">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="731db-129">В следующей таблице показаны свойства, необходимые при создании объекта androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="731db-129">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="731db-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="731db-130">Property</span></span>|<span data-ttu-id="731db-131">Тип</span><span class="sxs-lookup"><span data-stu-id="731db-131">Type</span></span>|<span data-ttu-id="731db-132">Описание</span><span class="sxs-lookup"><span data-stu-id="731db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="731db-133">id</span><span class="sxs-lookup"><span data-stu-id="731db-133">id</span></span>|<span data-ttu-id="731db-134">String</span><span class="sxs-lookup"><span data-stu-id="731db-134">String</span></span>|<span data-ttu-id="731db-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="731db-135">Key of the entity.</span></span> <span data-ttu-id="731db-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731db-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731db-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="731db-137">lastModifiedDateTime</span></span>|<span data-ttu-id="731db-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="731db-138">DateTimeOffset</span></span>|<span data-ttu-id="731db-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="731db-139">DateTime the object was last modified.</span></span> <span data-ttu-id="731db-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731db-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731db-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="731db-141">roleScopeTagIds</span></span>|<span data-ttu-id="731db-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="731db-142">String collection</span></span>|<span data-ttu-id="731db-143">Список тегов области для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="731db-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="731db-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731db-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731db-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="731db-145">supportsScopeTags</span></span>|<span data-ttu-id="731db-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-146">Boolean</span></span>|<span data-ttu-id="731db-147">Указывает, поддерживает ли конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="731db-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="731db-148">Назначение свойству ScopeTags не допускается, если это значение имеет значение false, а сущности не будут видны пользователям с заданной областью действия.</span><span class="sxs-lookup"><span data-stu-id="731db-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="731db-149">Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить, удавшись и повторно создав политику на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="731db-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="731db-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="731db-150">This property is read-only.</span></span> <span data-ttu-id="731db-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731db-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731db-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="731db-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="731db-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="731db-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="731db-154">Применимость выпуска ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="731db-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="731db-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731db-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731db-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="731db-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="731db-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="731db-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="731db-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="731db-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="731db-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731db-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731db-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="731db-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="731db-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="731db-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="731db-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="731db-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="731db-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731db-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731db-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="731db-164">createdDateTime</span></span>|<span data-ttu-id="731db-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="731db-165">DateTimeOffset</span></span>|<span data-ttu-id="731db-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="731db-166">DateTime the object was created.</span></span> <span data-ttu-id="731db-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731db-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731db-168">description</span><span class="sxs-lookup"><span data-stu-id="731db-168">description</span></span>|<span data-ttu-id="731db-169">String</span><span class="sxs-lookup"><span data-stu-id="731db-169">String</span></span>|<span data-ttu-id="731db-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="731db-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="731db-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731db-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731db-172">displayName</span><span class="sxs-lookup"><span data-stu-id="731db-172">displayName</span></span>|<span data-ttu-id="731db-173">String</span><span class="sxs-lookup"><span data-stu-id="731db-173">String</span></span>|<span data-ttu-id="731db-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="731db-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="731db-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731db-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731db-176">version</span><span class="sxs-lookup"><span data-stu-id="731db-176">version</span></span>|<span data-ttu-id="731db-177">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-177">Int32</span></span>|<span data-ttu-id="731db-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="731db-178">Version of the device configuration.</span></span> <span data-ttu-id="731db-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731db-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731db-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="731db-180">accountsBlockModification</span></span>|<span data-ttu-id="731db-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-181">Boolean</span></span>|<span data-ttu-id="731db-182">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="731db-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="731db-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="731db-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="731db-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-184">Boolean</span></span>|<span data-ttu-id="731db-185">Указывает, разрешено ли пользователю включить параметр неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="731db-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="731db-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="731db-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="731db-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="731db-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="731db-188">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="731db-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="731db-189">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="731db-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="731db-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="731db-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="731db-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="731db-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="731db-192">Указывает политику разрешений для запросов разрешений во время работы, если она не определена для конкретного приложения.</span><span class="sxs-lookup"><span data-stu-id="731db-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="731db-193">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="731db-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="731db-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="731db-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="731db-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-195">Boolean</span></span>|<span data-ttu-id="731db-196">Следует ли рекомендовать всем приложениям пропускать любые добавленные подсказки о первом использовании.</span><span class="sxs-lookup"><span data-stu-id="731db-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="731db-197">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="731db-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="731db-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-198">Boolean</span></span>|<span data-ttu-id="731db-199">Указывает, следует ли заблокировать для пользователя настройку Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="731db-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="731db-200">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="731db-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="731db-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-201">Boolean</span></span>|<span data-ttu-id="731db-202">Указывает, следует ли заблокировать для пользователя общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="731db-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="731db-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="731db-203">cameraBlocked</span></span>|<span data-ttu-id="731db-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-204">Boolean</span></span>|<span data-ttu-id="731db-205">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="731db-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="731db-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="731db-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="731db-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-207">Boolean</span></span>|<span data-ttu-id="731db-208">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="731db-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="731db-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="731db-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="731db-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-210">Boolean</span></span>|<span data-ttu-id="731db-211">Указывает, следует ли заблокировать для пользователей какие-либо настройки учетных данных сертификата.</span><span class="sxs-lookup"><span data-stu-id="731db-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="731db-212">microsoftLauncherConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="731db-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="731db-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-213">Boolean</span></span>|<span data-ttu-id="731db-214">Указывает, нужно ли настраивать microsoft Launcher.</span><span class="sxs-lookup"><span data-stu-id="731db-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="731db-215">microsoftLauncherCustomWallpaperEnabled</span><span class="sxs-lookup"><span data-stu-id="731db-215">microsoftLauncherCustomWallpaperEnabled</span></span>|<span data-ttu-id="731db-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-216">Boolean</span></span>|<span data-ttu-id="731db-217">Указывает, следует ли настраивать фоновый фон на целевых устройствах.</span><span class="sxs-lookup"><span data-stu-id="731db-217">Indicates whether or not to configure the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="731db-218">microsoftLauncherCustomWallpaperImageUrl</span><span class="sxs-lookup"><span data-stu-id="731db-218">microsoftLauncherCustomWallpaperImageUrl</span></span>|<span data-ttu-id="731db-219">String</span><span class="sxs-lookup"><span data-stu-id="731db-219">String</span></span>|<span data-ttu-id="731db-220">Указывает URL-адрес файла изображения, который будет использовать в качестве фона на целевых устройствах.</span><span class="sxs-lookup"><span data-stu-id="731db-220">Indicates the URL for the image file to use as the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="731db-221">microsoftLauncherCustomWallpaperAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="731db-221">microsoftLauncherCustomWallpaperAllowUserModification</span></span>|<span data-ttu-id="731db-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-222">Boolean</span></span>|<span data-ttu-id="731db-223">Указывает, может ли пользователь изменить фоновый фон для персонализации устройства.</span><span class="sxs-lookup"><span data-stu-id="731db-223">Indicates whether or not the user can modify the wallpaper to personalize their device.</span></span>|
|<span data-ttu-id="731db-224">microsoftLauncherFeedEnabled</span><span class="sxs-lookup"><span data-stu-id="731db-224">microsoftLauncherFeedEnabled</span></span>|<span data-ttu-id="731db-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-225">Boolean</span></span>|<span data-ttu-id="731db-226">Указывает, следует ли включить канал запуска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="731db-226">Indicates whether or not you want to enable the launcher feed on the device.</span></span>|
|<span data-ttu-id="731db-227">microsoftLauncherFeedAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="731db-227">microsoftLauncherFeedAllowUserModification</span></span>|<span data-ttu-id="731db-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-228">Boolean</span></span>|<span data-ttu-id="731db-229">Указывает, может ли пользователь изменить канал запуска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="731db-229">Indicates whether or not the user can modify the launcher feed on the device.</span></span>|
|<span data-ttu-id="731db-230">microsoftLauncherDockPresenceConfiguration</span><span class="sxs-lookup"><span data-stu-id="731db-230">microsoftLauncherDockPresenceConfiguration</span></span>|[<span data-ttu-id="731db-231">microsoftLauncherDockPresence</span><span class="sxs-lookup"><span data-stu-id="731db-231">microsoftLauncherDockPresence</span></span>](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|<span data-ttu-id="731db-232">Указывает, нужно ли настраивать док-станцию устройства.</span><span class="sxs-lookup"><span data-stu-id="731db-232">Indicates whether or not you want to configure the device dock.</span></span> <span data-ttu-id="731db-233">Возможные значения: `notConfigured`, `show`, `hide`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="731db-233">Possible values are: `notConfigured`, `show`, `hide`, `disabled`.</span></span>|
|<span data-ttu-id="731db-234">microsoftLauncherDockPresenceAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="731db-234">microsoftLauncherDockPresenceAllowUserModification</span></span>|<span data-ttu-id="731db-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-235">Boolean</span></span>|<span data-ttu-id="731db-236">Указывает, может ли пользователь изменить конфигурацию док-станции устройства на устройстве.</span><span class="sxs-lookup"><span data-stu-id="731db-236">Indicates whether or not the user can modify the device dock configuration on the device.</span></span>|
|<span data-ttu-id="731db-237">microsoftLauncherSearchBarPlacementConfiguration</span><span class="sxs-lookup"><span data-stu-id="731db-237">microsoftLauncherSearchBarPlacementConfiguration</span></span>|[<span data-ttu-id="731db-238">microsoftLauncherSearchBarPlacement</span><span class="sxs-lookup"><span data-stu-id="731db-238">microsoftLauncherSearchBarPlacement</span></span>](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|<span data-ttu-id="731db-239">Указывает конфигурацию размещения панели поиска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="731db-239">Indicates the search bar placement configuration on the device.</span></span> <span data-ttu-id="731db-240">Возможные значения: `notConfigured`, `top`, `bottom`, `hide`.</span><span class="sxs-lookup"><span data-stu-id="731db-240">Possible values are: `notConfigured`, `top`, `bottom`, `hide`.</span></span>|
|<span data-ttu-id="731db-241">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="731db-241">enrollmentProfile</span></span>|[<span data-ttu-id="731db-242">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="731db-242">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="731db-243">Указывает профиль регистрации, который необходимо настроить.</span><span class="sxs-lookup"><span data-stu-id="731db-243">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="731db-244">Возможные значения: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span><span class="sxs-lookup"><span data-stu-id="731db-244">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="731db-245">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="731db-245">dataRoamingBlocked</span></span>|<span data-ttu-id="731db-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-246">Boolean</span></span>|<span data-ttu-id="731db-247">Указывает, следует ли заблокировать для пользователя роуминг данных.</span><span class="sxs-lookup"><span data-stu-id="731db-247">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="731db-248">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="731db-248">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="731db-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-249">Boolean</span></span>|<span data-ttu-id="731db-250">Указывает, следует ли заблокировать вручную изменение даты или времени на устройстве</span><span class="sxs-lookup"><span data-stu-id="731db-250">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="731db-251">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="731db-251">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="731db-252">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="731db-252">String collection</span></span>|<span data-ttu-id="731db-253">Список сообщений электронной почты учетной записи Google, которые потребуются для проверки подлинности после сброса заводской настройки устройства.</span><span class="sxs-lookup"><span data-stu-id="731db-253">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="731db-254">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="731db-254">factoryResetBlocked</span></span>|<span data-ttu-id="731db-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-255">Boolean</span></span>|<span data-ttu-id="731db-256">Указывает, отключен ли параметр сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="731db-256">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="731db-257">globalProxy</span><span class="sxs-lookup"><span data-stu-id="731db-257">globalProxy</span></span>|[<span data-ttu-id="731db-258">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="731db-258">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="731db-259">Прокси-сервер настроен непосредственно с хост-сервером, портом и исключенными хостами.</span><span class="sxs-lookup"><span data-stu-id="731db-259">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="731db-260">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="731db-260">googleAccountsBlocked</span></span>|<span data-ttu-id="731db-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-261">Boolean</span></span>|<span data-ttu-id="731db-262">Указывает, будут ли заблокированы учетные записи Google.</span><span class="sxs-lookup"><span data-stu-id="731db-262">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="731db-263">kioskCustomizationDeviceSettingsBlocked</span><span class="sxs-lookup"><span data-stu-id="731db-263">kioskCustomizationDeviceSettingsBlocked</span></span>|<span data-ttu-id="731db-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-264">Boolean</span></span>|<span data-ttu-id="731db-265">Указывает, может ли пользователь получить доступ к приложению "Параметры" устройства в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-265">Indicates whether a user can access the device's Settings app while in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-266">kioskCustomizationPowerButtonActionsBlocked</span><span class="sxs-lookup"><span data-stu-id="731db-266">kioskCustomizationPowerButtonActionsBlocked</span></span>|<span data-ttu-id="731db-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-267">Boolean</span></span>|<span data-ttu-id="731db-268">Отображается ли меню питания, когда пользователь долго нажимает кнопку питания устройства в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-268">Whether the power menu is shown when a user long presses the Power button of a device in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-269">kioskCustomizationStatusBar</span><span class="sxs-lookup"><span data-stu-id="731db-269">kioskCustomizationStatusBar</span></span>|[<span data-ttu-id="731db-270">androidDeviceOwnerKioskCustomizationStatusBar</span><span class="sxs-lookup"><span data-stu-id="731db-270">androidDeviceOwnerKioskCustomizationStatusBar</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|<span data-ttu-id="731db-271">Указывает, отключены ли системные сведения и уведомления в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-271">Indicates whether system info and notifications are disabled in Kiosk Mode.</span></span> <span data-ttu-id="731db-272">Возможные значения: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.</span><span class="sxs-lookup"><span data-stu-id="731db-272">Possible values are: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.</span></span>|
|<span data-ttu-id="731db-273">kioskCustomizationSystemErrorWarnings</span><span class="sxs-lookup"><span data-stu-id="731db-273">kioskCustomizationSystemErrorWarnings</span></span>|<span data-ttu-id="731db-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-274">Boolean</span></span>|<span data-ttu-id="731db-275">Указывает, показываются ли диалоги системных ошибок для приложений, сбой или неотвеживающие приложения, в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-275">Indicates whether system error dialogs for crashed or unresponsive apps are shown in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-276">kioskCustomizationSystemNavigation</span><span class="sxs-lookup"><span data-stu-id="731db-276">kioskCustomizationSystemNavigation</span></span>|[<span data-ttu-id="731db-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span><span class="sxs-lookup"><span data-stu-id="731db-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|<span data-ttu-id="731db-278">Указывает, какие функции навигации включены в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-278">Indicates which navigation features are enabled in Kiosk Mode.</span></span> <span data-ttu-id="731db-279">Возможные значения: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.</span><span class="sxs-lookup"><span data-stu-id="731db-279">Possible values are: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.</span></span>|
|<span data-ttu-id="731db-280">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="731db-280">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="731db-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-281">Boolean</span></span>|<span data-ttu-id="731db-282">Следует ли включить режим сохранения экрана или нет в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="731db-282">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-283">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="731db-283">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="731db-284">String</span><span class="sxs-lookup"><span data-stu-id="731db-284">String</span></span>|<span data-ttu-id="731db-285">URL-адрес изображения, которое будет сохранения экрана устройства в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-285">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-286">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="731db-286">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="731db-287">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-287">Int32</span></span>|<span data-ttu-id="731db-288">Время в секундах, в течение которое устройство отобразит режим сохранения экрана в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-288">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="731db-289">Допустимые значения: от 0 до 999 999 999</span><span class="sxs-lookup"><span data-stu-id="731db-289">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="731db-290">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="731db-290">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="731db-291">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-291">Int32</span></span>|<span data-ttu-id="731db-292">Время в секундах, в течение которое устройство должно быть неактивным, прежде чем режим сохранения экрана будет показан в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-292">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="731db-293">Допустимые значения: от 1 до 999 999 999</span><span class="sxs-lookup"><span data-stu-id="731db-293">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="731db-294">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="731db-294">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="731db-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-295">Boolean</span></span>|<span data-ttu-id="731db-296">Должен ли экран устройства показывать режим сохранения экрана, если воспроизведение звука и видео в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-296">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-297">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="731db-297">kioskModeApps</span></span>|<span data-ttu-id="731db-298">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="731db-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="731db-299">Список управляемых приложений, которые будут показаны, когда устройство находится в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-299">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="731db-300">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="731db-300">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="731db-301">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="731db-301">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="731db-302">String</span><span class="sxs-lookup"><span data-stu-id="731db-302">String</span></span>|<span data-ttu-id="731db-303">URL-адрес общедоступных изображений, которые будут использовать для фона, когда устройство находится в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-303">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-304">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="731db-304">kioskModeExitCode</span></span>|<span data-ttu-id="731db-305">String</span><span class="sxs-lookup"><span data-stu-id="731db-305">String</span></span>|<span data-ttu-id="731db-306">Код выхода, позволяющий пользователю выйти из режима терминала, когда устройство находится в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-306">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-307">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="731db-307">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="731db-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-308">Boolean</span></span>|<span data-ttu-id="731db-309">Следует ли отображать виртуальную кнопку "Домой", когда устройство находится в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-309">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-310">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="731db-310">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="731db-311">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="731db-311">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="731db-312">Указывает, является ли виртуальная кнопка "Домой" кнопкой прокрутки вверх или с плавающей кнопкой "Домой".</span><span class="sxs-lookup"><span data-stu-id="731db-312">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="731db-313">Возможные значения: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="731db-313">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="731db-314">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="731db-314">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="731db-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-315">Boolean</span></span>|<span data-ttu-id="731db-316">Позволяет ли пользователь настраивать параметры Bluetooth режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-316">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-317">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="731db-317">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="731db-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-318">Boolean</span></span>|<span data-ttu-id="731db-319">Позволяет ли пользователь настраивать параметры Wi-Fi режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-319">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-320">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="731db-320">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="731db-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-321">Boolean</span></span>|<span data-ttu-id="731db-322">Разрешается ли пользователю использовать фонарик в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-322">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-323">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="731db-323">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="731db-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-324">Boolean</span></span>|<span data-ttu-id="731db-325">Позволяет ли пользователь изменять громкость мультимедиа в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-325">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-326">kioskModeShowDeviceInfo</span><span class="sxs-lookup"><span data-stu-id="731db-326">kioskModeShowDeviceInfo</span></span>|<span data-ttu-id="731db-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-327">Boolean</span></span>|<span data-ttu-id="731db-328">Следует ли разрешить пользователю доступ к базовым сведениям об устройстве.</span><span class="sxs-lookup"><span data-stu-id="731db-328">Whether or not to allow a user to access basic device information.</span></span>|
|<span data-ttu-id="731db-329">kioskModeManagedSettingsEntryDisabled</span><span class="sxs-lookup"><span data-stu-id="731db-329">kioskModeManagedSettingsEntryDisabled</span></span>|<span data-ttu-id="731db-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-330">Boolean</span></span>|<span data-ttu-id="731db-331">Следует ли отображать точку входа управляемых параметров на управляемом начальном экране в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-331">Whether or not to display the Managed Settings entry point on the managed home screen in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-332">kioskModeDebugMenuEasyAccessEnabled</span><span class="sxs-lookup"><span data-stu-id="731db-332">kioskModeDebugMenuEasyAccessEnabled</span></span>|<span data-ttu-id="731db-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-333">Boolean</span></span>|<span data-ttu-id="731db-334">Позволяет ли пользователю легко получать доступ к меню отлаживания в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-334">Whether or not to allow a user to easy access to the debug menu in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-335">kioskModeShowAppNotificationBadge</span><span class="sxs-lookup"><span data-stu-id="731db-335">kioskModeShowAppNotificationBadge</span></span>|<span data-ttu-id="731db-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-336">Boolean</span></span>|<span data-ttu-id="731db-337">Следует ли отображать индикаторы событий уведомлений приложения в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-337">Whether or not to display application notification badges in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-338">kioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="731db-338">kioskModeScreenOrientation</span></span>|[<span data-ttu-id="731db-339">androidDeviceOwnerKioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="731db-339">androidDeviceOwnerKioskModeScreenOrientation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|<span data-ttu-id="731db-340">Настройка ориентации экрана для управляемого домашнего экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="731db-340">Screen orientation configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="731db-341">Возможные значения: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span><span class="sxs-lookup"><span data-stu-id="731db-341">Possible values are: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span></span>|
|<span data-ttu-id="731db-342">kioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="731db-342">kioskModeIconSize</span></span>|[<span data-ttu-id="731db-343">androidDeviceOwnerKioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="731db-343">androidDeviceOwnerKioskModeIconSize</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|<span data-ttu-id="731db-344">Конфигурация размера значка для управляемого домашнего экрана в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-344">Icon size configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="731db-345">Возможные значения: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span><span class="sxs-lookup"><span data-stu-id="731db-345">Possible values are: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span></span>|
|<span data-ttu-id="731db-346">kioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="731db-346">kioskModeFolderIcon</span></span>|[<span data-ttu-id="731db-347">androidDeviceOwnerKioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="731db-347">androidDeviceOwnerKioskModeFolderIcon</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|<span data-ttu-id="731db-348">Настройка значков папок для управляемого домашнего экрана в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-348">Folder icon configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="731db-349">Возможные значения: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span><span class="sxs-lookup"><span data-stu-id="731db-349">Possible values are: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span></span>|
|<span data-ttu-id="731db-350">kioskModeWifiAllowedSsids</span><span class="sxs-lookup"><span data-stu-id="731db-350">kioskModeWifiAllowedSsids</span></span>|<span data-ttu-id="731db-351">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="731db-351">String collection</span></span>|<span data-ttu-id="731db-352">Ограниченный набор SSID WIFI, доступный пользователю для настройки в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-352">The restricted set of WIFI SSIDs available for the user to configure in Kiosk Mode.</span></span> <span data-ttu-id="731db-353">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="731db-353">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="731db-354">kioskModeAppOrderEnabled</span><span class="sxs-lookup"><span data-stu-id="731db-354">kioskModeAppOrderEnabled</span></span>|<span data-ttu-id="731db-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-355">Boolean</span></span>|<span data-ttu-id="731db-356">Следует ли включить порядок приложений в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-356">Whether or not to enable app ordering in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-357">kioskModeAppsInFolderOrderedByName</span><span class="sxs-lookup"><span data-stu-id="731db-357">kioskModeAppsInFolderOrderedByName</span></span>|<span data-ttu-id="731db-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-358">Boolean</span></span>|<span data-ttu-id="731db-359">Следует ли в алфавитном порядке определить приложения в папке в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-359">Whether or not to alphabetize applications within a folder in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-360">kioskModeGridHeight</span><span class="sxs-lookup"><span data-stu-id="731db-360">kioskModeGridHeight</span></span>|<span data-ttu-id="731db-361">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-361">Int32</span></span>|<span data-ttu-id="731db-362">Количество строк для сетки управляемого домашнего экрана с включенным порядком приложения в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-362">Number of rows for Managed Home Screen grid with app ordering enabled in Kiosk Mode.</span></span> <span data-ttu-id="731db-363">Допустимые значения: от 1 до 999 999 999</span><span class="sxs-lookup"><span data-stu-id="731db-363">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="731db-364">kioskModeGridWidth</span><span class="sxs-lookup"><span data-stu-id="731db-364">kioskModeGridWidth</span></span>|<span data-ttu-id="731db-365">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-365">Int32</span></span>|<span data-ttu-id="731db-366">Количество столбцов для сетки управляемого домашнего экрана с включенным порядком приложения в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-366">Number of columns for Managed Home Screen grid with app ordering enabled in Kiosk Mode.</span></span> <span data-ttu-id="731db-367">Допустимые значения: от 1 до 999 999 999</span><span class="sxs-lookup"><span data-stu-id="731db-367">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="731db-368">kioskModeLockHomeScreen</span><span class="sxs-lookup"><span data-stu-id="731db-368">kioskModeLockHomeScreen</span></span>|<span data-ttu-id="731db-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-369">Boolean</span></span>|<span data-ttu-id="731db-370">Следует ли заблокировать домашний экран для пользователя в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-370">Whether or not to lock home screen to the end user in Kiosk Mode.</span></span>|
|<span data-ttu-id="731db-371">kioskModeManagedFolders</span><span class="sxs-lookup"><span data-stu-id="731db-371">kioskModeManagedFolders</span></span>|<span data-ttu-id="731db-372">[Коллекция androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md)</span><span class="sxs-lookup"><span data-stu-id="731db-372">[androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md) collection</span></span>|<span data-ttu-id="731db-373">Список управляемых папок для устройства в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-373">A list of managed folders for a device in Kiosk Mode.</span></span> <span data-ttu-id="731db-374">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="731db-374">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="731db-375">kioskModeAppPositions</span><span class="sxs-lookup"><span data-stu-id="731db-375">kioskModeAppPositions</span></span>|<span data-ttu-id="731db-376">[Коллекция androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md)</span><span class="sxs-lookup"><span data-stu-id="731db-376">[androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md) collection</span></span>|<span data-ttu-id="731db-377">Порядок элементов на управляемом домашнем экране в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="731db-377">The ordering of items on Kiosk Mode Managed Home Screen.</span></span> <span data-ttu-id="731db-378">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="731db-378">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="731db-379">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="731db-379">microphoneForceMute</span></span>|<span data-ttu-id="731db-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-380">Boolean</span></span>|<span data-ttu-id="731db-381">Указывает, следует ли заблокировать микрофон на устройстве.</span><span class="sxs-lookup"><span data-stu-id="731db-381">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="731db-382">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="731db-382">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="731db-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-383">Boolean</span></span>|<span data-ttu-id="731db-384">Указывает, разрешит ли устройство подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="731db-384">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="731db-385">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="731db-385">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="731db-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-386">Boolean</span></span>|<span data-ttu-id="731db-387">Указывает, следует ли заблокировать исходяние NFC.</span><span class="sxs-lookup"><span data-stu-id="731db-387">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="731db-388">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="731db-388">passwordBlockKeyguard</span></span>|<span data-ttu-id="731db-389">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-389">Boolean</span></span>|<span data-ttu-id="731db-390">Указывает, отключен ли keyguard.</span><span class="sxs-lookup"><span data-stu-id="731db-390">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="731db-391">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="731db-391">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="731db-392">[Коллекция androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="731db-392">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="731db-393">Список функций keyguard устройства, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="731db-393">List of device keyguard features to block.</span></span> <span data-ttu-id="731db-394">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="731db-394">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="731db-395">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="731db-395">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="731db-396">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="731db-396">passwordExpirationDays</span></span>|<span data-ttu-id="731db-397">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-397">Int32</span></span>|<span data-ttu-id="731db-398">Указывает время, в течение которого можно установить пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="731db-398">Indicates the amount of time that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="731db-399">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="731db-399">Valid values 1 to 365</span></span>|
|<span data-ttu-id="731db-400">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="731db-400">passwordMinimumLength</span></span>|<span data-ttu-id="731db-401">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-401">Int32</span></span>|<span data-ttu-id="731db-402">Указывает минимальную длину пароля, необходимого на устройстве.</span><span class="sxs-lookup"><span data-stu-id="731db-402">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="731db-403">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="731db-403">Valid values 4 to 16</span></span>|
|<span data-ttu-id="731db-404">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="731db-404">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="731db-405">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-405">Int32</span></span>|<span data-ttu-id="731db-406">Указывает минимальное количество букв, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="731db-406">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="731db-407">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="731db-407">Valid values 1 to 16</span></span>|
|<span data-ttu-id="731db-408">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="731db-408">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="731db-409">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-409">Int32</span></span>|<span data-ttu-id="731db-410">Указывает минимальное количество символов нижнего дела, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="731db-410">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="731db-411">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="731db-411">Valid values 1 to 16</span></span>|
|<span data-ttu-id="731db-412">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="731db-412">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="731db-413">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-413">Int32</span></span>|<span data-ttu-id="731db-414">Указывает минимальное количество символов, не букв, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="731db-414">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="731db-415">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="731db-415">Valid values 1 to 16</span></span>|
|<span data-ttu-id="731db-416">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="731db-416">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="731db-417">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-417">Int32</span></span>|<span data-ttu-id="731db-418">Указывает минимальное число цифр, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="731db-418">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="731db-419">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="731db-419">Valid values 1 to 16</span></span>|
|<span data-ttu-id="731db-420">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="731db-420">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="731db-421">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-421">Int32</span></span>|<span data-ttu-id="731db-422">Указывает минимальное количество символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="731db-422">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="731db-423">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="731db-423">Valid values 1 to 16</span></span>|
|<span data-ttu-id="731db-424">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="731db-424">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="731db-425">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-425">Int32</span></span>|<span data-ttu-id="731db-426">Указывает минимальное количество символов в верхнем букве, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="731db-426">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="731db-427">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="731db-427">Valid values 1 to 16</span></span>|
|<span data-ttu-id="731db-428">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="731db-428">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="731db-429">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-429">Int32</span></span>|<span data-ttu-id="731db-430">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="731db-430">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="731db-431">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="731db-431">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="731db-432">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-432">Int32</span></span>|<span data-ttu-id="731db-433">Указывает длину истории паролей, в которой пользователь не сможет ввести новый пароль, который будет таким же, как любой пароль в истории.</span><span class="sxs-lookup"><span data-stu-id="731db-433">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="731db-434">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="731db-434">Valid values 0 to 24</span></span>|
|<span data-ttu-id="731db-435">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="731db-435">passwordRequiredType</span></span>|[<span data-ttu-id="731db-436">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="731db-436">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="731db-437">Указывает минимальное качество пароля, необходимое для устройства.</span><span class="sxs-lookup"><span data-stu-id="731db-437">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="731db-438">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="731db-438">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="731db-439">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="731db-439">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="731db-440">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-440">Int32</span></span>|<span data-ttu-id="731db-441">Указывает, сколько раз пользователь может ввести неправильный пароль перед тем, как стирать устройство.</span><span class="sxs-lookup"><span data-stu-id="731db-441">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="731db-442">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="731db-442">Valid values 4 to 11</span></span>|
|<span data-ttu-id="731db-443">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="731db-443">playStoreMode</span></span>|[<span data-ttu-id="731db-444">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="731db-444">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="731db-445">Указывает режим воспроизведения устройства.</span><span class="sxs-lookup"><span data-stu-id="731db-445">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="731db-446">Возможные значения: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="731db-446">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="731db-447">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="731db-447">safeBootBlocked</span></span>|<span data-ttu-id="731db-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-448">Boolean</span></span>|<span data-ttu-id="731db-449">Указывает, отключена ли перезагрузка устройства в безопасной загрузке.</span><span class="sxs-lookup"><span data-stu-id="731db-449">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="731db-450">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="731db-450">screenCaptureBlocked</span></span>|<span data-ttu-id="731db-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-451">Boolean</span></span>|<span data-ttu-id="731db-452">Указывает, следует ли отключить возможность делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="731db-452">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="731db-453">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="731db-453">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="731db-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-454">Boolean</span></span>|<span data-ttu-id="731db-455">Указывает, следует ли заблокировать для пользователя включение функций отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="731db-455">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="731db-456">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="731db-456">securityRequireVerifyApps</span></span>|<span data-ttu-id="731db-457">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-457">Boolean</span></span>|<span data-ttu-id="731db-458">Указывает, требуются ли приложения.</span><span class="sxs-lookup"><span data-stu-id="731db-458">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="731db-459">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="731db-459">statusBarBlocked</span></span>|<span data-ttu-id="731db-460">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-460">Boolean</span></span>|<span data-ttu-id="731db-461">Указывает, отключена ли ли ни одна из них, включая уведомления, быстрые параметры и другие наложения экрана.</span><span class="sxs-lookup"><span data-stu-id="731db-461">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="731db-462">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="731db-462">stayOnModes</span></span>|<span data-ttu-id="731db-463">[Коллекция androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="731db-463">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="731db-464">Список режимов, в которых дисплей устройства будет оставаться в режиме питания.</span><span class="sxs-lookup"><span data-stu-id="731db-464">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="731db-465">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="731db-465">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="731db-466">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="731db-466">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="731db-467">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="731db-467">storageAllowUsb</span></span>|<span data-ttu-id="731db-468">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-468">Boolean</span></span>|<span data-ttu-id="731db-469">Указывает, следует ли разрешить usb-накопитель.</span><span class="sxs-lookup"><span data-stu-id="731db-469">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="731db-470">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="731db-470">storageBlockExternalMedia</span></span>|<span data-ttu-id="731db-471">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-471">Boolean</span></span>|<span data-ttu-id="731db-472">Указывает, следует ли блокировать внешние носитли.</span><span class="sxs-lookup"><span data-stu-id="731db-472">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="731db-473">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="731db-473">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="731db-474">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-474">Boolean</span></span>|<span data-ttu-id="731db-475">Указывает, следует ли заблокировать передачу USB-файла.</span><span class="sxs-lookup"><span data-stu-id="731db-475">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="731db-476">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="731db-476">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="731db-477">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-477">Int32</span></span>|<span data-ttu-id="731db-478">Указывает количество минут после полуночи, в течение чего начинается окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="731db-478">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="731db-479">Допустимые значения: от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="731db-479">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="731db-480">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="731db-480">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="731db-481">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-481">Int32</span></span>|<span data-ttu-id="731db-482">Указывает количество минут после полуночи окончания окна обновления системы.</span><span class="sxs-lookup"><span data-stu-id="731db-482">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="731db-483">Допустимые значения: от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="731db-483">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="731db-484">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="731db-484">systemUpdateInstallType</span></span>|[<span data-ttu-id="731db-485">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="731db-485">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="731db-486">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="731db-486">The type of system update configuration.</span></span> <span data-ttu-id="731db-487">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="731db-487">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="731db-488">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="731db-488">systemWindowsBlocked</span></span>|<span data-ttu-id="731db-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-489">Boolean</span></span>|<span data-ttu-id="731db-490">Следует ли блокировать окна системных подсказок Android, например всплывающие уведомления, действия с телефоном и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="731db-490">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="731db-491">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="731db-491">usersBlockAdd</span></span>|<span data-ttu-id="731db-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-492">Boolean</span></span>|<span data-ttu-id="731db-493">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="731db-493">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="731db-494">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="731db-494">usersBlockRemove</span></span>|<span data-ttu-id="731db-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-495">Boolean</span></span>|<span data-ttu-id="731db-496">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="731db-496">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="731db-497">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="731db-497">volumeBlockAdjustment</span></span>|<span data-ttu-id="731db-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-498">Boolean</span></span>|<span data-ttu-id="731db-499">Указывает, отключена ли настройка этого тома.</span><span class="sxs-lookup"><span data-stu-id="731db-499">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="731db-500">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="731db-500">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="731db-501">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-501">Boolean</span></span>|<span data-ttu-id="731db-502">Если указано имя пакета VPN, следует ли заблокировать сетевой трафик при отключении vpn.</span><span class="sxs-lookup"><span data-stu-id="731db-502">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="731db-503">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="731db-503">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="731db-504">String</span><span class="sxs-lookup"><span data-stu-id="731db-504">String</span></span>|<span data-ttu-id="731db-505">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="731db-505">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="731db-506">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="731db-506">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="731db-507">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-507">Boolean</span></span>|<span data-ttu-id="731db-508">Указывает, следует ли заблокировать для пользователя изменение параметров подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="731db-508">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="731db-509">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="731db-509">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="731db-510">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-510">Boolean</span></span>|<span data-ttu-id="731db-511">Указывает, следует ли заблокировать для пользователя редактирование только сетей, определенных политикой.</span><span class="sxs-lookup"><span data-stu-id="731db-511">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|
|<span data-ttu-id="731db-512">personalProfileAppsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="731db-512">personalProfileAppsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="731db-513">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-513">Boolean</span></span>|<span data-ttu-id="731db-514">Указывает, может ли пользователь устанавливать приложения из неизвестных источников в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="731db-514">Indicates whether the user can install apps from unknown sources on the personal profile.</span></span>|
|<span data-ttu-id="731db-515">personalProfileCameraBlocked</span><span class="sxs-lookup"><span data-stu-id="731db-515">personalProfileCameraBlocked</span></span>|<span data-ttu-id="731db-516">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-516">Boolean</span></span>|<span data-ttu-id="731db-517">Указывает, следует ли отключить использование камеры в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="731db-517">Indicates whether to disable the use of the camera on the personal profile.</span></span>|
|<span data-ttu-id="731db-518">personalProfileScreenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="731db-518">personalProfileScreenCaptureBlocked</span></span>|<span data-ttu-id="731db-519">Boolean</span><span class="sxs-lookup"><span data-stu-id="731db-519">Boolean</span></span>|<span data-ttu-id="731db-520">Указывает, следует ли отключить возможность делать снимки экрана в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="731db-520">Indicates whether to disable the capability to take screenshots on the personal profile.</span></span>|
|<span data-ttu-id="731db-521">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="731db-521">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="731db-522">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-522">Int32</span></span>|<span data-ttu-id="731db-523">Указывает количество дней, в течение которых можно установить пароль профиля работы до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="731db-523">Indicates the number of days that a work profile password can be set before it expires and a new password will be required.</span></span> <span data-ttu-id="731db-524">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="731db-524">Valid values 1 to 365</span></span>|
|<span data-ttu-id="731db-525">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="731db-525">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="731db-526">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-526">Int32</span></span>|<span data-ttu-id="731db-527">Указывает минимальную длину пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="731db-527">Indicates the minimum length of the work profile password.</span></span> <span data-ttu-id="731db-528">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="731db-528">Valid values 4 to 16</span></span>|
|<span data-ttu-id="731db-529">workProfilePasswordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="731db-529">workProfilePasswordMinimumNumericCharacters</span></span>|<span data-ttu-id="731db-530">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-530">Int32</span></span>|<span data-ttu-id="731db-531">Указывает минимальное число цифр, необходимое для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="731db-531">Indicates the minimum number of numeric characters required for the work profile password.</span></span> <span data-ttu-id="731db-532">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="731db-532">Valid values 1 to 16</span></span>|
|<span data-ttu-id="731db-533">workProfilePasswordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="731db-533">workProfilePasswordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="731db-534">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-534">Int32</span></span>|<span data-ttu-id="731db-535">Указывает минимальное количество символов, не букв, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="731db-535">Indicates the minimum number of non-letter characters required for the work profile password.</span></span> <span data-ttu-id="731db-536">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="731db-536">Valid values 1 to 16</span></span>|
|<span data-ttu-id="731db-537">workProfilePasswordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="731db-537">workProfilePasswordMinimumLetterCharacters</span></span>|<span data-ttu-id="731db-538">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-538">Int32</span></span>|<span data-ttu-id="731db-539">Указывает минимальное количество букв, необходимое для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="731db-539">Indicates the minimum number of letter characters required for the work profile password.</span></span> <span data-ttu-id="731db-540">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="731db-540">Valid values 1 to 16</span></span>|
|<span data-ttu-id="731db-541">workProfilePasswordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="731db-541">workProfilePasswordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="731db-542">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-542">Int32</span></span>|<span data-ttu-id="731db-543">Указывает минимальное количество символов нижнего уровня, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="731db-543">Indicates the minimum number of lower-case characters required for the work profile password.</span></span> <span data-ttu-id="731db-544">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="731db-544">Valid values 1 to 16</span></span>|
|<span data-ttu-id="731db-545">workProfilePasswordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="731db-545">workProfilePasswordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="731db-546">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-546">Int32</span></span>|<span data-ttu-id="731db-547">Указывает минимальное количество символов в верхнем букве, необходимое для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="731db-547">Indicates the minimum number of upper-case letter characters required for the work profile password.</span></span> <span data-ttu-id="731db-548">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="731db-548">Valid values 1 to 16</span></span>|
|<span data-ttu-id="731db-549">workProfilePasswordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="731db-549">workProfilePasswordMinimumSymbolCharacters</span></span>|<span data-ttu-id="731db-550">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-550">Int32</span></span>|<span data-ttu-id="731db-551">Указывает минимальное количество символов, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="731db-551">Indicates the minimum number of symbol characters required for the work profile password.</span></span> <span data-ttu-id="731db-552">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="731db-552">Valid values 1 to 16</span></span>|
|<span data-ttu-id="731db-553">workProfilePasswordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="731db-553">workProfilePasswordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="731db-554">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-554">Int32</span></span>|<span data-ttu-id="731db-555">Указывает длину истории паролей профиля работы, в которой пользователь не сможет ввести новый пароль, который будет таким же, как любой пароль в истории.</span><span class="sxs-lookup"><span data-stu-id="731db-555">Indicates the length of the work profile password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="731db-556">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="731db-556">Valid values 0 to 24</span></span>|
|<span data-ttu-id="731db-557">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="731db-557">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="731db-558">Int32</span><span class="sxs-lookup"><span data-stu-id="731db-558">Int32</span></span>|<span data-ttu-id="731db-559">Указывает, сколько раз пользователь может ввести неправильный пароль к профилю работы перед тем, как устройство будет стирано.</span><span class="sxs-lookup"><span data-stu-id="731db-559">Indicates the number of times a user can enter an incorrect work profile password before the device is wiped.</span></span> <span data-ttu-id="731db-560">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="731db-560">Valid values 4 to 11</span></span>|
|<span data-ttu-id="731db-561">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="731db-561">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="731db-562">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="731db-562">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="731db-563">Указывает минимальное качество пароля, необходимое для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="731db-563">Indicates the minimum password quality required on the work profile password.</span></span> <span data-ttu-id="731db-564">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="731db-564">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="731db-565">Отклик</span><span class="sxs-lookup"><span data-stu-id="731db-565">Response</span></span>
<span data-ttu-id="731db-566">В случае успеха этот метод возвращает код отклика и объект `201 Created` [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="731db-566">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="731db-567">Пример</span><span class="sxs-lookup"><span data-stu-id="731db-567">Example</span></span>

### <a name="request"></a><span data-ttu-id="731db-568">Запрос</span><span class="sxs-lookup"><span data-stu-id="731db-568">Request</span></span>
<span data-ttu-id="731db-569">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="731db-569">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 7313

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
  "kioskModeAppOrderEnabled": true,
  "kioskModeAppsInFolderOrderedByName": true,
  "kioskModeGridHeight": 3,
  "kioskModeGridWidth": 2,
  "kioskModeLockHomeScreen": true,
  "kioskModeManagedFolders": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
      "folderName": "Folder Name value",
      "folderIdentifier": "Folder Identifier value",
      "items": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
          "label": "Label value",
          "link": "Link value"
        }
      ]
    }
  ],
  "kioskModeAppPositions": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
      "position": 8,
      "item": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
        "label": "Label value",
        "link": "Link value"
      }
    }
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

### <a name="response"></a><span data-ttu-id="731db-570">Отклик</span><span class="sxs-lookup"><span data-stu-id="731db-570">Response</span></span>
<span data-ttu-id="731db-p160">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="731db-p160">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7485

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
  "kioskModeAppOrderEnabled": true,
  "kioskModeAppsInFolderOrderedByName": true,
  "kioskModeGridHeight": 3,
  "kioskModeGridWidth": 2,
  "kioskModeLockHomeScreen": true,
  "kioskModeManagedFolders": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
      "folderName": "Folder Name value",
      "folderIdentifier": "Folder Identifier value",
      "items": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
          "label": "Label value",
          "link": "Link value"
        }
      ]
    }
  ],
  "kioskModeAppPositions": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
      "position": 8,
      "item": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
        "label": "Label value",
        "link": "Link value"
      }
    }
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




