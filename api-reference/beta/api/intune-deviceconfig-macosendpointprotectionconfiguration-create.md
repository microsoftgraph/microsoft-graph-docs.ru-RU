---
title: Создание Макосендпоинтпротектионконфигуратион
description: Создание нового объекта Макосендпоинтпротектионконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 47c63dfac9f9cc5d79c05634d9e837892e193541
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948389"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="5c739-103">Создание Макосендпоинтпротектионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="5c739-103">Create macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="5c739-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c739-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c739-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c739-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c739-106">Создание нового объекта [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5c739-106">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c739-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5c739-107">Prerequisites</span></span>
<span data-ttu-id="5c739-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c739-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c739-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c739-110">Permission type</span></span>|<span data-ttu-id="5c739-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c739-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c739-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c739-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c739-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c739-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5c739-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c739-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c739-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c739-115">Not supported.</span></span>|
|<span data-ttu-id="5c739-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c739-116">Application</span></span>|<span data-ttu-id="5c739-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c739-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c739-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c739-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5c739-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5c739-119">Request headers</span></span>
|<span data-ttu-id="5c739-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c739-120">Header</span></span>|<span data-ttu-id="5c739-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5c739-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c739-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c739-122">Authorization</span></span>|<span data-ttu-id="5c739-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c739-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c739-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5c739-124">Accept</span></span>|<span data-ttu-id="5c739-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5c739-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c739-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c739-126">Request body</span></span>
<span data-ttu-id="5c739-127">В тексте запроса добавьте представление объекта Макосендпоинтпротектионконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c739-127">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="5c739-128">В следующей таблице приведены свойства, необходимые при создании Макосендпоинтпротектионконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="5c739-128">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="5c739-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c739-129">Property</span></span>|<span data-ttu-id="5c739-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5c739-130">Type</span></span>|<span data-ttu-id="5c739-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5c739-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c739-132">id</span><span class="sxs-lookup"><span data-stu-id="5c739-132">id</span></span>|<span data-ttu-id="5c739-133">String</span><span class="sxs-lookup"><span data-stu-id="5c739-133">String</span></span>|<span data-ttu-id="5c739-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5c739-134">Key of the entity.</span></span> <span data-ttu-id="5c739-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c739-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c739-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c739-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5c739-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c739-137">DateTimeOffset</span></span>|<span data-ttu-id="5c739-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5c739-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5c739-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c739-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c739-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5c739-140">roleScopeTagIds</span></span>|<span data-ttu-id="5c739-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5c739-141">String collection</span></span>|<span data-ttu-id="5c739-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5c739-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5c739-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c739-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c739-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="5c739-144">supportsScopeTags</span></span>|<span data-ttu-id="5c739-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c739-145">Boolean</span></span>|<span data-ttu-id="5c739-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="5c739-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5c739-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="5c739-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5c739-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5c739-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5c739-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c739-149">This property is read-only.</span></span> <span data-ttu-id="5c739-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c739-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c739-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5c739-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5c739-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5c739-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5c739-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5c739-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5c739-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c739-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c739-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5c739-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5c739-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5c739-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5c739-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5c739-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5c739-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c739-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c739-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5c739-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5c739-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5c739-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5c739-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5c739-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5c739-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c739-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c739-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c739-163">createdDateTime</span></span>|<span data-ttu-id="5c739-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c739-164">DateTimeOffset</span></span>|<span data-ttu-id="5c739-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5c739-165">DateTime the object was created.</span></span> <span data-ttu-id="5c739-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c739-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c739-167">description</span><span class="sxs-lookup"><span data-stu-id="5c739-167">description</span></span>|<span data-ttu-id="5c739-168">String</span><span class="sxs-lookup"><span data-stu-id="5c739-168">String</span></span>|<span data-ttu-id="5c739-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5c739-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5c739-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c739-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c739-171">displayName</span><span class="sxs-lookup"><span data-stu-id="5c739-171">displayName</span></span>|<span data-ttu-id="5c739-172">Строка</span><span class="sxs-lookup"><span data-stu-id="5c739-172">String</span></span>|<span data-ttu-id="5c739-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5c739-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5c739-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c739-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c739-175">version</span><span class="sxs-lookup"><span data-stu-id="5c739-175">version</span></span>|<span data-ttu-id="5c739-176">Int32</span><span class="sxs-lookup"><span data-stu-id="5c739-176">Int32</span></span>|<span data-ttu-id="5c739-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5c739-177">Version of the device configuration.</span></span> <span data-ttu-id="5c739-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c739-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c739-179">гатекипералловедаппсаурце</span><span class="sxs-lookup"><span data-stu-id="5c739-179">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="5c739-180">макосгатекипераппсаурцес</span><span class="sxs-lookup"><span data-stu-id="5c739-180">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="5c739-181">Параметры системы и конфиденциальности, которые определяют, какие расположения скачивания приложения можно запускать с устройства macOS.</span><span class="sxs-lookup"><span data-stu-id="5c739-181">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="5c739-182">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="5c739-182">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="5c739-183">гатекиперблокковерриде</span><span class="sxs-lookup"><span data-stu-id="5c739-183">gatekeeperBlockOverride</span></span>|<span data-ttu-id="5c739-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c739-184">Boolean</span></span>|<span data-ttu-id="5c739-185">Если задано значение true, переопределение пользователя для привратника будет отключено.</span><span class="sxs-lookup"><span data-stu-id="5c739-185">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="5c739-186">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="5c739-186">firewallEnabled</span></span>|<span data-ttu-id="5c739-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c739-187">Boolean</span></span>|<span data-ttu-id="5c739-188">Указывает, следует ли включить брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="5c739-188">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="5c739-189">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="5c739-189">firewallBlockAllIncoming</span></span>|<span data-ttu-id="5c739-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c739-190">Boolean</span></span>|<span data-ttu-id="5c739-191">Соответствует параметру "блокировать все входящие подключения".</span><span class="sxs-lookup"><span data-stu-id="5c739-191">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="5c739-192">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="5c739-192">firewallEnableStealthMode</span></span>|<span data-ttu-id="5c739-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c739-193">Boolean</span></span>|<span data-ttu-id="5c739-194">Соответствует параметру "включить скрытый режим".</span><span class="sxs-lookup"><span data-stu-id="5c739-194">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="5c739-195">фиреваллаппликатионс</span><span class="sxs-lookup"><span data-stu-id="5c739-195">firewallApplications</span></span>|<span data-ttu-id="5c739-196">Коллекция [макосфиреваллаппликатион](../resources/intune-deviceconfig-macosfirewallapplication.md)</span><span class="sxs-lookup"><span data-stu-id="5c739-196">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="5c739-197">Список приложений с параметрами брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="5c739-197">List of applications with firewall settings.</span></span> <span data-ttu-id="5c739-198">Параметры брандмауэра для приложений, не включенных в этот список, определяются пользователем.</span><span class="sxs-lookup"><span data-stu-id="5c739-198">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="5c739-199">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="5c739-199">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5c739-200">филеваултенаблед</span><span class="sxs-lookup"><span data-stu-id="5c739-200">fileVaultEnabled</span></span>|<span data-ttu-id="5c739-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c739-201">Boolean</span></span>|<span data-ttu-id="5c739-202">Указывает, следует ли включить Филеваулт.</span><span class="sxs-lookup"><span data-stu-id="5c739-202">Whether FileVault should be enabled or not.</span></span>|
|<span data-ttu-id="5c739-203">филеваултселектедрековерикэйтипес</span><span class="sxs-lookup"><span data-stu-id="5c739-203">fileVaultSelectedRecoveryKeyTypes</span></span>|[<span data-ttu-id="5c739-204">macOSFileVaultRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="5c739-204">macOSFileVaultRecoveryKeyTypes</span></span>](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|<span data-ttu-id="5c739-205">Обязательно если включен Филеваулт, определяет типы ключа восстановления, которые необходимо использовать.</span><span class="sxs-lookup"><span data-stu-id="5c739-205">Required if FileVault is enabled, determines the type(s) of recovery key to use.</span></span> <span data-ttu-id="5c739-206">.</span><span class="sxs-lookup"><span data-stu-id="5c739-206"></span></span> <span data-ttu-id="5c739-207">Возможные значения: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span><span class="sxs-lookup"><span data-stu-id="5c739-207">Possible values are: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span></span>|
|<span data-ttu-id="5c739-208">филеваултинститутионалрековерикэйцертификате</span><span class="sxs-lookup"><span data-stu-id="5c739-208">fileVaultInstitutionalRecoveryKeyCertificate</span></span>|<span data-ttu-id="5c739-209">Binary</span><span class="sxs-lookup"><span data-stu-id="5c739-209">Binary</span></span>|<span data-ttu-id="5c739-210">Обязательно, если выбранные типы ключей восстановления включают Институтионалрековерикэй.</span><span class="sxs-lookup"><span data-stu-id="5c739-210">Required if selected recovery key type(s) include InstitutionalRecoveryKey.</span></span> <span data-ttu-id="5c739-211">Файл сертификата в кодировке DER, который использовался для установки ключа восстановления в учреждений.</span><span class="sxs-lookup"><span data-stu-id="5c739-211">The DER Encoded certificate file used to set an institutional recovery key.</span></span>|
|<span data-ttu-id="5c739-212">филеваултинститутионалрековерикэйцертификатефиленаме</span><span class="sxs-lookup"><span data-stu-id="5c739-212">fileVaultInstitutionalRecoveryKeyCertificateFileName</span></span>|<span data-ttu-id="5c739-213">Строка</span><span class="sxs-lookup"><span data-stu-id="5c739-213">String</span></span>|<span data-ttu-id="5c739-214">Имя файла сертификата ключа восстановления для сотрудников, который будет отображаться в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="5c739-214">File name of the institutional recovery key certificate to display in UI.</span></span> <span data-ttu-id="5c739-215">(\*. der).</span><span class="sxs-lookup"><span data-stu-id="5c739-215">(\*.der).</span></span>|
|<span data-ttu-id="5c739-216">филеваултперсоналрековерикэйхелпмессаже</span><span class="sxs-lookup"><span data-stu-id="5c739-216">fileVaultPersonalRecoveryKeyHelpMessage</span></span>|<span data-ttu-id="5c739-217">Строка</span><span class="sxs-lookup"><span data-stu-id="5c739-217">String</span></span>|<span data-ttu-id="5c739-218">Обязательно, если выбранные типы ключей восстановления включают Персоналрековерикэй.</span><span class="sxs-lookup"><span data-stu-id="5c739-218">Required if selected recovery key type(s) include PersonalRecoveryKey.</span></span> <span data-ttu-id="5c739-219">Короткое сообщение, в котором показано, как получить свой ключ восстановления личных настроек.</span><span class="sxs-lookup"><span data-stu-id="5c739-219">A short message displayed to the user that explains how they can retrieve their personal recovery key.</span></span>|
|<span data-ttu-id="5c739-220">филеваулталловдеферралунтилсигнаут</span><span class="sxs-lookup"><span data-stu-id="5c739-220">fileVaultAllowDeferralUntilSignOut</span></span>|<span data-ttu-id="5c739-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c739-221">Boolean</span></span>|<span data-ttu-id="5c739-222">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="5c739-222">Optional.</span></span> <span data-ttu-id="5c739-223">Если задано значение true, пользователь может отложить включение Филеваулт, пока не выйдете из системы.</span><span class="sxs-lookup"><span data-stu-id="5c739-223">If set to true, the user can defer the enabling of FileVault until they sign out.</span></span>|
|<span data-ttu-id="5c739-224">филеваултнумберофтимесусерканигноре</span><span class="sxs-lookup"><span data-stu-id="5c739-224">fileVaultNumberOfTimesUserCanIgnore</span></span>|<span data-ttu-id="5c739-225">Int32</span><span class="sxs-lookup"><span data-stu-id="5c739-225">Int32</span></span>|<span data-ttu-id="5c739-226">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="5c739-226">Optional.</span></span> <span data-ttu-id="5c739-227">При использовании параметра "отложить" это максимальное число раз, когда пользователь может игнорировать приглашения на включение Филеваулт, чтобы пользователь мог выполнить вход.</span><span class="sxs-lookup"><span data-stu-id="5c739-227">When using the Defer option, this is the maximum number of times the user can ignore prompts to enable FileVault before FileVault will be required for the user to sign in.</span></span> <span data-ttu-id="5c739-228">Если задано значение-1, всегда будет выдаваться запрос на включение Филеваулт, пока Филеваулт не будет включен, хотя разрешить пользователю обходить включение Филеваулт.</span><span class="sxs-lookup"><span data-stu-id="5c739-228">If set to -1, it will always prompt to enable FileVault until FileVault is enabled, though it will allow the user to bypass enabling FileVault.</span></span> <span data-ttu-id="5c739-229">Если задать для этого параметра значение 0, эта функция будет отключена.</span><span class="sxs-lookup"><span data-stu-id="5c739-229">Setting this to 0 will disable the feature.</span></span>|
|<span data-ttu-id="5c739-230">филеваултдисаблепромптатсигнаут</span><span class="sxs-lookup"><span data-stu-id="5c739-230">fileVaultDisablePromptAtSignOut</span></span>|<span data-ttu-id="5c739-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c739-231">Boolean</span></span>|<span data-ttu-id="5c739-232">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="5c739-232">Optional.</span></span> <span data-ttu-id="5c739-233">При использовании параметра отсрочки, если задано значение true, пользователю не предлагается включить Филеваулт при входе.</span><span class="sxs-lookup"><span data-stu-id="5c739-233">When using the Defer option, if set to true, the user is not prompted to enable FileVault at sign-out.</span></span>|
|<span data-ttu-id="5c739-234">филеваултперсоналрековерикэйротатионинмонсс</span><span class="sxs-lookup"><span data-stu-id="5c739-234">fileVaultPersonalRecoveryKeyRotationInMonths</span></span>|<span data-ttu-id="5c739-235">Int32</span><span class="sxs-lookup"><span data-stu-id="5c739-235">Int32</span></span>|<span data-ttu-id="5c739-236">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="5c739-236">Optional.</span></span> <span data-ttu-id="5c739-237">Если выбранные типы ключей восстановления включают Персоналрековерикэй, частота вращения этого ключа в месяцах.</span><span class="sxs-lookup"><span data-stu-id="5c739-237">If selected recovery key type(s) include PersonalRecoveryKey, the frequency to rotate that key, in months.</span></span>|



## <a name="response"></a><span data-ttu-id="5c739-238">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c739-238">Response</span></span>
<span data-ttu-id="5c739-239">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5c739-239">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c739-240">Пример</span><span class="sxs-lookup"><span data-stu-id="5c739-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c739-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c739-241">Request</span></span>
<span data-ttu-id="5c739-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c739-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2052

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
  "fileVaultPersonalRecoveryKeyRotationInMonths": 12
}
```

### <a name="response"></a><span data-ttu-id="5c739-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c739-243">Response</span></span>
<span data-ttu-id="5c739-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c739-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2224

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
  "fileVaultPersonalRecoveryKeyRotationInMonths": 12
}
```





