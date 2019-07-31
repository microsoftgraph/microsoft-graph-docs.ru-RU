---
title: Создание Макосендпоинтпротектионконфигуратион
description: Создание нового объекта Макосендпоинтпротектионконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 01ae2365d0b86b185dc28a87b082a8058d927ea9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35947370"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="8a8f2-103">Создание Макосендпоинтпротектионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8a8f2-103">Create macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="8a8f2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a8f2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a8f2-106">Создание нового объекта [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8a8f2-106">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a8f2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8a8f2-107">Prerequisites</span></span>
<span data-ttu-id="8a8f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a8f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a8f2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a8f2-110">Permission type</span></span>|<span data-ttu-id="8a8f2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a8f2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a8f2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a8f2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8a8f2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a8f2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8a8f2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a8f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a8f2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-115">Not supported.</span></span>|
|<span data-ttu-id="8a8f2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a8f2-116">Application</span></span>|<span data-ttu-id="8a8f2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a8f2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a8f2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8a8f2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a8f2-119">Request headers</span></span>
|<span data-ttu-id="8a8f2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8a8f2-120">Header</span></span>|<span data-ttu-id="8a8f2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8a8f2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a8f2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a8f2-122">Authorization</span></span>|<span data-ttu-id="8a8f2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a8f2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8a8f2-124">Accept</span></span>|<span data-ttu-id="8a8f2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8a8f2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a8f2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8a8f2-126">Request body</span></span>
<span data-ttu-id="8a8f2-127">В тексте запроса добавьте представление объекта Макосендпоинтпротектионконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-127">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="8a8f2-128">В следующей таблице приведены свойства, необходимые при создании Макосендпоинтпротектионконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-128">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="8a8f2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a8f2-129">Property</span></span>|<span data-ttu-id="8a8f2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8a8f2-130">Type</span></span>|<span data-ttu-id="8a8f2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8a8f2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a8f2-132">id</span><span class="sxs-lookup"><span data-stu-id="8a8f2-132">id</span></span>|<span data-ttu-id="8a8f2-133">String</span><span class="sxs-lookup"><span data-stu-id="8a8f2-133">String</span></span>|<span data-ttu-id="8a8f2-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-134">Key of the entity.</span></span> <span data-ttu-id="8a8f2-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8a8f2-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a8f2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a8f2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8a8f2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a8f2-137">DateTimeOffset</span></span>|<span data-ttu-id="8a8f2-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8a8f2-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8a8f2-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a8f2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8a8f2-140">roleScopeTagIds</span></span>|<span data-ttu-id="8a8f2-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8a8f2-141">String collection</span></span>|<span data-ttu-id="8a8f2-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8a8f2-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8a8f2-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a8f2-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="8a8f2-144">supportsScopeTags</span></span>|<span data-ttu-id="8a8f2-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a8f2-145">Boolean</span></span>|<span data-ttu-id="8a8f2-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8a8f2-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8a8f2-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8a8f2-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-149">This property is read-only.</span></span> <span data-ttu-id="8a8f2-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8a8f2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a8f2-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8a8f2-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8a8f2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8a8f2-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8a8f2-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8a8f2-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8a8f2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a8f2-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8a8f2-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8a8f2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8a8f2-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8a8f2-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8a8f2-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8a8f2-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a8f2-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="8a8f2-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8a8f2-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="8a8f2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8a8f2-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8a8f2-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8a8f2-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a8f2-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a8f2-163">createdDateTime</span></span>|<span data-ttu-id="8a8f2-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a8f2-164">DateTimeOffset</span></span>|<span data-ttu-id="8a8f2-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-165">DateTime the object was created.</span></span> <span data-ttu-id="8a8f2-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8a8f2-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a8f2-167">description</span><span class="sxs-lookup"><span data-stu-id="8a8f2-167">description</span></span>|<span data-ttu-id="8a8f2-168">String</span><span class="sxs-lookup"><span data-stu-id="8a8f2-168">String</span></span>|<span data-ttu-id="8a8f2-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8a8f2-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8a8f2-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a8f2-171">displayName</span><span class="sxs-lookup"><span data-stu-id="8a8f2-171">displayName</span></span>|<span data-ttu-id="8a8f2-172">Строка</span><span class="sxs-lookup"><span data-stu-id="8a8f2-172">String</span></span>|<span data-ttu-id="8a8f2-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8a8f2-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8a8f2-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a8f2-175">version</span><span class="sxs-lookup"><span data-stu-id="8a8f2-175">version</span></span>|<span data-ttu-id="8a8f2-176">Int32</span><span class="sxs-lookup"><span data-stu-id="8a8f2-176">Int32</span></span>|<span data-ttu-id="8a8f2-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-177">Version of the device configuration.</span></span> <span data-ttu-id="8a8f2-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8a8f2-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a8f2-179">Гатекипералловедаппсаурце</span><span class="sxs-lookup"><span data-stu-id="8a8f2-179">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="8a8f2-180">Макосгатекипераппсаурцес</span><span class="sxs-lookup"><span data-stu-id="8a8f2-180">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="8a8f2-181">Параметры системы и конфиденциальности, которые определяют, какие расположения скачивания приложения можно запускать с устройства macOS.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-181">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="8a8f2-182">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-182">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="8a8f2-183">Гатекиперблокковерриде</span><span class="sxs-lookup"><span data-stu-id="8a8f2-183">gatekeeperBlockOverride</span></span>|<span data-ttu-id="8a8f2-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a8f2-184">Boolean</span></span>|<span data-ttu-id="8a8f2-185">Если задано значение true, переопределение пользователя для привратника будет отключено.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-185">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="8a8f2-186">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="8a8f2-186">firewallEnabled</span></span>|<span data-ttu-id="8a8f2-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a8f2-187">Boolean</span></span>|<span data-ttu-id="8a8f2-188">Указывает, следует ли включить брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-188">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="8a8f2-189">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="8a8f2-189">firewallBlockAllIncoming</span></span>|<span data-ttu-id="8a8f2-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a8f2-190">Boolean</span></span>|<span data-ttu-id="8a8f2-191">Соответствует параметру "блокировать все входящие подключения".</span><span class="sxs-lookup"><span data-stu-id="8a8f2-191">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="8a8f2-192">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="8a8f2-192">firewallEnableStealthMode</span></span>|<span data-ttu-id="8a8f2-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a8f2-193">Boolean</span></span>|<span data-ttu-id="8a8f2-194">Соответствует параметру "включить скрытый режим".</span><span class="sxs-lookup"><span data-stu-id="8a8f2-194">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="8a8f2-195">Фиреваллаппликатионс</span><span class="sxs-lookup"><span data-stu-id="8a8f2-195">firewallApplications</span></span>|<span data-ttu-id="8a8f2-196">Коллекция [макосфиреваллаппликатион](../resources/intune-deviceconfig-macosfirewallapplication.md)</span><span class="sxs-lookup"><span data-stu-id="8a8f2-196">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="8a8f2-197">Список приложений с параметрами брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-197">List of applications with firewall settings.</span></span> <span data-ttu-id="8a8f2-198">Параметры брандмауэра для приложений, не включенных в этот список, определяются пользователем.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-198">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="8a8f2-199">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-199">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8a8f2-200">Филеваултенаблед</span><span class="sxs-lookup"><span data-stu-id="8a8f2-200">fileVaultEnabled</span></span>|<span data-ttu-id="8a8f2-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a8f2-201">Boolean</span></span>|<span data-ttu-id="8a8f2-202">Указывает, следует ли включить Филеваулт.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-202">Whether FileVault should be enabled or not.</span></span>|
|<span data-ttu-id="8a8f2-203">Филеваултселектедрековерикэйтипес</span><span class="sxs-lookup"><span data-stu-id="8a8f2-203">fileVaultSelectedRecoveryKeyTypes</span></span>|[<span data-ttu-id="8a8f2-204">Макосфилеваултрековерикэйтипес</span><span class="sxs-lookup"><span data-stu-id="8a8f2-204">macOSFileVaultRecoveryKeyTypes</span></span>](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|<span data-ttu-id="8a8f2-205">Обязательно если включен Филеваулт, определяет типы ключа восстановления, которые необходимо использовать.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-205">Required if FileVault is enabled, determines the type(s) of recovery key to use.</span></span> <span data-ttu-id="8a8f2-206">.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-206"></span></span> <span data-ttu-id="8a8f2-207">Возможные значения: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-207">Possible values are: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span></span>|
|<span data-ttu-id="8a8f2-208">Филеваултинститутионалрековерикэйцертификате</span><span class="sxs-lookup"><span data-stu-id="8a8f2-208">fileVaultInstitutionalRecoveryKeyCertificate</span></span>|<span data-ttu-id="8a8f2-209">Binary</span><span class="sxs-lookup"><span data-stu-id="8a8f2-209">Binary</span></span>|<span data-ttu-id="8a8f2-210">Обязательно, если выбранные типы ключей восстановления включают Институтионалрековерикэй.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-210">Required if selected recovery key type(s) include InstitutionalRecoveryKey.</span></span> <span data-ttu-id="8a8f2-211">Файл сертификата в кодировке DER, который использовался для установки ключа восстановления в учреждений.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-211">The DER Encoded certificate file used to set an institutional recovery key.</span></span>|
|<span data-ttu-id="8a8f2-212">Филеваултинститутионалрековерикэйцертификатефиленаме</span><span class="sxs-lookup"><span data-stu-id="8a8f2-212">fileVaultInstitutionalRecoveryKeyCertificateFileName</span></span>|<span data-ttu-id="8a8f2-213">String</span><span class="sxs-lookup"><span data-stu-id="8a8f2-213">String</span></span>|<span data-ttu-id="8a8f2-214">Имя файла сертификата ключа восстановления для сотрудников, который будет отображаться в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-214">File name of the institutional recovery key certificate to display in UI.</span></span> <span data-ttu-id="8a8f2-215">(\*. der).</span><span class="sxs-lookup"><span data-stu-id="8a8f2-215">(\*.der).</span></span>|
|<span data-ttu-id="8a8f2-216">Филеваултперсоналрековерикэйхелпмессаже</span><span class="sxs-lookup"><span data-stu-id="8a8f2-216">fileVaultPersonalRecoveryKeyHelpMessage</span></span>|<span data-ttu-id="8a8f2-217">String</span><span class="sxs-lookup"><span data-stu-id="8a8f2-217">String</span></span>|<span data-ttu-id="8a8f2-218">Обязательно, если выбранные типы ключей восстановления включают Персоналрековерикэй.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-218">Required if selected recovery key type(s) include PersonalRecoveryKey.</span></span> <span data-ttu-id="8a8f2-219">Короткое сообщение, в котором показано, как получить свой ключ восстановления личных настроек.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-219">A short message displayed to the user that explains how they can retrieve their personal recovery key.</span></span>|
|<span data-ttu-id="8a8f2-220">Филеваулталловдеферралунтилсигнаут</span><span class="sxs-lookup"><span data-stu-id="8a8f2-220">fileVaultAllowDeferralUntilSignOut</span></span>|<span data-ttu-id="8a8f2-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a8f2-221">Boolean</span></span>|<span data-ttu-id="8a8f2-222">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-222">Optional.</span></span> <span data-ttu-id="8a8f2-223">Если задано значение true, пользователь может отложить включение Филеваулт, пока не выйдете из системы.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-223">If set to true, the user can defer the enabling of FileVault until they sign out.</span></span>|
|<span data-ttu-id="8a8f2-224">Филеваултнумберофтимесусерканигноре</span><span class="sxs-lookup"><span data-stu-id="8a8f2-224">fileVaultNumberOfTimesUserCanIgnore</span></span>|<span data-ttu-id="8a8f2-225">Int32</span><span class="sxs-lookup"><span data-stu-id="8a8f2-225">Int32</span></span>|<span data-ttu-id="8a8f2-226">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-226">Optional.</span></span> <span data-ttu-id="8a8f2-227">При использовании параметра "отложить" это максимальное число раз, когда пользователь может игнорировать приглашения на включение Филеваулт, чтобы пользователь мог выполнить вход.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-227">When using the Defer option, this is the maximum number of times the user can ignore prompts to enable FileVault before FileVault will be required for the user to sign in.</span></span> <span data-ttu-id="8a8f2-228">Если задано значение-1, всегда будет выдаваться запрос на включение Филеваулт, пока Филеваулт не будет включен, хотя разрешить пользователю обходить включение Филеваулт.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-228">If set to -1, it will always prompt to enable FileVault until FileVault is enabled, though it will allow the user to bypass enabling FileVault.</span></span> <span data-ttu-id="8a8f2-229">Если задать для этого параметра значение 0, эта функция будет отключена.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-229">Setting this to 0 will disable the feature.</span></span>|
|<span data-ttu-id="8a8f2-230">Филеваултдисаблепромптатсигнаут</span><span class="sxs-lookup"><span data-stu-id="8a8f2-230">fileVaultDisablePromptAtSignOut</span></span>|<span data-ttu-id="8a8f2-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a8f2-231">Boolean</span></span>|<span data-ttu-id="8a8f2-232">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-232">Optional.</span></span> <span data-ttu-id="8a8f2-233">При использовании параметра отсрочки, если задано значение true, пользователю не предлагается включить Филеваулт при входе.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-233">When using the Defer option, if set to true, the user is not prompted to enable FileVault at sign-out.</span></span>|
|<span data-ttu-id="8a8f2-234">Филеваултперсоналрековерикэйротатионинмонсс</span><span class="sxs-lookup"><span data-stu-id="8a8f2-234">fileVaultPersonalRecoveryKeyRotationInMonths</span></span>|<span data-ttu-id="8a8f2-235">Int32</span><span class="sxs-lookup"><span data-stu-id="8a8f2-235">Int32</span></span>|<span data-ttu-id="8a8f2-236">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-236">Optional.</span></span> <span data-ttu-id="8a8f2-237">Если выбранные типы ключей восстановления включают Персоналрековерикэй, частота вращения этого ключа в месяцах.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-237">If selected recovery key type(s) include PersonalRecoveryKey, the frequency to rotate that key, in months.</span></span>|



## <a name="response"></a><span data-ttu-id="8a8f2-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a8f2-238">Response</span></span>
<span data-ttu-id="8a8f2-239">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-239">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a8f2-240">Пример</span><span class="sxs-lookup"><span data-stu-id="8a8f2-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a8f2-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a8f2-241">Request</span></span>
<span data-ttu-id="8a8f2-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-242">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8a8f2-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a8f2-243">Response</span></span>
<span data-ttu-id="8a8f2-p123">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a8f2-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





