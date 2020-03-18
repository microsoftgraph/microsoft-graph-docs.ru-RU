---
title: Обновление Макосендпоинтпротектионконфигуратион
description: Обновление свойств объекта Макосендпоинтпротектионконфигуратион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 32c304b4ac704709a5ed3542580125aea79fcdf6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42746509"
---
# <a name="update-macosendpointprotectionconfiguration"></a><span data-ttu-id="4b741-103">Обновление Макосендпоинтпротектионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4b741-103">Update macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="4b741-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b741-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b741-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b741-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b741-106">Обновление свойств объекта [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4b741-106">Update the properties of a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b741-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4b741-107">Prerequisites</span></span>
<span data-ttu-id="4b741-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b741-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b741-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b741-110">Permission type</span></span>|<span data-ttu-id="4b741-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b741-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b741-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b741-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b741-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b741-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b741-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b741-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b741-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b741-115">Not supported.</span></span>|
|<span data-ttu-id="4b741-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4b741-116">Application</span></span>|<span data-ttu-id="4b741-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b741-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b741-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b741-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4b741-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4b741-119">Request headers</span></span>
|<span data-ttu-id="4b741-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b741-120">Header</span></span>|<span data-ttu-id="4b741-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4b741-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b741-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b741-122">Authorization</span></span>|<span data-ttu-id="4b741-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b741-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b741-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4b741-124">Accept</span></span>|<span data-ttu-id="4b741-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4b741-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b741-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b741-126">Request body</span></span>
<span data-ttu-id="4b741-127">В тексте запроса добавьте представление объекта [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b741-127">In the request body, supply a JSON representation for the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="4b741-128">В следующей таблице приведены свойства, необходимые при создании [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b741-128">The following table shows the properties that are required when you create the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="4b741-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b741-129">Property</span></span>|<span data-ttu-id="4b741-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4b741-130">Type</span></span>|<span data-ttu-id="4b741-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4b741-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b741-132">id</span><span class="sxs-lookup"><span data-stu-id="4b741-132">id</span></span>|<span data-ttu-id="4b741-133">String</span><span class="sxs-lookup"><span data-stu-id="4b741-133">String</span></span>|<span data-ttu-id="4b741-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4b741-134">Key of the entity.</span></span> <span data-ttu-id="4b741-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b741-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b741-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b741-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4b741-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b741-137">DateTimeOffset</span></span>|<span data-ttu-id="4b741-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4b741-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4b741-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b741-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b741-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4b741-140">roleScopeTagIds</span></span>|<span data-ttu-id="4b741-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b741-141">String collection</span></span>|<span data-ttu-id="4b741-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4b741-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4b741-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b741-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b741-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4b741-144">supportsScopeTags</span></span>|<span data-ttu-id="4b741-145">Логический</span><span class="sxs-lookup"><span data-stu-id="4b741-145">Boolean</span></span>|<span data-ttu-id="4b741-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4b741-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4b741-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4b741-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4b741-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4b741-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4b741-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4b741-149">This property is read-only.</span></span> <span data-ttu-id="4b741-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b741-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b741-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4b741-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4b741-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4b741-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4b741-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4b741-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4b741-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b741-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b741-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4b741-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4b741-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4b741-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4b741-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4b741-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4b741-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b741-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b741-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4b741-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4b741-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4b741-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4b741-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4b741-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4b741-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b741-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b741-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b741-163">createdDateTime</span></span>|<span data-ttu-id="4b741-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b741-164">DateTimeOffset</span></span>|<span data-ttu-id="4b741-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4b741-165">DateTime the object was created.</span></span> <span data-ttu-id="4b741-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b741-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b741-167">description</span><span class="sxs-lookup"><span data-stu-id="4b741-167">description</span></span>|<span data-ttu-id="4b741-168">String</span><span class="sxs-lookup"><span data-stu-id="4b741-168">String</span></span>|<span data-ttu-id="4b741-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b741-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4b741-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b741-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b741-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4b741-171">displayName</span></span>|<span data-ttu-id="4b741-172">Строка</span><span class="sxs-lookup"><span data-stu-id="4b741-172">String</span></span>|<span data-ttu-id="4b741-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b741-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4b741-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b741-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b741-175">version</span><span class="sxs-lookup"><span data-stu-id="4b741-175">version</span></span>|<span data-ttu-id="4b741-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4b741-176">Int32</span></span>|<span data-ttu-id="4b741-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b741-177">Version of the device configuration.</span></span> <span data-ttu-id="4b741-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b741-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b741-179">гатекипералловедаппсаурце</span><span class="sxs-lookup"><span data-stu-id="4b741-179">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="4b741-180">макосгатекипераппсаурцес</span><span class="sxs-lookup"><span data-stu-id="4b741-180">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="4b741-181">Параметры системы и конфиденциальности, которые определяют, какие расположения скачивания приложения можно запускать с устройства macOS.</span><span class="sxs-lookup"><span data-stu-id="4b741-181">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="4b741-182">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="4b741-182">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="4b741-183">гатекиперблокковерриде</span><span class="sxs-lookup"><span data-stu-id="4b741-183">gatekeeperBlockOverride</span></span>|<span data-ttu-id="4b741-184">Логический</span><span class="sxs-lookup"><span data-stu-id="4b741-184">Boolean</span></span>|<span data-ttu-id="4b741-185">Если задано значение true, переопределение пользователя для привратника будет отключено.</span><span class="sxs-lookup"><span data-stu-id="4b741-185">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="4b741-186">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="4b741-186">firewallEnabled</span></span>|<span data-ttu-id="4b741-187">Логический</span><span class="sxs-lookup"><span data-stu-id="4b741-187">Boolean</span></span>|<span data-ttu-id="4b741-188">Указывает, следует ли включить брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="4b741-188">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="4b741-189">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="4b741-189">firewallBlockAllIncoming</span></span>|<span data-ttu-id="4b741-190">Логический</span><span class="sxs-lookup"><span data-stu-id="4b741-190">Boolean</span></span>|<span data-ttu-id="4b741-191">Соответствует параметру "блокировать все входящие подключения".</span><span class="sxs-lookup"><span data-stu-id="4b741-191">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="4b741-192">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="4b741-192">firewallEnableStealthMode</span></span>|<span data-ttu-id="4b741-193">Логический</span><span class="sxs-lookup"><span data-stu-id="4b741-193">Boolean</span></span>|<span data-ttu-id="4b741-194">Соответствует параметру "включить скрытый режим".</span><span class="sxs-lookup"><span data-stu-id="4b741-194">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="4b741-195">фиреваллаппликатионс</span><span class="sxs-lookup"><span data-stu-id="4b741-195">firewallApplications</span></span>|<span data-ttu-id="4b741-196">Коллекция [макосфиреваллаппликатион](../resources/intune-deviceconfig-macosfirewallapplication.md)</span><span class="sxs-lookup"><span data-stu-id="4b741-196">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="4b741-197">Список приложений с параметрами брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="4b741-197">List of applications with firewall settings.</span></span> <span data-ttu-id="4b741-198">Параметры брандмауэра для приложений, не включенных в этот список, определяются пользователем.</span><span class="sxs-lookup"><span data-stu-id="4b741-198">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="4b741-199">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4b741-199">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4b741-200">филеваултенаблед</span><span class="sxs-lookup"><span data-stu-id="4b741-200">fileVaultEnabled</span></span>|<span data-ttu-id="4b741-201">Логический</span><span class="sxs-lookup"><span data-stu-id="4b741-201">Boolean</span></span>|<span data-ttu-id="4b741-202">Указывает, следует ли включить Филеваулт.</span><span class="sxs-lookup"><span data-stu-id="4b741-202">Whether FileVault should be enabled or not.</span></span>|
|<span data-ttu-id="4b741-203">филеваултселектедрековерикэйтипес</span><span class="sxs-lookup"><span data-stu-id="4b741-203">fileVaultSelectedRecoveryKeyTypes</span></span>|[<span data-ttu-id="4b741-204">macOSFileVaultRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="4b741-204">macOSFileVaultRecoveryKeyTypes</span></span>](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|<span data-ttu-id="4b741-205">Обязательно если включен Филеваулт, определяет типы ключа восстановления, которые необходимо использовать.</span><span class="sxs-lookup"><span data-stu-id="4b741-205">Required if FileVault is enabled, determines the type(s) of recovery key to use.</span></span> <span data-ttu-id="4b741-206">.</span><span class="sxs-lookup"><span data-stu-id="4b741-206">.</span></span> <span data-ttu-id="4b741-207">Возможные значения: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span><span class="sxs-lookup"><span data-stu-id="4b741-207">Possible values are: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span></span>|
|<span data-ttu-id="4b741-208">филеваултинститутионалрековерикэйцертификате</span><span class="sxs-lookup"><span data-stu-id="4b741-208">fileVaultInstitutionalRecoveryKeyCertificate</span></span>|<span data-ttu-id="4b741-209">Binary</span><span class="sxs-lookup"><span data-stu-id="4b741-209">Binary</span></span>|<span data-ttu-id="4b741-210">Обязательно, если выбранные типы ключей восстановления включают Институтионалрековерикэй.</span><span class="sxs-lookup"><span data-stu-id="4b741-210">Required if selected recovery key type(s) include InstitutionalRecoveryKey.</span></span> <span data-ttu-id="4b741-211">Файл сертификата в кодировке DER, который использовался для установки ключа восстановления в учреждений.</span><span class="sxs-lookup"><span data-stu-id="4b741-211">The DER Encoded certificate file used to set an institutional recovery key.</span></span>|
|<span data-ttu-id="4b741-212">филеваултинститутионалрековерикэйцертификатефиленаме</span><span class="sxs-lookup"><span data-stu-id="4b741-212">fileVaultInstitutionalRecoveryKeyCertificateFileName</span></span>|<span data-ttu-id="4b741-213">String</span><span class="sxs-lookup"><span data-stu-id="4b741-213">String</span></span>|<span data-ttu-id="4b741-214">Имя файла сертификата ключа восстановления для сотрудников, который будет отображаться в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="4b741-214">File name of the institutional recovery key certificate to display in UI.</span></span> <span data-ttu-id="4b741-215">(\*. der).</span><span class="sxs-lookup"><span data-stu-id="4b741-215">(\*.der).</span></span>|
|<span data-ttu-id="4b741-216">филеваултперсоналрековерикэйхелпмессаже</span><span class="sxs-lookup"><span data-stu-id="4b741-216">fileVaultPersonalRecoveryKeyHelpMessage</span></span>|<span data-ttu-id="4b741-217">String</span><span class="sxs-lookup"><span data-stu-id="4b741-217">String</span></span>|<span data-ttu-id="4b741-218">Обязательно, если выбранные типы ключей восстановления включают Персоналрековерикэй.</span><span class="sxs-lookup"><span data-stu-id="4b741-218">Required if selected recovery key type(s) include PersonalRecoveryKey.</span></span> <span data-ttu-id="4b741-219">Короткое сообщение, в котором показано, как получить свой ключ восстановления личных настроек.</span><span class="sxs-lookup"><span data-stu-id="4b741-219">A short message displayed to the user that explains how they can retrieve their personal recovery key.</span></span>|
|<span data-ttu-id="4b741-220">филеваулталловдеферралунтилсигнаут</span><span class="sxs-lookup"><span data-stu-id="4b741-220">fileVaultAllowDeferralUntilSignOut</span></span>|<span data-ttu-id="4b741-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b741-221">Boolean</span></span>|<span data-ttu-id="4b741-222">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="4b741-222">Optional.</span></span> <span data-ttu-id="4b741-223">Если задано значение true, пользователь может отложить включение Филеваулт, пока не выйдете из системы.</span><span class="sxs-lookup"><span data-stu-id="4b741-223">If set to true, the user can defer the enabling of FileVault until they sign out.</span></span>|
|<span data-ttu-id="4b741-224">филеваултнумберофтимесусерканигноре</span><span class="sxs-lookup"><span data-stu-id="4b741-224">fileVaultNumberOfTimesUserCanIgnore</span></span>|<span data-ttu-id="4b741-225">Int32</span><span class="sxs-lookup"><span data-stu-id="4b741-225">Int32</span></span>|<span data-ttu-id="4b741-226">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="4b741-226">Optional.</span></span> <span data-ttu-id="4b741-227">При использовании параметра "отложить" это максимальное число раз, когда пользователь может игнорировать приглашения на включение Филеваулт, чтобы пользователь мог выполнить вход.</span><span class="sxs-lookup"><span data-stu-id="4b741-227">When using the Defer option, this is the maximum number of times the user can ignore prompts to enable FileVault before FileVault will be required for the user to sign in.</span></span> <span data-ttu-id="4b741-228">Если задано значение-1, всегда будет выдаваться запрос на включение Филеваулт, пока Филеваулт не будет включен, хотя разрешить пользователю обходить включение Филеваулт.</span><span class="sxs-lookup"><span data-stu-id="4b741-228">If set to -1, it will always prompt to enable FileVault until FileVault is enabled, though it will allow the user to bypass enabling FileVault.</span></span> <span data-ttu-id="4b741-229">Если задать для этого параметра значение 0, эта функция будет отключена.</span><span class="sxs-lookup"><span data-stu-id="4b741-229">Setting this to 0 will disable the feature.</span></span>|
|<span data-ttu-id="4b741-230">филеваултдисаблепромптатсигнаут</span><span class="sxs-lookup"><span data-stu-id="4b741-230">fileVaultDisablePromptAtSignOut</span></span>|<span data-ttu-id="4b741-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b741-231">Boolean</span></span>|<span data-ttu-id="4b741-232">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="4b741-232">Optional.</span></span> <span data-ttu-id="4b741-233">При использовании параметра отсрочки, если задано значение true, пользователю не предлагается включить Филеваулт при входе.</span><span class="sxs-lookup"><span data-stu-id="4b741-233">When using the Defer option, if set to true, the user is not prompted to enable FileVault at sign-out.</span></span>|
|<span data-ttu-id="4b741-234">филеваултперсоналрековерикэйротатионинмонсс</span><span class="sxs-lookup"><span data-stu-id="4b741-234">fileVaultPersonalRecoveryKeyRotationInMonths</span></span>|<span data-ttu-id="4b741-235">Int32</span><span class="sxs-lookup"><span data-stu-id="4b741-235">Int32</span></span>|<span data-ttu-id="4b741-236">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="4b741-236">Optional.</span></span> <span data-ttu-id="4b741-237">Если выбранные типы ключей восстановления включают Персоналрековерикэй, частота вращения этого ключа в месяцах.</span><span class="sxs-lookup"><span data-stu-id="4b741-237">If selected recovery key type(s) include PersonalRecoveryKey, the frequency to rotate that key, in months.</span></span>|
|<span data-ttu-id="4b741-238">филеваулсидеперсоналрековерикэй</span><span class="sxs-lookup"><span data-stu-id="4b741-238">fileVaultHidePersonalRecoveryKey</span></span>|<span data-ttu-id="4b741-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b741-239">Boolean</span></span>|<span data-ttu-id="4b741-240">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="4b741-240">Optional.</span></span> <span data-ttu-id="4b741-241">Скрытый персональный ключ восстановления не отображается на экране пользователя во время шифрования Филеваулт, что снижает риск его завершения в неправильной руки.</span><span class="sxs-lookup"><span data-stu-id="4b741-241">A hidden personal recovery key does not appear on the user's screen during FileVault encryption, reducing the risk of it ending up in the wrong hands.</span></span>|
|<span data-ttu-id="4b741-242">адванцедсреатпротектионреалтиме</span><span class="sxs-lookup"><span data-stu-id="4b741-242">advancedThreatProtectionRealTime</span></span>|[<span data-ttu-id="4b741-243">Включение</span><span class="sxs-lookup"><span data-stu-id="4b741-243">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4b741-244">Определяет, следует ли включить защиту в режиме реального времени для функции Advanced Threat Protection для защитника Майкрософт в macOS.</span><span class="sxs-lookup"><span data-stu-id="4b741-244">Determines whether or not to enable real-time protection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="4b741-245">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4b741-245">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4b741-246">адванцедсреатпротектионклаудделиверед</span><span class="sxs-lookup"><span data-stu-id="4b741-246">advancedThreatProtectionCloudDelivered</span></span>|[<span data-ttu-id="4b741-247">Включение</span><span class="sxs-lookup"><span data-stu-id="4b741-247">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4b741-248">Определяет, следует ли включить защиту от облачной защиты для Advanced Threat Protection в защитнике Майкрософт для macOS.</span><span class="sxs-lookup"><span data-stu-id="4b741-248">Determines whether or not to enable cloud-delivered protection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="4b741-249">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4b741-249">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4b741-250">адванцедсреатпротектионаутоматиксамплесубмиссион</span><span class="sxs-lookup"><span data-stu-id="4b741-250">advancedThreatProtectionAutomaticSampleSubmission</span></span>|[<span data-ttu-id="4b741-251">Включение</span><span class="sxs-lookup"><span data-stu-id="4b741-251">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4b741-252">Определяет, следует ли включать автоматическую отправку образца файлов для Advanced Threat Protection в защитнике Майкрософт в macOS.</span><span class="sxs-lookup"><span data-stu-id="4b741-252">Determines whether or not to enable automatic file sample submission for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="4b741-253">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4b741-253">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4b741-254">адванцедсреатпротектиондиагностикдатаколлектион</span><span class="sxs-lookup"><span data-stu-id="4b741-254">advancedThreatProtectionDiagnosticDataCollection</span></span>|[<span data-ttu-id="4b741-255">Включение</span><span class="sxs-lookup"><span data-stu-id="4b741-255">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4b741-256">Определяет, следует ли включить сбор данных диагностики и использования для Advanced Threat Protection для защитника Майкрософт в macOS.</span><span class="sxs-lookup"><span data-stu-id="4b741-256">Determines whether or not to enable diagnostic and usage data collection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="4b741-257">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4b741-257">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4b741-258">адванцедсреатпротектионексклудедфолдерс</span><span class="sxs-lookup"><span data-stu-id="4b741-258">advancedThreatProtectionExcludedFolders</span></span>|<span data-ttu-id="4b741-259">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b741-259">String collection</span></span>|<span data-ttu-id="4b741-260">Список путей к папкам, которые необходимо исключить из антивирусной проверки для Advanced Threat protection защитника Майкрософт в macOS.</span><span class="sxs-lookup"><span data-stu-id="4b741-260">A list of paths to folders to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="4b741-261">адванцедсреатпротектионексклудедфилес</span><span class="sxs-lookup"><span data-stu-id="4b741-261">advancedThreatProtectionExcludedFiles</span></span>|<span data-ttu-id="4b741-262">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b741-262">String collection</span></span>|<span data-ttu-id="4b741-263">Список путей к файлам, которые необходимо исключить из антивирусной проверки для Advanced Threat Protection в macOS.</span><span class="sxs-lookup"><span data-stu-id="4b741-263">A list of paths to files to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="4b741-264">адванцедсреатпротектионексклудедекстенсионс</span><span class="sxs-lookup"><span data-stu-id="4b741-264">advancedThreatProtectionExcludedExtensions</span></span>|<span data-ttu-id="4b741-265">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b741-265">String collection</span></span>|<span data-ttu-id="4b741-266">Список расширений файлов, которые необходимо исключить из антивирусного сканирования для Advanced Threat Protection в macOS.</span><span class="sxs-lookup"><span data-stu-id="4b741-266">A list of file extensions to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="4b741-267">адванцедсреатпротектионексклудедпроцессес</span><span class="sxs-lookup"><span data-stu-id="4b741-267">advancedThreatProtectionExcludedProcesses</span></span>|<span data-ttu-id="4b741-268">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b741-268">String collection</span></span>|<span data-ttu-id="4b741-269">Список имен процессов, которые необходимо исключить из антивирусной проверки для Advanced Threat Protection в macOS.</span><span class="sxs-lookup"><span data-stu-id="4b741-269">A list of process names to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|



## <a name="response"></a><span data-ttu-id="4b741-270">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b741-270">Response</span></span>
<span data-ttu-id="4b741-271">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b741-271">If successful, this method returns a `200 OK` response code and an updated [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b741-272">Пример</span><span class="sxs-lookup"><span data-stu-id="4b741-272">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b741-273">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b741-273">Request</span></span>
<span data-ttu-id="4b741-274">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b741-274">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4b741-275">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b741-275">Response</span></span>
<span data-ttu-id="4b741-p128">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b741-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




