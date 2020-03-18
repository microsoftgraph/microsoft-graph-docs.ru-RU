---
title: Создание Макосендпоинтпротектионконфигуратион
description: Создание нового объекта Макосендпоинтпротектионконфигуратион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: add0da374dd4dcdd11f9a516f241604ad538f91b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42746901"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="0de5d-103">Создание Макосендпоинтпротектионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="0de5d-103">Create macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="0de5d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0de5d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0de5d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0de5d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0de5d-106">Создание нового объекта [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0de5d-106">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0de5d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0de5d-107">Prerequisites</span></span>
<span data-ttu-id="0de5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0de5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0de5d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0de5d-110">Permission type</span></span>|<span data-ttu-id="0de5d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0de5d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0de5d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0de5d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0de5d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0de5d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0de5d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0de5d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0de5d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0de5d-115">Not supported.</span></span>|
|<span data-ttu-id="0de5d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0de5d-116">Application</span></span>|<span data-ttu-id="0de5d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0de5d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0de5d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0de5d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0de5d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0de5d-119">Request headers</span></span>
|<span data-ttu-id="0de5d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0de5d-120">Header</span></span>|<span data-ttu-id="0de5d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0de5d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0de5d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0de5d-122">Authorization</span></span>|<span data-ttu-id="0de5d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0de5d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0de5d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0de5d-124">Accept</span></span>|<span data-ttu-id="0de5d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0de5d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0de5d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0de5d-126">Request body</span></span>
<span data-ttu-id="0de5d-127">В тексте запроса добавьте представление объекта Макосендпоинтпротектионконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0de5d-127">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="0de5d-128">В следующей таблице приведены свойства, необходимые при создании Макосендпоинтпротектионконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="0de5d-128">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="0de5d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0de5d-129">Property</span></span>|<span data-ttu-id="0de5d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0de5d-130">Type</span></span>|<span data-ttu-id="0de5d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0de5d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0de5d-132">id</span><span class="sxs-lookup"><span data-stu-id="0de5d-132">id</span></span>|<span data-ttu-id="0de5d-133">String</span><span class="sxs-lookup"><span data-stu-id="0de5d-133">String</span></span>|<span data-ttu-id="0de5d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0de5d-134">Key of the entity.</span></span> <span data-ttu-id="0de5d-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0de5d-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0de5d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0de5d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0de5d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0de5d-137">DateTimeOffset</span></span>|<span data-ttu-id="0de5d-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0de5d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0de5d-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0de5d-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0de5d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0de5d-140">roleScopeTagIds</span></span>|<span data-ttu-id="0de5d-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0de5d-141">String collection</span></span>|<span data-ttu-id="0de5d-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="0de5d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0de5d-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0de5d-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0de5d-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="0de5d-144">supportsScopeTags</span></span>|<span data-ttu-id="0de5d-145">Логический</span><span class="sxs-lookup"><span data-stu-id="0de5d-145">Boolean</span></span>|<span data-ttu-id="0de5d-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="0de5d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0de5d-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="0de5d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0de5d-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="0de5d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0de5d-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0de5d-149">This property is read-only.</span></span> <span data-ttu-id="0de5d-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0de5d-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0de5d-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0de5d-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0de5d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0de5d-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0de5d-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0de5d-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0de5d-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0de5d-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0de5d-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0de5d-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0de5d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0de5d-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0de5d-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0de5d-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0de5d-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0de5d-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0de5d-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0de5d-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0de5d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0de5d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0de5d-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0de5d-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0de5d-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0de5d-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0de5d-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0de5d-163">createdDateTime</span></span>|<span data-ttu-id="0de5d-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0de5d-164">DateTimeOffset</span></span>|<span data-ttu-id="0de5d-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0de5d-165">DateTime the object was created.</span></span> <span data-ttu-id="0de5d-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0de5d-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0de5d-167">description</span><span class="sxs-lookup"><span data-stu-id="0de5d-167">description</span></span>|<span data-ttu-id="0de5d-168">String</span><span class="sxs-lookup"><span data-stu-id="0de5d-168">String</span></span>|<span data-ttu-id="0de5d-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0de5d-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0de5d-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0de5d-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0de5d-171">displayName</span><span class="sxs-lookup"><span data-stu-id="0de5d-171">displayName</span></span>|<span data-ttu-id="0de5d-172">Строка</span><span class="sxs-lookup"><span data-stu-id="0de5d-172">String</span></span>|<span data-ttu-id="0de5d-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0de5d-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0de5d-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0de5d-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0de5d-175">version</span><span class="sxs-lookup"><span data-stu-id="0de5d-175">version</span></span>|<span data-ttu-id="0de5d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0de5d-176">Int32</span></span>|<span data-ttu-id="0de5d-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0de5d-177">Version of the device configuration.</span></span> <span data-ttu-id="0de5d-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0de5d-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0de5d-179">гатекипералловедаппсаурце</span><span class="sxs-lookup"><span data-stu-id="0de5d-179">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="0de5d-180">макосгатекипераппсаурцес</span><span class="sxs-lookup"><span data-stu-id="0de5d-180">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="0de5d-181">Параметры системы и конфиденциальности, которые определяют, какие расположения скачивания приложения можно запускать с устройства macOS.</span><span class="sxs-lookup"><span data-stu-id="0de5d-181">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="0de5d-182">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="0de5d-182">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="0de5d-183">гатекиперблокковерриде</span><span class="sxs-lookup"><span data-stu-id="0de5d-183">gatekeeperBlockOverride</span></span>|<span data-ttu-id="0de5d-184">Логический</span><span class="sxs-lookup"><span data-stu-id="0de5d-184">Boolean</span></span>|<span data-ttu-id="0de5d-185">Если задано значение true, переопределение пользователя для привратника будет отключено.</span><span class="sxs-lookup"><span data-stu-id="0de5d-185">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="0de5d-186">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="0de5d-186">firewallEnabled</span></span>|<span data-ttu-id="0de5d-187">Логический</span><span class="sxs-lookup"><span data-stu-id="0de5d-187">Boolean</span></span>|<span data-ttu-id="0de5d-188">Указывает, следует ли включить брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="0de5d-188">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="0de5d-189">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="0de5d-189">firewallBlockAllIncoming</span></span>|<span data-ttu-id="0de5d-190">Логический</span><span class="sxs-lookup"><span data-stu-id="0de5d-190">Boolean</span></span>|<span data-ttu-id="0de5d-191">Соответствует параметру "блокировать все входящие подключения".</span><span class="sxs-lookup"><span data-stu-id="0de5d-191">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="0de5d-192">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="0de5d-192">firewallEnableStealthMode</span></span>|<span data-ttu-id="0de5d-193">Логический</span><span class="sxs-lookup"><span data-stu-id="0de5d-193">Boolean</span></span>|<span data-ttu-id="0de5d-194">Соответствует параметру "включить скрытый режим".</span><span class="sxs-lookup"><span data-stu-id="0de5d-194">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="0de5d-195">фиреваллаппликатионс</span><span class="sxs-lookup"><span data-stu-id="0de5d-195">firewallApplications</span></span>|<span data-ttu-id="0de5d-196">Коллекция [макосфиреваллаппликатион](../resources/intune-deviceconfig-macosfirewallapplication.md)</span><span class="sxs-lookup"><span data-stu-id="0de5d-196">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="0de5d-197">Список приложений с параметрами брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="0de5d-197">List of applications with firewall settings.</span></span> <span data-ttu-id="0de5d-198">Параметры брандмауэра для приложений, не включенных в этот список, определяются пользователем.</span><span class="sxs-lookup"><span data-stu-id="0de5d-198">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="0de5d-199">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="0de5d-199">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0de5d-200">филеваултенаблед</span><span class="sxs-lookup"><span data-stu-id="0de5d-200">fileVaultEnabled</span></span>|<span data-ttu-id="0de5d-201">Логический</span><span class="sxs-lookup"><span data-stu-id="0de5d-201">Boolean</span></span>|<span data-ttu-id="0de5d-202">Указывает, следует ли включить Филеваулт.</span><span class="sxs-lookup"><span data-stu-id="0de5d-202">Whether FileVault should be enabled or not.</span></span>|
|<span data-ttu-id="0de5d-203">филеваултселектедрековерикэйтипес</span><span class="sxs-lookup"><span data-stu-id="0de5d-203">fileVaultSelectedRecoveryKeyTypes</span></span>|[<span data-ttu-id="0de5d-204">macOSFileVaultRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="0de5d-204">macOSFileVaultRecoveryKeyTypes</span></span>](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|<span data-ttu-id="0de5d-205">Обязательно если включен Филеваулт, определяет типы ключа восстановления, которые необходимо использовать.</span><span class="sxs-lookup"><span data-stu-id="0de5d-205">Required if FileVault is enabled, determines the type(s) of recovery key to use.</span></span> <span data-ttu-id="0de5d-206">.</span><span class="sxs-lookup"><span data-stu-id="0de5d-206">.</span></span> <span data-ttu-id="0de5d-207">Возможные значения: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span><span class="sxs-lookup"><span data-stu-id="0de5d-207">Possible values are: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span></span>|
|<span data-ttu-id="0de5d-208">филеваултинститутионалрековерикэйцертификате</span><span class="sxs-lookup"><span data-stu-id="0de5d-208">fileVaultInstitutionalRecoveryKeyCertificate</span></span>|<span data-ttu-id="0de5d-209">Binary</span><span class="sxs-lookup"><span data-stu-id="0de5d-209">Binary</span></span>|<span data-ttu-id="0de5d-210">Обязательно, если выбранные типы ключей восстановления включают Институтионалрековерикэй.</span><span class="sxs-lookup"><span data-stu-id="0de5d-210">Required if selected recovery key type(s) include InstitutionalRecoveryKey.</span></span> <span data-ttu-id="0de5d-211">Файл сертификата в кодировке DER, который использовался для установки ключа восстановления в учреждений.</span><span class="sxs-lookup"><span data-stu-id="0de5d-211">The DER Encoded certificate file used to set an institutional recovery key.</span></span>|
|<span data-ttu-id="0de5d-212">филеваултинститутионалрековерикэйцертификатефиленаме</span><span class="sxs-lookup"><span data-stu-id="0de5d-212">fileVaultInstitutionalRecoveryKeyCertificateFileName</span></span>|<span data-ttu-id="0de5d-213">String</span><span class="sxs-lookup"><span data-stu-id="0de5d-213">String</span></span>|<span data-ttu-id="0de5d-214">Имя файла сертификата ключа восстановления для сотрудников, который будет отображаться в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="0de5d-214">File name of the institutional recovery key certificate to display in UI.</span></span> <span data-ttu-id="0de5d-215">(\*. der).</span><span class="sxs-lookup"><span data-stu-id="0de5d-215">(\*.der).</span></span>|
|<span data-ttu-id="0de5d-216">филеваултперсоналрековерикэйхелпмессаже</span><span class="sxs-lookup"><span data-stu-id="0de5d-216">fileVaultPersonalRecoveryKeyHelpMessage</span></span>|<span data-ttu-id="0de5d-217">String</span><span class="sxs-lookup"><span data-stu-id="0de5d-217">String</span></span>|<span data-ttu-id="0de5d-218">Обязательно, если выбранные типы ключей восстановления включают Персоналрековерикэй.</span><span class="sxs-lookup"><span data-stu-id="0de5d-218">Required if selected recovery key type(s) include PersonalRecoveryKey.</span></span> <span data-ttu-id="0de5d-219">Короткое сообщение, в котором показано, как получить свой ключ восстановления личных настроек.</span><span class="sxs-lookup"><span data-stu-id="0de5d-219">A short message displayed to the user that explains how they can retrieve their personal recovery key.</span></span>|
|<span data-ttu-id="0de5d-220">филеваулталловдеферралунтилсигнаут</span><span class="sxs-lookup"><span data-stu-id="0de5d-220">fileVaultAllowDeferralUntilSignOut</span></span>|<span data-ttu-id="0de5d-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="0de5d-221">Boolean</span></span>|<span data-ttu-id="0de5d-222">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="0de5d-222">Optional.</span></span> <span data-ttu-id="0de5d-223">Если задано значение true, пользователь может отложить включение Филеваулт, пока не выйдете из системы.</span><span class="sxs-lookup"><span data-stu-id="0de5d-223">If set to true, the user can defer the enabling of FileVault until they sign out.</span></span>|
|<span data-ttu-id="0de5d-224">филеваултнумберофтимесусерканигноре</span><span class="sxs-lookup"><span data-stu-id="0de5d-224">fileVaultNumberOfTimesUserCanIgnore</span></span>|<span data-ttu-id="0de5d-225">Int32</span><span class="sxs-lookup"><span data-stu-id="0de5d-225">Int32</span></span>|<span data-ttu-id="0de5d-226">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="0de5d-226">Optional.</span></span> <span data-ttu-id="0de5d-227">При использовании параметра "отложить" это максимальное число раз, когда пользователь может игнорировать приглашения на включение Филеваулт, чтобы пользователь мог выполнить вход.</span><span class="sxs-lookup"><span data-stu-id="0de5d-227">When using the Defer option, this is the maximum number of times the user can ignore prompts to enable FileVault before FileVault will be required for the user to sign in.</span></span> <span data-ttu-id="0de5d-228">Если задано значение-1, всегда будет выдаваться запрос на включение Филеваулт, пока Филеваулт не будет включен, хотя разрешить пользователю обходить включение Филеваулт.</span><span class="sxs-lookup"><span data-stu-id="0de5d-228">If set to -1, it will always prompt to enable FileVault until FileVault is enabled, though it will allow the user to bypass enabling FileVault.</span></span> <span data-ttu-id="0de5d-229">Если задать для этого параметра значение 0, эта функция будет отключена.</span><span class="sxs-lookup"><span data-stu-id="0de5d-229">Setting this to 0 will disable the feature.</span></span>|
|<span data-ttu-id="0de5d-230">филеваултдисаблепромптатсигнаут</span><span class="sxs-lookup"><span data-stu-id="0de5d-230">fileVaultDisablePromptAtSignOut</span></span>|<span data-ttu-id="0de5d-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="0de5d-231">Boolean</span></span>|<span data-ttu-id="0de5d-232">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="0de5d-232">Optional.</span></span> <span data-ttu-id="0de5d-233">При использовании параметра отсрочки, если задано значение true, пользователю не предлагается включить Филеваулт при входе.</span><span class="sxs-lookup"><span data-stu-id="0de5d-233">When using the Defer option, if set to true, the user is not prompted to enable FileVault at sign-out.</span></span>|
|<span data-ttu-id="0de5d-234">филеваултперсоналрековерикэйротатионинмонсс</span><span class="sxs-lookup"><span data-stu-id="0de5d-234">fileVaultPersonalRecoveryKeyRotationInMonths</span></span>|<span data-ttu-id="0de5d-235">Int32</span><span class="sxs-lookup"><span data-stu-id="0de5d-235">Int32</span></span>|<span data-ttu-id="0de5d-236">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="0de5d-236">Optional.</span></span> <span data-ttu-id="0de5d-237">Если выбранные типы ключей восстановления включают Персоналрековерикэй, частота вращения этого ключа в месяцах.</span><span class="sxs-lookup"><span data-stu-id="0de5d-237">If selected recovery key type(s) include PersonalRecoveryKey, the frequency to rotate that key, in months.</span></span>|
|<span data-ttu-id="0de5d-238">филеваулсидеперсоналрековерикэй</span><span class="sxs-lookup"><span data-stu-id="0de5d-238">fileVaultHidePersonalRecoveryKey</span></span>|<span data-ttu-id="0de5d-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="0de5d-239">Boolean</span></span>|<span data-ttu-id="0de5d-240">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="0de5d-240">Optional.</span></span> <span data-ttu-id="0de5d-241">Скрытый персональный ключ восстановления не отображается на экране пользователя во время шифрования Филеваулт, что снижает риск его завершения в неправильной руки.</span><span class="sxs-lookup"><span data-stu-id="0de5d-241">A hidden personal recovery key does not appear on the user's screen during FileVault encryption, reducing the risk of it ending up in the wrong hands.</span></span>|
|<span data-ttu-id="0de5d-242">адванцедсреатпротектионреалтиме</span><span class="sxs-lookup"><span data-stu-id="0de5d-242">advancedThreatProtectionRealTime</span></span>|[<span data-ttu-id="0de5d-243">Включение</span><span class="sxs-lookup"><span data-stu-id="0de5d-243">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="0de5d-244">Определяет, следует ли включить защиту в режиме реального времени для функции Advanced Threat Protection для защитника Майкрософт в macOS.</span><span class="sxs-lookup"><span data-stu-id="0de5d-244">Determines whether or not to enable real-time protection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="0de5d-245">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="0de5d-245">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="0de5d-246">адванцедсреатпротектионклаудделиверед</span><span class="sxs-lookup"><span data-stu-id="0de5d-246">advancedThreatProtectionCloudDelivered</span></span>|[<span data-ttu-id="0de5d-247">Включение</span><span class="sxs-lookup"><span data-stu-id="0de5d-247">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="0de5d-248">Определяет, следует ли включить защиту от облачной защиты для Advanced Threat Protection в защитнике Майкрософт для macOS.</span><span class="sxs-lookup"><span data-stu-id="0de5d-248">Determines whether or not to enable cloud-delivered protection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="0de5d-249">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="0de5d-249">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="0de5d-250">адванцедсреатпротектионаутоматиксамплесубмиссион</span><span class="sxs-lookup"><span data-stu-id="0de5d-250">advancedThreatProtectionAutomaticSampleSubmission</span></span>|[<span data-ttu-id="0de5d-251">Включение</span><span class="sxs-lookup"><span data-stu-id="0de5d-251">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="0de5d-252">Определяет, следует ли включать автоматическую отправку образца файлов для Advanced Threat Protection в защитнике Майкрософт в macOS.</span><span class="sxs-lookup"><span data-stu-id="0de5d-252">Determines whether or not to enable automatic file sample submission for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="0de5d-253">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="0de5d-253">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="0de5d-254">адванцедсреатпротектиондиагностикдатаколлектион</span><span class="sxs-lookup"><span data-stu-id="0de5d-254">advancedThreatProtectionDiagnosticDataCollection</span></span>|[<span data-ttu-id="0de5d-255">Включение</span><span class="sxs-lookup"><span data-stu-id="0de5d-255">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="0de5d-256">Определяет, следует ли включить сбор данных диагностики и использования для Advanced Threat Protection для защитника Майкрософт в macOS.</span><span class="sxs-lookup"><span data-stu-id="0de5d-256">Determines whether or not to enable diagnostic and usage data collection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="0de5d-257">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="0de5d-257">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="0de5d-258">адванцедсреатпротектионексклудедфолдерс</span><span class="sxs-lookup"><span data-stu-id="0de5d-258">advancedThreatProtectionExcludedFolders</span></span>|<span data-ttu-id="0de5d-259">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0de5d-259">String collection</span></span>|<span data-ttu-id="0de5d-260">Список путей к папкам, которые необходимо исключить из антивирусной проверки для Advanced Threat protection защитника Майкрософт в macOS.</span><span class="sxs-lookup"><span data-stu-id="0de5d-260">A list of paths to folders to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="0de5d-261">адванцедсреатпротектионексклудедфилес</span><span class="sxs-lookup"><span data-stu-id="0de5d-261">advancedThreatProtectionExcludedFiles</span></span>|<span data-ttu-id="0de5d-262">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0de5d-262">String collection</span></span>|<span data-ttu-id="0de5d-263">Список путей к файлам, которые необходимо исключить из антивирусной проверки для Advanced Threat Protection в macOS.</span><span class="sxs-lookup"><span data-stu-id="0de5d-263">A list of paths to files to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="0de5d-264">адванцедсреатпротектионексклудедекстенсионс</span><span class="sxs-lookup"><span data-stu-id="0de5d-264">advancedThreatProtectionExcludedExtensions</span></span>|<span data-ttu-id="0de5d-265">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0de5d-265">String collection</span></span>|<span data-ttu-id="0de5d-266">Список расширений файлов, которые необходимо исключить из антивирусного сканирования для Advanced Threat Protection в macOS.</span><span class="sxs-lookup"><span data-stu-id="0de5d-266">A list of file extensions to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="0de5d-267">адванцедсреатпротектионексклудедпроцессес</span><span class="sxs-lookup"><span data-stu-id="0de5d-267">advancedThreatProtectionExcludedProcesses</span></span>|<span data-ttu-id="0de5d-268">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0de5d-268">String collection</span></span>|<span data-ttu-id="0de5d-269">Список имен процессов, которые необходимо исключить из антивирусной проверки для Advanced Threat Protection в macOS.</span><span class="sxs-lookup"><span data-stu-id="0de5d-269">A list of process names to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|



## <a name="response"></a><span data-ttu-id="0de5d-270">Отклик</span><span class="sxs-lookup"><span data-stu-id="0de5d-270">Response</span></span>
<span data-ttu-id="0de5d-271">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0de5d-271">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0de5d-272">Пример</span><span class="sxs-lookup"><span data-stu-id="0de5d-272">Example</span></span>

### <a name="request"></a><span data-ttu-id="0de5d-273">Запрос</span><span class="sxs-lookup"><span data-stu-id="0de5d-273">Request</span></span>
<span data-ttu-id="0de5d-274">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0de5d-274">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0de5d-275">Отклик</span><span class="sxs-lookup"><span data-stu-id="0de5d-275">Response</span></span>
<span data-ttu-id="0de5d-p128">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0de5d-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




