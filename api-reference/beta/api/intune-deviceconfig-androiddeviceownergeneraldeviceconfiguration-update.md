---
title: Обновление androidDeviceOwnerGeneralDeviceConfiguration
description: Обновление свойств объекта androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a64994ec79fe60e121d920027576302837bcbaa
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155246"
---
# <a name="update-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="37d91-103">Обновление androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="37d91-103">Update androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="37d91-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37d91-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37d91-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37d91-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37d91-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37d91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37d91-107">Обновление свойств объекта [androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37d91-107">Update the properties of a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37d91-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="37d91-108">Prerequisites</span></span>
<span data-ttu-id="37d91-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37d91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37d91-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37d91-111">Permission type</span></span>|<span data-ttu-id="37d91-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="37d91-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37d91-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37d91-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37d91-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37d91-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37d91-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37d91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37d91-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37d91-116">Not supported.</span></span>|
|<span data-ttu-id="37d91-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37d91-117">Application</span></span>|<span data-ttu-id="37d91-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37d91-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37d91-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37d91-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="37d91-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="37d91-120">Request headers</span></span>
|<span data-ttu-id="37d91-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37d91-121">Header</span></span>|<span data-ttu-id="37d91-122">Значение</span><span class="sxs-lookup"><span data-stu-id="37d91-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37d91-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37d91-123">Authorization</span></span>|<span data-ttu-id="37d91-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37d91-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37d91-125">Accept</span><span class="sxs-lookup"><span data-stu-id="37d91-125">Accept</span></span>|<span data-ttu-id="37d91-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37d91-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37d91-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37d91-127">Request body</span></span>
<span data-ttu-id="37d91-128">В теле запроса предоставляем представление объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="37d91-128">In the request body, supply a JSON representation for the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="37d91-129">В следующей таблице показаны свойства, необходимые при создании [объекта androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37d91-129">The following table shows the properties that are required when you create the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="37d91-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="37d91-130">Property</span></span>|<span data-ttu-id="37d91-131">Тип</span><span class="sxs-lookup"><span data-stu-id="37d91-131">Type</span></span>|<span data-ttu-id="37d91-132">Описание</span><span class="sxs-lookup"><span data-stu-id="37d91-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37d91-133">id</span><span class="sxs-lookup"><span data-stu-id="37d91-133">id</span></span>|<span data-ttu-id="37d91-134">String</span><span class="sxs-lookup"><span data-stu-id="37d91-134">String</span></span>|<span data-ttu-id="37d91-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="37d91-135">Key of the entity.</span></span> <span data-ttu-id="37d91-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37d91-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37d91-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37d91-137">lastModifiedDateTime</span></span>|<span data-ttu-id="37d91-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37d91-138">DateTimeOffset</span></span>|<span data-ttu-id="37d91-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="37d91-139">DateTime the object was last modified.</span></span> <span data-ttu-id="37d91-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37d91-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37d91-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="37d91-141">roleScopeTagIds</span></span>|<span data-ttu-id="37d91-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="37d91-142">String collection</span></span>|<span data-ttu-id="37d91-143">Список тегов области для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="37d91-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="37d91-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37d91-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37d91-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="37d91-145">supportsScopeTags</span></span>|<span data-ttu-id="37d91-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-146">Boolean</span></span>|<span data-ttu-id="37d91-147">Указывает, поддерживает ли конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="37d91-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="37d91-148">Назначение свойству ScopeTags не допускается, если это значение имеет значение false, а сущности не будут видны пользователям с заданной областью действия.</span><span class="sxs-lookup"><span data-stu-id="37d91-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="37d91-149">Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="37d91-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="37d91-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37d91-150">This property is read-only.</span></span> <span data-ttu-id="37d91-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37d91-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37d91-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="37d91-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="37d91-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="37d91-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="37d91-154">Применимость выпуска ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="37d91-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="37d91-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37d91-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37d91-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="37d91-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="37d91-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="37d91-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="37d91-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="37d91-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="37d91-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37d91-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37d91-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="37d91-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="37d91-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="37d91-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="37d91-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="37d91-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="37d91-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37d91-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37d91-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37d91-164">createdDateTime</span></span>|<span data-ttu-id="37d91-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37d91-165">DateTimeOffset</span></span>|<span data-ttu-id="37d91-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="37d91-166">DateTime the object was created.</span></span> <span data-ttu-id="37d91-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37d91-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37d91-168">description</span><span class="sxs-lookup"><span data-stu-id="37d91-168">description</span></span>|<span data-ttu-id="37d91-169">String</span><span class="sxs-lookup"><span data-stu-id="37d91-169">String</span></span>|<span data-ttu-id="37d91-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="37d91-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="37d91-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37d91-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37d91-172">displayName</span><span class="sxs-lookup"><span data-stu-id="37d91-172">displayName</span></span>|<span data-ttu-id="37d91-173">String</span><span class="sxs-lookup"><span data-stu-id="37d91-173">String</span></span>|<span data-ttu-id="37d91-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="37d91-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="37d91-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37d91-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37d91-176">version</span><span class="sxs-lookup"><span data-stu-id="37d91-176">version</span></span>|<span data-ttu-id="37d91-177">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-177">Int32</span></span>|<span data-ttu-id="37d91-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="37d91-178">Version of the device configuration.</span></span> <span data-ttu-id="37d91-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37d91-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37d91-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="37d91-180">accountsBlockModification</span></span>|<span data-ttu-id="37d91-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-181">Boolean</span></span>|<span data-ttu-id="37d91-182">Указывает, отключено ли добавление или удаление учетных записей.</span><span class="sxs-lookup"><span data-stu-id="37d91-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="37d91-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="37d91-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="37d91-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-184">Boolean</span></span>|<span data-ttu-id="37d91-185">Указывает, разрешено ли пользователю включить параметр неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="37d91-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="37d91-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="37d91-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="37d91-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="37d91-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="37d91-188">Указывает значение политики автоматического обновления приложения.</span><span class="sxs-lookup"><span data-stu-id="37d91-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="37d91-189">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="37d91-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="37d91-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="37d91-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="37d91-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="37d91-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="37d91-192">Указывает политику разрешений для запросов разрешений во время работы, если она не определена для конкретного приложения.</span><span class="sxs-lookup"><span data-stu-id="37d91-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="37d91-193">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="37d91-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="37d91-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="37d91-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="37d91-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-195">Boolean</span></span>|<span data-ttu-id="37d91-196">Следует ли рекомендовать всем приложениям пропускать любые добавленные подсказки о первом использовании.</span><span class="sxs-lookup"><span data-stu-id="37d91-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="37d91-197">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="37d91-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="37d91-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-198">Boolean</span></span>|<span data-ttu-id="37d91-199">Указывает, следует ли заблокировать для пользователя настройку Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="37d91-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="37d91-200">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="37d91-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="37d91-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-201">Boolean</span></span>|<span data-ttu-id="37d91-202">Указывает, следует ли заблокировать для пользователя общий доступ к контактам через Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="37d91-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="37d91-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="37d91-203">cameraBlocked</span></span>|<span data-ttu-id="37d91-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-204">Boolean</span></span>|<span data-ttu-id="37d91-205">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="37d91-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="37d91-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="37d91-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="37d91-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-207">Boolean</span></span>|<span data-ttu-id="37d91-208">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="37d91-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="37d91-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="37d91-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="37d91-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-210">Boolean</span></span>|<span data-ttu-id="37d91-211">Указывает, следует ли заблокировать для пользователей какие-либо настройки учетных данных сертификата.</span><span class="sxs-lookup"><span data-stu-id="37d91-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="37d91-212">microsoftLauncherConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="37d91-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="37d91-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-213">Boolean</span></span>|<span data-ttu-id="37d91-214">Указывает, нужно ли настраивать microsoft Launcher.</span><span class="sxs-lookup"><span data-stu-id="37d91-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="37d91-215">microsoftLauncherCustomWallpaperEnabled</span><span class="sxs-lookup"><span data-stu-id="37d91-215">microsoftLauncherCustomWallpaperEnabled</span></span>|<span data-ttu-id="37d91-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-216">Boolean</span></span>|<span data-ttu-id="37d91-217">Указывает, следует ли настраивать фоновый фон на целевых устройствах.</span><span class="sxs-lookup"><span data-stu-id="37d91-217">Indicates whether or not to configure the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="37d91-218">microsoftLauncherCustomWallpaperImageUrl</span><span class="sxs-lookup"><span data-stu-id="37d91-218">microsoftLauncherCustomWallpaperImageUrl</span></span>|<span data-ttu-id="37d91-219">String</span><span class="sxs-lookup"><span data-stu-id="37d91-219">String</span></span>|<span data-ttu-id="37d91-220">Указывает URL-адрес файла изображения, который будет использовать в качестве фона на целевых устройствах.</span><span class="sxs-lookup"><span data-stu-id="37d91-220">Indicates the URL for the image file to use as the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="37d91-221">microsoftLauncherCustomWallpaperAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="37d91-221">microsoftLauncherCustomWallpaperAllowUserModification</span></span>|<span data-ttu-id="37d91-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-222">Boolean</span></span>|<span data-ttu-id="37d91-223">Указывает, может ли пользователь изменить фоновый фон для персонализации устройства.</span><span class="sxs-lookup"><span data-stu-id="37d91-223">Indicates whether or not the user can modify the wallpaper to personalize their device.</span></span>|
|<span data-ttu-id="37d91-224">microsoftLauncherFeedEnabled</span><span class="sxs-lookup"><span data-stu-id="37d91-224">microsoftLauncherFeedEnabled</span></span>|<span data-ttu-id="37d91-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-225">Boolean</span></span>|<span data-ttu-id="37d91-226">Указывает, следует ли включить канал запуска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="37d91-226">Indicates whether or not you want to enable the launcher feed on the device.</span></span>|
|<span data-ttu-id="37d91-227">microsoftLauncherFeedAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="37d91-227">microsoftLauncherFeedAllowUserModification</span></span>|<span data-ttu-id="37d91-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-228">Boolean</span></span>|<span data-ttu-id="37d91-229">Указывает, может ли пользователь изменить канал запуска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="37d91-229">Indicates whether or not the user can modify the launcher feed on the device.</span></span>|
|<span data-ttu-id="37d91-230">microsoftLauncherDockPresenceConfiguration</span><span class="sxs-lookup"><span data-stu-id="37d91-230">microsoftLauncherDockPresenceConfiguration</span></span>|[<span data-ttu-id="37d91-231">microsoftLauncherDockPresence</span><span class="sxs-lookup"><span data-stu-id="37d91-231">microsoftLauncherDockPresence</span></span>](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|<span data-ttu-id="37d91-232">Указывает, нужно ли настраивать док-станцию устройства.</span><span class="sxs-lookup"><span data-stu-id="37d91-232">Indicates whether or not you want to configure the device dock.</span></span> <span data-ttu-id="37d91-233">Возможные значения: `notConfigured`, `show`, `hide`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="37d91-233">Possible values are: `notConfigured`, `show`, `hide`, `disabled`.</span></span>|
|<span data-ttu-id="37d91-234">microsoftLauncherDockPresenceAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="37d91-234">microsoftLauncherDockPresenceAllowUserModification</span></span>|<span data-ttu-id="37d91-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-235">Boolean</span></span>|<span data-ttu-id="37d91-236">Указывает, может ли пользователь изменить конфигурацию док-станции устройства на устройстве.</span><span class="sxs-lookup"><span data-stu-id="37d91-236">Indicates whether or not the user can modify the device dock configuration on the device.</span></span>|
|<span data-ttu-id="37d91-237">microsoftLauncherSearchBarPlacementConfiguration</span><span class="sxs-lookup"><span data-stu-id="37d91-237">microsoftLauncherSearchBarPlacementConfiguration</span></span>|[<span data-ttu-id="37d91-238">microsoftLauncherSearchBarPlacement</span><span class="sxs-lookup"><span data-stu-id="37d91-238">microsoftLauncherSearchBarPlacement</span></span>](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|<span data-ttu-id="37d91-239">Указывает конфигурацию размещения панели поиска на устройстве.</span><span class="sxs-lookup"><span data-stu-id="37d91-239">Indicates the search bar placement configuration on the device.</span></span> <span data-ttu-id="37d91-240">Возможные значения: `notConfigured`, `top`, `bottom`, `hide`.</span><span class="sxs-lookup"><span data-stu-id="37d91-240">Possible values are: `notConfigured`, `top`, `bottom`, `hide`.</span></span>|
|<span data-ttu-id="37d91-241">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="37d91-241">enrollmentProfile</span></span>|[<span data-ttu-id="37d91-242">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="37d91-242">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="37d91-243">Указывает профиль регистрации, который необходимо настроить.</span><span class="sxs-lookup"><span data-stu-id="37d91-243">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="37d91-244">Возможные значения: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span><span class="sxs-lookup"><span data-stu-id="37d91-244">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="37d91-245">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="37d91-245">dataRoamingBlocked</span></span>|<span data-ttu-id="37d91-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-246">Boolean</span></span>|<span data-ttu-id="37d91-247">Указывает, следует ли заблокировать для пользователя роуминг данных.</span><span class="sxs-lookup"><span data-stu-id="37d91-247">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="37d91-248">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="37d91-248">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="37d91-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-249">Boolean</span></span>|<span data-ttu-id="37d91-250">Указывает, следует ли заблокировать вручную изменение даты или времени на устройстве</span><span class="sxs-lookup"><span data-stu-id="37d91-250">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="37d91-251">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="37d91-251">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="37d91-252">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="37d91-252">String collection</span></span>|<span data-ttu-id="37d91-253">Список сообщений электронной почты учетной записи Google, которые потребуются для проверки подлинности после сброса заводской настройки устройства.</span><span class="sxs-lookup"><span data-stu-id="37d91-253">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="37d91-254">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="37d91-254">factoryResetBlocked</span></span>|<span data-ttu-id="37d91-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-255">Boolean</span></span>|<span data-ttu-id="37d91-256">Указывает, отключен ли параметр сброса заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="37d91-256">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="37d91-257">globalProxy</span><span class="sxs-lookup"><span data-stu-id="37d91-257">globalProxy</span></span>|[<span data-ttu-id="37d91-258">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="37d91-258">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="37d91-259">Прокси-сервер настроен непосредственно с хост-сервером, портом и исключенными хостами.</span><span class="sxs-lookup"><span data-stu-id="37d91-259">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="37d91-260">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="37d91-260">googleAccountsBlocked</span></span>|<span data-ttu-id="37d91-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-261">Boolean</span></span>|<span data-ttu-id="37d91-262">Указывает, будут ли заблокированы учетные записи Google.</span><span class="sxs-lookup"><span data-stu-id="37d91-262">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="37d91-263">kioskCustomizationDeviceSettingsBlocked</span><span class="sxs-lookup"><span data-stu-id="37d91-263">kioskCustomizationDeviceSettingsBlocked</span></span>|<span data-ttu-id="37d91-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-264">Boolean</span></span>|<span data-ttu-id="37d91-265">Указывает, может ли пользователь получить доступ к приложению "Параметры" устройства в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-265">Indicates whether a user can access the device's Settings app while in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-266">kioskCustomizationPowerButtonActionsBlocked</span><span class="sxs-lookup"><span data-stu-id="37d91-266">kioskCustomizationPowerButtonActionsBlocked</span></span>|<span data-ttu-id="37d91-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-267">Boolean</span></span>|<span data-ttu-id="37d91-268">Отображается ли меню питания, когда пользователь долго нажимает кнопку питания устройства в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-268">Whether the power menu is shown when a user long presses the Power button of a device in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-269">kioskCustomizationStatusBar</span><span class="sxs-lookup"><span data-stu-id="37d91-269">kioskCustomizationStatusBar</span></span>|[<span data-ttu-id="37d91-270">androidDeviceOwnerKioskCustomizationStatusBar</span><span class="sxs-lookup"><span data-stu-id="37d91-270">androidDeviceOwnerKioskCustomizationStatusBar</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|<span data-ttu-id="37d91-271">Указывает, отключены ли системные сведения и уведомления в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-271">Indicates whether system info and notifications are disabled in Kiosk Mode.</span></span> <span data-ttu-id="37d91-272">Возможные значения: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.</span><span class="sxs-lookup"><span data-stu-id="37d91-272">Possible values are: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.</span></span>|
|<span data-ttu-id="37d91-273">kioskCustomizationSystemErrorWarnings</span><span class="sxs-lookup"><span data-stu-id="37d91-273">kioskCustomizationSystemErrorWarnings</span></span>|<span data-ttu-id="37d91-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-274">Boolean</span></span>|<span data-ttu-id="37d91-275">Указывает, показываются ли диалоги системных ошибок для приложений, сбой или неотвеживающие приложения, в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-275">Indicates whether system error dialogs for crashed or unresponsive apps are shown in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-276">kioskCustomizationSystemNavigation</span><span class="sxs-lookup"><span data-stu-id="37d91-276">kioskCustomizationSystemNavigation</span></span>|[<span data-ttu-id="37d91-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span><span class="sxs-lookup"><span data-stu-id="37d91-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|<span data-ttu-id="37d91-278">Указывает, какие функции навигации включены в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-278">Indicates which navigation features are enabled in Kiosk Mode.</span></span> <span data-ttu-id="37d91-279">Возможные значения: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.</span><span class="sxs-lookup"><span data-stu-id="37d91-279">Possible values are: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.</span></span>|
|<span data-ttu-id="37d91-280">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="37d91-280">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="37d91-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-281">Boolean</span></span>|<span data-ttu-id="37d91-282">Следует ли включить режим сохранения экрана или нет в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="37d91-282">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-283">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="37d91-283">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="37d91-284">String</span><span class="sxs-lookup"><span data-stu-id="37d91-284">String</span></span>|<span data-ttu-id="37d91-285">URL-адрес изображения, которое будет экранной копией устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="37d91-285">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-286">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="37d91-286">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="37d91-287">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-287">Int32</span></span>|<span data-ttu-id="37d91-288">Время в секундах, в течение которое устройство отобразит режим сохранения экрана в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-288">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="37d91-289">Допустимые значения: от 0 до 999 999 999</span><span class="sxs-lookup"><span data-stu-id="37d91-289">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="37d91-290">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="37d91-290">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="37d91-291">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-291">Int32</span></span>|<span data-ttu-id="37d91-292">Время в секундах, в течение которое устройство должно быть неактивно до того, как режим сохранения экрана будет показан в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-292">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="37d91-293">Допустимые значения: от 1 до 999 999 999</span><span class="sxs-lookup"><span data-stu-id="37d91-293">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="37d91-294">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="37d91-294">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="37d91-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-295">Boolean</span></span>|<span data-ttu-id="37d91-296">Должен ли экран устройства показывать режим сохранения экрана, если воспроизведение звука и видео в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-296">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-297">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="37d91-297">kioskModeApps</span></span>|<span data-ttu-id="37d91-298">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="37d91-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="37d91-299">Список управляемых приложений, которые будут показаны, когда устройство находится в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-299">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="37d91-300">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="37d91-300">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="37d91-301">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="37d91-301">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="37d91-302">String</span><span class="sxs-lookup"><span data-stu-id="37d91-302">String</span></span>|<span data-ttu-id="37d91-303">URL-адрес общедоступных изображений, которые будут использовать для фона, когда устройство находится в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-303">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-304">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="37d91-304">kioskModeExitCode</span></span>|<span data-ttu-id="37d91-305">String</span><span class="sxs-lookup"><span data-stu-id="37d91-305">String</span></span>|<span data-ttu-id="37d91-306">Код выхода, позволяющий пользователю выйти из режима терминала, когда устройство находится в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-306">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-307">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="37d91-307">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="37d91-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-308">Boolean</span></span>|<span data-ttu-id="37d91-309">Следует ли отображать виртуальную кнопку "Домой", когда устройство находится в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-309">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-310">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="37d91-310">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="37d91-311">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="37d91-311">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="37d91-312">Указывает, является ли виртуальная кнопка "Домой" кнопкой прокрутки вверх или с плавающей кнопкой "Домой".</span><span class="sxs-lookup"><span data-stu-id="37d91-312">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="37d91-313">Возможные значения: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="37d91-313">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="37d91-314">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="37d91-314">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="37d91-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-315">Boolean</span></span>|<span data-ttu-id="37d91-316">Позволяет ли пользователь настраивать параметры Bluetooth режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-316">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-317">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="37d91-317">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="37d91-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-318">Boolean</span></span>|<span data-ttu-id="37d91-319">Позволяет ли пользователь настраивать параметры Wi-Fi режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-319">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-320">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="37d91-320">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="37d91-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-321">Boolean</span></span>|<span data-ttu-id="37d91-322">Разрешается ли пользователю использовать фонарик в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-322">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-323">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="37d91-323">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="37d91-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-324">Boolean</span></span>|<span data-ttu-id="37d91-325">Позволяет ли пользователь изменять громкость мультимедиа в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-325">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-326">kioskModeShowDeviceInfo</span><span class="sxs-lookup"><span data-stu-id="37d91-326">kioskModeShowDeviceInfo</span></span>|<span data-ttu-id="37d91-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-327">Boolean</span></span>|<span data-ttu-id="37d91-328">Следует ли разрешить пользователю доступ к базовым сведениям об устройстве.</span><span class="sxs-lookup"><span data-stu-id="37d91-328">Whether or not to allow a user to access basic device information.</span></span>|
|<span data-ttu-id="37d91-329">kioskModeManagedSettingsEntryDisabled</span><span class="sxs-lookup"><span data-stu-id="37d91-329">kioskModeManagedSettingsEntryDisabled</span></span>|<span data-ttu-id="37d91-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-330">Boolean</span></span>|<span data-ttu-id="37d91-331">Следует ли отображать точку входа управляемых параметров на управляемом начальном экране в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-331">Whether or not to display the Managed Settings entry point on the managed home screen in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-332">kioskModeDebugMenuEasyAccessEnabled</span><span class="sxs-lookup"><span data-stu-id="37d91-332">kioskModeDebugMenuEasyAccessEnabled</span></span>|<span data-ttu-id="37d91-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-333">Boolean</span></span>|<span data-ttu-id="37d91-334">Позволяет ли пользователю легко получать доступ к меню отлаживания в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-334">Whether or not to allow a user to easy access to the debug menu in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-335">kioskModeShowAppNotificationBadge</span><span class="sxs-lookup"><span data-stu-id="37d91-335">kioskModeShowAppNotificationBadge</span></span>|<span data-ttu-id="37d91-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-336">Boolean</span></span>|<span data-ttu-id="37d91-337">Следует ли отображать индикаторы событий уведомлений приложения в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-337">Whether or not to display application notification badges in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-338">kioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="37d91-338">kioskModeScreenOrientation</span></span>|[<span data-ttu-id="37d91-339">androidDeviceOwnerKioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="37d91-339">androidDeviceOwnerKioskModeScreenOrientation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|<span data-ttu-id="37d91-340">Настройка ориентации экрана для управляемого домашнего экрана в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-340">Screen orientation configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="37d91-341">Возможные значения: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span><span class="sxs-lookup"><span data-stu-id="37d91-341">Possible values are: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span></span>|
|<span data-ttu-id="37d91-342">kioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="37d91-342">kioskModeIconSize</span></span>|[<span data-ttu-id="37d91-343">androidDeviceOwnerKioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="37d91-343">androidDeviceOwnerKioskModeIconSize</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|<span data-ttu-id="37d91-344">Конфигурация размера значка для управляемого домашнего экрана в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-344">Icon size configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="37d91-345">Возможные значения: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span><span class="sxs-lookup"><span data-stu-id="37d91-345">Possible values are: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span></span>|
|<span data-ttu-id="37d91-346">kioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="37d91-346">kioskModeFolderIcon</span></span>|[<span data-ttu-id="37d91-347">androidDeviceOwnerKioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="37d91-347">androidDeviceOwnerKioskModeFolderIcon</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|<span data-ttu-id="37d91-348">Настройка значков папок для управляемого домашнего экрана в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-348">Folder icon configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="37d91-349">Возможные значения: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span><span class="sxs-lookup"><span data-stu-id="37d91-349">Possible values are: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span></span>|
|<span data-ttu-id="37d91-350">kioskModeWifiAllowedSsids</span><span class="sxs-lookup"><span data-stu-id="37d91-350">kioskModeWifiAllowedSsids</span></span>|<span data-ttu-id="37d91-351">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="37d91-351">String collection</span></span>|<span data-ttu-id="37d91-352">Ограниченный набор SSID WIFI, доступный пользователю для настройки в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-352">The restricted set of WIFI SSIDs available for the user to configure in Kiosk Mode.</span></span> <span data-ttu-id="37d91-353">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="37d91-353">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="37d91-354">kioskModeAppOrderEnabled</span><span class="sxs-lookup"><span data-stu-id="37d91-354">kioskModeAppOrderEnabled</span></span>|<span data-ttu-id="37d91-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-355">Boolean</span></span>|<span data-ttu-id="37d91-356">Следует ли включить порядок приложений в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-356">Whether or not to enable app ordering in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-357">kioskModeAppsInFolderOrderedByName</span><span class="sxs-lookup"><span data-stu-id="37d91-357">kioskModeAppsInFolderOrderedByName</span></span>|<span data-ttu-id="37d91-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-358">Boolean</span></span>|<span data-ttu-id="37d91-359">Следует ли в алфавитном порядке определить приложения в папке в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-359">Whether or not to alphabetize applications within a folder in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-360">kioskModeGridHeight</span><span class="sxs-lookup"><span data-stu-id="37d91-360">kioskModeGridHeight</span></span>|<span data-ttu-id="37d91-361">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-361">Int32</span></span>|<span data-ttu-id="37d91-362">Количество строк для сетки управляемого домашнего экрана с включенным порядком приложения в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-362">Number of rows for Managed Home Screen grid with app ordering enabled in Kiosk Mode.</span></span> <span data-ttu-id="37d91-363">Допустимые значения: от 1 до 999 999 999</span><span class="sxs-lookup"><span data-stu-id="37d91-363">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="37d91-364">kioskModeGridWidth</span><span class="sxs-lookup"><span data-stu-id="37d91-364">kioskModeGridWidth</span></span>|<span data-ttu-id="37d91-365">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-365">Int32</span></span>|<span data-ttu-id="37d91-366">Количество столбцов для сетки управляемого домашнего экрана с включенным порядком приложения в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-366">Number of columns for Managed Home Screen grid with app ordering enabled in Kiosk Mode.</span></span> <span data-ttu-id="37d91-367">Допустимые значения: от 1 до 999 999 999</span><span class="sxs-lookup"><span data-stu-id="37d91-367">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="37d91-368">kioskModeLockHomeScreen</span><span class="sxs-lookup"><span data-stu-id="37d91-368">kioskModeLockHomeScreen</span></span>|<span data-ttu-id="37d91-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-369">Boolean</span></span>|<span data-ttu-id="37d91-370">Следует ли заблокировать домашний экран для пользователя в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-370">Whether or not to lock home screen to the end user in Kiosk Mode.</span></span>|
|<span data-ttu-id="37d91-371">kioskModeManagedFolders</span><span class="sxs-lookup"><span data-stu-id="37d91-371">kioskModeManagedFolders</span></span>|<span data-ttu-id="37d91-372">[Коллекция androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md)</span><span class="sxs-lookup"><span data-stu-id="37d91-372">[androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md) collection</span></span>|<span data-ttu-id="37d91-373">Список управляемых папок для устройства в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-373">A list of managed folders for a device in Kiosk Mode.</span></span> <span data-ttu-id="37d91-374">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="37d91-374">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="37d91-375">kioskModeAppPositions</span><span class="sxs-lookup"><span data-stu-id="37d91-375">kioskModeAppPositions</span></span>|<span data-ttu-id="37d91-376">[Коллекция androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md)</span><span class="sxs-lookup"><span data-stu-id="37d91-376">[androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md) collection</span></span>|<span data-ttu-id="37d91-377">Порядок элементов на управляемом домашнем экране в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="37d91-377">The ordering of items on Kiosk Mode Managed Home Screen.</span></span> <span data-ttu-id="37d91-378">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="37d91-378">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="37d91-379">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="37d91-379">microphoneForceMute</span></span>|<span data-ttu-id="37d91-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-380">Boolean</span></span>|<span data-ttu-id="37d91-381">Указывает, следует ли заблокировать микрофон на устройстве.</span><span class="sxs-lookup"><span data-stu-id="37d91-381">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="37d91-382">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="37d91-382">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="37d91-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-383">Boolean</span></span>|<span data-ttu-id="37d91-384">Указывает, разрешит ли устройство подключение к временному сетевому подключению во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="37d91-384">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="37d91-385">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="37d91-385">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="37d91-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-386">Boolean</span></span>|<span data-ttu-id="37d91-387">Указывает, следует ли заблокировать исходяние NFC.</span><span class="sxs-lookup"><span data-stu-id="37d91-387">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="37d91-388">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="37d91-388">passwordBlockKeyguard</span></span>|<span data-ttu-id="37d91-389">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-389">Boolean</span></span>|<span data-ttu-id="37d91-390">Указывает, отключен ли keyguard.</span><span class="sxs-lookup"><span data-stu-id="37d91-390">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="37d91-391">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="37d91-391">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="37d91-392">[Коллекция androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="37d91-392">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="37d91-393">Список функций keyguard устройства, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="37d91-393">List of device keyguard features to block.</span></span> <span data-ttu-id="37d91-394">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="37d91-394">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="37d91-395">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="37d91-395">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="37d91-396">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="37d91-396">passwordExpirationDays</span></span>|<span data-ttu-id="37d91-397">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-397">Int32</span></span>|<span data-ttu-id="37d91-398">Указывает время, в течение которого можно установить пароль до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="37d91-398">Indicates the amount of time that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="37d91-399">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="37d91-399">Valid values 1 to 365</span></span>|
|<span data-ttu-id="37d91-400">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="37d91-400">passwordMinimumLength</span></span>|<span data-ttu-id="37d91-401">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-401">Int32</span></span>|<span data-ttu-id="37d91-402">Указывает минимальную длину пароля, необходимого на устройстве.</span><span class="sxs-lookup"><span data-stu-id="37d91-402">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="37d91-403">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="37d91-403">Valid values 4 to 16</span></span>|
|<span data-ttu-id="37d91-404">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="37d91-404">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="37d91-405">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-405">Int32</span></span>|<span data-ttu-id="37d91-406">Указывает минимальное количество букв, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="37d91-406">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="37d91-407">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="37d91-407">Valid values 1 to 16</span></span>|
|<span data-ttu-id="37d91-408">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="37d91-408">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="37d91-409">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-409">Int32</span></span>|<span data-ttu-id="37d91-410">Указывает минимальное количество символов нижнего дела, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="37d91-410">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="37d91-411">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="37d91-411">Valid values 1 to 16</span></span>|
|<span data-ttu-id="37d91-412">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="37d91-412">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="37d91-413">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-413">Int32</span></span>|<span data-ttu-id="37d91-414">Указывает минимальное количество символов, не букв, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="37d91-414">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="37d91-415">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="37d91-415">Valid values 1 to 16</span></span>|
|<span data-ttu-id="37d91-416">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="37d91-416">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="37d91-417">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-417">Int32</span></span>|<span data-ttu-id="37d91-418">Указывает минимальное число цифр, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="37d91-418">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="37d91-419">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="37d91-419">Valid values 1 to 16</span></span>|
|<span data-ttu-id="37d91-420">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="37d91-420">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="37d91-421">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-421">Int32</span></span>|<span data-ttu-id="37d91-422">Указывает минимальное количество символов, необходимых для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="37d91-422">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="37d91-423">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="37d91-423">Valid values 1 to 16</span></span>|
|<span data-ttu-id="37d91-424">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="37d91-424">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="37d91-425">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-425">Int32</span></span>|<span data-ttu-id="37d91-426">Указывает минимальное количество символов в верхнем букве, необходимое для пароля устройства.</span><span class="sxs-lookup"><span data-stu-id="37d91-426">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="37d91-427">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="37d91-427">Valid values 1 to 16</span></span>|
|<span data-ttu-id="37d91-428">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="37d91-428">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="37d91-429">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-429">Int32</span></span>|<span data-ttu-id="37d91-430">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="37d91-430">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="37d91-431">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="37d91-431">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="37d91-432">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-432">Int32</span></span>|<span data-ttu-id="37d91-433">Указывает длину истории паролей, в которой пользователь не сможет ввести новый пароль, который будет таким же, как любой пароль в истории.</span><span class="sxs-lookup"><span data-stu-id="37d91-433">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="37d91-434">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="37d91-434">Valid values 0 to 24</span></span>|
|<span data-ttu-id="37d91-435">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="37d91-435">passwordRequiredType</span></span>|[<span data-ttu-id="37d91-436">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="37d91-436">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="37d91-437">Указывает минимальное качество пароля, необходимое на устройстве.</span><span class="sxs-lookup"><span data-stu-id="37d91-437">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="37d91-438">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="37d91-438">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="37d91-439">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="37d91-439">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="37d91-440">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-440">Int32</span></span>|<span data-ttu-id="37d91-441">Указывает, сколько раз пользователь может ввести неправильный пароль перед тем, как стирать устройство.</span><span class="sxs-lookup"><span data-stu-id="37d91-441">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="37d91-442">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="37d91-442">Valid values 4 to 11</span></span>|
|<span data-ttu-id="37d91-443">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="37d91-443">playStoreMode</span></span>|[<span data-ttu-id="37d91-444">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="37d91-444">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="37d91-445">Указывает режим воспроизведения устройства.</span><span class="sxs-lookup"><span data-stu-id="37d91-445">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="37d91-446">Возможные значения: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="37d91-446">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="37d91-447">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="37d91-447">safeBootBlocked</span></span>|<span data-ttu-id="37d91-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-448">Boolean</span></span>|<span data-ttu-id="37d91-449">Указывает, отключена ли перезагрузка устройства в безопасной загрузке.</span><span class="sxs-lookup"><span data-stu-id="37d91-449">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="37d91-450">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="37d91-450">screenCaptureBlocked</span></span>|<span data-ttu-id="37d91-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-451">Boolean</span></span>|<span data-ttu-id="37d91-452">Указывает, следует ли отключить возможность делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="37d91-452">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="37d91-453">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="37d91-453">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="37d91-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-454">Boolean</span></span>|<span data-ttu-id="37d91-455">Указывает, следует ли заблокировать для пользователя включение функций отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="37d91-455">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="37d91-456">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="37d91-456">securityRequireVerifyApps</span></span>|<span data-ttu-id="37d91-457">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-457">Boolean</span></span>|<span data-ttu-id="37d91-458">Указывает, требуются ли приложения.</span><span class="sxs-lookup"><span data-stu-id="37d91-458">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="37d91-459">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="37d91-459">statusBarBlocked</span></span>|<span data-ttu-id="37d91-460">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-460">Boolean</span></span>|<span data-ttu-id="37d91-461">Указывает, отключена ли ли ни одна из них, включая уведомления, быстрые параметры и другие наложения экрана.</span><span class="sxs-lookup"><span data-stu-id="37d91-461">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="37d91-462">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="37d91-462">stayOnModes</span></span>|<span data-ttu-id="37d91-463">[Коллекция androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="37d91-463">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="37d91-464">Список режимов, в которых дисплей устройства будет оставаться в режиме питания.</span><span class="sxs-lookup"><span data-stu-id="37d91-464">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="37d91-465">Эта коллекция может содержать не более 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="37d91-465">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="37d91-466">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="37d91-466">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="37d91-467">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="37d91-467">storageAllowUsb</span></span>|<span data-ttu-id="37d91-468">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-468">Boolean</span></span>|<span data-ttu-id="37d91-469">Указывает, следует ли разрешить usb-накопитель.</span><span class="sxs-lookup"><span data-stu-id="37d91-469">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="37d91-470">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="37d91-470">storageBlockExternalMedia</span></span>|<span data-ttu-id="37d91-471">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-471">Boolean</span></span>|<span data-ttu-id="37d91-472">Указывает, следует ли блокировать внешние носитли.</span><span class="sxs-lookup"><span data-stu-id="37d91-472">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="37d91-473">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="37d91-473">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="37d91-474">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-474">Boolean</span></span>|<span data-ttu-id="37d91-475">Указывает, следует ли заблокировать передачу USB-файла.</span><span class="sxs-lookup"><span data-stu-id="37d91-475">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="37d91-476">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="37d91-476">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="37d91-477">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-477">Int32</span></span>|<span data-ttu-id="37d91-478">Указывает количество минут после полуночи, в течение чего начинается окно обновления системы.</span><span class="sxs-lookup"><span data-stu-id="37d91-478">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="37d91-479">Допустимые значения: от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="37d91-479">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="37d91-480">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="37d91-480">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="37d91-481">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-481">Int32</span></span>|<span data-ttu-id="37d91-482">Указывает количество минут после полуночи окончания окна обновления системы.</span><span class="sxs-lookup"><span data-stu-id="37d91-482">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="37d91-483">Допустимые значения: от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="37d91-483">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="37d91-484">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="37d91-484">systemUpdateInstallType</span></span>|[<span data-ttu-id="37d91-485">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="37d91-485">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="37d91-486">Тип конфигурации обновления системы.</span><span class="sxs-lookup"><span data-stu-id="37d91-486">The type of system update configuration.</span></span> <span data-ttu-id="37d91-487">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="37d91-487">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="37d91-488">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="37d91-488">systemWindowsBlocked</span></span>|<span data-ttu-id="37d91-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-489">Boolean</span></span>|<span data-ttu-id="37d91-490">Следует ли блокировать окна системных подсказок Android, например всплывающие уведомления, действия с телефоном и системные оповещения.</span><span class="sxs-lookup"><span data-stu-id="37d91-490">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="37d91-491">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="37d91-491">usersBlockAdd</span></span>|<span data-ttu-id="37d91-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-492">Boolean</span></span>|<span data-ttu-id="37d91-493">Указывает, отключено ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="37d91-493">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="37d91-494">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="37d91-494">usersBlockRemove</span></span>|<span data-ttu-id="37d91-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-495">Boolean</span></span>|<span data-ttu-id="37d91-496">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="37d91-496">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="37d91-497">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="37d91-497">volumeBlockAdjustment</span></span>|<span data-ttu-id="37d91-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-498">Boolean</span></span>|<span data-ttu-id="37d91-499">Указывает, отключена ли настройка этого тома.</span><span class="sxs-lookup"><span data-stu-id="37d91-499">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="37d91-500">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="37d91-500">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="37d91-501">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-501">Boolean</span></span>|<span data-ttu-id="37d91-502">Если указано имя пакета VPN, следует ли заблокировать сетевой трафик при отключении vpn.</span><span class="sxs-lookup"><span data-stu-id="37d91-502">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="37d91-503">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="37d91-503">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="37d91-504">String</span><span class="sxs-lookup"><span data-stu-id="37d91-504">String</span></span>|<span data-ttu-id="37d91-505">Имя пакета приложения Android для приложения, которое будет обрабатывать постоянное VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="37d91-505">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="37d91-506">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="37d91-506">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="37d91-507">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-507">Boolean</span></span>|<span data-ttu-id="37d91-508">Указывает, следует ли заблокировать для пользователя изменение параметров подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="37d91-508">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="37d91-509">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="37d91-509">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="37d91-510">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-510">Boolean</span></span>|<span data-ttu-id="37d91-511">Указывает, следует ли заблокировать для пользователя редактирование только сетей, определенных политикой.</span><span class="sxs-lookup"><span data-stu-id="37d91-511">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|
|<span data-ttu-id="37d91-512">personalProfileAppsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="37d91-512">personalProfileAppsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="37d91-513">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-513">Boolean</span></span>|<span data-ttu-id="37d91-514">Указывает, может ли пользователь устанавливать приложения из неизвестных источников в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="37d91-514">Indicates whether the user can install apps from unknown sources on the personal profile.</span></span>|
|<span data-ttu-id="37d91-515">personalProfileCameraBlocked</span><span class="sxs-lookup"><span data-stu-id="37d91-515">personalProfileCameraBlocked</span></span>|<span data-ttu-id="37d91-516">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-516">Boolean</span></span>|<span data-ttu-id="37d91-517">Указывает, следует ли отключить использование камеры в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="37d91-517">Indicates whether to disable the use of the camera on the personal profile.</span></span>|
|<span data-ttu-id="37d91-518">personalProfileScreenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="37d91-518">personalProfileScreenCaptureBlocked</span></span>|<span data-ttu-id="37d91-519">Boolean</span><span class="sxs-lookup"><span data-stu-id="37d91-519">Boolean</span></span>|<span data-ttu-id="37d91-520">Указывает, следует ли отключить возможность делать снимки экрана в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="37d91-520">Indicates whether to disable the capability to take screenshots on the personal profile.</span></span>|
|<span data-ttu-id="37d91-521">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="37d91-521">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="37d91-522">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-522">Int32</span></span>|<span data-ttu-id="37d91-523">Указывает количество дней, в течение которых можно установить пароль профиля работы до истечения срока его действия, и потребуется новый пароль.</span><span class="sxs-lookup"><span data-stu-id="37d91-523">Indicates the number of days that a work profile password can be set before it expires and a new password will be required.</span></span> <span data-ttu-id="37d91-524">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="37d91-524">Valid values 1 to 365</span></span>|
|<span data-ttu-id="37d91-525">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="37d91-525">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="37d91-526">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-526">Int32</span></span>|<span data-ttu-id="37d91-527">Указывает минимальную длину пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="37d91-527">Indicates the minimum length of the work profile password.</span></span> <span data-ttu-id="37d91-528">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="37d91-528">Valid values 4 to 16</span></span>|
|<span data-ttu-id="37d91-529">workProfilePasswordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="37d91-529">workProfilePasswordMinimumNumericCharacters</span></span>|<span data-ttu-id="37d91-530">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-530">Int32</span></span>|<span data-ttu-id="37d91-531">Указывает минимальное число цифр, необходимое для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="37d91-531">Indicates the minimum number of numeric characters required for the work profile password.</span></span> <span data-ttu-id="37d91-532">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="37d91-532">Valid values 1 to 16</span></span>|
|<span data-ttu-id="37d91-533">workProfilePasswordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="37d91-533">workProfilePasswordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="37d91-534">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-534">Int32</span></span>|<span data-ttu-id="37d91-535">Указывает минимальное количество символов, не букв, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="37d91-535">Indicates the minimum number of non-letter characters required for the work profile password.</span></span> <span data-ttu-id="37d91-536">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="37d91-536">Valid values 1 to 16</span></span>|
|<span data-ttu-id="37d91-537">workProfilePasswordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="37d91-537">workProfilePasswordMinimumLetterCharacters</span></span>|<span data-ttu-id="37d91-538">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-538">Int32</span></span>|<span data-ttu-id="37d91-539">Указывает минимальное количество букв, необходимое для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="37d91-539">Indicates the minimum number of letter characters required for the work profile password.</span></span> <span data-ttu-id="37d91-540">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="37d91-540">Valid values 1 to 16</span></span>|
|<span data-ttu-id="37d91-541">workProfilePasswordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="37d91-541">workProfilePasswordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="37d91-542">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-542">Int32</span></span>|<span data-ttu-id="37d91-543">Указывает минимальное количество символов нижнего уровня, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="37d91-543">Indicates the minimum number of lower-case characters required for the work profile password.</span></span> <span data-ttu-id="37d91-544">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="37d91-544">Valid values 1 to 16</span></span>|
|<span data-ttu-id="37d91-545">workProfilePasswordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="37d91-545">workProfilePasswordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="37d91-546">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-546">Int32</span></span>|<span data-ttu-id="37d91-547">Указывает минимальное количество символов в верхнем случае, необходимое для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="37d91-547">Indicates the minimum number of upper-case letter characters required for the work profile password.</span></span> <span data-ttu-id="37d91-548">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="37d91-548">Valid values 1 to 16</span></span>|
|<span data-ttu-id="37d91-549">workProfilePasswordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="37d91-549">workProfilePasswordMinimumSymbolCharacters</span></span>|<span data-ttu-id="37d91-550">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-550">Int32</span></span>|<span data-ttu-id="37d91-551">Указывает минимальное количество символов, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="37d91-551">Indicates the minimum number of symbol characters required for the work profile password.</span></span> <span data-ttu-id="37d91-552">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="37d91-552">Valid values 1 to 16</span></span>|
|<span data-ttu-id="37d91-553">workProfilePasswordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="37d91-553">workProfilePasswordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="37d91-554">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-554">Int32</span></span>|<span data-ttu-id="37d91-555">Указывает длину истории паролей профиля работы, в которой пользователь не сможет ввести новый пароль, который будет таким же, как любой пароль в истории.</span><span class="sxs-lookup"><span data-stu-id="37d91-555">Indicates the length of the work profile password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="37d91-556">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="37d91-556">Valid values 0 to 24</span></span>|
|<span data-ttu-id="37d91-557">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="37d91-557">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="37d91-558">Int32</span><span class="sxs-lookup"><span data-stu-id="37d91-558">Int32</span></span>|<span data-ttu-id="37d91-559">Указывает, сколько раз пользователь может ввести неправильный пароль к профилю работы перед тем, как устройство будет стирано.</span><span class="sxs-lookup"><span data-stu-id="37d91-559">Indicates the number of times a user can enter an incorrect work profile password before the device is wiped.</span></span> <span data-ttu-id="37d91-560">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="37d91-560">Valid values 4 to 11</span></span>|
|<span data-ttu-id="37d91-561">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="37d91-561">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="37d91-562">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="37d91-562">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="37d91-563">Указывает минимальное качество пароля, необходимое для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="37d91-563">Indicates the minimum password quality required on the work profile password.</span></span> <span data-ttu-id="37d91-564">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="37d91-564">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="37d91-565">Отклик</span><span class="sxs-lookup"><span data-stu-id="37d91-565">Response</span></span>
<span data-ttu-id="37d91-566">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="37d91-566">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37d91-567">Пример</span><span class="sxs-lookup"><span data-stu-id="37d91-567">Example</span></span>

### <a name="request"></a><span data-ttu-id="37d91-568">Запрос</span><span class="sxs-lookup"><span data-stu-id="37d91-568">Request</span></span>
<span data-ttu-id="37d91-569">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37d91-569">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37d91-570">Отклик</span><span class="sxs-lookup"><span data-stu-id="37d91-570">Response</span></span>
<span data-ttu-id="37d91-p160">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37d91-p160">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




