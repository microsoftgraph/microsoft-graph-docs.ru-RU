---
title: Обновление androidDeviceOwnerGeneralDeviceConfiguration
description: Обновление свойств объекта AndroidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7385173e59aded355bc3f1967e3d3e8f68280269
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138674"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="26129-103">Обновление androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="26129-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="26129-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26129-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26129-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26129-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26129-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26129-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26129-107">Обновление свойств объекта [AndroidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26129-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26129-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="26129-108">Prerequisites</span></span>
<span data-ttu-id="26129-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26129-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26129-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26129-111">Permission type</span></span>|<span data-ttu-id="26129-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26129-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26129-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26129-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26129-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26129-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26129-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26129-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26129-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26129-116">Not supported.</span></span>|
|<span data-ttu-id="26129-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="26129-117">Application</span></span>|<span data-ttu-id="26129-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26129-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26129-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26129-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="26129-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="26129-120">Request headers</span></span>
|<span data-ttu-id="26129-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26129-121">Header</span></span>|<span data-ttu-id="26129-122">Значение</span><span class="sxs-lookup"><span data-stu-id="26129-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26129-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="26129-123">Authorization</span></span>|<span data-ttu-id="26129-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26129-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26129-125">Accept</span><span class="sxs-lookup"><span data-stu-id="26129-125">Accept</span></span>|<span data-ttu-id="26129-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26129-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26129-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26129-127">Request body</span></span>
<span data-ttu-id="26129-128">В теле запроса предоставляем представление JSON для [объекта AndroidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26129-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="26129-129">В следующей таблице показаны свойства, необходимые при создании [androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26129-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="26129-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="26129-130">Property</span></span>|<span data-ttu-id="26129-131">Тип</span><span class="sxs-lookup"><span data-stu-id="26129-131">Type</span></span>|<span data-ttu-id="26129-132">Описание</span><span class="sxs-lookup"><span data-stu-id="26129-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26129-133">id</span><span class="sxs-lookup"><span data-stu-id="26129-133">id</span></span>|<span data-ttu-id="26129-134">Строка</span><span class="sxs-lookup"><span data-stu-id="26129-134">String</span></span>|<span data-ttu-id="26129-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="26129-135">Key of the entity.</span></span> <span data-ttu-id="26129-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26129-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26129-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26129-137">lastModifiedDateTime</span></span>|<span data-ttu-id="26129-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26129-138">DateTimeOffset</span></span>|<span data-ttu-id="26129-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="26129-139">DateTime the object was last modified.</span></span> <span data-ttu-id="26129-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26129-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26129-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="26129-141">roleScopeTagIds</span></span>|<span data-ttu-id="26129-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="26129-142">String collection</span></span>|<span data-ttu-id="26129-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="26129-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="26129-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26129-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26129-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="26129-145">supportsScopeTags</span></span>|<span data-ttu-id="26129-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-146">Boolean</span></span>|<span data-ttu-id="26129-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="26129-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="26129-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="26129-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="26129-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="26129-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="26129-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26129-150">This property is read-only.</span></span> <span data-ttu-id="26129-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26129-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26129-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="26129-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="26129-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="26129-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="26129-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="26129-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="26129-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26129-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26129-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="26129-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="26129-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="26129-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="26129-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="26129-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="26129-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26129-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26129-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="26129-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="26129-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="26129-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="26129-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="26129-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="26129-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26129-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26129-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26129-164">createdDateTime</span></span>|<span data-ttu-id="26129-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26129-165">DateTimeOffset</span></span>|<span data-ttu-id="26129-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="26129-166">DateTime the object was created.</span></span> <span data-ttu-id="26129-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26129-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26129-168">description</span><span class="sxs-lookup"><span data-stu-id="26129-168">description</span></span>|<span data-ttu-id="26129-169">Строка</span><span class="sxs-lookup"><span data-stu-id="26129-169">String</span></span>|<span data-ttu-id="26129-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="26129-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="26129-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26129-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26129-172">displayName</span><span class="sxs-lookup"><span data-stu-id="26129-172">displayName</span></span>|<span data-ttu-id="26129-173">Строка</span><span class="sxs-lookup"><span data-stu-id="26129-173">String</span></span>|<span data-ttu-id="26129-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="26129-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="26129-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26129-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26129-176">version</span><span class="sxs-lookup"><span data-stu-id="26129-176">version</span></span>|<span data-ttu-id="26129-177">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-177">Int32</span></span>|<span data-ttu-id="26129-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="26129-178">Version of the device configuration.</span></span> <span data-ttu-id="26129-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26129-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26129-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="26129-180">accountsBlockModification</span></span>|<span data-ttu-id="26129-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-181">Boolean</span></span>|<span data-ttu-id="26129-182">Указывает, отключена ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="26129-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="26129-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="26129-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="26129-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-184">Boolean</span></span>|<span data-ttu-id="26129-185">Указывает, разрешено ли пользователю включить параметр неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="26129-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="26129-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="26129-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="26129-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="26129-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="26129-188">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="26129-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="26129-189">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="26129-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="26129-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="26129-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="26129-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="26129-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="26129-192">Указывает политику разрешений для запросов на разрешения на время запуска, если она не определена специально для приложения.</span><span class="sxs-lookup"><span data-stu-id="26129-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="26129-193">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="26129-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="26129-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="26129-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="26129-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-195">Boolean</span></span>|<span data-ttu-id="26129-196">Следует ли рекомендовать всем приложениям пропускать добавленные в первый раз подсказки.</span><span class="sxs-lookup"><span data-stu-id="26129-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="26129-197">BluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="26129-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="26129-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-198">Boolean</span></span>|<span data-ttu-id="26129-199">Указывает, следует ли блокировать пользователю настройку Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="26129-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="26129-200">BluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="26129-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="26129-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-201">Boolean</span></span>|<span data-ttu-id="26129-202">Указывает, следует ли блокировать пользователю доступ к контактам по Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="26129-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="26129-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="26129-203">cameraBlocked</span></span>|<span data-ttu-id="26129-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-204">Boolean</span></span>|<span data-ttu-id="26129-205">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="26129-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="26129-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="26129-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="26129-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-207">Boolean</span></span>|<span data-ttu-id="26129-208">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="26129-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="26129-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="26129-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="26129-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-210">Boolean</span></span>|<span data-ttu-id="26129-211">Указывает, следует ли блокировать пользователям любую конфигурацию учетных данных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="26129-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="26129-212">MicrosoftLauncherConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="26129-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="26129-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-213">Boolean</span></span>|<span data-ttu-id="26129-214">Указывает, нужно ли настраивать Microsoft Launcher или нет.</span><span class="sxs-lookup"><span data-stu-id="26129-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="26129-215">MicrosoftLauncherCustomWallpaperEnabled</span><span class="sxs-lookup"><span data-stu-id="26129-215">microsoftLauncherCustomWallpaperEnabled</span></span>|<span data-ttu-id="26129-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-216">Boolean</span></span>|<span data-ttu-id="26129-217">Указывает, следует ли настраивать обои на целевых устройствах.</span><span class="sxs-lookup"><span data-stu-id="26129-217">Indicates whether or not to configure the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="26129-218">MicrosoftLauncherCustomWallpaperImageUrl</span><span class="sxs-lookup"><span data-stu-id="26129-218">microsoftLauncherCustomWallpaperImageUrl</span></span>|<span data-ttu-id="26129-219">Строка</span><span class="sxs-lookup"><span data-stu-id="26129-219">String</span></span>|<span data-ttu-id="26129-220">Указывает URL-адрес для файла изображений, который будет использовать в качестве обои на целевых устройствах.</span><span class="sxs-lookup"><span data-stu-id="26129-220">Indicates the URL for the image file to use as the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="26129-221">MicrosoftLauncherCustomWallpaperAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="26129-221">microsoftLauncherCustomWallpaperAllowUserModification</span></span>|<span data-ttu-id="26129-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-222">Boolean</span></span>|<span data-ttu-id="26129-223">Указывает, может ли пользователь изменить обои, чтобы персонализировать свое устройство.</span><span class="sxs-lookup"><span data-stu-id="26129-223">Indicates whether or not the user can modify the wallpaper to personalize their device.</span></span>|
|<span data-ttu-id="26129-224">microsoftLauncherFeedEnabled</span><span class="sxs-lookup"><span data-stu-id="26129-224">microsoftLauncherFeedEnabled</span></span>|<span data-ttu-id="26129-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-225">Boolean</span></span>|<span data-ttu-id="26129-226">Указывает, хотите ли вы включить канал запуска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="26129-226">Indicates whether or not you want to enable the launcher feed on the device.</span></span>|
|<span data-ttu-id="26129-227">MicrosoftLauncherFeedAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="26129-227">microsoftLauncherFeedAllowUserModification</span></span>|<span data-ttu-id="26129-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-228">Boolean</span></span>|<span data-ttu-id="26129-229">Указывает, может ли пользователь изменить канал запуска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="26129-229">Indicates whether or not the user can modify the launcher feed on the device.</span></span>|
|<span data-ttu-id="26129-230">MicrosoftLauncherDockPresenceConfiguration</span><span class="sxs-lookup"><span data-stu-id="26129-230">microsoftLauncherDockPresenceConfiguration</span></span>|[<span data-ttu-id="26129-231">microsoftLauncherDockPresence</span><span class="sxs-lookup"><span data-stu-id="26129-231">microsoftLauncherDockPresence</span></span>](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|<span data-ttu-id="26129-232">Указывает, нужно ли настраивать док-станцию устройства.</span><span class="sxs-lookup"><span data-stu-id="26129-232">Indicates whether or not you want to configure the device dock.</span></span> <span data-ttu-id="26129-233">Возможные значения: `notConfigured`, `show`, `hide`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="26129-233">Possible values are: `notConfigured`, `show`, `hide`, `disabled`.</span></span>|
|<span data-ttu-id="26129-234">MicrosoftLauncherDockPresenceAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="26129-234">microsoftLauncherDockPresenceAllowUserModification</span></span>|<span data-ttu-id="26129-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-235">Boolean</span></span>|<span data-ttu-id="26129-236">Указывает, может ли пользователь изменить конфигурацию док-станции устройства на устройстве.</span><span class="sxs-lookup"><span data-stu-id="26129-236">Indicates whether or not the user can modify the device dock configuration on the device.</span></span>|
|<span data-ttu-id="26129-237">MicrosoftLauncherSearchBarPlacementConfiguration</span><span class="sxs-lookup"><span data-stu-id="26129-237">microsoftLauncherSearchBarPlacementConfiguration</span></span>|[<span data-ttu-id="26129-238">microsoftLauncherSearchBarPlacement</span><span class="sxs-lookup"><span data-stu-id="26129-238">microsoftLauncherSearchBarPlacement</span></span>](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|<span data-ttu-id="26129-239">Указывает конфигурацию размещения панели поиска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="26129-239">Indicates the search bar placement configuration on the device.</span></span> <span data-ttu-id="26129-240">Возможные значения: `notConfigured`, `top`, `bottom`, `hide`.</span><span class="sxs-lookup"><span data-stu-id="26129-240">Possible values are: `notConfigured`, `top`, `bottom`, `hide`.</span></span>|
|<span data-ttu-id="26129-241">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="26129-241">enrollmentProfile</span></span>|[<span data-ttu-id="26129-242">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="26129-242">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="26129-243">Указывает, какой профиль регистрации необходимо настроить.</span><span class="sxs-lookup"><span data-stu-id="26129-243">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="26129-244">Возможные значения: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span><span class="sxs-lookup"><span data-stu-id="26129-244">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="26129-245">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="26129-245">dataRoamingBlocked</span></span>|<span data-ttu-id="26129-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-246">Boolean</span></span>|<span data-ttu-id="26129-247">Указывает, следует ли блокировать пользователю роуминг данных.</span><span class="sxs-lookup"><span data-stu-id="26129-247">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="26129-248">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="26129-248">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="26129-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-249">Boolean</span></span>|<span data-ttu-id="26129-250">Указывает, следует ли блокировать пользователю вручную изменять дату или время на устройстве</span><span class="sxs-lookup"><span data-stu-id="26129-250">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="26129-251">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="26129-251">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="26129-252">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="26129-252">String collection</span></span>|<span data-ttu-id="26129-253">Список электронных писем учетной записи Google, которые необходимо будет проверить подлинность после сброса устройства перед его настройками.</span><span class="sxs-lookup"><span data-stu-id="26129-253">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="26129-254">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="26129-254">factoryResetBlocked</span></span>|<span data-ttu-id="26129-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-255">Boolean</span></span>|<span data-ttu-id="26129-256">Указывает, отключен ли параметр сброса фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="26129-256">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="26129-257">globalProxy</span><span class="sxs-lookup"><span data-stu-id="26129-257">globalProxy</span></span>|[<span data-ttu-id="26129-258">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="26129-258">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="26129-259">Прокси настроен непосредственно с хостом, портом и исключенными хостами.</span><span class="sxs-lookup"><span data-stu-id="26129-259">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="26129-260">GoogleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="26129-260">googleAccountsBlocked</span></span>|<span data-ttu-id="26129-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-261">Boolean</span></span>|<span data-ttu-id="26129-262">Указывает, будут ли заблокированы учетные записи Google.</span><span class="sxs-lookup"><span data-stu-id="26129-262">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="26129-263">kioskCustomizationDeviceSettingsBlocked</span><span class="sxs-lookup"><span data-stu-id="26129-263">kioskCustomizationDeviceSettingsBlocked</span></span>|<span data-ttu-id="26129-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-264">Boolean</span></span>|<span data-ttu-id="26129-265">Указывает, может ли пользователь получить доступ к приложению Параметры устройства во время работы в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-265">Indicates whether a user can access the device's Settings app while in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-266">kioskCustomizationPowerButtonActionsBlocked</span><span class="sxs-lookup"><span data-stu-id="26129-266">kioskCustomizationPowerButtonActionsBlocked</span></span>|<span data-ttu-id="26129-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-267">Boolean</span></span>|<span data-ttu-id="26129-268">Отображается ли меню питания при длительном нажатии кнопки Power устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-268">Whether the power menu is shown when a user long presses the Power button of a device in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-269">kioskCustomizationStatusBar</span><span class="sxs-lookup"><span data-stu-id="26129-269">kioskCustomizationStatusBar</span></span>|[<span data-ttu-id="26129-270">androidDeviceOwnerKioskCustomizationStatusBar</span><span class="sxs-lookup"><span data-stu-id="26129-270">androidDeviceOwnerKioskCustomizationStatusBar</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|<span data-ttu-id="26129-271">Указывает отключение системных данных и уведомлений в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-271">Indicates whether system info and notifications are disabled in Kiosk Mode.</span></span> <span data-ttu-id="26129-272">Возможные значения: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.</span><span class="sxs-lookup"><span data-stu-id="26129-272">Possible values are: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.</span></span>|
|<span data-ttu-id="26129-273">kioskCustomizationSystemErrorWarnings</span><span class="sxs-lookup"><span data-stu-id="26129-273">kioskCustomizationSystemErrorWarnings</span></span>|<span data-ttu-id="26129-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-274">Boolean</span></span>|<span data-ttu-id="26129-275">Указывает, показаны ли в режиме киоска диалоги системных ошибок для сбоя или безответных приложений.</span><span class="sxs-lookup"><span data-stu-id="26129-275">Indicates whether system error dialogs for crashed or unresponsive apps are shown in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-276">kioskCustomizationSystemNavigation</span><span class="sxs-lookup"><span data-stu-id="26129-276">kioskCustomizationSystemNavigation</span></span>|[<span data-ttu-id="26129-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span><span class="sxs-lookup"><span data-stu-id="26129-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|<span data-ttu-id="26129-278">Указывает, какие функции навигации включены в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-278">Indicates which navigation features are enabled in Kiosk Mode.</span></span> <span data-ttu-id="26129-279">Возможные значения: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.</span><span class="sxs-lookup"><span data-stu-id="26129-279">Possible values are: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.</span></span>|
|<span data-ttu-id="26129-280">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="26129-280">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="26129-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-281">Boolean</span></span>|<span data-ttu-id="26129-282">Включить или не включить режим сохранения экрана или нет в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-282">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-283">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="26129-283">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="26129-284">Строка</span><span class="sxs-lookup"><span data-stu-id="26129-284">String</span></span>|<span data-ttu-id="26129-285">URL-адрес для изображения, которое будет сохранения экрана устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-285">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-286">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="26129-286">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="26129-287">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-287">Int32</span></span>|<span data-ttu-id="26129-288">Количество секунд, за которые устройство будет отображать за исключением экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-288">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="26129-289">Допустимые значения от 0 до 9999999</span><span class="sxs-lookup"><span data-stu-id="26129-289">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="26129-290">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="26129-290">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="26129-291">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-291">Int32</span></span>|<span data-ttu-id="26129-292">Количество секунд, за которые устройство должно быть неактивным до того, как забереговка экрана будет показана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-292">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="26129-293">Допустимые значения от 1 до 9999999</span><span class="sxs-lookup"><span data-stu-id="26129-293">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="26129-294">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="26129-294">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="26129-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-295">Boolean</span></span>|<span data-ttu-id="26129-296">Должен ли на экране устройства показываться закаверка экрана, если звук/видео играет в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-296">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-297">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="26129-297">kioskModeApps</span></span>|<span data-ttu-id="26129-298">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="26129-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="26129-299">Список управляемых приложений, которые будут показаны, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-299">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="26129-300">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="26129-300">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="26129-301">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="26129-301">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="26129-302">Строка</span><span class="sxs-lookup"><span data-stu-id="26129-302">String</span></span>|<span data-ttu-id="26129-303">URL-адрес общедоступных изображений, которые можно использовать для обоев, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-303">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-304">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="26129-304">kioskModeExitCode</span></span>|<span data-ttu-id="26129-305">Строка</span><span class="sxs-lookup"><span data-stu-id="26129-305">String</span></span>|<span data-ttu-id="26129-306">Код выхода, чтобы позволить пользователю выйти из режима киоска, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-306">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-307">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="26129-307">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="26129-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-308">Boolean</span></span>|<span data-ttu-id="26129-309">Следует ли отображать виртуальную домашняя кнопка, когда устройство находится в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-309">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-310">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="26129-310">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="26129-311">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="26129-311">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="26129-312">Указывает, является ли виртуальная домашняя кнопка пальцем вверх по домашней кнопке или плавающей домашней кнопкой.</span><span class="sxs-lookup"><span data-stu-id="26129-312">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="26129-313">Возможные значения: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="26129-313">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="26129-314">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="26129-314">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="26129-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-315">Boolean</span></span>|<span data-ttu-id="26129-316">Следует ли разрешить пользователю настраивать Bluetooth в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-316">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-317">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="26129-317">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="26129-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-318">Boolean</span></span>|<span data-ttu-id="26129-319">Разрешить пользователю настраивать параметры Wi-Fi в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-319">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-320">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="26129-320">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="26129-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-321">Boolean</span></span>|<span data-ttu-id="26129-322">Разрешить или не разрешить пользователю использовать фонарик в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-322">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-323">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="26129-323">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="26129-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-324">Boolean</span></span>|<span data-ttu-id="26129-325">Разрешить или не разрешить пользователю изменять объем мультимедиа в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-325">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-326">kioskModeShowDeviceInfo</span><span class="sxs-lookup"><span data-stu-id="26129-326">kioskModeShowDeviceInfo</span></span>|<span data-ttu-id="26129-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-327">Boolean</span></span>|<span data-ttu-id="26129-328">Разрешить пользователю доступ к основным сведениям об устройстве.</span><span class="sxs-lookup"><span data-stu-id="26129-328">Whether or not to allow a user to access basic device information.</span></span>|
|<span data-ttu-id="26129-329">kioskModeManagedSettingsEntryDisabled</span><span class="sxs-lookup"><span data-stu-id="26129-329">kioskModeManagedSettingsEntryDisabled</span></span>|<span data-ttu-id="26129-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-330">Boolean</span></span>|<span data-ttu-id="26129-331">Отображение точки входа управляемых параметров на управляемом домашнем экране в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-331">Whether or not to display the Managed Settings entry point on the managed home screen in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-332">kioskModeDebugMenuEasyAccessEnabled</span><span class="sxs-lookup"><span data-stu-id="26129-332">kioskModeDebugMenuEasyAccessEnabled</span></span>|<span data-ttu-id="26129-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-333">Boolean</span></span>|<span data-ttu-id="26129-334">Следует ли разрешить пользователю легкий доступ к меню отлаживания в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-334">Whether or not to allow a user to easy access to the debug menu in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-335">kioskModeShowAppNotificationBadge</span><span class="sxs-lookup"><span data-stu-id="26129-335">kioskModeShowAppNotificationBadge</span></span>|<span data-ttu-id="26129-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-336">Boolean</span></span>|<span data-ttu-id="26129-337">Отображение значков уведомлений приложений в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-337">Whether or not to display application notification badges in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-338">kioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="26129-338">kioskModeScreenOrientation</span></span>|[<span data-ttu-id="26129-339">androidDeviceOwnerKioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="26129-339">androidDeviceOwnerKioskModeScreenOrientation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|<span data-ttu-id="26129-340">Конфигурация ориентации экрана для управляемого домашнего экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-340">Screen orientation configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="26129-341">Возможные значения: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span><span class="sxs-lookup"><span data-stu-id="26129-341">Possible values are: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span></span>|
|<span data-ttu-id="26129-342">kioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="26129-342">kioskModeIconSize</span></span>|[<span data-ttu-id="26129-343">androidDeviceOwnerKioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="26129-343">androidDeviceOwnerKioskModeIconSize</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|<span data-ttu-id="26129-344">Конфигурация размера значка для управляемого домашнего экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-344">Icon size configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="26129-345">Возможные значения: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span><span class="sxs-lookup"><span data-stu-id="26129-345">Possible values are: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span></span>|
|<span data-ttu-id="26129-346">kioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="26129-346">kioskModeFolderIcon</span></span>|[<span data-ttu-id="26129-347">androidDeviceOwnerKioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="26129-347">androidDeviceOwnerKioskModeFolderIcon</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|<span data-ttu-id="26129-348">Конфигурация значка папки для управляемого домашнего экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-348">Folder icon configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="26129-349">Возможные значения: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span><span class="sxs-lookup"><span data-stu-id="26129-349">Possible values are: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span></span>|
|<span data-ttu-id="26129-350">kioskModeWifiAllowedSsids</span><span class="sxs-lookup"><span data-stu-id="26129-350">kioskModeWifiAllowedSsids</span></span>|<span data-ttu-id="26129-351">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="26129-351">String collection</span></span>|<span data-ttu-id="26129-352">Ограниченный набор SSID WIFI, доступный пользователю для настройки в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-352">The restricted set of WIFI SSIDs available for the user to configure in Kiosk Mode.</span></span> <span data-ttu-id="26129-353">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="26129-353">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="26129-354">kioskModeAppOrderEnabled</span><span class="sxs-lookup"><span data-stu-id="26129-354">kioskModeAppOrderEnabled</span></span>|<span data-ttu-id="26129-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-355">Boolean</span></span>|<span data-ttu-id="26129-356">Включить или не включить заказ приложений в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-356">Whether or not to enable app ordering in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-357">kioskModeAppsInFolderOrderedByName</span><span class="sxs-lookup"><span data-stu-id="26129-357">kioskModeAppsInFolderOrderedByName</span></span>|<span data-ttu-id="26129-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-358">Boolean</span></span>|<span data-ttu-id="26129-359">Следует ли алфавитизировать приложения в папке в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-359">Whether or not to alphabetize applications within a folder in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-360">kioskModeGridHeight</span><span class="sxs-lookup"><span data-stu-id="26129-360">kioskModeGridHeight</span></span>|<span data-ttu-id="26129-361">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-361">Int32</span></span>|<span data-ttu-id="26129-362">Количество строк для сетки управляемого домашнего экрана с включенной в режиме киоска упорядочением приложений.</span><span class="sxs-lookup"><span data-stu-id="26129-362">Number of rows for Managed Home Screen grid with app ordering enabled in Kiosk Mode.</span></span> <span data-ttu-id="26129-363">Допустимые значения от 1 до 9999999</span><span class="sxs-lookup"><span data-stu-id="26129-363">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="26129-364">kioskModeGridWidth</span><span class="sxs-lookup"><span data-stu-id="26129-364">kioskModeGridWidth</span></span>|<span data-ttu-id="26129-365">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-365">Int32</span></span>|<span data-ttu-id="26129-366">Количество столбцов для сетки управляемого домашнего экрана с включенной в режиме киоска упорядочением приложений.</span><span class="sxs-lookup"><span data-stu-id="26129-366">Number of columns for Managed Home Screen grid with app ordering enabled in Kiosk Mode.</span></span> <span data-ttu-id="26129-367">Допустимые значения от 1 до 9999999</span><span class="sxs-lookup"><span data-stu-id="26129-367">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="26129-368">kioskModeLockHomeScreen</span><span class="sxs-lookup"><span data-stu-id="26129-368">kioskModeLockHomeScreen</span></span>|<span data-ttu-id="26129-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-369">Boolean</span></span>|<span data-ttu-id="26129-370">Следует ли заблокировать домашний экран конечному пользователю в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-370">Whether or not to lock home screen to the end user in Kiosk Mode.</span></span>|
|<span data-ttu-id="26129-371">kioskModeManagedFolders</span><span class="sxs-lookup"><span data-stu-id="26129-371">kioskModeManagedFolders</span></span>|<span data-ttu-id="26129-372">[коллекция androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md)</span><span class="sxs-lookup"><span data-stu-id="26129-372">[androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md) collection</span></span>|<span data-ttu-id="26129-373">Список управляемых папок для устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-373">A list of managed folders for a device in Kiosk Mode.</span></span> <span data-ttu-id="26129-374">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="26129-374">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="26129-375">kioskModeAppPositions</span><span class="sxs-lookup"><span data-stu-id="26129-375">kioskModeAppPositions</span></span>|<span data-ttu-id="26129-376">[коллекция androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md)</span><span class="sxs-lookup"><span data-stu-id="26129-376">[androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md) collection</span></span>|<span data-ttu-id="26129-377">Упорядочение элементов на управляемом домашнем экране режима киоска.</span><span class="sxs-lookup"><span data-stu-id="26129-377">The ordering of items on Kiosk Mode Managed Home Screen.</span></span> <span data-ttu-id="26129-378">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="26129-378">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="26129-379">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="26129-379">microphoneForceMute</span></span>|<span data-ttu-id="26129-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-380">Boolean</span></span>|<span data-ttu-id="26129-381">Указывает, следует ли блокировать разгрузку микрофона на устройстве.</span><span class="sxs-lookup"><span data-stu-id="26129-381">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="26129-382">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="26129-382">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="26129-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-383">Boolean</span></span>|<span data-ttu-id="26129-384">Указывает, разрешит ли устройство подключаться к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="26129-384">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="26129-385">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="26129-385">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="26129-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-386">Boolean</span></span>|<span data-ttu-id="26129-387">Указывает, следует ли блокировать исходяющий луч NFC.</span><span class="sxs-lookup"><span data-stu-id="26129-387">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="26129-388">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="26129-388">passwordBlockKeyguard</span></span>|<span data-ttu-id="26129-389">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-389">Boolean</span></span>|<span data-ttu-id="26129-390">Указывает, отключен ли ключ-гарант.</span><span class="sxs-lookup"><span data-stu-id="26129-390">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="26129-391">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="26129-391">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="26129-392">[коллекция androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="26129-392">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="26129-393">Список функций keyguard устройства, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="26129-393">List of device keyguard features to block.</span></span> <span data-ttu-id="26129-394">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="26129-394">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="26129-395">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="26129-395">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="26129-396">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="26129-396">passwordExpirationDays</span></span>|<span data-ttu-id="26129-397">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-397">Int32</span></span>|<span data-ttu-id="26129-398">Указывает время, за которое может быть установлен пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="26129-398">Indicates the amount of time that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="26129-399">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="26129-399">Valid values 1 to 365</span></span>|
|<span data-ttu-id="26129-400">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="26129-400">passwordMinimumLength</span></span>|<span data-ttu-id="26129-401">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-401">Int32</span></span>|<span data-ttu-id="26129-402">Указывает минимальную длину пароля, необходимого на устройстве.</span><span class="sxs-lookup"><span data-stu-id="26129-402">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="26129-403">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="26129-403">Valid values 4 to 16</span></span>|
|<span data-ttu-id="26129-404">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="26129-404">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="26129-405">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-405">Int32</span></span>|<span data-ttu-id="26129-406">Указывает минимальное количество букв, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="26129-406">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="26129-407">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="26129-407">Valid values 1 to 16</span></span>|
|<span data-ttu-id="26129-408">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="26129-408">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="26129-409">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-409">Int32</span></span>|<span data-ttu-id="26129-410">Указывает минимальное число символов более низкого уровня, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="26129-410">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="26129-411">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="26129-411">Valid values 1 to 16</span></span>|
|<span data-ttu-id="26129-412">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="26129-412">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="26129-413">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-413">Int32</span></span>|<span data-ttu-id="26129-414">Указывает минимальное количество символов без букв, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="26129-414">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="26129-415">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="26129-415">Valid values 1 to 16</span></span>|
|<span data-ttu-id="26129-416">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="26129-416">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="26129-417">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-417">Int32</span></span>|<span data-ttu-id="26129-418">Указывает минимальное число числимые символы, необходимые для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="26129-418">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="26129-419">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="26129-419">Valid values 1 to 16</span></span>|
|<span data-ttu-id="26129-420">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="26129-420">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="26129-421">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-421">Int32</span></span>|<span data-ttu-id="26129-422">Указывает минимальное количество символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="26129-422">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="26129-423">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="26129-423">Valid values 1 to 16</span></span>|
|<span data-ttu-id="26129-424">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="26129-424">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="26129-425">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-425">Int32</span></span>|<span data-ttu-id="26129-426">Указывает минимальное количество символов верхней буквы, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="26129-426">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="26129-427">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="26129-427">Valid values 1 to 16</span></span>|
|<span data-ttu-id="26129-428">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="26129-428">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="26129-429">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-429">Int32</span></span>|<span data-ttu-id="26129-430">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="26129-430">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="26129-431">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="26129-431">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="26129-432">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-432">Int32</span></span>|<span data-ttu-id="26129-433">Указывает длину истории паролей, в которой пользователь не сможет ввести новый пароль, который будет таким же, как любой пароль в истории.</span><span class="sxs-lookup"><span data-stu-id="26129-433">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="26129-434">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="26129-434">Valid values 0 to 24</span></span>|
|<span data-ttu-id="26129-435">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="26129-435">passwordRequiredType</span></span>|[<span data-ttu-id="26129-436">AndroidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="26129-436">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="26129-437">Указывает минимальное качество пароля, необходимое на устройстве.</span><span class="sxs-lookup"><span data-stu-id="26129-437">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="26129-438">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="26129-438">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="26129-439">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="26129-439">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="26129-440">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-440">Int32</span></span>|<span data-ttu-id="26129-441">Указывает количество случаев, когда пользователь может ввести неправильный пароль до стирки устройства.</span><span class="sxs-lookup"><span data-stu-id="26129-441">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="26129-442">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="26129-442">Valid values 4 to 11</span></span>|
|<span data-ttu-id="26129-443">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="26129-443">playStoreMode</span></span>|[<span data-ttu-id="26129-444">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="26129-444">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="26129-445">Указывает режим Play Store устройства.</span><span class="sxs-lookup"><span data-stu-id="26129-445">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="26129-446">Возможные значения: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="26129-446">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="26129-447">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="26129-447">safeBootBlocked</span></span>|<span data-ttu-id="26129-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-448">Boolean</span></span>|<span data-ttu-id="26129-449">Указывает, отключена ли перезагрузка устройства в безопасную загрузку.</span><span class="sxs-lookup"><span data-stu-id="26129-449">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="26129-450">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="26129-450">screenCaptureBlocked</span></span>|<span data-ttu-id="26129-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-451">Boolean</span></span>|<span data-ttu-id="26129-452">Указывает, следует ли отключить возможность делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="26129-452">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="26129-453">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="26129-453">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="26129-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-454">Boolean</span></span>|<span data-ttu-id="26129-455">Указывает, следует ли блокировать пользователю включение функций отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="26129-455">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="26129-456">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="26129-456">securityRequireVerifyApps</span></span>|<span data-ttu-id="26129-457">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-457">Boolean</span></span>|<span data-ttu-id="26129-458">Указывает, требуется ли проверка приложений.</span><span class="sxs-lookup"><span data-stu-id="26129-458">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="26129-459">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="26129-459">statusBarBlocked</span></span>|<span data-ttu-id="26129-460">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-460">Boolean</span></span>|<span data-ttu-id="26129-461">Указывает, отключена ли или отключена планка состояния, включая уведомления, быстрые параметры и другие экранные наложения.</span><span class="sxs-lookup"><span data-stu-id="26129-461">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="26129-462">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="26129-462">stayOnModes</span></span>|<span data-ttu-id="26129-463">[коллекция androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="26129-463">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="26129-464">Список режимов, в которых дисплей устройства будет работать с питанием.</span><span class="sxs-lookup"><span data-stu-id="26129-464">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="26129-465">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="26129-465">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="26129-466">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="26129-466">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="26129-467">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="26129-467">storageAllowUsb</span></span>|<span data-ttu-id="26129-468">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-468">Boolean</span></span>|<span data-ttu-id="26129-469">Указывает, следует ли разрешить массовое хранилище USB.</span><span class="sxs-lookup"><span data-stu-id="26129-469">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="26129-470">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="26129-470">storageBlockExternalMedia</span></span>|<span data-ttu-id="26129-471">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-471">Boolean</span></span>|<span data-ttu-id="26129-472">Указывает, следует ли блокировать внешние носитли.</span><span class="sxs-lookup"><span data-stu-id="26129-472">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="26129-473">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="26129-473">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="26129-474">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-474">Boolean</span></span>|<span data-ttu-id="26129-475">Указывает, следует ли блокировать передачу usb-файлов.</span><span class="sxs-lookup"><span data-stu-id="26129-475">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="26129-476">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="26129-476">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="26129-477">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-477">Int32</span></span>|<span data-ttu-id="26129-478">Указывает количество минут после полуночи, когда начинается окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="26129-478">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="26129-479">Допустимые значения от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="26129-479">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="26129-480">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="26129-480">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="26129-481">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-481">Int32</span></span>|<span data-ttu-id="26129-482">Указывает количество минут после полуночи, когда заканчивается окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="26129-482">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="26129-483">Допустимые значения от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="26129-483">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="26129-484">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="26129-484">systemUpdateInstallType</span></span>|[<span data-ttu-id="26129-485">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="26129-485">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="26129-486">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="26129-486">The type of system update configuration.</span></span> <span data-ttu-id="26129-487">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="26129-487">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="26129-488">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="26129-488">systemWindowsBlocked</span></span>|<span data-ttu-id="26129-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-489">Boolean</span></span>|<span data-ttu-id="26129-490">Блокировка windows системы Android, например всплывающие уведомления, телефонные действия и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="26129-490">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="26129-491">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="26129-491">usersBlockAdd</span></span>|<span data-ttu-id="26129-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-492">Boolean</span></span>|<span data-ttu-id="26129-493">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="26129-493">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="26129-494">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="26129-494">usersBlockRemove</span></span>|<span data-ttu-id="26129-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-495">Boolean</span></span>|<span data-ttu-id="26129-496">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="26129-496">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="26129-497">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="26129-497">volumeBlockAdjustment</span></span>|<span data-ttu-id="26129-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-498">Boolean</span></span>|<span data-ttu-id="26129-499">Указывает, отключена ли настройка магистрали.</span><span class="sxs-lookup"><span data-stu-id="26129-499">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="26129-500">VPNAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="26129-500">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="26129-501">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-501">Boolean</span></span>|<span data-ttu-id="26129-502">Если всегда указано имя пакета VPN, следует ли заблокировать сетевой трафик при отключении VPN.</span><span class="sxs-lookup"><span data-stu-id="26129-502">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="26129-503">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="26129-503">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="26129-504">Строка</span><span class="sxs-lookup"><span data-stu-id="26129-504">String</span></span>|<span data-ttu-id="26129-505">Имя пакета приложений для Android для приложения, которое будет обрабатывать всегда на VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="26129-505">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="26129-506">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="26129-506">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="26129-507">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-507">Boolean</span></span>|<span data-ttu-id="26129-508">Указывает, следует ли блокировать пользователю редактирование параметров подключения к Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="26129-508">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="26129-509">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="26129-509">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="26129-510">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-510">Boolean</span></span>|<span data-ttu-id="26129-511">Указывает, следует ли блокировать пользователю редактирование только сетей, определенных политикой.</span><span class="sxs-lookup"><span data-stu-id="26129-511">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|
|<span data-ttu-id="26129-512">personalProfileAppsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="26129-512">personalProfileAppsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="26129-513">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-513">Boolean</span></span>|<span data-ttu-id="26129-514">Указывает, может ли пользователь устанавливать приложения из неизвестных источников в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="26129-514">Indicates whether the user can install apps from unknown sources on the personal profile.</span></span>|
|<span data-ttu-id="26129-515">personalProfileCameraBlocked</span><span class="sxs-lookup"><span data-stu-id="26129-515">personalProfileCameraBlocked</span></span>|<span data-ttu-id="26129-516">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-516">Boolean</span></span>|<span data-ttu-id="26129-517">Указывает, следует ли отключить использование камеры в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="26129-517">Indicates whether to disable the use of the camera on the personal profile.</span></span>|
|<span data-ttu-id="26129-518">personalProfileScreenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="26129-518">personalProfileScreenCaptureBlocked</span></span>|<span data-ttu-id="26129-519">Boolean</span><span class="sxs-lookup"><span data-stu-id="26129-519">Boolean</span></span>|<span data-ttu-id="26129-520">Указывает, следует ли отключить возможность делать скриншоты в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="26129-520">Indicates whether to disable the capability to take screenshots on the personal profile.</span></span>|
|<span data-ttu-id="26129-521">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="26129-521">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="26129-522">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-522">Int32</span></span>|<span data-ttu-id="26129-523">Указывает количество дней, в течение которых можно установить пароль профиля работы до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="26129-523">Indicates the number of days that a work profile password can be set before it expires and a new password will be required.</span></span> <span data-ttu-id="26129-524">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="26129-524">Valid values 1 to 365</span></span>|
|<span data-ttu-id="26129-525">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="26129-525">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="26129-526">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-526">Int32</span></span>|<span data-ttu-id="26129-527">Указывает минимальную длину пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="26129-527">Indicates the minimum length of the work profile password.</span></span> <span data-ttu-id="26129-528">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="26129-528">Valid values 4 to 16</span></span>|
|<span data-ttu-id="26129-529">workProfilePasswordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="26129-529">workProfilePasswordMinimumNumericCharacters</span></span>|<span data-ttu-id="26129-530">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-530">Int32</span></span>|<span data-ttu-id="26129-531">Указывает минимальное число числимые символы, необходимые для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="26129-531">Indicates the minimum number of numeric characters required for the work profile password.</span></span> <span data-ttu-id="26129-532">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="26129-532">Valid values 1 to 16</span></span>|
|<span data-ttu-id="26129-533">workProfilePasswordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="26129-533">workProfilePasswordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="26129-534">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-534">Int32</span></span>|<span data-ttu-id="26129-535">Указывает минимальное количество символов без букв, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="26129-535">Indicates the minimum number of non-letter characters required for the work profile password.</span></span> <span data-ttu-id="26129-536">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="26129-536">Valid values 1 to 16</span></span>|
|<span data-ttu-id="26129-537">workProfilePasswordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="26129-537">workProfilePasswordMinimumLetterCharacters</span></span>|<span data-ttu-id="26129-538">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-538">Int32</span></span>|<span data-ttu-id="26129-539">Указывает минимальное количество букв, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="26129-539">Indicates the minimum number of letter characters required for the work profile password.</span></span> <span data-ttu-id="26129-540">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="26129-540">Valid values 1 to 16</span></span>|
|<span data-ttu-id="26129-541">workProfilePasswordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="26129-541">workProfilePasswordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="26129-542">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-542">Int32</span></span>|<span data-ttu-id="26129-543">Указывает минимальное количество символов нижнего уровня, необходимое для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="26129-543">Indicates the minimum number of lower-case characters required for the work profile password.</span></span> <span data-ttu-id="26129-544">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="26129-544">Valid values 1 to 16</span></span>|
|<span data-ttu-id="26129-545">workProfilePasswordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="26129-545">workProfilePasswordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="26129-546">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-546">Int32</span></span>|<span data-ttu-id="26129-547">Указывает минимальное количество символов буквы верхнего уровня, необходимое для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="26129-547">Indicates the minimum number of upper-case letter characters required for the work profile password.</span></span> <span data-ttu-id="26129-548">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="26129-548">Valid values 1 to 16</span></span>|
|<span data-ttu-id="26129-549">workProfilePasswordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="26129-549">workProfilePasswordMinimumSymbolCharacters</span></span>|<span data-ttu-id="26129-550">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-550">Int32</span></span>|<span data-ttu-id="26129-551">Указывает минимальное количество символов, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="26129-551">Indicates the minimum number of symbol characters required for the work profile password.</span></span> <span data-ttu-id="26129-552">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="26129-552">Valid values 1 to 16</span></span>|
|<span data-ttu-id="26129-553">workProfilePasswordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="26129-553">workProfilePasswordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="26129-554">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-554">Int32</span></span>|<span data-ttu-id="26129-555">Указывает длину истории паролей профиля работы, в которой пользователь не сможет ввести новый пароль, который будет таким же, как любой пароль в истории.</span><span class="sxs-lookup"><span data-stu-id="26129-555">Indicates the length of the work profile password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="26129-556">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="26129-556">Valid values 0 to 24</span></span>|
|<span data-ttu-id="26129-557">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="26129-557">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="26129-558">Int32</span><span class="sxs-lookup"><span data-stu-id="26129-558">Int32</span></span>|<span data-ttu-id="26129-559">Указывает количество случаев, когда пользователь может ввести неправильный пароль профиля работы до стирки устройства.</span><span class="sxs-lookup"><span data-stu-id="26129-559">Indicates the number of times a user can enter an incorrect work profile password before the device is wiped.</span></span> <span data-ttu-id="26129-560">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="26129-560">Valid values 4 to 11</span></span>|
|<span data-ttu-id="26129-561">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="26129-561">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="26129-562">AndroidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="26129-562">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="26129-563">Указывает минимальное качество пароля, необходимое для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="26129-563">Indicates the minimum password quality required on the work profile password.</span></span> <span data-ttu-id="26129-564">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="26129-564">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="26129-565">Отклик</span><span class="sxs-lookup"><span data-stu-id="26129-565">Response</span></span>
<span data-ttu-id="26129-566">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="26129-566">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26129-567">Пример</span><span class="sxs-lookup"><span data-stu-id="26129-567">Example</span></span>

### <a name="request"></a><span data-ttu-id="26129-568">Запрос</span><span class="sxs-lookup"><span data-stu-id="26129-568">Request</span></span>
<span data-ttu-id="26129-569">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26129-569">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="26129-570">Отклик</span><span class="sxs-lookup"><span data-stu-id="26129-570">Response</span></span>
<span data-ttu-id="26129-p160">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26129-p160">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




