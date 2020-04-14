---
title: Обновление Макосендпоинтпротектионконфигуратион
description: Обновление свойств объекта Макосендпоинтпротектионконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 78eaad30f26db7cfcf9172ba6676a87516391b4e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43438034"
---
# <a name="update-macosendpointprotectionconfiguration"></a><span data-ttu-id="330df-103">Обновление Макосендпоинтпротектионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="330df-103">Update macOSEndpointProtectionConfiguration</span></span>

<span data-ttu-id="330df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="330df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="330df-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="330df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="330df-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="330df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="330df-107">Обновление свойств объекта [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="330df-107">Update the properties of a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="330df-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="330df-108">Prerequisites</span></span>
<span data-ttu-id="330df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="330df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="330df-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="330df-111">Permission type</span></span>|<span data-ttu-id="330df-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="330df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="330df-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="330df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="330df-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="330df-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="330df-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="330df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="330df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="330df-116">Not supported.</span></span>|
|<span data-ttu-id="330df-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="330df-117">Application</span></span>|<span data-ttu-id="330df-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="330df-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="330df-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="330df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="330df-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="330df-120">Request headers</span></span>
|<span data-ttu-id="330df-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="330df-121">Header</span></span>|<span data-ttu-id="330df-122">Значение</span><span class="sxs-lookup"><span data-stu-id="330df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="330df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="330df-123">Authorization</span></span>|<span data-ttu-id="330df-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="330df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="330df-125">Accept</span><span class="sxs-lookup"><span data-stu-id="330df-125">Accept</span></span>|<span data-ttu-id="330df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="330df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="330df-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="330df-127">Request body</span></span>
<span data-ttu-id="330df-128">В тексте запроса добавьте представление объекта [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="330df-128">In the request body, supply a JSON representation for the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="330df-129">В следующей таблице приведены свойства, необходимые при создании [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330df-129">The following table shows the properties that are required when you create the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="330df-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="330df-130">Property</span></span>|<span data-ttu-id="330df-131">Тип</span><span class="sxs-lookup"><span data-stu-id="330df-131">Type</span></span>|<span data-ttu-id="330df-132">Описание</span><span class="sxs-lookup"><span data-stu-id="330df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="330df-133">id</span><span class="sxs-lookup"><span data-stu-id="330df-133">id</span></span>|<span data-ttu-id="330df-134">String</span><span class="sxs-lookup"><span data-stu-id="330df-134">String</span></span>|<span data-ttu-id="330df-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="330df-135">Key of the entity.</span></span> <span data-ttu-id="330df-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330df-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330df-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="330df-137">lastModifiedDateTime</span></span>|<span data-ttu-id="330df-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="330df-138">DateTimeOffset</span></span>|<span data-ttu-id="330df-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="330df-139">DateTime the object was last modified.</span></span> <span data-ttu-id="330df-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330df-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330df-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="330df-141">roleScopeTagIds</span></span>|<span data-ttu-id="330df-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="330df-142">String collection</span></span>|<span data-ttu-id="330df-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="330df-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="330df-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330df-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330df-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="330df-145">supportsScopeTags</span></span>|<span data-ttu-id="330df-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="330df-146">Boolean</span></span>|<span data-ttu-id="330df-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="330df-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="330df-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="330df-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="330df-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="330df-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="330df-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="330df-150">This property is read-only.</span></span> <span data-ttu-id="330df-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330df-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330df-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="330df-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="330df-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="330df-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="330df-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="330df-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="330df-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330df-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330df-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="330df-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="330df-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="330df-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="330df-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="330df-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="330df-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330df-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330df-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="330df-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="330df-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="330df-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="330df-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="330df-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="330df-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330df-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330df-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="330df-164">createdDateTime</span></span>|<span data-ttu-id="330df-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="330df-165">DateTimeOffset</span></span>|<span data-ttu-id="330df-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="330df-166">DateTime the object was created.</span></span> <span data-ttu-id="330df-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330df-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330df-168">description</span><span class="sxs-lookup"><span data-stu-id="330df-168">description</span></span>|<span data-ttu-id="330df-169">String</span><span class="sxs-lookup"><span data-stu-id="330df-169">String</span></span>|<span data-ttu-id="330df-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="330df-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="330df-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330df-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330df-172">displayName</span><span class="sxs-lookup"><span data-stu-id="330df-172">displayName</span></span>|<span data-ttu-id="330df-173">Строка</span><span class="sxs-lookup"><span data-stu-id="330df-173">String</span></span>|<span data-ttu-id="330df-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="330df-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="330df-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330df-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330df-176">version</span><span class="sxs-lookup"><span data-stu-id="330df-176">version</span></span>|<span data-ttu-id="330df-177">Int32</span><span class="sxs-lookup"><span data-stu-id="330df-177">Int32</span></span>|<span data-ttu-id="330df-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="330df-178">Version of the device configuration.</span></span> <span data-ttu-id="330df-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330df-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330df-180">гатекипералловедаппсаурце</span><span class="sxs-lookup"><span data-stu-id="330df-180">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="330df-181">макосгатекипераппсаурцес</span><span class="sxs-lookup"><span data-stu-id="330df-181">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="330df-182">Параметры системы и конфиденциальности, которые определяют, какие расположения скачивания приложения можно запускать с устройства macOS.</span><span class="sxs-lookup"><span data-stu-id="330df-182">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="330df-183">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="330df-183">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="330df-184">гатекиперблокковерриде</span><span class="sxs-lookup"><span data-stu-id="330df-184">gatekeeperBlockOverride</span></span>|<span data-ttu-id="330df-185">Логическое</span><span class="sxs-lookup"><span data-stu-id="330df-185">Boolean</span></span>|<span data-ttu-id="330df-186">Если задано значение true, переопределение пользователя для привратника будет отключено.</span><span class="sxs-lookup"><span data-stu-id="330df-186">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="330df-187">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="330df-187">firewallEnabled</span></span>|<span data-ttu-id="330df-188">Логическое</span><span class="sxs-lookup"><span data-stu-id="330df-188">Boolean</span></span>|<span data-ttu-id="330df-189">Указывает, следует ли включить брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="330df-189">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="330df-190">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="330df-190">firewallBlockAllIncoming</span></span>|<span data-ttu-id="330df-191">Логическое</span><span class="sxs-lookup"><span data-stu-id="330df-191">Boolean</span></span>|<span data-ttu-id="330df-192">Соответствует параметру "блокировать все входящие подключения".</span><span class="sxs-lookup"><span data-stu-id="330df-192">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="330df-193">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="330df-193">firewallEnableStealthMode</span></span>|<span data-ttu-id="330df-194">Логическое</span><span class="sxs-lookup"><span data-stu-id="330df-194">Boolean</span></span>|<span data-ttu-id="330df-195">Соответствует параметру "включить скрытый режим".</span><span class="sxs-lookup"><span data-stu-id="330df-195">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="330df-196">фиреваллаппликатионс</span><span class="sxs-lookup"><span data-stu-id="330df-196">firewallApplications</span></span>|<span data-ttu-id="330df-197">Коллекция [макосфиреваллаппликатион](../resources/intune-deviceconfig-macosfirewallapplication.md)</span><span class="sxs-lookup"><span data-stu-id="330df-197">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="330df-198">Список приложений с параметрами брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="330df-198">List of applications with firewall settings.</span></span> <span data-ttu-id="330df-199">Параметры брандмауэра для приложений, не включенных в этот список, определяются пользователем.</span><span class="sxs-lookup"><span data-stu-id="330df-199">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="330df-200">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="330df-200">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="330df-201">филеваултенаблед</span><span class="sxs-lookup"><span data-stu-id="330df-201">fileVaultEnabled</span></span>|<span data-ttu-id="330df-202">Логическое</span><span class="sxs-lookup"><span data-stu-id="330df-202">Boolean</span></span>|<span data-ttu-id="330df-203">Указывает, следует ли включить Филеваулт.</span><span class="sxs-lookup"><span data-stu-id="330df-203">Whether FileVault should be enabled or not.</span></span>|
|<span data-ttu-id="330df-204">филеваултселектедрековерикэйтипес</span><span class="sxs-lookup"><span data-stu-id="330df-204">fileVaultSelectedRecoveryKeyTypes</span></span>|[<span data-ttu-id="330df-205">macOSFileVaultRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="330df-205">macOSFileVaultRecoveryKeyTypes</span></span>](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|<span data-ttu-id="330df-206">Обязательно если включен Филеваулт, определяет типы ключа восстановления, которые необходимо использовать.</span><span class="sxs-lookup"><span data-stu-id="330df-206">Required if FileVault is enabled, determines the type(s) of recovery key to use.</span></span> <span data-ttu-id="330df-207">.</span><span class="sxs-lookup"><span data-stu-id="330df-207">.</span></span> <span data-ttu-id="330df-208">Возможные значения: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span><span class="sxs-lookup"><span data-stu-id="330df-208">Possible values are: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span></span>|
|<span data-ttu-id="330df-209">филеваултинститутионалрековерикэйцертификате</span><span class="sxs-lookup"><span data-stu-id="330df-209">fileVaultInstitutionalRecoveryKeyCertificate</span></span>|<span data-ttu-id="330df-210">Binary</span><span class="sxs-lookup"><span data-stu-id="330df-210">Binary</span></span>|<span data-ttu-id="330df-211">Обязательно, если выбранные типы ключей восстановления включают Институтионалрековерикэй.</span><span class="sxs-lookup"><span data-stu-id="330df-211">Required if selected recovery key type(s) include InstitutionalRecoveryKey.</span></span> <span data-ttu-id="330df-212">Файл сертификата в кодировке DER, который использовался для установки ключа восстановления в учреждений.</span><span class="sxs-lookup"><span data-stu-id="330df-212">The DER Encoded certificate file used to set an institutional recovery key.</span></span>|
|<span data-ttu-id="330df-213">филеваултинститутионалрековерикэйцертификатефиленаме</span><span class="sxs-lookup"><span data-stu-id="330df-213">fileVaultInstitutionalRecoveryKeyCertificateFileName</span></span>|<span data-ttu-id="330df-214">String</span><span class="sxs-lookup"><span data-stu-id="330df-214">String</span></span>|<span data-ttu-id="330df-215">Имя файла сертификата ключа восстановления для сотрудников, который будет отображаться в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="330df-215">File name of the institutional recovery key certificate to display in UI.</span></span> <span data-ttu-id="330df-216">(\*. der).</span><span class="sxs-lookup"><span data-stu-id="330df-216">(\*.der).</span></span>|
|<span data-ttu-id="330df-217">филеваултперсоналрековерикэйхелпмессаже</span><span class="sxs-lookup"><span data-stu-id="330df-217">fileVaultPersonalRecoveryKeyHelpMessage</span></span>|<span data-ttu-id="330df-218">String</span><span class="sxs-lookup"><span data-stu-id="330df-218">String</span></span>|<span data-ttu-id="330df-219">Обязательно, если выбранные типы ключей восстановления включают Персоналрековерикэй.</span><span class="sxs-lookup"><span data-stu-id="330df-219">Required if selected recovery key type(s) include PersonalRecoveryKey.</span></span> <span data-ttu-id="330df-220">Короткое сообщение, в котором показано, как получить свой ключ восстановления личных настроек.</span><span class="sxs-lookup"><span data-stu-id="330df-220">A short message displayed to the user that explains how they can retrieve their personal recovery key.</span></span>|
|<span data-ttu-id="330df-221">филеваулталловдеферралунтилсигнаут</span><span class="sxs-lookup"><span data-stu-id="330df-221">fileVaultAllowDeferralUntilSignOut</span></span>|<span data-ttu-id="330df-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="330df-222">Boolean</span></span>|<span data-ttu-id="330df-223">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="330df-223">Optional.</span></span> <span data-ttu-id="330df-224">Если задано значение true, пользователь может отложить включение Филеваулт, пока не выйдете из системы.</span><span class="sxs-lookup"><span data-stu-id="330df-224">If set to true, the user can defer the enabling of FileVault until they sign out.</span></span>|
|<span data-ttu-id="330df-225">филеваултнумберофтимесусерканигноре</span><span class="sxs-lookup"><span data-stu-id="330df-225">fileVaultNumberOfTimesUserCanIgnore</span></span>|<span data-ttu-id="330df-226">Int32</span><span class="sxs-lookup"><span data-stu-id="330df-226">Int32</span></span>|<span data-ttu-id="330df-227">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="330df-227">Optional.</span></span> <span data-ttu-id="330df-228">При использовании параметра "отложить" это максимальное число раз, когда пользователь может игнорировать приглашения на включение Филеваулт, чтобы пользователь мог выполнить вход.</span><span class="sxs-lookup"><span data-stu-id="330df-228">When using the Defer option, this is the maximum number of times the user can ignore prompts to enable FileVault before FileVault will be required for the user to sign in.</span></span> <span data-ttu-id="330df-229">Если задано значение-1, всегда будет выдаваться запрос на включение Филеваулт, пока Филеваулт не будет включен, хотя разрешить пользователю обходить включение Филеваулт.</span><span class="sxs-lookup"><span data-stu-id="330df-229">If set to -1, it will always prompt to enable FileVault until FileVault is enabled, though it will allow the user to bypass enabling FileVault.</span></span> <span data-ttu-id="330df-230">Если задать для этого параметра значение 0, эта функция будет отключена.</span><span class="sxs-lookup"><span data-stu-id="330df-230">Setting this to 0 will disable the feature.</span></span>|
|<span data-ttu-id="330df-231">филеваултдисаблепромптатсигнаут</span><span class="sxs-lookup"><span data-stu-id="330df-231">fileVaultDisablePromptAtSignOut</span></span>|<span data-ttu-id="330df-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="330df-232">Boolean</span></span>|<span data-ttu-id="330df-233">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="330df-233">Optional.</span></span> <span data-ttu-id="330df-234">При использовании параметра отсрочки, если задано значение true, пользователю не предлагается включить Филеваулт при входе.</span><span class="sxs-lookup"><span data-stu-id="330df-234">When using the Defer option, if set to true, the user is not prompted to enable FileVault at sign-out.</span></span>|
|<span data-ttu-id="330df-235">филеваултперсоналрековерикэйротатионинмонсс</span><span class="sxs-lookup"><span data-stu-id="330df-235">fileVaultPersonalRecoveryKeyRotationInMonths</span></span>|<span data-ttu-id="330df-236">Int32</span><span class="sxs-lookup"><span data-stu-id="330df-236">Int32</span></span>|<span data-ttu-id="330df-237">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="330df-237">Optional.</span></span> <span data-ttu-id="330df-238">Если выбранные типы ключей восстановления включают Персоналрековерикэй, частота вращения этого ключа в месяцах.</span><span class="sxs-lookup"><span data-stu-id="330df-238">If selected recovery key type(s) include PersonalRecoveryKey, the frequency to rotate that key, in months.</span></span>|
|<span data-ttu-id="330df-239">филеваулсидеперсоналрековерикэй</span><span class="sxs-lookup"><span data-stu-id="330df-239">fileVaultHidePersonalRecoveryKey</span></span>|<span data-ttu-id="330df-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="330df-240">Boolean</span></span>|<span data-ttu-id="330df-241">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="330df-241">Optional.</span></span> <span data-ttu-id="330df-242">Скрытый персональный ключ восстановления не отображается на экране пользователя во время шифрования Филеваулт, что снижает риск его завершения в неправильной руки.</span><span class="sxs-lookup"><span data-stu-id="330df-242">A hidden personal recovery key does not appear on the user's screen during FileVault encryption, reducing the risk of it ending up in the wrong hands.</span></span>|
|<span data-ttu-id="330df-243">адванцедсреатпротектионреалтиме</span><span class="sxs-lookup"><span data-stu-id="330df-243">advancedThreatProtectionRealTime</span></span>|[<span data-ttu-id="330df-244">Включение</span><span class="sxs-lookup"><span data-stu-id="330df-244">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="330df-245">Определяет, следует ли включить защиту в режиме реального времени для функции Advanced Threat Protection для защитника Майкрософт в macOS.</span><span class="sxs-lookup"><span data-stu-id="330df-245">Determines whether or not to enable real-time protection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="330df-246">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="330df-246">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="330df-247">адванцедсреатпротектионклаудделиверед</span><span class="sxs-lookup"><span data-stu-id="330df-247">advancedThreatProtectionCloudDelivered</span></span>|[<span data-ttu-id="330df-248">Включение</span><span class="sxs-lookup"><span data-stu-id="330df-248">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="330df-249">Определяет, следует ли включить защиту от облачной защиты для Advanced Threat Protection в защитнике Майкрософт для macOS.</span><span class="sxs-lookup"><span data-stu-id="330df-249">Determines whether or not to enable cloud-delivered protection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="330df-250">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="330df-250">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="330df-251">адванцедсреатпротектионаутоматиксамплесубмиссион</span><span class="sxs-lookup"><span data-stu-id="330df-251">advancedThreatProtectionAutomaticSampleSubmission</span></span>|[<span data-ttu-id="330df-252">Включение</span><span class="sxs-lookup"><span data-stu-id="330df-252">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="330df-253">Определяет, следует ли включать автоматическую отправку образца файлов для Advanced Threat Protection в защитнике Майкрософт в macOS.</span><span class="sxs-lookup"><span data-stu-id="330df-253">Determines whether or not to enable automatic file sample submission for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="330df-254">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="330df-254">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="330df-255">адванцедсреатпротектиондиагностикдатаколлектион</span><span class="sxs-lookup"><span data-stu-id="330df-255">advancedThreatProtectionDiagnosticDataCollection</span></span>|[<span data-ttu-id="330df-256">Включение</span><span class="sxs-lookup"><span data-stu-id="330df-256">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="330df-257">Определяет, следует ли включить сбор данных диагностики и использования для Advanced Threat Protection для защитника Майкрософт в macOS.</span><span class="sxs-lookup"><span data-stu-id="330df-257">Determines whether or not to enable diagnostic and usage data collection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="330df-258">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="330df-258">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="330df-259">адванцедсреатпротектионексклудедфолдерс</span><span class="sxs-lookup"><span data-stu-id="330df-259">advancedThreatProtectionExcludedFolders</span></span>|<span data-ttu-id="330df-260">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="330df-260">String collection</span></span>|<span data-ttu-id="330df-261">Список путей к папкам, которые необходимо исключить из антивирусной проверки для Advanced Threat protection защитника Майкрософт в macOS.</span><span class="sxs-lookup"><span data-stu-id="330df-261">A list of paths to folders to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="330df-262">адванцедсреатпротектионексклудедфилес</span><span class="sxs-lookup"><span data-stu-id="330df-262">advancedThreatProtectionExcludedFiles</span></span>|<span data-ttu-id="330df-263">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="330df-263">String collection</span></span>|<span data-ttu-id="330df-264">Список путей к файлам, которые необходимо исключить из антивирусной проверки для Advanced Threat Protection в macOS.</span><span class="sxs-lookup"><span data-stu-id="330df-264">A list of paths to files to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="330df-265">адванцедсреатпротектионексклудедекстенсионс</span><span class="sxs-lookup"><span data-stu-id="330df-265">advancedThreatProtectionExcludedExtensions</span></span>|<span data-ttu-id="330df-266">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="330df-266">String collection</span></span>|<span data-ttu-id="330df-267">Список расширений файлов, которые необходимо исключить из антивирусного сканирования для Advanced Threat Protection в macOS.</span><span class="sxs-lookup"><span data-stu-id="330df-267">A list of file extensions to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="330df-268">адванцедсреатпротектионексклудедпроцессес</span><span class="sxs-lookup"><span data-stu-id="330df-268">advancedThreatProtectionExcludedProcesses</span></span>|<span data-ttu-id="330df-269">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="330df-269">String collection</span></span>|<span data-ttu-id="330df-270">Список имен процессов, которые необходимо исключить из антивирусной проверки для Advanced Threat Protection в macOS.</span><span class="sxs-lookup"><span data-stu-id="330df-270">A list of process names to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|



## <a name="response"></a><span data-ttu-id="330df-271">Отклик</span><span class="sxs-lookup"><span data-stu-id="330df-271">Response</span></span>
<span data-ttu-id="330df-272">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="330df-272">If successful, this method returns a `200 OK` response code and an updated [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="330df-273">Пример</span><span class="sxs-lookup"><span data-stu-id="330df-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="330df-274">Запрос</span><span class="sxs-lookup"><span data-stu-id="330df-274">Request</span></span>
<span data-ttu-id="330df-275">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="330df-275">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="330df-276">Отклик</span><span class="sxs-lookup"><span data-stu-id="330df-276">Response</span></span>
<span data-ttu-id="330df-p128">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="330df-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



