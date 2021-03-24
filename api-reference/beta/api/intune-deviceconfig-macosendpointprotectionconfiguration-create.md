---
title: Создание macOSEndpointProtectionConfiguration
description: Создание нового объекта macOSEndpointProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cebda22f1fbff27c6f2c3baea333e9caaf5f1fb8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131346"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="4ef37-103">Создание macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ef37-103">Create macOSEndpointProtectionConfiguration</span></span>

<span data-ttu-id="4ef37-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ef37-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ef37-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ef37-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ef37-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ef37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ef37-107">Создание нового [объекта macOSEndpointProtectionConfiguration.](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ef37-107">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ef37-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4ef37-108">Prerequisites</span></span>
<span data-ttu-id="4ef37-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ef37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ef37-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ef37-111">Permission type</span></span>|<span data-ttu-id="4ef37-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ef37-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ef37-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ef37-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ef37-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ef37-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ef37-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ef37-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ef37-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ef37-116">Not supported.</span></span>|
|<span data-ttu-id="4ef37-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4ef37-117">Application</span></span>|<span data-ttu-id="4ef37-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ef37-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ef37-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ef37-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4ef37-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4ef37-120">Request headers</span></span>
|<span data-ttu-id="4ef37-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ef37-121">Header</span></span>|<span data-ttu-id="4ef37-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4ef37-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ef37-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ef37-123">Authorization</span></span>|<span data-ttu-id="4ef37-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ef37-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ef37-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4ef37-125">Accept</span></span>|<span data-ttu-id="4ef37-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ef37-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ef37-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ef37-127">Request body</span></span>
<span data-ttu-id="4ef37-128">В теле запроса устройте представление JSON для объекта macOSEndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4ef37-128">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="4ef37-129">В следующей таблице показаны свойства, необходимые при создании macOSEndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4ef37-129">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="4ef37-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ef37-130">Property</span></span>|<span data-ttu-id="4ef37-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4ef37-131">Type</span></span>|<span data-ttu-id="4ef37-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4ef37-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ef37-133">id</span><span class="sxs-lookup"><span data-stu-id="4ef37-133">id</span></span>|<span data-ttu-id="4ef37-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4ef37-134">String</span></span>|<span data-ttu-id="4ef37-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4ef37-135">Key of the entity.</span></span> <span data-ttu-id="4ef37-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ef37-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ef37-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ef37-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4ef37-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ef37-138">DateTimeOffset</span></span>|<span data-ttu-id="4ef37-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4ef37-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4ef37-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ef37-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ef37-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4ef37-141">roleScopeTagIds</span></span>|<span data-ttu-id="4ef37-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4ef37-142">String collection</span></span>|<span data-ttu-id="4ef37-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="4ef37-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4ef37-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ef37-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ef37-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4ef37-145">supportsScopeTags</span></span>|<span data-ttu-id="4ef37-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ef37-146">Boolean</span></span>|<span data-ttu-id="4ef37-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4ef37-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4ef37-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="4ef37-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4ef37-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4ef37-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4ef37-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ef37-150">This property is read-only.</span></span> <span data-ttu-id="4ef37-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ef37-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ef37-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4ef37-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4ef37-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4ef37-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4ef37-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4ef37-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4ef37-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ef37-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ef37-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4ef37-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4ef37-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4ef37-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4ef37-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4ef37-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4ef37-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ef37-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ef37-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4ef37-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4ef37-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4ef37-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4ef37-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4ef37-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4ef37-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ef37-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ef37-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ef37-164">createdDateTime</span></span>|<span data-ttu-id="4ef37-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ef37-165">DateTimeOffset</span></span>|<span data-ttu-id="4ef37-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4ef37-166">DateTime the object was created.</span></span> <span data-ttu-id="4ef37-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ef37-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ef37-168">description</span><span class="sxs-lookup"><span data-stu-id="4ef37-168">description</span></span>|<span data-ttu-id="4ef37-169">Строка</span><span class="sxs-lookup"><span data-stu-id="4ef37-169">String</span></span>|<span data-ttu-id="4ef37-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4ef37-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4ef37-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ef37-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ef37-172">displayName</span><span class="sxs-lookup"><span data-stu-id="4ef37-172">displayName</span></span>|<span data-ttu-id="4ef37-173">Строка</span><span class="sxs-lookup"><span data-stu-id="4ef37-173">String</span></span>|<span data-ttu-id="4ef37-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4ef37-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4ef37-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ef37-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ef37-176">version</span><span class="sxs-lookup"><span data-stu-id="4ef37-176">version</span></span>|<span data-ttu-id="4ef37-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4ef37-177">Int32</span></span>|<span data-ttu-id="4ef37-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4ef37-178">Version of the device configuration.</span></span> <span data-ttu-id="4ef37-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ef37-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ef37-180">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="4ef37-180">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="4ef37-181">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="4ef37-181">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="4ef37-182">Параметр System и Privacy, который определяет, какие приложения для скачивания можно запускать на macOS-устройстве.</span><span class="sxs-lookup"><span data-stu-id="4ef37-182">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="4ef37-183">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="4ef37-183">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="4ef37-184">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="4ef37-184">gatekeeperBlockOverride</span></span>|<span data-ttu-id="4ef37-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ef37-185">Boolean</span></span>|<span data-ttu-id="4ef37-186">Если задана истина, переопределения пользователя для Gatekeeper будут отключены.</span><span class="sxs-lookup"><span data-stu-id="4ef37-186">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="4ef37-187">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="4ef37-187">firewallEnabled</span></span>|<span data-ttu-id="4ef37-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ef37-188">Boolean</span></span>|<span data-ttu-id="4ef37-189">Следует ли включить брандмауэр или нет.</span><span class="sxs-lookup"><span data-stu-id="4ef37-189">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="4ef37-190">брандмауэрBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="4ef37-190">firewallBlockAllIncoming</span></span>|<span data-ttu-id="4ef37-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ef37-191">Boolean</span></span>|<span data-ttu-id="4ef37-192">Соответствует параметру "Блокировка всех входящих подключений".</span><span class="sxs-lookup"><span data-stu-id="4ef37-192">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="4ef37-193">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="4ef37-193">firewallEnableStealthMode</span></span>|<span data-ttu-id="4ef37-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ef37-194">Boolean</span></span>|<span data-ttu-id="4ef37-195">Соответствует режиму "Включить режим стелс".</span><span class="sxs-lookup"><span data-stu-id="4ef37-195">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="4ef37-196">брандмауэрАпплиляции</span><span class="sxs-lookup"><span data-stu-id="4ef37-196">firewallApplications</span></span>|<span data-ttu-id="4ef37-197">[коллекция macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)</span><span class="sxs-lookup"><span data-stu-id="4ef37-197">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="4ef37-198">Список приложений с настройками брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="4ef37-198">List of applications with firewall settings.</span></span> <span data-ttu-id="4ef37-199">Параметры брандмауэра для приложений, не входящего в этот список, определяются пользователем.</span><span class="sxs-lookup"><span data-stu-id="4ef37-199">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="4ef37-200">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4ef37-200">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4ef37-201">fileVaultEnabled</span><span class="sxs-lookup"><span data-stu-id="4ef37-201">fileVaultEnabled</span></span>|<span data-ttu-id="4ef37-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ef37-202">Boolean</span></span>|<span data-ttu-id="4ef37-203">Следует ли включить FileVault или нет.</span><span class="sxs-lookup"><span data-stu-id="4ef37-203">Whether FileVault should be enabled or not.</span></span>|
|<span data-ttu-id="4ef37-204">fileVaultSelectedRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="4ef37-204">fileVaultSelectedRecoveryKeyTypes</span></span>|[<span data-ttu-id="4ef37-205">macOSFileVaultRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="4ef37-205">macOSFileVaultRecoveryKeyTypes</span></span>](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|<span data-ttu-id="4ef37-206">Требуется, если включен FileVault, определяет тип(ы) ключа восстановления для использования.</span><span class="sxs-lookup"><span data-stu-id="4ef37-206">Required if FileVault is enabled, determines the type(s) of recovery key to use.</span></span> <span data-ttu-id="4ef37-207">.</span><span class="sxs-lookup"><span data-stu-id="4ef37-207">.</span></span> <span data-ttu-id="4ef37-208">Возможные значения: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span><span class="sxs-lookup"><span data-stu-id="4ef37-208">Possible values are: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span></span>|
|<span data-ttu-id="4ef37-209">fileVaultInstitutionalRecoveryKeyCertificate</span><span class="sxs-lookup"><span data-stu-id="4ef37-209">fileVaultInstitutionalRecoveryKeyCertificate</span></span>|<span data-ttu-id="4ef37-210">Binary</span><span class="sxs-lookup"><span data-stu-id="4ef37-210">Binary</span></span>|<span data-ttu-id="4ef37-211">Необходимый, если выбранный тип ключа восстановления (s) включает InstitutionalRecoveryKey.</span><span class="sxs-lookup"><span data-stu-id="4ef37-211">Required if selected recovery key type(s) include InstitutionalRecoveryKey.</span></span> <span data-ttu-id="4ef37-212">Кодированный файл сертификата DER, используемый для задавания институционального ключа восстановления.</span><span class="sxs-lookup"><span data-stu-id="4ef37-212">The DER Encoded certificate file used to set an institutional recovery key.</span></span>|
|<span data-ttu-id="4ef37-213">fileVaultInstitutionalRecoveryKeyCertificateFileName</span><span class="sxs-lookup"><span data-stu-id="4ef37-213">fileVaultInstitutionalRecoveryKeyCertificateFileName</span></span>|<span data-ttu-id="4ef37-214">Строка</span><span class="sxs-lookup"><span data-stu-id="4ef37-214">String</span></span>|<span data-ttu-id="4ef37-215">Имя файла сертификата ключа восстановления, отображаемого в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="4ef37-215">File name of the institutional recovery key certificate to display in UI.</span></span> <span data-ttu-id="4ef37-216">(\*.der).</span><span class="sxs-lookup"><span data-stu-id="4ef37-216">(\*.der).</span></span>|
|<span data-ttu-id="4ef37-217">fileVaultPersonalRecoveryKeyHelpMessage</span><span class="sxs-lookup"><span data-stu-id="4ef37-217">fileVaultPersonalRecoveryKeyHelpMessage</span></span>|<span data-ttu-id="4ef37-218">Строка</span><span class="sxs-lookup"><span data-stu-id="4ef37-218">String</span></span>|<span data-ttu-id="4ef37-219">Необходимый, если выбранный тип ключа восстановления (s) включает PersonalRecoveryKey.</span><span class="sxs-lookup"><span data-stu-id="4ef37-219">Required if selected recovery key type(s) include PersonalRecoveryKey.</span></span> <span data-ttu-id="4ef37-220">Короткое сообщение, отображаемая пользователю, которое объясняет, как он может получить свой личный ключ восстановления.</span><span class="sxs-lookup"><span data-stu-id="4ef37-220">A short message displayed to the user that explains how they can retrieve their personal recovery key.</span></span>|
|<span data-ttu-id="4ef37-221">fileVaultAllowDeferralUntilSignOut</span><span class="sxs-lookup"><span data-stu-id="4ef37-221">fileVaultAllowDeferralUntilSignOut</span></span>|<span data-ttu-id="4ef37-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ef37-222">Boolean</span></span>|<span data-ttu-id="4ef37-223">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="4ef37-223">Optional.</span></span> <span data-ttu-id="4ef37-224">Если установлена истина, пользователь может отложить включение FileVault до тех пор, пока они не выпишутся.</span><span class="sxs-lookup"><span data-stu-id="4ef37-224">If set to true, the user can defer the enabling of FileVault until they sign out.</span></span>|
|<span data-ttu-id="4ef37-225">fileVaultNumberOfTimesUserCanIgnore</span><span class="sxs-lookup"><span data-stu-id="4ef37-225">fileVaultNumberOfTimesUserCanIgnore</span></span>|<span data-ttu-id="4ef37-226">Int32</span><span class="sxs-lookup"><span data-stu-id="4ef37-226">Int32</span></span>|<span data-ttu-id="4ef37-227">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="4ef37-227">Optional.</span></span> <span data-ttu-id="4ef37-228">При использовании параметра Defer это максимальное количество раз, когда пользователь может игнорировать подсказки, чтобы включить FileVault, прежде чем fileVault потребуется для пользователя, чтобы войти.</span><span class="sxs-lookup"><span data-stu-id="4ef37-228">When using the Defer option, this is the maximum number of times the user can ignore prompts to enable FileVault before FileVault will be required for the user to sign in.</span></span> <span data-ttu-id="4ef37-229">Если установлено до -1, всегда будет предложено включить FileVault до включения FileVault, хотя это позволит пользователю обойти включение FileVault.</span><span class="sxs-lookup"><span data-stu-id="4ef37-229">If set to -1, it will always prompt to enable FileVault until FileVault is enabled, though it will allow the user to bypass enabling FileVault.</span></span> <span data-ttu-id="4ef37-230">Настройка этого параметра до 0 отключит функцию.</span><span class="sxs-lookup"><span data-stu-id="4ef37-230">Setting this to 0 will disable the feature.</span></span>|
|<span data-ttu-id="4ef37-231">fileVaultDisablePromptAtSignOut</span><span class="sxs-lookup"><span data-stu-id="4ef37-231">fileVaultDisablePromptAtSignOut</span></span>|<span data-ttu-id="4ef37-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ef37-232">Boolean</span></span>|<span data-ttu-id="4ef37-233">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="4ef37-233">Optional.</span></span> <span data-ttu-id="4ef37-234">При использовании параметра Defer, если задается true, пользователю не предложено включить FileVault при входе.</span><span class="sxs-lookup"><span data-stu-id="4ef37-234">When using the Defer option, if set to true, the user is not prompted to enable FileVault at sign-out.</span></span>|
|<span data-ttu-id="4ef37-235">fileVaultPersonalRecoveryKeyRotationInMonths</span><span class="sxs-lookup"><span data-stu-id="4ef37-235">fileVaultPersonalRecoveryKeyRotationInMonths</span></span>|<span data-ttu-id="4ef37-236">Int32</span><span class="sxs-lookup"><span data-stu-id="4ef37-236">Int32</span></span>|<span data-ttu-id="4ef37-237">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="4ef37-237">Optional.</span></span> <span data-ttu-id="4ef37-238">Если выбранный тип ключа восстановления (s) включает PersonalRecoveryKey, частота вращения этого ключа в месяцах.</span><span class="sxs-lookup"><span data-stu-id="4ef37-238">If selected recovery key type(s) include PersonalRecoveryKey, the frequency to rotate that key, in months.</span></span>|
|<span data-ttu-id="4ef37-239">fileVaultHidePersonalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="4ef37-239">fileVaultHidePersonalRecoveryKey</span></span>|<span data-ttu-id="4ef37-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ef37-240">Boolean</span></span>|<span data-ttu-id="4ef37-241">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="4ef37-241">Optional.</span></span> <span data-ttu-id="4ef37-242">Скрытый личный ключ восстановления не появляется на экране пользователя во время шифрования FileVault, что снижает риск его оказаться в неправильных руках.</span><span class="sxs-lookup"><span data-stu-id="4ef37-242">A hidden personal recovery key does not appear on the user's screen during FileVault encryption, reducing the risk of it ending up in the wrong hands.</span></span>|
|<span data-ttu-id="4ef37-243">advancedThreatProtectionRealTime</span><span class="sxs-lookup"><span data-stu-id="4ef37-243">advancedThreatProtectionRealTime</span></span>|[<span data-ttu-id="4ef37-244">включить</span><span class="sxs-lookup"><span data-stu-id="4ef37-244">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4ef37-245">Определяет, следует ли включить защиту в режиме реального времени для microsoft Defender Advanced Threat Protection на macOS.</span><span class="sxs-lookup"><span data-stu-id="4ef37-245">Determines whether or not to enable real-time protection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="4ef37-246">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4ef37-246">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4ef37-247">advancedThreatProtectionCloudDelivered</span><span class="sxs-lookup"><span data-stu-id="4ef37-247">advancedThreatProtectionCloudDelivered</span></span>|[<span data-ttu-id="4ef37-248">включить</span><span class="sxs-lookup"><span data-stu-id="4ef37-248">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4ef37-249">Определяет, следует ли включить облачную защиту для microsoft Defender Advanced Threat Protection на macOS.</span><span class="sxs-lookup"><span data-stu-id="4ef37-249">Determines whether or not to enable cloud-delivered protection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="4ef37-250">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4ef37-250">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4ef37-251">advancedThreatProtectionAutomaticSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="4ef37-251">advancedThreatProtectionAutomaticSampleSubmission</span></span>|[<span data-ttu-id="4ef37-252">включить</span><span class="sxs-lookup"><span data-stu-id="4ef37-252">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4ef37-253">Определяет, следует ли включить автоматическую отправку образца файла для microsoft Defender Advanced Threat Protection на macOS.</span><span class="sxs-lookup"><span data-stu-id="4ef37-253">Determines whether or not to enable automatic file sample submission for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="4ef37-254">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4ef37-254">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4ef37-255">advancedThreatProtectionDiagnosticDataCollection</span><span class="sxs-lookup"><span data-stu-id="4ef37-255">advancedThreatProtectionDiagnosticDataCollection</span></span>|[<span data-ttu-id="4ef37-256">включить</span><span class="sxs-lookup"><span data-stu-id="4ef37-256">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4ef37-257">Определяет, следует ли включить сбор данных диагностики и использования для microsoft Defender Advanced Threat Protection на macOS.</span><span class="sxs-lookup"><span data-stu-id="4ef37-257">Determines whether or not to enable diagnostic and usage data collection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="4ef37-258">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4ef37-258">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4ef37-259">advancedThreatProtectionExcludedFolders</span><span class="sxs-lookup"><span data-stu-id="4ef37-259">advancedThreatProtectionExcludedFolders</span></span>|<span data-ttu-id="4ef37-260">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4ef37-260">String collection</span></span>|<span data-ttu-id="4ef37-261">Список путей к папкам, исключающих антивирусное сканирование для microsoft Defender Advanced Threat Protection на macOS.</span><span class="sxs-lookup"><span data-stu-id="4ef37-261">A list of paths to folders to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="4ef37-262">advancedThreatProtectionExcludedFiles</span><span class="sxs-lookup"><span data-stu-id="4ef37-262">advancedThreatProtectionExcludedFiles</span></span>|<span data-ttu-id="4ef37-263">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4ef37-263">String collection</span></span>|<span data-ttu-id="4ef37-264">Список путей к файлам, которые необходимо исключить из антивирусного сканирования для microsoft Defender Advanced Threat Protection на macOS.</span><span class="sxs-lookup"><span data-stu-id="4ef37-264">A list of paths to files to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="4ef37-265">advancedThreatProtectionExcludedExtensions</span><span class="sxs-lookup"><span data-stu-id="4ef37-265">advancedThreatProtectionExcludedExtensions</span></span>|<span data-ttu-id="4ef37-266">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4ef37-266">String collection</span></span>|<span data-ttu-id="4ef37-267">Список расширений файлов, которые необходимо исключить из антивирусного сканирования для Microsoft Defender Advanced Threat Protection на macOS.</span><span class="sxs-lookup"><span data-stu-id="4ef37-267">A list of file extensions to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="4ef37-268">advancedThreatProtectionExcludedProcesses</span><span class="sxs-lookup"><span data-stu-id="4ef37-268">advancedThreatProtectionExcludedProcesses</span></span>|<span data-ttu-id="4ef37-269">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4ef37-269">String collection</span></span>|<span data-ttu-id="4ef37-270">Список имен процессов, которые необходимо исключить из антивирусного сканирования для microsoft Defender Advanced Threat Protection на macOS.</span><span class="sxs-lookup"><span data-stu-id="4ef37-270">A list of process names to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|



## <a name="response"></a><span data-ttu-id="4ef37-271">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ef37-271">Response</span></span>
<span data-ttu-id="4ef37-272">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4ef37-272">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ef37-273">Пример</span><span class="sxs-lookup"><span data-stu-id="4ef37-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ef37-274">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ef37-274">Request</span></span>
<span data-ttu-id="4ef37-275">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ef37-275">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="4ef37-276">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ef37-276">Response</span></span>
<span data-ttu-id="4ef37-p128">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ef37-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




