---
title: Создание Макосендпоинтпротектионконфигуратион
description: Создание нового объекта Макосендпоинтпротектионконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c7b0fcbdcb2507f2a260ca972360c5f28ba3f7fb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733009"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="9810f-103">Создание Макосендпоинтпротектионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9810f-103">Create macOSEndpointProtectionConfiguration</span></span>

<span data-ttu-id="9810f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9810f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9810f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9810f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9810f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9810f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9810f-107">Создание нового объекта [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9810f-107">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9810f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9810f-108">Prerequisites</span></span>
<span data-ttu-id="9810f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9810f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9810f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9810f-111">Permission type</span></span>|<span data-ttu-id="9810f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9810f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9810f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9810f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9810f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9810f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9810f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9810f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9810f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9810f-116">Not supported.</span></span>|
|<span data-ttu-id="9810f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9810f-117">Application</span></span>|<span data-ttu-id="9810f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9810f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9810f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9810f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9810f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9810f-120">Request headers</span></span>
|<span data-ttu-id="9810f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9810f-121">Header</span></span>|<span data-ttu-id="9810f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9810f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9810f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9810f-123">Authorization</span></span>|<span data-ttu-id="9810f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9810f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9810f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9810f-125">Accept</span></span>|<span data-ttu-id="9810f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9810f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9810f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9810f-127">Request body</span></span>
<span data-ttu-id="9810f-128">В тексте запроса добавьте представление объекта Макосендпоинтпротектионконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9810f-128">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="9810f-129">В следующей таблице приведены свойства, необходимые при создании Макосендпоинтпротектионконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="9810f-129">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="9810f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9810f-130">Property</span></span>|<span data-ttu-id="9810f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9810f-131">Type</span></span>|<span data-ttu-id="9810f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9810f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9810f-133">id</span><span class="sxs-lookup"><span data-stu-id="9810f-133">id</span></span>|<span data-ttu-id="9810f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9810f-134">String</span></span>|<span data-ttu-id="9810f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9810f-135">Key of the entity.</span></span> <span data-ttu-id="9810f-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9810f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9810f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9810f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9810f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9810f-138">DateTimeOffset</span></span>|<span data-ttu-id="9810f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9810f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9810f-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9810f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9810f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9810f-141">roleScopeTagIds</span></span>|<span data-ttu-id="9810f-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9810f-142">String collection</span></span>|<span data-ttu-id="9810f-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="9810f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9810f-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9810f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9810f-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="9810f-145">supportsScopeTags</span></span>|<span data-ttu-id="9810f-146">Логический</span><span class="sxs-lookup"><span data-stu-id="9810f-146">Boolean</span></span>|<span data-ttu-id="9810f-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="9810f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9810f-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="9810f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9810f-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="9810f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9810f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9810f-150">This property is read-only.</span></span> <span data-ttu-id="9810f-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9810f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9810f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9810f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9810f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9810f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9810f-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9810f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9810f-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9810f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9810f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9810f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9810f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9810f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9810f-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9810f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9810f-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9810f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9810f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9810f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9810f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9810f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9810f-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9810f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9810f-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9810f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9810f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9810f-164">createdDateTime</span></span>|<span data-ttu-id="9810f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9810f-165">DateTimeOffset</span></span>|<span data-ttu-id="9810f-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9810f-166">DateTime the object was created.</span></span> <span data-ttu-id="9810f-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9810f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9810f-168">description</span><span class="sxs-lookup"><span data-stu-id="9810f-168">description</span></span>|<span data-ttu-id="9810f-169">Строка</span><span class="sxs-lookup"><span data-stu-id="9810f-169">String</span></span>|<span data-ttu-id="9810f-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9810f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9810f-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9810f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9810f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9810f-172">displayName</span></span>|<span data-ttu-id="9810f-173">Строка</span><span class="sxs-lookup"><span data-stu-id="9810f-173">String</span></span>|<span data-ttu-id="9810f-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9810f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9810f-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9810f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9810f-176">version</span><span class="sxs-lookup"><span data-stu-id="9810f-176">version</span></span>|<span data-ttu-id="9810f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9810f-177">Int32</span></span>|<span data-ttu-id="9810f-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9810f-178">Version of the device configuration.</span></span> <span data-ttu-id="9810f-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9810f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9810f-180">гатекипералловедаппсаурце</span><span class="sxs-lookup"><span data-stu-id="9810f-180">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="9810f-181">макосгатекипераппсаурцес</span><span class="sxs-lookup"><span data-stu-id="9810f-181">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="9810f-182">Параметры системы и конфиденциальности, которые определяют, какие расположения скачивания приложения можно запускать с устройства macOS.</span><span class="sxs-lookup"><span data-stu-id="9810f-182">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="9810f-183">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="9810f-183">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="9810f-184">гатекиперблокковерриде</span><span class="sxs-lookup"><span data-stu-id="9810f-184">gatekeeperBlockOverride</span></span>|<span data-ttu-id="9810f-185">Логический</span><span class="sxs-lookup"><span data-stu-id="9810f-185">Boolean</span></span>|<span data-ttu-id="9810f-186">Если задано значение true, переопределение пользователя для привратника будет отключено.</span><span class="sxs-lookup"><span data-stu-id="9810f-186">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="9810f-187">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="9810f-187">firewallEnabled</span></span>|<span data-ttu-id="9810f-188">Логический</span><span class="sxs-lookup"><span data-stu-id="9810f-188">Boolean</span></span>|<span data-ttu-id="9810f-189">Указывает, следует ли включить брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="9810f-189">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="9810f-190">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="9810f-190">firewallBlockAllIncoming</span></span>|<span data-ttu-id="9810f-191">Логический</span><span class="sxs-lookup"><span data-stu-id="9810f-191">Boolean</span></span>|<span data-ttu-id="9810f-192">Соответствует параметру "блокировать все входящие подключения".</span><span class="sxs-lookup"><span data-stu-id="9810f-192">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="9810f-193">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="9810f-193">firewallEnableStealthMode</span></span>|<span data-ttu-id="9810f-194">Логический</span><span class="sxs-lookup"><span data-stu-id="9810f-194">Boolean</span></span>|<span data-ttu-id="9810f-195">Соответствует параметру "включить скрытый режим".</span><span class="sxs-lookup"><span data-stu-id="9810f-195">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="9810f-196">фиреваллаппликатионс</span><span class="sxs-lookup"><span data-stu-id="9810f-196">firewallApplications</span></span>|<span data-ttu-id="9810f-197">Коллекция [макосфиреваллаппликатион](../resources/intune-deviceconfig-macosfirewallapplication.md)</span><span class="sxs-lookup"><span data-stu-id="9810f-197">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="9810f-198">Список приложений с параметрами брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="9810f-198">List of applications with firewall settings.</span></span> <span data-ttu-id="9810f-199">Параметры брандмауэра для приложений, не включенных в этот список, определяются пользователем.</span><span class="sxs-lookup"><span data-stu-id="9810f-199">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="9810f-200">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="9810f-200">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9810f-201">филеваултенаблед</span><span class="sxs-lookup"><span data-stu-id="9810f-201">fileVaultEnabled</span></span>|<span data-ttu-id="9810f-202">Логический</span><span class="sxs-lookup"><span data-stu-id="9810f-202">Boolean</span></span>|<span data-ttu-id="9810f-203">Указывает, следует ли включить Филеваулт.</span><span class="sxs-lookup"><span data-stu-id="9810f-203">Whether FileVault should be enabled or not.</span></span>|
|<span data-ttu-id="9810f-204">филеваултселектедрековерикэйтипес</span><span class="sxs-lookup"><span data-stu-id="9810f-204">fileVaultSelectedRecoveryKeyTypes</span></span>|[<span data-ttu-id="9810f-205">macOSFileVaultRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="9810f-205">macOSFileVaultRecoveryKeyTypes</span></span>](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|<span data-ttu-id="9810f-206">Обязательно если включен Филеваулт, определяет типы ключа восстановления, которые необходимо использовать.</span><span class="sxs-lookup"><span data-stu-id="9810f-206">Required if FileVault is enabled, determines the type(s) of recovery key to use.</span></span> <span data-ttu-id="9810f-207">.</span><span class="sxs-lookup"><span data-stu-id="9810f-207">.</span></span> <span data-ttu-id="9810f-208">Возможные значения: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span><span class="sxs-lookup"><span data-stu-id="9810f-208">Possible values are: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span></span>|
|<span data-ttu-id="9810f-209">филеваултинститутионалрековерикэйцертификате</span><span class="sxs-lookup"><span data-stu-id="9810f-209">fileVaultInstitutionalRecoveryKeyCertificate</span></span>|<span data-ttu-id="9810f-210">Binary</span><span class="sxs-lookup"><span data-stu-id="9810f-210">Binary</span></span>|<span data-ttu-id="9810f-211">Обязательно, если выбранные типы ключей восстановления включают Институтионалрековерикэй.</span><span class="sxs-lookup"><span data-stu-id="9810f-211">Required if selected recovery key type(s) include InstitutionalRecoveryKey.</span></span> <span data-ttu-id="9810f-212">Файл сертификата в кодировке DER, который использовался для установки ключа восстановления в учреждений.</span><span class="sxs-lookup"><span data-stu-id="9810f-212">The DER Encoded certificate file used to set an institutional recovery key.</span></span>|
|<span data-ttu-id="9810f-213">филеваултинститутионалрековерикэйцертификатефиленаме</span><span class="sxs-lookup"><span data-stu-id="9810f-213">fileVaultInstitutionalRecoveryKeyCertificateFileName</span></span>|<span data-ttu-id="9810f-214">Строка</span><span class="sxs-lookup"><span data-stu-id="9810f-214">String</span></span>|<span data-ttu-id="9810f-215">Имя файла сертификата ключа восстановления для сотрудников, который будет отображаться в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="9810f-215">File name of the institutional recovery key certificate to display in UI.</span></span> <span data-ttu-id="9810f-216">(\*. der).</span><span class="sxs-lookup"><span data-stu-id="9810f-216">(\*.der).</span></span>|
|<span data-ttu-id="9810f-217">филеваултперсоналрековерикэйхелпмессаже</span><span class="sxs-lookup"><span data-stu-id="9810f-217">fileVaultPersonalRecoveryKeyHelpMessage</span></span>|<span data-ttu-id="9810f-218">Строка</span><span class="sxs-lookup"><span data-stu-id="9810f-218">String</span></span>|<span data-ttu-id="9810f-219">Обязательно, если выбранные типы ключей восстановления включают Персоналрековерикэй.</span><span class="sxs-lookup"><span data-stu-id="9810f-219">Required if selected recovery key type(s) include PersonalRecoveryKey.</span></span> <span data-ttu-id="9810f-220">Короткое сообщение, в котором показано, как получить свой ключ восстановления личных настроек.</span><span class="sxs-lookup"><span data-stu-id="9810f-220">A short message displayed to the user that explains how they can retrieve their personal recovery key.</span></span>|
|<span data-ttu-id="9810f-221">филеваулталловдеферралунтилсигнаут</span><span class="sxs-lookup"><span data-stu-id="9810f-221">fileVaultAllowDeferralUntilSignOut</span></span>|<span data-ttu-id="9810f-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="9810f-222">Boolean</span></span>|<span data-ttu-id="9810f-223">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9810f-223">Optional.</span></span> <span data-ttu-id="9810f-224">Если задано значение true, пользователь может отложить включение Филеваулт, пока не выйдете из системы.</span><span class="sxs-lookup"><span data-stu-id="9810f-224">If set to true, the user can defer the enabling of FileVault until they sign out.</span></span>|
|<span data-ttu-id="9810f-225">филеваултнумберофтимесусерканигноре</span><span class="sxs-lookup"><span data-stu-id="9810f-225">fileVaultNumberOfTimesUserCanIgnore</span></span>|<span data-ttu-id="9810f-226">Int32</span><span class="sxs-lookup"><span data-stu-id="9810f-226">Int32</span></span>|<span data-ttu-id="9810f-227">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="9810f-227">Optional.</span></span> <span data-ttu-id="9810f-228">При использовании параметра "отложить" это максимальное число раз, когда пользователь может игнорировать приглашения на включение Филеваулт, чтобы пользователь мог выполнить вход.</span><span class="sxs-lookup"><span data-stu-id="9810f-228">When using the Defer option, this is the maximum number of times the user can ignore prompts to enable FileVault before FileVault will be required for the user to sign in.</span></span> <span data-ttu-id="9810f-229">Если задано значение-1, всегда будет выдаваться запрос на включение Филеваулт, пока Филеваулт не будет включен, хотя разрешить пользователю обходить включение Филеваулт.</span><span class="sxs-lookup"><span data-stu-id="9810f-229">If set to -1, it will always prompt to enable FileVault until FileVault is enabled, though it will allow the user to bypass enabling FileVault.</span></span> <span data-ttu-id="9810f-230">Если задать для этого параметра значение 0, эта функция будет отключена.</span><span class="sxs-lookup"><span data-stu-id="9810f-230">Setting this to 0 will disable the feature.</span></span>|
|<span data-ttu-id="9810f-231">филеваултдисаблепромптатсигнаут</span><span class="sxs-lookup"><span data-stu-id="9810f-231">fileVaultDisablePromptAtSignOut</span></span>|<span data-ttu-id="9810f-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="9810f-232">Boolean</span></span>|<span data-ttu-id="9810f-233">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9810f-233">Optional.</span></span> <span data-ttu-id="9810f-234">При использовании параметра отсрочки, если задано значение true, пользователю не предлагается включить Филеваулт при входе.</span><span class="sxs-lookup"><span data-stu-id="9810f-234">When using the Defer option, if set to true, the user is not prompted to enable FileVault at sign-out.</span></span>|
|<span data-ttu-id="9810f-235">филеваултперсоналрековерикэйротатионинмонсс</span><span class="sxs-lookup"><span data-stu-id="9810f-235">fileVaultPersonalRecoveryKeyRotationInMonths</span></span>|<span data-ttu-id="9810f-236">Int32</span><span class="sxs-lookup"><span data-stu-id="9810f-236">Int32</span></span>|<span data-ttu-id="9810f-237">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="9810f-237">Optional.</span></span> <span data-ttu-id="9810f-238">Если выбранные типы ключей восстановления включают Персоналрековерикэй, частота вращения этого ключа в месяцах.</span><span class="sxs-lookup"><span data-stu-id="9810f-238">If selected recovery key type(s) include PersonalRecoveryKey, the frequency to rotate that key, in months.</span></span>|
|<span data-ttu-id="9810f-239">филеваулсидеперсоналрековерикэй</span><span class="sxs-lookup"><span data-stu-id="9810f-239">fileVaultHidePersonalRecoveryKey</span></span>|<span data-ttu-id="9810f-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="9810f-240">Boolean</span></span>|<span data-ttu-id="9810f-241">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9810f-241">Optional.</span></span> <span data-ttu-id="9810f-242">Скрытый персональный ключ восстановления не отображается на экране пользователя во время шифрования Филеваулт, что снижает риск его завершения в неправильной руки.</span><span class="sxs-lookup"><span data-stu-id="9810f-242">A hidden personal recovery key does not appear on the user's screen during FileVault encryption, reducing the risk of it ending up in the wrong hands.</span></span>|
|<span data-ttu-id="9810f-243">адванцедсреатпротектионреалтиме</span><span class="sxs-lookup"><span data-stu-id="9810f-243">advancedThreatProtectionRealTime</span></span>|[<span data-ttu-id="9810f-244">Включение</span><span class="sxs-lookup"><span data-stu-id="9810f-244">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9810f-245">Определяет, следует ли включить защиту в режиме реального времени для функции Advanced Threat Protection для защитника Майкрософт в macOS.</span><span class="sxs-lookup"><span data-stu-id="9810f-245">Determines whether or not to enable real-time protection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="9810f-246">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9810f-246">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9810f-247">адванцедсреатпротектионклаудделиверед</span><span class="sxs-lookup"><span data-stu-id="9810f-247">advancedThreatProtectionCloudDelivered</span></span>|[<span data-ttu-id="9810f-248">Включение</span><span class="sxs-lookup"><span data-stu-id="9810f-248">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9810f-249">Определяет, следует ли включить защиту от облачной защиты для Advanced Threat Protection в защитнике Майкрософт для macOS.</span><span class="sxs-lookup"><span data-stu-id="9810f-249">Determines whether or not to enable cloud-delivered protection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="9810f-250">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9810f-250">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9810f-251">адванцедсреатпротектионаутоматиксамплесубмиссион</span><span class="sxs-lookup"><span data-stu-id="9810f-251">advancedThreatProtectionAutomaticSampleSubmission</span></span>|[<span data-ttu-id="9810f-252">Включение</span><span class="sxs-lookup"><span data-stu-id="9810f-252">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9810f-253">Определяет, следует ли включать автоматическую отправку образца файлов для Advanced Threat Protection в защитнике Майкрософт в macOS.</span><span class="sxs-lookup"><span data-stu-id="9810f-253">Determines whether or not to enable automatic file sample submission for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="9810f-254">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9810f-254">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9810f-255">адванцедсреатпротектиондиагностикдатаколлектион</span><span class="sxs-lookup"><span data-stu-id="9810f-255">advancedThreatProtectionDiagnosticDataCollection</span></span>|[<span data-ttu-id="9810f-256">Включение</span><span class="sxs-lookup"><span data-stu-id="9810f-256">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9810f-257">Определяет, следует ли включить сбор данных диагностики и использования для Advanced Threat Protection для защитника Майкрософт в macOS.</span><span class="sxs-lookup"><span data-stu-id="9810f-257">Determines whether or not to enable diagnostic and usage data collection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="9810f-258">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9810f-258">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9810f-259">адванцедсреатпротектионексклудедфолдерс</span><span class="sxs-lookup"><span data-stu-id="9810f-259">advancedThreatProtectionExcludedFolders</span></span>|<span data-ttu-id="9810f-260">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9810f-260">String collection</span></span>|<span data-ttu-id="9810f-261">Список путей к папкам, которые необходимо исключить из антивирусной проверки для Advanced Threat protection защитника Майкрософт в macOS.</span><span class="sxs-lookup"><span data-stu-id="9810f-261">A list of paths to folders to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="9810f-262">адванцедсреатпротектионексклудедфилес</span><span class="sxs-lookup"><span data-stu-id="9810f-262">advancedThreatProtectionExcludedFiles</span></span>|<span data-ttu-id="9810f-263">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9810f-263">String collection</span></span>|<span data-ttu-id="9810f-264">Список путей к файлам, которые необходимо исключить из антивирусной проверки для Advanced Threat Protection в macOS.</span><span class="sxs-lookup"><span data-stu-id="9810f-264">A list of paths to files to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="9810f-265">адванцедсреатпротектионексклудедекстенсионс</span><span class="sxs-lookup"><span data-stu-id="9810f-265">advancedThreatProtectionExcludedExtensions</span></span>|<span data-ttu-id="9810f-266">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9810f-266">String collection</span></span>|<span data-ttu-id="9810f-267">Список расширений файлов, которые необходимо исключить из антивирусного сканирования для Advanced Threat Protection в macOS.</span><span class="sxs-lookup"><span data-stu-id="9810f-267">A list of file extensions to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="9810f-268">адванцедсреатпротектионексклудедпроцессес</span><span class="sxs-lookup"><span data-stu-id="9810f-268">advancedThreatProtectionExcludedProcesses</span></span>|<span data-ttu-id="9810f-269">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9810f-269">String collection</span></span>|<span data-ttu-id="9810f-270">Список имен процессов, которые необходимо исключить из антивирусной проверки для Advanced Threat Protection в macOS.</span><span class="sxs-lookup"><span data-stu-id="9810f-270">A list of process names to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|



## <a name="response"></a><span data-ttu-id="9810f-271">Ответ</span><span class="sxs-lookup"><span data-stu-id="9810f-271">Response</span></span>
<span data-ttu-id="9810f-272">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9810f-272">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9810f-273">Пример</span><span class="sxs-lookup"><span data-stu-id="9810f-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="9810f-274">Запрос</span><span class="sxs-lookup"><span data-stu-id="9810f-274">Request</span></span>
<span data-ttu-id="9810f-275">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9810f-275">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9810f-276">Отклик</span><span class="sxs-lookup"><span data-stu-id="9810f-276">Response</span></span>
<span data-ttu-id="9810f-p128">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9810f-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





