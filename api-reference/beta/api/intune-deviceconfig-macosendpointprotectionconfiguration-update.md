---
title: Обновление macOSEndpointProtectionConfiguration
description: Обновление свойств объекта macOSEndpointProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 23e7bc30a9b5410e6f33e96d628654e1f9f69ebc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131325"
---
# <a name="update-macosendpointprotectionconfiguration"></a><span data-ttu-id="0ea1a-103">Обновление macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ea1a-103">Update macOSEndpointProtectionConfiguration</span></span>

<span data-ttu-id="0ea1a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ea1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ea1a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ea1a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ea1a-107">Обновление свойств объекта [macOSEndpointProtectionConfiguration.](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ea1a-107">Update the properties of a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ea1a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0ea1a-108">Prerequisites</span></span>
<span data-ttu-id="0ea1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ea1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ea1a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ea1a-111">Permission type</span></span>|<span data-ttu-id="0ea1a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ea1a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ea1a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ea1a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ea1a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ea1a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ea1a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ea1a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ea1a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-116">Not supported.</span></span>|
|<span data-ttu-id="0ea1a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0ea1a-117">Application</span></span>|<span data-ttu-id="0ea1a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ea1a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ea1a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ea1a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0ea1a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0ea1a-120">Request headers</span></span>
|<span data-ttu-id="0ea1a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ea1a-121">Header</span></span>|<span data-ttu-id="0ea1a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0ea1a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ea1a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ea1a-123">Authorization</span></span>|<span data-ttu-id="0ea1a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ea1a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ea1a-125">Accept</span></span>|<span data-ttu-id="0ea1a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ea1a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ea1a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ea1a-127">Request body</span></span>
<span data-ttu-id="0ea1a-128">В теле запроса устройте представление JSON для [объекта macOSEndpointProtectionConfiguration.](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ea1a-128">In the request body, supply a JSON representation for the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="0ea1a-129">В следующей таблице показаны свойства, необходимые при создании [macOSEndpointProtectionConfiguration.](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ea1a-129">The following table shows the properties that are required when you create the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="0ea1a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ea1a-130">Property</span></span>|<span data-ttu-id="0ea1a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0ea1a-131">Type</span></span>|<span data-ttu-id="0ea1a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0ea1a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ea1a-133">id</span><span class="sxs-lookup"><span data-stu-id="0ea1a-133">id</span></span>|<span data-ttu-id="0ea1a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0ea1a-134">String</span></span>|<span data-ttu-id="0ea1a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-135">Key of the entity.</span></span> <span data-ttu-id="0ea1a-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ea1a-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ea1a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ea1a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0ea1a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ea1a-138">DateTimeOffset</span></span>|<span data-ttu-id="0ea1a-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0ea1a-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ea1a-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ea1a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0ea1a-141">roleScopeTagIds</span></span>|<span data-ttu-id="0ea1a-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0ea1a-142">String collection</span></span>|<span data-ttu-id="0ea1a-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0ea1a-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ea1a-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ea1a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0ea1a-145">supportsScopeTags</span></span>|<span data-ttu-id="0ea1a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ea1a-146">Boolean</span></span>|<span data-ttu-id="0ea1a-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0ea1a-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0ea1a-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0ea1a-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-150">This property is read-only.</span></span> <span data-ttu-id="0ea1a-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ea1a-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ea1a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0ea1a-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0ea1a-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0ea1a-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0ea1a-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0ea1a-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ea1a-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ea1a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0ea1a-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0ea1a-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0ea1a-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0ea1a-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0ea1a-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ea1a-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ea1a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0ea1a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0ea1a-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0ea1a-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0ea1a-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0ea1a-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ea1a-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ea1a-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ea1a-164">createdDateTime</span></span>|<span data-ttu-id="0ea1a-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ea1a-165">DateTimeOffset</span></span>|<span data-ttu-id="0ea1a-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-166">DateTime the object was created.</span></span> <span data-ttu-id="0ea1a-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ea1a-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ea1a-168">description</span><span class="sxs-lookup"><span data-stu-id="0ea1a-168">description</span></span>|<span data-ttu-id="0ea1a-169">Строка</span><span class="sxs-lookup"><span data-stu-id="0ea1a-169">String</span></span>|<span data-ttu-id="0ea1a-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0ea1a-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ea1a-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ea1a-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0ea1a-172">displayName</span></span>|<span data-ttu-id="0ea1a-173">Строка</span><span class="sxs-lookup"><span data-stu-id="0ea1a-173">String</span></span>|<span data-ttu-id="0ea1a-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0ea1a-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ea1a-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ea1a-176">version</span><span class="sxs-lookup"><span data-stu-id="0ea1a-176">version</span></span>|<span data-ttu-id="0ea1a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0ea1a-177">Int32</span></span>|<span data-ttu-id="0ea1a-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-178">Version of the device configuration.</span></span> <span data-ttu-id="0ea1a-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0ea1a-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ea1a-180">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="0ea1a-180">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="0ea1a-181">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="0ea1a-181">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="0ea1a-182">Параметр System и Privacy, который определяет, какие приложения для скачивания можно запускать на macOS-устройстве.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-182">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="0ea1a-183">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-183">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="0ea1a-184">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="0ea1a-184">gatekeeperBlockOverride</span></span>|<span data-ttu-id="0ea1a-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ea1a-185">Boolean</span></span>|<span data-ttu-id="0ea1a-186">Если задана истина, переопределения пользователя для Gatekeeper будут отключены.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-186">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="0ea1a-187">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="0ea1a-187">firewallEnabled</span></span>|<span data-ttu-id="0ea1a-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ea1a-188">Boolean</span></span>|<span data-ttu-id="0ea1a-189">Следует ли включить брандмауэр или нет.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-189">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="0ea1a-190">брандмауэрBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="0ea1a-190">firewallBlockAllIncoming</span></span>|<span data-ttu-id="0ea1a-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ea1a-191">Boolean</span></span>|<span data-ttu-id="0ea1a-192">Соответствует параметру "Блокировка всех входящих подключений".</span><span class="sxs-lookup"><span data-stu-id="0ea1a-192">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="0ea1a-193">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="0ea1a-193">firewallEnableStealthMode</span></span>|<span data-ttu-id="0ea1a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ea1a-194">Boolean</span></span>|<span data-ttu-id="0ea1a-195">Соответствует режиму "Включить режим стелс".</span><span class="sxs-lookup"><span data-stu-id="0ea1a-195">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="0ea1a-196">брандмауэрАпплиляции</span><span class="sxs-lookup"><span data-stu-id="0ea1a-196">firewallApplications</span></span>|<span data-ttu-id="0ea1a-197">[коллекция macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)</span><span class="sxs-lookup"><span data-stu-id="0ea1a-197">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="0ea1a-198">Список приложений с настройками брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-198">List of applications with firewall settings.</span></span> <span data-ttu-id="0ea1a-199">Параметры брандмауэра для приложений, не входящего в этот список, определяются пользователем.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-199">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="0ea1a-200">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-200">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0ea1a-201">fileVaultEnabled</span><span class="sxs-lookup"><span data-stu-id="0ea1a-201">fileVaultEnabled</span></span>|<span data-ttu-id="0ea1a-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ea1a-202">Boolean</span></span>|<span data-ttu-id="0ea1a-203">Следует ли включить FileVault или нет.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-203">Whether FileVault should be enabled or not.</span></span>|
|<span data-ttu-id="0ea1a-204">fileVaultSelectedRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="0ea1a-204">fileVaultSelectedRecoveryKeyTypes</span></span>|[<span data-ttu-id="0ea1a-205">macOSFileVaultRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="0ea1a-205">macOSFileVaultRecoveryKeyTypes</span></span>](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|<span data-ttu-id="0ea1a-206">Требуется, если включен FileVault, определяет тип(ы) ключа восстановления для использования.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-206">Required if FileVault is enabled, determines the type(s) of recovery key to use.</span></span> <span data-ttu-id="0ea1a-207">.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-207">.</span></span> <span data-ttu-id="0ea1a-208">Возможные значения: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-208">Possible values are: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span></span>|
|<span data-ttu-id="0ea1a-209">fileVaultInstitutionalRecoveryKeyCertificate</span><span class="sxs-lookup"><span data-stu-id="0ea1a-209">fileVaultInstitutionalRecoveryKeyCertificate</span></span>|<span data-ttu-id="0ea1a-210">Binary</span><span class="sxs-lookup"><span data-stu-id="0ea1a-210">Binary</span></span>|<span data-ttu-id="0ea1a-211">Необходимый, если выбранный тип ключа восстановления (s) включает InstitutionalRecoveryKey.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-211">Required if selected recovery key type(s) include InstitutionalRecoveryKey.</span></span> <span data-ttu-id="0ea1a-212">Кодированный файл сертификата DER, используемый для задавания институционального ключа восстановления.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-212">The DER Encoded certificate file used to set an institutional recovery key.</span></span>|
|<span data-ttu-id="0ea1a-213">fileVaultInstitutionalRecoveryKeyCertificateFileName</span><span class="sxs-lookup"><span data-stu-id="0ea1a-213">fileVaultInstitutionalRecoveryKeyCertificateFileName</span></span>|<span data-ttu-id="0ea1a-214">Строка</span><span class="sxs-lookup"><span data-stu-id="0ea1a-214">String</span></span>|<span data-ttu-id="0ea1a-215">Имя файла сертификата ключа восстановления, отображаемого в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-215">File name of the institutional recovery key certificate to display in UI.</span></span> <span data-ttu-id="0ea1a-216">(\*.der).</span><span class="sxs-lookup"><span data-stu-id="0ea1a-216">(\*.der).</span></span>|
|<span data-ttu-id="0ea1a-217">fileVaultPersonalRecoveryKeyHelpMessage</span><span class="sxs-lookup"><span data-stu-id="0ea1a-217">fileVaultPersonalRecoveryKeyHelpMessage</span></span>|<span data-ttu-id="0ea1a-218">Строка</span><span class="sxs-lookup"><span data-stu-id="0ea1a-218">String</span></span>|<span data-ttu-id="0ea1a-219">Необходимый, если выбранный тип ключа восстановления (s) включает PersonalRecoveryKey.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-219">Required if selected recovery key type(s) include PersonalRecoveryKey.</span></span> <span data-ttu-id="0ea1a-220">Короткое сообщение, отображаемая пользователю, которое объясняет, как он может получить свой личный ключ восстановления.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-220">A short message displayed to the user that explains how they can retrieve their personal recovery key.</span></span>|
|<span data-ttu-id="0ea1a-221">fileVaultAllowDeferralUntilSignOut</span><span class="sxs-lookup"><span data-stu-id="0ea1a-221">fileVaultAllowDeferralUntilSignOut</span></span>|<span data-ttu-id="0ea1a-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ea1a-222">Boolean</span></span>|<span data-ttu-id="0ea1a-223">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-223">Optional.</span></span> <span data-ttu-id="0ea1a-224">Если установлена истина, пользователь может отложить включение FileVault до тех пор, пока они не выпишутся.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-224">If set to true, the user can defer the enabling of FileVault until they sign out.</span></span>|
|<span data-ttu-id="0ea1a-225">fileVaultNumberOfTimesUserCanIgnore</span><span class="sxs-lookup"><span data-stu-id="0ea1a-225">fileVaultNumberOfTimesUserCanIgnore</span></span>|<span data-ttu-id="0ea1a-226">Int32</span><span class="sxs-lookup"><span data-stu-id="0ea1a-226">Int32</span></span>|<span data-ttu-id="0ea1a-227">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-227">Optional.</span></span> <span data-ttu-id="0ea1a-228">При использовании параметра Defer это максимальное количество раз, когда пользователь может игнорировать подсказки, чтобы включить FileVault, прежде чем fileVault потребуется для пользователя, чтобы войти.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-228">When using the Defer option, this is the maximum number of times the user can ignore prompts to enable FileVault before FileVault will be required for the user to sign in.</span></span> <span data-ttu-id="0ea1a-229">Если установлено до -1, всегда будет предложено включить FileVault до включения FileVault, хотя это позволит пользователю обойти включение FileVault.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-229">If set to -1, it will always prompt to enable FileVault until FileVault is enabled, though it will allow the user to bypass enabling FileVault.</span></span> <span data-ttu-id="0ea1a-230">Настройка этого параметра до 0 отключит функцию.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-230">Setting this to 0 will disable the feature.</span></span>|
|<span data-ttu-id="0ea1a-231">fileVaultDisablePromptAtSignOut</span><span class="sxs-lookup"><span data-stu-id="0ea1a-231">fileVaultDisablePromptAtSignOut</span></span>|<span data-ttu-id="0ea1a-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ea1a-232">Boolean</span></span>|<span data-ttu-id="0ea1a-233">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-233">Optional.</span></span> <span data-ttu-id="0ea1a-234">При использовании параметра Defer, если задается true, пользователю не предложено включить FileVault при входе.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-234">When using the Defer option, if set to true, the user is not prompted to enable FileVault at sign-out.</span></span>|
|<span data-ttu-id="0ea1a-235">fileVaultPersonalRecoveryKeyRotationInMonths</span><span class="sxs-lookup"><span data-stu-id="0ea1a-235">fileVaultPersonalRecoveryKeyRotationInMonths</span></span>|<span data-ttu-id="0ea1a-236">Int32</span><span class="sxs-lookup"><span data-stu-id="0ea1a-236">Int32</span></span>|<span data-ttu-id="0ea1a-237">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-237">Optional.</span></span> <span data-ttu-id="0ea1a-238">Если выбранный тип ключа восстановления (s) включает PersonalRecoveryKey, частота вращения этого ключа в месяцах.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-238">If selected recovery key type(s) include PersonalRecoveryKey, the frequency to rotate that key, in months.</span></span>|
|<span data-ttu-id="0ea1a-239">fileVaultHidePersonalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="0ea1a-239">fileVaultHidePersonalRecoveryKey</span></span>|<span data-ttu-id="0ea1a-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ea1a-240">Boolean</span></span>|<span data-ttu-id="0ea1a-241">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-241">Optional.</span></span> <span data-ttu-id="0ea1a-242">Скрытый личный ключ восстановления не появляется на экране пользователя во время шифрования FileVault, что снижает риск его оказаться в неправильных руках.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-242">A hidden personal recovery key does not appear on the user's screen during FileVault encryption, reducing the risk of it ending up in the wrong hands.</span></span>|
|<span data-ttu-id="0ea1a-243">advancedThreatProtectionRealTime</span><span class="sxs-lookup"><span data-stu-id="0ea1a-243">advancedThreatProtectionRealTime</span></span>|[<span data-ttu-id="0ea1a-244">включить</span><span class="sxs-lookup"><span data-stu-id="0ea1a-244">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="0ea1a-245">Определяет, следует ли включить защиту в режиме реального времени для microsoft Defender Advanced Threat Protection на macOS.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-245">Determines whether or not to enable real-time protection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="0ea1a-246">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-246">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="0ea1a-247">advancedThreatProtectionCloudDelivered</span><span class="sxs-lookup"><span data-stu-id="0ea1a-247">advancedThreatProtectionCloudDelivered</span></span>|[<span data-ttu-id="0ea1a-248">включить</span><span class="sxs-lookup"><span data-stu-id="0ea1a-248">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="0ea1a-249">Определяет, следует ли включить облачную защиту для microsoft Defender Advanced Threat Protection на macOS.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-249">Determines whether or not to enable cloud-delivered protection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="0ea1a-250">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-250">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="0ea1a-251">advancedThreatProtectionAutomaticSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="0ea1a-251">advancedThreatProtectionAutomaticSampleSubmission</span></span>|[<span data-ttu-id="0ea1a-252">включить</span><span class="sxs-lookup"><span data-stu-id="0ea1a-252">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="0ea1a-253">Определяет, следует ли включить автоматическую отправку образца файла для microsoft Defender Advanced Threat Protection на macOS.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-253">Determines whether or not to enable automatic file sample submission for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="0ea1a-254">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-254">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="0ea1a-255">advancedThreatProtectionDiagnosticDataCollection</span><span class="sxs-lookup"><span data-stu-id="0ea1a-255">advancedThreatProtectionDiagnosticDataCollection</span></span>|[<span data-ttu-id="0ea1a-256">включить</span><span class="sxs-lookup"><span data-stu-id="0ea1a-256">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="0ea1a-257">Определяет, следует ли включить сбор данных диагностики и использования для microsoft Defender Advanced Threat Protection на macOS.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-257">Determines whether or not to enable diagnostic and usage data collection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="0ea1a-258">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-258">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="0ea1a-259">advancedThreatProtectionExcludedFolders</span><span class="sxs-lookup"><span data-stu-id="0ea1a-259">advancedThreatProtectionExcludedFolders</span></span>|<span data-ttu-id="0ea1a-260">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0ea1a-260">String collection</span></span>|<span data-ttu-id="0ea1a-261">Список путей к папкам, исключающих антивирусное сканирование для microsoft Defender Advanced Threat Protection на macOS.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-261">A list of paths to folders to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="0ea1a-262">advancedThreatProtectionExcludedFiles</span><span class="sxs-lookup"><span data-stu-id="0ea1a-262">advancedThreatProtectionExcludedFiles</span></span>|<span data-ttu-id="0ea1a-263">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0ea1a-263">String collection</span></span>|<span data-ttu-id="0ea1a-264">Список путей к файлам, которые необходимо исключить из антивирусного сканирования для microsoft Defender Advanced Threat Protection на macOS.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-264">A list of paths to files to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="0ea1a-265">advancedThreatProtectionExcludedExtensions</span><span class="sxs-lookup"><span data-stu-id="0ea1a-265">advancedThreatProtectionExcludedExtensions</span></span>|<span data-ttu-id="0ea1a-266">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0ea1a-266">String collection</span></span>|<span data-ttu-id="0ea1a-267">Список расширений файлов, которые необходимо исключить из антивирусного сканирования для Microsoft Defender Advanced Threat Protection на macOS.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-267">A list of file extensions to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="0ea1a-268">advancedThreatProtectionExcludedProcesses</span><span class="sxs-lookup"><span data-stu-id="0ea1a-268">advancedThreatProtectionExcludedProcesses</span></span>|<span data-ttu-id="0ea1a-269">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0ea1a-269">String collection</span></span>|<span data-ttu-id="0ea1a-270">Список имен процессов, которые необходимо исключить из антивирусного сканирования для microsoft Defender Advanced Threat Protection на macOS.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-270">A list of process names to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|



## <a name="response"></a><span data-ttu-id="0ea1a-271">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ea1a-271">Response</span></span>
<span data-ttu-id="0ea1a-272">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-272">If successful, this method returns a `200 OK` response code and an updated [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ea1a-273">Пример</span><span class="sxs-lookup"><span data-stu-id="0ea1a-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ea1a-274">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ea1a-274">Request</span></span>
<span data-ttu-id="0ea1a-275">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-275">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2786

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
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
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ],
  "fileVaultEnabled": true,
  "fileVaultSelectedRecoveryKeyTypes": "institutionalRecoveryKey",
  "fileVaultInstitutionalRecoveryKeyCertificate": "ZmlsZVZhdWx0SW5zdGl0dXRpb25hbFJlY292ZXJ5S2V5Q2VydGlmaWNhdGU=",
  "fileVaultInstitutionalRecoveryKeyCertificateFileName": "File Vault Institutional Recovery Key Certificate File Name value",
  "fileVaultPersonalRecoveryKeyHelpMessage": "File Vault Personal Recovery Key Help Message value",
  "fileVaultAllowDeferralUntilSignOut": true,
  "fileVaultNumberOfTimesUserCanIgnore": 3,
  "fileVaultDisablePromptAtSignOut": true,
  "fileVaultPersonalRecoveryKeyRotationInMonths": 12,
  "fileVaultHidePersonalRecoveryKey": true,
  "advancedThreatProtectionRealTime": "enabled",
  "advancedThreatProtectionCloudDelivered": "enabled",
  "advancedThreatProtectionAutomaticSampleSubmission": "enabled",
  "advancedThreatProtectionDiagnosticDataCollection": "enabled",
  "advancedThreatProtectionExcludedFolders": [
    "Advanced Threat Protection Excluded Folders value"
  ],
  "advancedThreatProtectionExcludedFiles": [
    "Advanced Threat Protection Excluded Files value"
  ],
  "advancedThreatProtectionExcludedExtensions": [
    "Advanced Threat Protection Excluded Extensions value"
  ],
  "advancedThreatProtectionExcludedProcesses": [
    "Advanced Threat Protection Excluded Processes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="0ea1a-276">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ea1a-276">Response</span></span>
<span data-ttu-id="0ea1a-p128">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ea1a-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2958

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "id": "7bf7f3ca-f3ca-7bf7-caf3-f77bcaf3f77b",
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
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ],
  "fileVaultEnabled": true,
  "fileVaultSelectedRecoveryKeyTypes": "institutionalRecoveryKey",
  "fileVaultInstitutionalRecoveryKeyCertificate": "ZmlsZVZhdWx0SW5zdGl0dXRpb25hbFJlY292ZXJ5S2V5Q2VydGlmaWNhdGU=",
  "fileVaultInstitutionalRecoveryKeyCertificateFileName": "File Vault Institutional Recovery Key Certificate File Name value",
  "fileVaultPersonalRecoveryKeyHelpMessage": "File Vault Personal Recovery Key Help Message value",
  "fileVaultAllowDeferralUntilSignOut": true,
  "fileVaultNumberOfTimesUserCanIgnore": 3,
  "fileVaultDisablePromptAtSignOut": true,
  "fileVaultPersonalRecoveryKeyRotationInMonths": 12,
  "fileVaultHidePersonalRecoveryKey": true,
  "advancedThreatProtectionRealTime": "enabled",
  "advancedThreatProtectionCloudDelivered": "enabled",
  "advancedThreatProtectionAutomaticSampleSubmission": "enabled",
  "advancedThreatProtectionDiagnosticDataCollection": "enabled",
  "advancedThreatProtectionExcludedFolders": [
    "Advanced Threat Protection Excluded Folders value"
  ],
  "advancedThreatProtectionExcludedFiles": [
    "Advanced Threat Protection Excluded Files value"
  ],
  "advancedThreatProtectionExcludedExtensions": [
    "Advanced Threat Protection Excluded Extensions value"
  ],
  "advancedThreatProtectionExcludedProcesses": [
    "Advanced Threat Protection Excluded Processes value"
  ]
}
```




