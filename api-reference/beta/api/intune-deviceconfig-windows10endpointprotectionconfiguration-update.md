---
title: Обновление объекта windows10EndpointProtectionConfiguration
description: Обновляет свойства объекта windows10EndpointProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bb2f2544863272aee3c37bba78c1e95237e75ac5
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533209"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="99cd5-103">Обновление объекта windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="99cd5-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="99cd5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99cd5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99cd5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99cd5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99cd5-106">Обновляет свойства объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99cd5-106">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99cd5-107">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="99cd5-107">Prerequisites</span></span>
<span data-ttu-id="99cd5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99cd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99cd5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99cd5-110">Permission type</span></span>|<span data-ttu-id="99cd5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="99cd5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99cd5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99cd5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="99cd5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99cd5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="99cd5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99cd5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99cd5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99cd5-115">Not supported.</span></span>|
|<span data-ttu-id="99cd5-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="99cd5-116">Application</span></span>|<span data-ttu-id="99cd5-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99cd5-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99cd5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99cd5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="99cd5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99cd5-119">Request headers</span></span>
|<span data-ttu-id="99cd5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="99cd5-120">Header</span></span>|<span data-ttu-id="99cd5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="99cd5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99cd5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99cd5-122">Authorization</span></span>|<span data-ttu-id="99cd5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99cd5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99cd5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="99cd5-124">Accept</span></span>|<span data-ttu-id="99cd5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="99cd5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99cd5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99cd5-126">Request body</span></span>
<span data-ttu-id="99cd5-127">В теле запроса добавьте представление объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99cd5-127">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="99cd5-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99cd5-128">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="99cd5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="99cd5-129">Property</span></span>|<span data-ttu-id="99cd5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="99cd5-130">Type</span></span>|<span data-ttu-id="99cd5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="99cd5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99cd5-132">id</span><span class="sxs-lookup"><span data-stu-id="99cd5-132">id</span></span>|<span data-ttu-id="99cd5-133">String</span><span class="sxs-lookup"><span data-stu-id="99cd5-133">String</span></span>|<span data-ttu-id="99cd5-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="99cd5-134">Key of the entity.</span></span> <span data-ttu-id="99cd5-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99cd5-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99cd5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99cd5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="99cd5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99cd5-137">DateTimeOffset</span></span>|<span data-ttu-id="99cd5-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="99cd5-138">DateTime the object was last modified.</span></span> <span data-ttu-id="99cd5-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99cd5-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99cd5-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="99cd5-140">roleScopeTagIds</span></span>|<span data-ttu-id="99cd5-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="99cd5-141">String collection</span></span>|<span data-ttu-id="99cd5-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="99cd5-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="99cd5-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99cd5-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99cd5-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="99cd5-144">supportsScopeTags</span></span>|<span data-ttu-id="99cd5-145">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-145">Boolean</span></span>|<span data-ttu-id="99cd5-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="99cd5-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="99cd5-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="99cd5-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="99cd5-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="99cd5-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="99cd5-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="99cd5-149">This property is read-only.</span></span> <span data-ttu-id="99cd5-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99cd5-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99cd5-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="99cd5-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="99cd5-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="99cd5-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="99cd5-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="99cd5-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="99cd5-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99cd5-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99cd5-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="99cd5-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="99cd5-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="99cd5-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="99cd5-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="99cd5-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="99cd5-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99cd5-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99cd5-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="99cd5-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="99cd5-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="99cd5-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="99cd5-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="99cd5-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="99cd5-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99cd5-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99cd5-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99cd5-163">createdDateTime</span></span>|<span data-ttu-id="99cd5-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99cd5-164">DateTimeOffset</span></span>|<span data-ttu-id="99cd5-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="99cd5-165">DateTime the object was created.</span></span> <span data-ttu-id="99cd5-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99cd5-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99cd5-167">description</span><span class="sxs-lookup"><span data-stu-id="99cd5-167">description</span></span>|<span data-ttu-id="99cd5-168">String</span><span class="sxs-lookup"><span data-stu-id="99cd5-168">String</span></span>|<span data-ttu-id="99cd5-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="99cd5-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="99cd5-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99cd5-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99cd5-171">displayName</span><span class="sxs-lookup"><span data-stu-id="99cd5-171">displayName</span></span>|<span data-ttu-id="99cd5-172">Строка</span><span class="sxs-lookup"><span data-stu-id="99cd5-172">String</span></span>|<span data-ttu-id="99cd5-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="99cd5-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="99cd5-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99cd5-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99cd5-175">version</span><span class="sxs-lookup"><span data-stu-id="99cd5-175">version</span></span>|<span data-ttu-id="99cd5-176">Int32</span><span class="sxs-lookup"><span data-stu-id="99cd5-176">Int32</span></span>|<span data-ttu-id="99cd5-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="99cd5-177">Version of the device configuration.</span></span> <span data-ttu-id="99cd5-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99cd5-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99cd5-179">дмагуарддевицеенумератионполици</span><span class="sxs-lookup"><span data-stu-id="99cd5-179">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="99cd5-180">дмагуарддевицеенумератионполицитипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-180">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="99cd5-181">Эта политика предназначена для обеспечения дополнительной защиты от внешних устройств с поддержкой прямого доступа к памяти.</span><span class="sxs-lookup"><span data-stu-id="99cd5-181">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="99cd5-182">Он обеспечивает более полный контроль над перечислением устройств с поддержкой внешних устройств с поддержкой прямого доступа к памяти, несовместимых с пересопоставлением и изоляцией памяти устройств и изолированной средой.</span><span class="sxs-lookup"><span data-stu-id="99cd5-182">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="99cd5-183">Эта политика вступает в силу только тогда, когда система защиты DMA поддерживается и включена встроенным встроенным по.</span><span class="sxs-lookup"><span data-stu-id="99cd5-183">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="99cd5-184">Защита от DMA ядра — это компонент платформы, который невозможно контролировать с помощью политики или конечным пользователем.</span><span class="sxs-lookup"><span data-stu-id="99cd5-184">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="99cd5-185">Она должна поддерживаться системой на момент производства.</span><span class="sxs-lookup"><span data-stu-id="99cd5-185">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="99cd5-186">Чтобы проверить, поддерживает ли система защиту DMA, проверьте поле Защита ядра DMA на странице Сводка объекта MSINFO32. exe.</span><span class="sxs-lookup"><span data-stu-id="99cd5-186">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="99cd5-187">Возможные значения: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-187">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="99cd5-188">фиреваллрулес</span><span class="sxs-lookup"><span data-stu-id="99cd5-188">firewallRules</span></span>|<span data-ttu-id="99cd5-189">Коллекция [виндовсфиреваллруле](../resources/intune-deviceconfig-windowsfirewallrule.md)</span><span class="sxs-lookup"><span data-stu-id="99cd5-189">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="99cd5-190">Настраивает параметры правила брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="99cd5-190">Configures the firewall rule settings.</span></span> <span data-ttu-id="99cd5-191">Эта коллекция может содержать не более 150 элементов.</span><span class="sxs-lookup"><span data-stu-id="99cd5-191">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="99cd5-192">усерригхтсакцесскредентиалманажераструстедкаллер</span><span class="sxs-lookup"><span data-stu-id="99cd5-192">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="99cd5-193">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-193">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-194">Это право пользователя используется диспетчером учетных данных во время резервного копирования и восстановления.</span><span class="sxs-lookup"><span data-stu-id="99cd5-194">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="99cd5-195">Сохраненные учетные данные пользователей могут быть скомпрометированы, если эта привилегия передана другим субъектам.</span><span class="sxs-lookup"><span data-stu-id="99cd5-195">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="99cd5-196">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-196">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="99cd5-197">усерригхтсалловакцессфромнетворк</span><span class="sxs-lookup"><span data-stu-id="99cd5-197">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="99cd5-198">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-198">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-199">Это право пользователя определяет, какие пользователи и группы могут подключаться к компьютеру через сеть.</span><span class="sxs-lookup"><span data-stu-id="99cd5-199">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="99cd5-200">Допустимое состояние — Supported.</span><span class="sxs-lookup"><span data-stu-id="99cd5-200">State Allowed is supported.</span></span>|
|<span data-ttu-id="99cd5-201">усерригхтсблоккакцессфромнетворк</span><span class="sxs-lookup"><span data-stu-id="99cd5-201">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="99cd5-202">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-202">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-203">Это право пользователя определяет, каким пользователям и группам запрещается подключаться к компьютеру через сеть.</span><span class="sxs-lookup"><span data-stu-id="99cd5-203">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="99cd5-204">Блок состояния поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99cd5-204">State Block is supported.</span></span>|
|<span data-ttu-id="99cd5-205">усерригхтсактаспартофсеоператингсистем</span><span class="sxs-lookup"><span data-stu-id="99cd5-205">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="99cd5-206">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-206">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-207">Это право пользователя позволяет процессу олицетворять любого пользователя без проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="99cd5-207">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="99cd5-208">Таким образом, процесс может получить доступ к тем же локальным ресурсам, что и пользователь.</span><span class="sxs-lookup"><span data-stu-id="99cd5-208">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="99cd5-209">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="99cd5-210">усерригхтслокаллогон</span><span class="sxs-lookup"><span data-stu-id="99cd5-210">userRightsLocalLogOn</span></span>|[<span data-ttu-id="99cd5-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-212">Это право пользователя определяет, какие пользователи могут входить на компьютер.</span><span class="sxs-lookup"><span data-stu-id="99cd5-212">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="99cd5-213">Допустимые состояния NotConfigured, Поддерживаемые</span><span class="sxs-lookup"><span data-stu-id="99cd5-213">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="99cd5-214">усерригхтсденилокаллогон</span><span class="sxs-lookup"><span data-stu-id="99cd5-214">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="99cd5-215">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-215">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-216">Это право пользователя определяет, какие пользователи не могут войти на компьютер.</span><span class="sxs-lookup"><span data-stu-id="99cd5-216">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="99cd5-217">Состояния NotConfigured, блокировки поддерживаются</span><span class="sxs-lookup"><span data-stu-id="99cd5-217">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="99cd5-218">усерригхтсбаккупдата</span><span class="sxs-lookup"><span data-stu-id="99cd5-218">userRightsBackupData</span></span>|[<span data-ttu-id="99cd5-219">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-219">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-220">Это право пользователя определяет, какие пользователи могут обходить разрешения для файлов, каталогов, реестра и других постоянных объектов при резервном копировании файлов и каталогов.</span><span class="sxs-lookup"><span data-stu-id="99cd5-220">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="99cd5-221">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-221">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="99cd5-222">усерригхтсчанжесистемтиме</span><span class="sxs-lookup"><span data-stu-id="99cd5-222">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="99cd5-223">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-223">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-224">Это право пользователя определяет, какие пользователи и группы могут изменять время и дату на внутреннем часовом компьютере.</span><span class="sxs-lookup"><span data-stu-id="99cd5-224">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="99cd5-225">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-225">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="99cd5-226">усерригхтскреатеглобалобжектс</span><span class="sxs-lookup"><span data-stu-id="99cd5-226">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="99cd5-227">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-227">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-228">Этот параметр безопасности определяет, могут ли пользователи создавать глобальные объекты, доступные для всех сеансов.</span><span class="sxs-lookup"><span data-stu-id="99cd5-228">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="99cd5-229">Пользователи, которые могут создавать глобальные объекты, могут повлиять на процессы, выполняемые в сеансах других пользователей, что может привести к сбою приложения или повреждению данных.</span><span class="sxs-lookup"><span data-stu-id="99cd5-229">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="99cd5-230">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="99cd5-231">усерригхтскреатепажефиле</span><span class="sxs-lookup"><span data-stu-id="99cd5-231">userRightsCreatePageFile</span></span>|[<span data-ttu-id="99cd5-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-233">Это право пользователя определяет, какие пользователи и группы могут вызывать внутренний API, чтобы создать и изменить размер файла подкачки.</span><span class="sxs-lookup"><span data-stu-id="99cd5-233">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="99cd5-234">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="99cd5-235">усерригхтскреатеперманентшаредобжектс</span><span class="sxs-lookup"><span data-stu-id="99cd5-235">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="99cd5-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-237">Это право пользователя определяет, какие учетные записи могут использоваться процессами для создания объекта каталога с помощью диспетчера объектов.</span><span class="sxs-lookup"><span data-stu-id="99cd5-237">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="99cd5-238">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-238">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="99cd5-239">усерригхтскреатесимболиклинкс</span><span class="sxs-lookup"><span data-stu-id="99cd5-239">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="99cd5-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-241">Это право пользователя определяет, может ли пользователь создать символическую ссылку с компьютера, на который они входили.</span><span class="sxs-lookup"><span data-stu-id="99cd5-241">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="99cd5-242">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-242">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="99cd5-243">усерригхтскреатетокен</span><span class="sxs-lookup"><span data-stu-id="99cd5-243">userRightsCreateToken</span></span>|[<span data-ttu-id="99cd5-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-245">Это право пользователя определяет, какие пользователи и группы могут использоваться процессами для создания маркера, который можно использовать для получения доступа к любому локальному ресурсу, когда процесс использует внутренний API для создания маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="99cd5-245">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="99cd5-246">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-246">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="99cd5-247">усерригхтсдебугпрограмс</span><span class="sxs-lookup"><span data-stu-id="99cd5-247">userRightsDebugPrograms</span></span>|[<span data-ttu-id="99cd5-248">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-248">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-249">Это право пользователя определяет, какие пользователи могут прикреплять отладчик к любому процессу или ядру.</span><span class="sxs-lookup"><span data-stu-id="99cd5-249">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="99cd5-250">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-250">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="99cd5-251">усерригхтсремотедесктопсервицеслогон</span><span class="sxs-lookup"><span data-stu-id="99cd5-251">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="99cd5-252">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-252">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-253">Это право пользователя определяет, каким пользователям и группам запрещается вход в систему в качестве клиента служб удаленных рабочих столов.</span><span class="sxs-lookup"><span data-stu-id="99cd5-253">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="99cd5-254">Поддерживаются только состояния NotConfigured и Block</span><span class="sxs-lookup"><span data-stu-id="99cd5-254">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="99cd5-255">усерригхтсделегатион</span><span class="sxs-lookup"><span data-stu-id="99cd5-255">userRightsDelegation</span></span>|[<span data-ttu-id="99cd5-256">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-256">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-257">Это право пользователя определяет, какие пользователи могут устанавливать параметр "доверять для делегирования" для объекта пользователя или компьютера.</span><span class="sxs-lookup"><span data-stu-id="99cd5-257">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="99cd5-258">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-258">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="99cd5-259">усерригхтсженератесекуритяудитс</span><span class="sxs-lookup"><span data-stu-id="99cd5-259">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="99cd5-260">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-260">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-261">Это право пользователя определяет, какие учетные записи могут использоваться процессом для добавления записей в журнал безопасности.</span><span class="sxs-lookup"><span data-stu-id="99cd5-261">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="99cd5-262">Журнал безопасности используется для трассировки несанкционированного доступа к системе.</span><span class="sxs-lookup"><span data-stu-id="99cd5-262">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="99cd5-263">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-263">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="99cd5-264">усерригхтсимперсонатеклиент</span><span class="sxs-lookup"><span data-stu-id="99cd5-264">userRightsImpersonateClient</span></span>|[<span data-ttu-id="99cd5-265">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-265">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-266">Назначение этого права пользователю позволяет программам, выполняемым от имени этого пользователя, олицетворять клиента.</span><span class="sxs-lookup"><span data-stu-id="99cd5-266">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="99cd5-267">Требование этого пользователя для такого рода олицетворения запрещает несанкционированному пользователю подключаться к созданной им службе, а затем олицетворять этого клиента, что может повысить уровень разрешений неавторизованного пользователя до Уровни администрирования или системы.</span><span class="sxs-lookup"><span data-stu-id="99cd5-267">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="99cd5-268">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="99cd5-269">усерригхтсинкреасесчедулингприорити</span><span class="sxs-lookup"><span data-stu-id="99cd5-269">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="99cd5-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-271">Это право пользователя определяет, какие учетные записи могут использовать процесс с доступом к свойствам Write для другого процесса, чтобы увеличить приоритет выполнения, назначенный другому процессу.</span><span class="sxs-lookup"><span data-stu-id="99cd5-271">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="99cd5-272">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="99cd5-273">усерригхтслоадунлоаддриверс</span><span class="sxs-lookup"><span data-stu-id="99cd5-273">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="99cd5-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-275">Это право пользователя определяет, какие пользователи могут динамически загружать и выгружать драйверы устройств или другой код в режиме ядра.</span><span class="sxs-lookup"><span data-stu-id="99cd5-275">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="99cd5-276">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="99cd5-277">усерригхтслоккмемори</span><span class="sxs-lookup"><span data-stu-id="99cd5-277">userRightsLockMemory</span></span>|[<span data-ttu-id="99cd5-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-279">Это право пользователя определяет, какие учетные записи могут использовать процесс для хранения данных в физической памяти, что предотвращает их разбиение данных на виртуальную память на диске.</span><span class="sxs-lookup"><span data-stu-id="99cd5-279">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="99cd5-280">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="99cd5-281">усерригхтсманажеаудитингандсекуритилогс</span><span class="sxs-lookup"><span data-stu-id="99cd5-281">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="99cd5-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-283">Это право пользователя определяет, какие пользователи могут задавать параметры аудита доступа к объектам для отдельных ресурсов, таких как файлы, объекты Active Directory и разделы реестра.</span><span class="sxs-lookup"><span data-stu-id="99cd5-283">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="99cd5-284">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="99cd5-285">усерригхтсманажеволумес</span><span class="sxs-lookup"><span data-stu-id="99cd5-285">userRightsManageVolumes</span></span>|[<span data-ttu-id="99cd5-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-287">Это право пользователя определяет, какие пользователи и группы могут выполнять задачи обслуживания для тома, такие как удаленная дефрагментация.</span><span class="sxs-lookup"><span data-stu-id="99cd5-287">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="99cd5-288">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-288">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="99cd5-289">усерригхтсмодифифирмваринвиронмент</span><span class="sxs-lookup"><span data-stu-id="99cd5-289">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="99cd5-290">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-290">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-291">Это право пользователя определяет, кто может изменять значения в аппаратной среде.</span><span class="sxs-lookup"><span data-stu-id="99cd5-291">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="99cd5-292">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-292">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="99cd5-293">усерригхтсмодифйобжектлабелс</span><span class="sxs-lookup"><span data-stu-id="99cd5-293">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="99cd5-294">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-294">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-295">Это право пользователя определяет, какие учетные записи пользователей могут изменять метки целостности объектов, таких как файлы, разделы реестра или процессы, принадлежащие другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="99cd5-295">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="99cd5-296">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-296">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="99cd5-297">усерригхтспрофилесинглепроцесс</span><span class="sxs-lookup"><span data-stu-id="99cd5-297">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="99cd5-298">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-298">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-299">Это право пользователя определяет, какие пользователи могут использовать средства мониторинга производительности для наблюдения за производительностью системных процессов.</span><span class="sxs-lookup"><span data-stu-id="99cd5-299">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="99cd5-300">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-300">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="99cd5-301">усерригхтсремотешутдовн</span><span class="sxs-lookup"><span data-stu-id="99cd5-301">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="99cd5-302">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-302">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-303">Это право пользователя определяет, каким пользователям разрешено завершать работу компьютера из удаленного расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="99cd5-303">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="99cd5-304">Неправильное использование этого права пользователя может привести к отказу в обслуживании.</span><span class="sxs-lookup"><span data-stu-id="99cd5-304">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="99cd5-305">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-305">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="99cd5-306">усерригхтсресторедата</span><span class="sxs-lookup"><span data-stu-id="99cd5-306">userRightsRestoreData</span></span>|[<span data-ttu-id="99cd5-307">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-307">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-308">Это право пользователя определяет, какие пользователи могут обходить разрешения для файлов, каталогов, реестра и других постоянных объектов при восстановлении резервных копий файлов и каталогов, и определяет, какие пользователи могут устанавливать любой действительный субъект безопасности в качестве владельца объекта.</span><span class="sxs-lookup"><span data-stu-id="99cd5-308">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="99cd5-309">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-309">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="99cd5-310">усерригхтстакеовнершип</span><span class="sxs-lookup"><span data-stu-id="99cd5-310">userRightsTakeOwnership</span></span>|[<span data-ttu-id="99cd5-311">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="99cd5-311">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="99cd5-312">Это право пользователя определяет, какие пользователи могут становиться владельцами любого защищаемого объекта в системе, включая объекты Active Directory, файлы и папки, принтеры, разделы реестра, процессы и потоки.</span><span class="sxs-lookup"><span data-stu-id="99cd5-312">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="99cd5-313">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="99cd5-313">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="99cd5-314">ксбокссервицесенаблексбоксгамесаветаск</span><span class="sxs-lookup"><span data-stu-id="99cd5-314">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="99cd5-315">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-315">Boolean</span></span>|<span data-ttu-id="99cd5-316">Этот параметр определяет, включена ли функция сохранения игры Xbox (1) или отключена (0).</span><span class="sxs-lookup"><span data-stu-id="99cd5-316">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="99cd5-317">ксбокссервицесакцессориманажементсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="99cd5-317">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="99cd5-318">сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-318">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="99cd5-319">Этот параметр определяет, является ли тип запуска службы управления принадлежностью автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="99cd5-319">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="99cd5-320">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="99cd5-320">Default: Manual.</span></span> <span data-ttu-id="99cd5-321">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-321">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="99cd5-322">ксбокссервицесливеаусманажерсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="99cd5-322">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="99cd5-323">сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-323">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="99cd5-324">Этот параметр определяет, является ли тип запуска службы диспетчера Live auth автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="99cd5-324">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="99cd5-325">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="99cd5-325">Default: Manual.</span></span> <span data-ttu-id="99cd5-326">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-326">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="99cd5-327">ксбокссервицесливегамесавесервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="99cd5-327">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="99cd5-328">сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-328">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="99cd5-329">Этот параметр определяет, является ли тип запуска службы Live Save Service автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="99cd5-329">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="99cd5-330">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="99cd5-330">Default: Manual.</span></span> <span data-ttu-id="99cd5-331">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-331">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="99cd5-332">ксбокссервицесливенетворкингсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="99cd5-332">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="99cd5-333">сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-333">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="99cd5-334">Этот параметр определяет, является ли тип запуска сетевой службы автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="99cd5-334">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="99cd5-335">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="99cd5-335">Default: Manual.</span></span> <span data-ttu-id="99cd5-336">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-336">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="99cd5-337">локалсекуритйоптионсблоккмикрософтаккаунтс</span><span class="sxs-lookup"><span data-stu-id="99cd5-337">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="99cd5-338">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-338">Boolean</span></span>|<span data-ttu-id="99cd5-339">Запретить пользователям добавлять новые учетные записи Майкрософт на этот компьютер.</span><span class="sxs-lookup"><span data-stu-id="99cd5-339">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="99cd5-340">локалсекуритйоптионсблоккремотелогонвисбланкпассворд</span><span class="sxs-lookup"><span data-stu-id="99cd5-340">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="99cd5-341">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-341">Boolean</span></span>|<span data-ttu-id="99cd5-342">Включите локальные учетные записи, не защищенные паролем, для входа в систему из расположений, отличных от физического устройства. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="99cd5-342">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="99cd5-343">локалсекуритйоптионсдисаблеадминистратораккаунт</span><span class="sxs-lookup"><span data-stu-id="99cd5-343">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="99cd5-344">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-344">Boolean</span></span>|<span data-ttu-id="99cd5-345">Определяет, включена или отключена учетная запись локального администратора.</span><span class="sxs-lookup"><span data-stu-id="99cd5-345">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="99cd5-346">локалсекуритйоптионсадминистратораккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="99cd5-346">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="99cd5-347">String</span><span class="sxs-lookup"><span data-stu-id="99cd5-347">String</span></span>|<span data-ttu-id="99cd5-348">Определите имя другой учетной записи, которая будет связана с идентификатором безопасности (SID) учетной записи "Administrator".</span><span class="sxs-lookup"><span data-stu-id="99cd5-348">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="99cd5-349">локалсекуритйоптионсдисаблегуестаккаунт</span><span class="sxs-lookup"><span data-stu-id="99cd5-349">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="99cd5-350">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-350">Boolean</span></span>|<span data-ttu-id="99cd5-351">Определяет, включена или отключена Гостевая учетная запись.</span><span class="sxs-lookup"><span data-stu-id="99cd5-351">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="99cd5-352">локалсекуритйоптионсгуестаккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="99cd5-352">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="99cd5-353">String</span><span class="sxs-lookup"><span data-stu-id="99cd5-353">String</span></span>|<span data-ttu-id="99cd5-354">Определите имя другой учетной записи, которая будет связана с идентификатором безопасности (SID) для учетной записи "гость".</span><span class="sxs-lookup"><span data-stu-id="99cd5-354">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="99cd5-355">локалсекуритйоптионсалловундокквисаусавингтологон</span><span class="sxs-lookup"><span data-stu-id="99cd5-355">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="99cd5-356">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-356">Boolean</span></span>|<span data-ttu-id="99cd5-357">Запретите отстыковку портативного компьютера без необходимости входа в систему.</span><span class="sxs-lookup"><span data-stu-id="99cd5-357">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="99cd5-358">локалсекуритйоптионсблоккусерсинсталлингпринтердриверс</span><span class="sxs-lookup"><span data-stu-id="99cd5-358">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="99cd5-359">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-359">Boolean</span></span>|<span data-ttu-id="99cd5-360">Ограничьте установку драйверов принтеров в рамках подключения к общему принтеру только для администраторов.</span><span class="sxs-lookup"><span data-stu-id="99cd5-360">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="99cd5-361">локалсекуритйоптионсблоккремотеоптикалдривеакцесс</span><span class="sxs-lookup"><span data-stu-id="99cd5-361">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="99cd5-362">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-362">Boolean</span></span>|<span data-ttu-id="99cd5-363">Включение этого параметра позволяет интерактивно вошедший в систему пользователь получать доступ к устройству чтения компакт-дисков.</span><span class="sxs-lookup"><span data-stu-id="99cd5-363">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="99cd5-364">локалсекуритйоптионсформатандежектофремоваблемедиаалловедусер</span><span class="sxs-lookup"><span data-stu-id="99cd5-364">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="99cd5-365">локалсекуритйоптионсформатандежектофремоваблемедиаалловедусертипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="99cd5-366">Определите, кому разрешено форматировать и извлекать съемные носители NTFS.</span><span class="sxs-lookup"><span data-stu-id="99cd5-366">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="99cd5-367">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-367">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="99cd5-368">локалсекуритйоптионсмачинеинактивитилимит</span><span class="sxs-lookup"><span data-stu-id="99cd5-368">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="99cd5-369">Int32</span><span class="sxs-lookup"><span data-stu-id="99cd5-369">Int32</span></span>|<span data-ttu-id="99cd5-370">Определите максимальное количество минут отсутствия активности на экране входа интерактивного рабочего стола, пока не запустится экранная заставка.</span><span class="sxs-lookup"><span data-stu-id="99cd5-370">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="99cd5-371">Допустимые значения — от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="99cd5-371">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="99cd5-372">локалсекуритйоптионсмачинеинактивитилимитинминутес</span><span class="sxs-lookup"><span data-stu-id="99cd5-372">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="99cd5-373">Int32</span><span class="sxs-lookup"><span data-stu-id="99cd5-373">Int32</span></span>|<span data-ttu-id="99cd5-374">Определите максимальное количество минут отсутствия активности на экране входа интерактивного рабочего стола, пока не запустится экранная заставка.</span><span class="sxs-lookup"><span data-stu-id="99cd5-374">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="99cd5-375">Допустимые значения — от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="99cd5-375">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="99cd5-376">локалсекуритйоптионсдонотрекуиректрлалтдел</span><span class="sxs-lookup"><span data-stu-id="99cd5-376">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="99cd5-377">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-377">Boolean</span></span>|<span data-ttu-id="99cd5-378">Требовать нажатия клавиш CTRL + ALT + DEL, прежде чем пользователь сможет войти в систему.</span><span class="sxs-lookup"><span data-stu-id="99cd5-378">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="99cd5-379">локалсекуритйоптионшиделастсигнединусер</span><span class="sxs-lookup"><span data-stu-id="99cd5-379">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="99cd5-380">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-380">Boolean</span></span>|<span data-ttu-id="99cd5-381">Не отображать имя последнего пользователя, выполнившего вход на это устройство.</span><span class="sxs-lookup"><span data-stu-id="99cd5-381">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="99cd5-382">локалсекуритйоптионшидеусернамеатсигнин</span><span class="sxs-lookup"><span data-stu-id="99cd5-382">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="99cd5-383">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-383">Boolean</span></span>|<span data-ttu-id="99cd5-384">Не отображать имя пользователя, выполняющего вход на это устройство, после ввода учетных данных и отображения рабочего стола на устройстве.</span><span class="sxs-lookup"><span data-stu-id="99cd5-384">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="99cd5-385">локалсекуритйоптионслогонмессажетитле</span><span class="sxs-lookup"><span data-stu-id="99cd5-385">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="99cd5-386">String</span><span class="sxs-lookup"><span data-stu-id="99cd5-386">String</span></span>|<span data-ttu-id="99cd5-387">Задайте заголовок сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="99cd5-387">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="99cd5-388">локалсекуритйоптионслогонмессажетекст</span><span class="sxs-lookup"><span data-stu-id="99cd5-388">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="99cd5-389">String</span><span class="sxs-lookup"><span data-stu-id="99cd5-389">String</span></span>|<span data-ttu-id="99cd5-390">Задайте текст сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="99cd5-390">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="99cd5-391">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="99cd5-391">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="99cd5-392">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-392">Boolean</span></span>|<span data-ttu-id="99cd5-393">Блокировать запросы проверки подлинности PKU2U на этом устройстве для использования сетевых удостоверений.</span><span class="sxs-lookup"><span data-stu-id="99cd5-393">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="99cd5-394">локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажерхелпербул</span><span class="sxs-lookup"><span data-stu-id="99cd5-394">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="99cd5-395">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-395">Boolean</span></span>|<span data-ttu-id="99cd5-396">Помощник по пользовательскому интерфейсу Boolean для объекта Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажер</span><span class="sxs-lookup"><span data-stu-id="99cd5-396">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="99cd5-397">локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажер</span><span class="sxs-lookup"><span data-stu-id="99cd5-397">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="99cd5-398">String</span><span class="sxs-lookup"><span data-stu-id="99cd5-398">String</span></span>|<span data-ttu-id="99cd5-399">Измените строку языка определения дескрипторов безопасности по умолчанию, чтобы разрешить или запретить пользователям и группам совершать удаленные вызовы в SAM.</span><span class="sxs-lookup"><span data-stu-id="99cd5-399">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="99cd5-400">локалсекуритйоптионсминимумсессионсекуритифорнтлмсспбаседклиентс</span><span class="sxs-lookup"><span data-stu-id="99cd5-400">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="99cd5-401">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="99cd5-401">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="99cd5-402">Этот параметр безопасности позволяет клиенту требовать согласование 128-разрядного шифрования и/или сеанса защиты сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="99cd5-402">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="99cd5-403">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-403">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="99cd5-404">локалсекуритйоптионсминимумсессионсекуритифорнтлмсспбаседсерверс</span><span class="sxs-lookup"><span data-stu-id="99cd5-404">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="99cd5-405">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="99cd5-405">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="99cd5-406">Этот параметр безопасности позволяет серверу требовать согласование 128-разрядного шифрования и/или сеанса защиты сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="99cd5-406">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="99cd5-407">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-407">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="99cd5-408">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="99cd5-408">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="99cd5-409">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="99cd5-409">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="99cd5-410">Этот параметр безопасности определяет, какой протокол проверки подлинности "запрос/ответ" используется для входа в сеть.</span><span class="sxs-lookup"><span data-stu-id="99cd5-410">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="99cd5-411">Возможные значения: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-411">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="99cd5-412">ланманажерворкстатиондисаблеинсекурегуестлогонс</span><span class="sxs-lookup"><span data-stu-id="99cd5-412">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="99cd5-413">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-413">Boolean</span></span>|<span data-ttu-id="99cd5-414">Если этот параметр включен, клиент SMB будет разрешать небезопасные гостевые входы.</span><span class="sxs-lookup"><span data-stu-id="99cd5-414">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="99cd5-415">Если этот параметр не настроен, клиент SMB будет отклонять небезопасные гостевые входы.</span><span class="sxs-lookup"><span data-stu-id="99cd5-415">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="99cd5-416">локалсекуритйоптионсклеарвиртуалмеморипажефиле</span><span class="sxs-lookup"><span data-stu-id="99cd5-416">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="99cd5-417">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-417">Boolean</span></span>|<span data-ttu-id="99cd5-418">Этот параметр безопасности определяет, будет ли очищаться файл подкачки виртуальной памяти при завершении работы системы.</span><span class="sxs-lookup"><span data-stu-id="99cd5-418">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="99cd5-419">локалсекуритйоптионсалловсистемтобешутдовнвисаусавингтологон</span><span class="sxs-lookup"><span data-stu-id="99cd5-419">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="99cd5-420">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-420">Boolean</span></span>|<span data-ttu-id="99cd5-421">Этот параметр безопасности определяет, можно ли завершить работу компьютера, не выполняя вход в Windows.</span><span class="sxs-lookup"><span data-stu-id="99cd5-421">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="99cd5-422">локалсекуритйоптионсалловуиакцессаппликатионелеватион</span><span class="sxs-lookup"><span data-stu-id="99cd5-422">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="99cd5-423">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-423">Boolean</span></span>|<span data-ttu-id="99cd5-424">Разрешить UIAccess Apps запрос на повышение прав без использования безопасного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="99cd5-424">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="99cd5-425">локалсекуритйоптионсвиртуализефилеандрегистривритефаилурестоперусерлокатионс</span><span class="sxs-lookup"><span data-stu-id="99cd5-425">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="99cd5-426">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-426">Boolean</span></span>|<span data-ttu-id="99cd5-427">Виртуализация сбоев записи в файл и реестр для отдельных расположений пользователей</span><span class="sxs-lookup"><span data-stu-id="99cd5-427">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="99cd5-428">локалсекуритйоптионсонлелеватесигнедексекутаблес</span><span class="sxs-lookup"><span data-stu-id="99cd5-428">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="99cd5-429">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-429">Boolean</span></span>|<span data-ttu-id="99cd5-430">Принудительная проверка пути сертификации PKI для указанного исполняемого файла перед тем, как он будет разрешен для запуска.</span><span class="sxs-lookup"><span data-stu-id="99cd5-430">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="99cd5-431">локалсекуритйоптионсадминистраторелеватионпромптбехавиор</span><span class="sxs-lookup"><span data-stu-id="99cd5-431">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="99cd5-432">локалсекуритйоптионсадминистраторелеватионпромптбехавиортипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-432">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="99cd5-433">Определите поведение запросов на повышение прав для администраторов в режиме одобрения администратором.</span><span class="sxs-lookup"><span data-stu-id="99cd5-433">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="99cd5-434">Возможные значения: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-434">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="99cd5-435">локалсекуритйоптионсстандардусерелеватионпромптбехавиор</span><span class="sxs-lookup"><span data-stu-id="99cd5-435">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="99cd5-436">локалсекуритйоптионсстандардусерелеватионпромптбехавиортипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-436">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="99cd5-437">Определите поведение запросов на повышение прав для стандартных пользователей.</span><span class="sxs-lookup"><span data-stu-id="99cd5-437">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="99cd5-438">Возможные значения: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-438">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="99cd5-439">локалсекуритйоптионссвитчтосекуредесктопвхенпромптингфорелеватион</span><span class="sxs-lookup"><span data-stu-id="99cd5-439">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="99cd5-440">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-440">Boolean</span></span>|<span data-ttu-id="99cd5-441">Разрешить всем запросам на повышение прав доступ к рабочему столу интерактивного пользователя, а не к безопасному рабочему столу.</span><span class="sxs-lookup"><span data-stu-id="99cd5-441">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="99cd5-442">Используются параметры политики поведения запросов для администраторов и стандартных пользователей.</span><span class="sxs-lookup"><span data-stu-id="99cd5-442">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="99cd5-443">локалсекуритйоптионсдетектаппликатионинсталлатионсандпромптфорелеватион</span><span class="sxs-lookup"><span data-stu-id="99cd5-443">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="99cd5-444">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-444">Boolean</span></span>|<span data-ttu-id="99cd5-445">При установке приложений, требующих повышенных привилегий, запрашиваются учетные данные администратора. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="99cd5-445">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="99cd5-446">локалсекуритйоптионсалловуиакцессаппликатионсфорсекурелокатионс</span><span class="sxs-lookup"><span data-stu-id="99cd5-446">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="99cd5-447">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-447">Boolean</span></span>|<span data-ttu-id="99cd5-448">Разрешить UIAccess Apps запрос на повышение прав без использования безопасного рабочего стола. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="99cd5-448">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="99cd5-449">локалсекуритйоптионсусеадминаппровалмоде</span><span class="sxs-lookup"><span data-stu-id="99cd5-449">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="99cd5-450">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-450">Boolean</span></span>|<span data-ttu-id="99cd5-451">Определяет, использует ли встроенная учетная запись администратора режим одобрения администратором или выполняет все приложения с правами полного администратора. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="99cd5-451">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="99cd5-452">локалсекуритйоптионсусеадминаппровалмодефорадминистраторс</span><span class="sxs-lookup"><span data-stu-id="99cd5-452">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="99cd5-453">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-453">Boolean</span></span>|<span data-ttu-id="99cd5-454">Определить, включен ли режим одобрения администратором и все параметры политики контроля учетных записей, по умолчанию включено</span><span class="sxs-lookup"><span data-stu-id="99cd5-454">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="99cd5-455">локалсекуритйоптионсинформатионшовнонлоккскрин</span><span class="sxs-lookup"><span data-stu-id="99cd5-455">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="99cd5-456">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="99cd5-456">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="99cd5-457">Настройте сведения о пользователе, которые отображаются, когда сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="99cd5-457">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="99cd5-458">Если этот флажок не установлен, отображаются отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="99cd5-458">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="99cd5-459">Возможные значения: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-459">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="99cd5-460">локалсекуритйоптионсинформатиондисплайедонлоккскрин</span><span class="sxs-lookup"><span data-stu-id="99cd5-460">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="99cd5-461">локалсекуритйоптионсинформатиондисплайедонлоккскринтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-461">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="99cd5-462">Настройте сведения о пользователе, которые отображаются, когда сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="99cd5-462">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="99cd5-463">Если этот флажок не установлен, отображаются отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="99cd5-463">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="99cd5-464">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-464">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="99cd5-465">локалсекуритйоптионсдисаблеклиентдигиталлисигнкоммуникатионсифсерверагрис</span><span class="sxs-lookup"><span data-stu-id="99cd5-465">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="99cd5-466">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-466">Boolean</span></span>|<span data-ttu-id="99cd5-467">Этот параметр безопасности определяет, будет ли клиент SMB пытаться согласовать подписывание SMB пакетов.</span><span class="sxs-lookup"><span data-stu-id="99cd5-467">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="99cd5-468">локалсекуритйоптионсклиентдигиталлисигнкоммуникатионсалвайс</span><span class="sxs-lookup"><span data-stu-id="99cd5-468">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="99cd5-469">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-469">Boolean</span></span>|<span data-ttu-id="99cd5-470">Этот параметр безопасности определяет, требуется ли Подписывание пакетов для клиентского SMB-компонента.</span><span class="sxs-lookup"><span data-stu-id="99cd5-470">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="99cd5-471">локалсекуритйоптионсклиентсендуненкриптедпассвордтосирдпартисмбсерверс</span><span class="sxs-lookup"><span data-stu-id="99cd5-471">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="99cd5-472">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-472">Boolean</span></span>|<span data-ttu-id="99cd5-473">Если этот параметр безопасности включен, перенаправителем SMB (Server Message Block) разрешено отправлять пароли открытым текстом на серверы SMB сторонних производителей, не поддерживающие шифрование паролей во время проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="99cd5-473">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="99cd5-474">локалсекуритйоптионсдисаблесервердигиталлисигнкоммуникатионсалвайс</span><span class="sxs-lookup"><span data-stu-id="99cd5-474">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="99cd5-475">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-475">Boolean</span></span>|<span data-ttu-id="99cd5-476">Этот параметр безопасности определяет, требуется ли подписи пакетов для SMB-компонентов сервера.</span><span class="sxs-lookup"><span data-stu-id="99cd5-476">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="99cd5-477">локалсекуритйоптионсдисаблесервердигиталлисигнкоммуникатионсифклиентагрис</span><span class="sxs-lookup"><span data-stu-id="99cd5-477">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="99cd5-478">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-478">Boolean</span></span>|<span data-ttu-id="99cd5-479">Этот параметр безопасности определяет, будет ли SMB согласовывать подпись SMB Packet с клиентами, которые их запрашивают.</span><span class="sxs-lookup"><span data-stu-id="99cd5-479">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="99cd5-480">локалсекуритйоптионсрестриктанонимаусакцесстонамедпипесандшарес</span><span class="sxs-lookup"><span data-stu-id="99cd5-480">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="99cd5-481">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-481">Boolean</span></span>|<span data-ttu-id="99cd5-482">По умолчанию этот параметр безопасности запрещает анонимный доступ к ресурсам и каналам к параметрам именованных каналов, к которым возможен анонимный доступ, и к общедоступным ресурсам, к которым возможен анонимный доступ</span><span class="sxs-lookup"><span data-stu-id="99cd5-482">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="99cd5-483">локалсекуритйоптионсдоноталлованонимаусенумератионофсамаккаунтс</span><span class="sxs-lookup"><span data-stu-id="99cd5-483">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="99cd5-484">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-484">Boolean</span></span>|<span data-ttu-id="99cd5-485">Этот параметр безопасности определяет, какие дополнительные разрешения будут предоставлены анонимным подключениям к компьютеру.</span><span class="sxs-lookup"><span data-stu-id="99cd5-485">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="99cd5-486">локалсекуритйоптионсаллованонимаусенумератионофсамаккаунтсандшарес</span><span class="sxs-lookup"><span data-stu-id="99cd5-486">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="99cd5-487">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-487">Boolean</span></span>|<span data-ttu-id="99cd5-488">Этот параметр безопасности определяет, разрешено ли анонимным пользователям выполнять определенные действия, например перечислять имена доменных учетных записей и сетевые общие папки.</span><span class="sxs-lookup"><span data-stu-id="99cd5-488">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="99cd5-489">локалсекуритйоптионсдонотстореланманажерхашвалуеоннекстпассвордчанже</span><span class="sxs-lookup"><span data-stu-id="99cd5-489">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="99cd5-490">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-490">Boolean</span></span>|<span data-ttu-id="99cd5-491">Этот параметр безопасности определяет, будет ли сохраняться значение хэша LAN Manager (LM) для нового пароля при следующем изменении пароля.</span><span class="sxs-lookup"><span data-stu-id="99cd5-491">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="99cd5-492">По умолчанию он не хранится.</span><span class="sxs-lookup"><span data-stu-id="99cd5-492">It’s not stored by default.</span></span>|
|<span data-ttu-id="99cd5-493">локалсекуритйоптионссмарткардремовалбехавиор</span><span class="sxs-lookup"><span data-stu-id="99cd5-493">localSecurityOptionsSmartCardRemovalBehavior</span></span>|<span data-ttu-id="99cd5-494">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md);</span><span class="sxs-lookup"><span data-stu-id="99cd5-494">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)</span></span>|<span data-ttu-id="99cd5-495">Этот параметр безопасности определяет, что происходит при удалении смарт-карты пользователя, выполнившего вход в систему, из устройства чтения смарт-карт.</span><span class="sxs-lookup"><span data-stu-id="99cd5-495">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="99cd5-496">Возможные значения: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-496">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="99cd5-497">дефендерсекуритицентердисаблеаппбровсеруи</span><span class="sxs-lookup"><span data-stu-id="99cd5-497">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="99cd5-498">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-498">Boolean</span></span>|<span data-ttu-id="99cd5-499">Используется для отключения отображения области защиты приложений и браузера.</span><span class="sxs-lookup"><span data-stu-id="99cd5-499">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="99cd5-500">дефендерсекуритицентердисаблефамилюи</span><span class="sxs-lookup"><span data-stu-id="99cd5-500">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="99cd5-501">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-501">Boolean</span></span>|<span data-ttu-id="99cd5-502">Используется для отключения отображения области семьи.</span><span class="sxs-lookup"><span data-stu-id="99cd5-502">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="99cd5-503">дефендерсекуритицентердисаблехеалсуи</span><span class="sxs-lookup"><span data-stu-id="99cd5-503">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="99cd5-504">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-504">Boolean</span></span>|<span data-ttu-id="99cd5-505">Используется для отключения отображения области производительности и работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="99cd5-505">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="99cd5-506">дефендерсекуритицентердисабленетворкуи</span><span class="sxs-lookup"><span data-stu-id="99cd5-506">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="99cd5-507">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-507">Boolean</span></span>|<span data-ttu-id="99cd5-508">Используется для отключения отображения зоны "брандмауэр" и "Защита сети".</span><span class="sxs-lookup"><span data-stu-id="99cd5-508">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="99cd5-509">дефендерсекуритицентердисаблевирусуи</span><span class="sxs-lookup"><span data-stu-id="99cd5-509">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="99cd5-510">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-510">Boolean</span></span>|<span data-ttu-id="99cd5-511">Используется для отключения отображения области защиты от вирусов и угроз.</span><span class="sxs-lookup"><span data-stu-id="99cd5-511">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="99cd5-512">дефендерсекуритицентердисаблеаккаунтуи</span><span class="sxs-lookup"><span data-stu-id="99cd5-512">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="99cd5-513">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-513">Boolean</span></span>|<span data-ttu-id="99cd5-514">Используется для отключения отображения области защиты учетных записей.</span><span class="sxs-lookup"><span data-stu-id="99cd5-514">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="99cd5-515">дефендерсекуритицентердисаблеклеартпмуи</span><span class="sxs-lookup"><span data-stu-id="99cd5-515">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="99cd5-516">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-516">Boolean</span></span>|<span data-ttu-id="99cd5-517">Используется для отключения отображения кнопки Очистить доверенный платформенный модуль.</span><span class="sxs-lookup"><span data-stu-id="99cd5-517">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="99cd5-518">дефендерсекуритицентердисаблехардвареуи</span><span class="sxs-lookup"><span data-stu-id="99cd5-518">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="99cd5-519">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-519">Boolean</span></span>|<span data-ttu-id="99cd5-520">Используется для отключения отображения области аппаратной защиты.</span><span class="sxs-lookup"><span data-stu-id="99cd5-520">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="99cd5-521">дефендерсекуритицентердисабленотификатионареауи</span><span class="sxs-lookup"><span data-stu-id="99cd5-521">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="99cd5-522">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-522">Boolean</span></span>|<span data-ttu-id="99cd5-523">Используется для отключения отображения элемента управления "область уведомлений".</span><span class="sxs-lookup"><span data-stu-id="99cd5-523">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="99cd5-524">Для вступления этого параметра в силу пользователю необходимо выйти из системы и войти в нее, а затем перезагрузить компьютер.</span><span class="sxs-lookup"><span data-stu-id="99cd5-524">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="99cd5-525">дефендерсекуритицентердисаблерансомвареуи</span><span class="sxs-lookup"><span data-stu-id="99cd5-525">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="99cd5-526">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-526">Boolean</span></span>|<span data-ttu-id="99cd5-527">Используется для отключения отображения области защиты от пошантажистом.</span><span class="sxs-lookup"><span data-stu-id="99cd5-527">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="99cd5-528">дефендерсекуритицентердисаблесекуребутуи</span><span class="sxs-lookup"><span data-stu-id="99cd5-528">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="99cd5-529">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-529">Boolean</span></span>|<span data-ttu-id="99cd5-530">Используется для отключения отображения области безопасной загрузки в разделе Безопасность устройства.</span><span class="sxs-lookup"><span data-stu-id="99cd5-530">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="99cd5-531">дефендерсекуритицентердисаблетраублешутингуи</span><span class="sxs-lookup"><span data-stu-id="99cd5-531">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="99cd5-532">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-532">Boolean</span></span>|<span data-ttu-id="99cd5-533">Используется для отключения отображения устранения неполадок процесса безопасности в разделе Безопасность устройства.</span><span class="sxs-lookup"><span data-stu-id="99cd5-533">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="99cd5-534">дефендерсекуритицентердисаблевулнераблетпмфирмвареупдатеуи</span><span class="sxs-lookup"><span data-stu-id="99cd5-534">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="99cd5-535">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-535">Boolean</span></span>|<span data-ttu-id="99cd5-536">Используется для отключения отображения обновления микропрограммы доверенного платформенного модуля при обнаружении уязвимого программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="99cd5-536">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="99cd5-537">дефендерсекуритицентерорганизатиондисплайнаме</span><span class="sxs-lookup"><span data-stu-id="99cd5-537">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="99cd5-538">String</span><span class="sxs-lookup"><span data-stu-id="99cd5-538">String</span></span>|<span data-ttu-id="99cd5-539">Имя компании, которое отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="99cd5-539">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="99cd5-540">дефендерсекуритицентерхелпемаил</span><span class="sxs-lookup"><span data-stu-id="99cd5-540">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="99cd5-541">String</span><span class="sxs-lookup"><span data-stu-id="99cd5-541">String</span></span>|<span data-ttu-id="99cd5-542">Адрес электронной почты, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="99cd5-542">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="99cd5-543">дефендерсекуритицентерхелпфоне</span><span class="sxs-lookup"><span data-stu-id="99cd5-543">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="99cd5-544">String</span><span class="sxs-lookup"><span data-stu-id="99cd5-544">String</span></span>|<span data-ttu-id="99cd5-545">Номер телефона или идентификатор Skype, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="99cd5-545">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="99cd5-546">дефендерсекуритицентерхелпурл</span><span class="sxs-lookup"><span data-stu-id="99cd5-546">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="99cd5-547">String</span><span class="sxs-lookup"><span data-stu-id="99cd5-547">String</span></span>|<span data-ttu-id="99cd5-548">URL-адрес портала справки это отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="99cd5-548">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="99cd5-549">дефендерсекуритицентернотификатионсфромапп</span><span class="sxs-lookup"><span data-stu-id="99cd5-549">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="99cd5-550">дефендерсекуритицентернотификатионсфромапптипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-550">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="99cd5-551">Уведомления, отображаемые в отображаемых областях приложения.</span><span class="sxs-lookup"><span data-stu-id="99cd5-551">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="99cd5-552">Возможные значения: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-552">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="99cd5-553">дефендерсекуритицентеритконтактдисплай</span><span class="sxs-lookup"><span data-stu-id="99cd5-553">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="99cd5-554">дефендерсекуритицентеритконтактдисплайтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-554">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="99cd5-555">Настройка места отображения контактной информации для конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="99cd5-555">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="99cd5-556">Возможные значения: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-556">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="99cd5-557">виндовсдефендертамперпротектион</span><span class="sxs-lookup"><span data-stu-id="99cd5-557">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="99cd5-558">windowsDefenderTamperProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="99cd5-558">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="99cd5-559">Настройка параметров Тамперпротектион для защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="99cd5-559">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="99cd5-560">Возможные значения: `notConfigured`, `enable`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-560">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="99cd5-561">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="99cd5-561">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="99cd5-562">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-562">Boolean</span></span>|<span data-ttu-id="99cd5-563">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="99cd5-563">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="99cd5-564">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="99cd5-564">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="99cd5-565">Int32</span><span class="sxs-lookup"><span data-stu-id="99cd5-565">Int32</span></span>|<span data-ttu-id="99cd5-566">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="99cd5-566">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="99cd5-567">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="99cd5-567">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="99cd5-568">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="99cd5-568">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="99cd5-569">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="99cd5-569">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="99cd5-570">фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-570">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="99cd5-571">Выберите используемую кодировку с общим ключом.</span><span class="sxs-lookup"><span data-stu-id="99cd5-571">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="99cd5-572">Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-572">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="99cd5-573">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="99cd5-573">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="99cd5-574">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-574">Boolean</span></span>|<span data-ttu-id="99cd5-575">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="99cd5-575">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="99cd5-576">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="99cd5-576">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="99cd5-577">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-577">Boolean</span></span>|<span data-ttu-id="99cd5-578">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="99cd5-578">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="99cd5-579">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="99cd5-579">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="99cd5-580">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-580">Boolean</span></span>|<span data-ttu-id="99cd5-581">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="99cd5-581">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="99cd5-582">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="99cd5-582">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="99cd5-583">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-583">Boolean</span></span>|<span data-ttu-id="99cd5-584">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="99cd5-584">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="99cd5-585">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="99cd5-585">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="99cd5-586">фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-586">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="99cd5-587">Укажите способ применения списка отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="99cd5-587">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="99cd5-588">Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-588">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="99cd5-589">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="99cd5-589">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="99cd5-590">Boolean</span><span class="sxs-lookup"><span data-stu-id="99cd5-590">Boolean</span></span>|<span data-ttu-id="99cd5-591">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="99cd5-591">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="99cd5-592">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="99cd5-592">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="99cd5-593">фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-593">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="99cd5-594">Настраивает способ применения очередей пакетов в сценарии туннельного шлюза.</span><span class="sxs-lookup"><span data-stu-id="99cd5-594">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="99cd5-595">Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-595">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="99cd5-596">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="99cd5-596">firewallProfileDomain</span></span>|[<span data-ttu-id="99cd5-597">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="99cd5-597">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="99cd5-598">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="99cd5-598">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="99cd5-599">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="99cd5-599">firewallProfilePublic</span></span>|[<span data-ttu-id="99cd5-600">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="99cd5-600">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="99cd5-601">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="99cd5-601">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="99cd5-602">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="99cd5-602">firewallProfilePrivate</span></span>|[<span data-ttu-id="99cd5-603">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="99cd5-603">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="99cd5-604">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="99cd5-604">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="99cd5-605">дефендерадобереадерлаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="99cd5-605">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="99cd5-606">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-606">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="99cd5-607">Значение, указывающее поведение Adobe Reader при создании дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="99cd5-607">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="99cd5-608">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-608">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-609">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="99cd5-609">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="99cd5-610">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="99cd5-610">String collection</span></span>|<span data-ttu-id="99cd5-611">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="99cd5-611">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="99cd5-612">дефендероффицеаппсосерпроцессинжектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-612">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="99cd5-613">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-613">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="99cd5-614">Значение, указывающее поведение приложений Office, добавляемых в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="99cd5-614">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="99cd5-615">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-615">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-616">дефендероффицеаппсосерпроцессинжектион</span><span class="sxs-lookup"><span data-stu-id="99cd5-616">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="99cd5-617">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-617">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="99cd5-618">Значение, указывающее поведение приложений Office, добавляемых в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="99cd5-618">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="99cd5-619">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-619">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-620">дефендероффицекоммуникатионаппслаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="99cd5-620">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="99cd5-621">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-621">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="99cd5-622">Значение, определяющее поведение приложений для связи с Office, включая Microsoft Outlook, от создания дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="99cd5-622">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="99cd5-623">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-623">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-624">дефендероффицеаппсексекутаблеконтенткреатионорлаунчтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-624">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="99cd5-625">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-625">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="99cd5-626">Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого контента.</span><span class="sxs-lookup"><span data-stu-id="99cd5-626">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="99cd5-627">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-627">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-628">дефендероффицеаппсексекутаблеконтенткреатионорлаунч</span><span class="sxs-lookup"><span data-stu-id="99cd5-628">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="99cd5-629">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-629">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="99cd5-630">Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого контента.</span><span class="sxs-lookup"><span data-stu-id="99cd5-630">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="99cd5-631">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-631">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-632">дефендероффицеаппслаунччилдпроцесстипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-632">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="99cd5-633">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-633">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="99cd5-634">Значение, указывающее поведение запуска приложения Office для дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="99cd5-634">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="99cd5-635">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-635">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-636">дефендероффицеаппслаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="99cd5-636">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="99cd5-637">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-637">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="99cd5-638">Значение, указывающее поведение запуска приложения Office для дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="99cd5-638">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="99cd5-639">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-639">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-640">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="99cd5-640">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="99cd5-641">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-641">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="99cd5-642">Значение, указывающее поведение импорта Win32 из кода макросов в Office.</span><span class="sxs-lookup"><span data-stu-id="99cd5-642">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="99cd5-643">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-643">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-644">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="99cd5-644">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="99cd5-645">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-645">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="99cd5-646">Значение, указывающее поведение импорта Win32 из кода макросов в Office.</span><span class="sxs-lookup"><span data-stu-id="99cd5-646">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="99cd5-647">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-647">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-648">дефендерскриптобфускатедмакрокодетипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-648">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="99cd5-649">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-649">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="99cd5-650">Значение, определяющее поведение кода "замаскированный JS/VBS/PS/макрос".</span><span class="sxs-lookup"><span data-stu-id="99cd5-650">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="99cd5-651">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-651">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-652">дефендерскриптобфускатедмакрокоде</span><span class="sxs-lookup"><span data-stu-id="99cd5-652">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="99cd5-653">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-653">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="99cd5-654">Значение, определяющее поведение кода "замаскированный JS/VBS/PS/макрос".</span><span class="sxs-lookup"><span data-stu-id="99cd5-654">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="99cd5-655">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-655">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-656">дефендерскриптдовнлоадедпайлоадексекутионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-656">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="99cd5-657">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-657">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="99cd5-658">Значение, определяющее поведение JS-и VBS-данных, загруженных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="99cd5-658">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="99cd5-659">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-659">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-660">дефендерскриптдовнлоадедпайлоадексекутион</span><span class="sxs-lookup"><span data-stu-id="99cd5-660">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="99cd5-661">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-661">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="99cd5-662">Значение, определяющее поведение JS-и VBS-данных, загруженных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="99cd5-662">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="99cd5-663">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-663">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-664">дефендерпревенткредентиалстеалингтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-664">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="99cd5-665">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-665">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="99cd5-666">Значение, указывающее, разрешено ли перенос учетных данных из подсистемы локального центра безопасности Windows.</span><span class="sxs-lookup"><span data-stu-id="99cd5-666">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="99cd5-667">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-667">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-668">дефендерпроцесскреатионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-668">defenderProcessCreationType</span></span>|[<span data-ttu-id="99cd5-669">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-669">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="99cd5-670">Значение, указывающее ответ на создание процессов, исходящих от команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="99cd5-670">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="99cd5-671">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-671">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-672">дефендерпроцесскреатион</span><span class="sxs-lookup"><span data-stu-id="99cd5-672">defenderProcessCreation</span></span>|[<span data-ttu-id="99cd5-673">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-673">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="99cd5-674">Значение, указывающее ответ на создание процессов, исходящих от команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="99cd5-674">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="99cd5-675">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-675">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-676">дефендерунтрустедусбпроцесстипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-676">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="99cd5-677">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-677">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="99cd5-678">Значение, указывающее ответ на недоверенные и неподписанные процессы, которые запускаются с USB.</span><span class="sxs-lookup"><span data-stu-id="99cd5-678">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="99cd5-679">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-679">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-680">дефендерунтрустедусбпроцесс</span><span class="sxs-lookup"><span data-stu-id="99cd5-680">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="99cd5-681">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-681">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="99cd5-682">Значение, указывающее ответ на недоверенные и неподписанные процессы, которые запускаются с USB.</span><span class="sxs-lookup"><span data-stu-id="99cd5-682">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="99cd5-683">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-683">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-684">дефендерунтрустедексекутаблетипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-684">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="99cd5-685">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-685">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="99cd5-686">Значение, указывающее ответ на исполняемые файлы, которые не отвечают условиям преобладание, возраст или доверенного списка.</span><span class="sxs-lookup"><span data-stu-id="99cd5-686">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="99cd5-687">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-687">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-688">дефендерунтрустедексекутабле</span><span class="sxs-lookup"><span data-stu-id="99cd5-688">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="99cd5-689">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-689">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="99cd5-690">Значение, указывающее ответ на исполняемые файлы, которые не отвечают условиям преобладание, возраст или доверенного списка.</span><span class="sxs-lookup"><span data-stu-id="99cd5-690">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="99cd5-691">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-691">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-692">дефендеремаилконтентексекутионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-692">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="99cd5-693">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-693">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="99cd5-694">Значение, указывающее, следует ли удалять исполняемые файлы (exe, DLL, PS, JS, VBS и т. д.) из электронной почты (почтовая или почтовая программа).</span><span class="sxs-lookup"><span data-stu-id="99cd5-694">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="99cd5-695">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-695">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-696">дефендеремаилконтентексекутион</span><span class="sxs-lookup"><span data-stu-id="99cd5-696">defenderEmailContentExecution</span></span>|[<span data-ttu-id="99cd5-697">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-697">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="99cd5-698">Значение, указывающее, следует ли удалять исполняемые файлы (exe, DLL, PS, JS, VBS и т. д.) из электронной почты (почтовая или почтовая программа).</span><span class="sxs-lookup"><span data-stu-id="99cd5-698">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="99cd5-699">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-699">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-700">дефендерадванцедрансомеварепротектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-700">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="99cd5-701">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-701">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="99cd5-702">Значение, указывающее на использование расширенной защиты в рансомеваре.</span><span class="sxs-lookup"><span data-stu-id="99cd5-702">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="99cd5-703">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-703">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-704">дефендергуардмифолдерстипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-704">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="99cd5-705">фолдерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-705">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="99cd5-706">Значение, указывающее поведение защищенных папок.</span><span class="sxs-lookup"><span data-stu-id="99cd5-706">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="99cd5-707">Возможные значения: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-707">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="99cd5-708">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="99cd5-708">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="99cd5-709">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="99cd5-709">String collection</span></span>|<span data-ttu-id="99cd5-710">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="99cd5-710">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="99cd5-711">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="99cd5-711">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="99cd5-712">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="99cd5-712">String collection</span></span>|<span data-ttu-id="99cd5-713">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="99cd5-713">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="99cd5-714">дефендернетворкпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-714">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="99cd5-715">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-715">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="99cd5-716">Значение, указывающее поведение Нетворкпротектион.</span><span class="sxs-lookup"><span data-stu-id="99cd5-716">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="99cd5-717">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-717">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="99cd5-718">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="99cd5-718">defenderExploitProtectionXml</span></span>|<span data-ttu-id="99cd5-719">Binary</span><span class="sxs-lookup"><span data-stu-id="99cd5-719">Binary</span></span>|<span data-ttu-id="99cd5-720">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="99cd5-720">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="99cd5-721">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="99cd5-721">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="99cd5-722">String</span><span class="sxs-lookup"><span data-stu-id="99cd5-722">String</span></span>|<span data-ttu-id="99cd5-723">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="99cd5-723">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="99cd5-724">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="99cd5-724">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="99cd5-725">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-725">Boolean</span></span>|<span data-ttu-id="99cd5-726">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="99cd5-726">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="99cd5-727">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="99cd5-727">appLockerApplicationControl</span></span>|[<span data-ttu-id="99cd5-728">апплоккераппликатионконтролтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-728">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="99cd5-729">Позволяет администратору выбирать разрешенные типы приложений для устройств.</span><span class="sxs-lookup"><span data-stu-id="99cd5-729">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="99cd5-730">Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-730">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="99cd5-731">девицегуардлокалсистемаусоритикредентиалгуардсеттингс</span><span class="sxs-lookup"><span data-stu-id="99cd5-731">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="99cd5-732">девицегуардлокалсистемаусоритикредентиалгуардтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-732">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="99cd5-733">Включите Guard в учетных данных, когда включен уровень безопасности платформы с безопасной загрузкой и безопасностью на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="99cd5-733">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="99cd5-734">Возможные значения: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-734">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="99cd5-735">девицегуарденаблевиртуализатионбаседсекурити</span><span class="sxs-lookup"><span data-stu-id="99cd5-735">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="99cd5-736">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-736">Boolean</span></span>|<span data-ttu-id="99cd5-737">Включает безопасность на основе виртуализации (VBS).</span><span class="sxs-lookup"><span data-stu-id="99cd5-737">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="99cd5-738">девицегуарденаблесекуребутвисдма</span><span class="sxs-lookup"><span data-stu-id="99cd5-738">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="99cd5-739">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-739">Boolean</span></span>|<span data-ttu-id="99cd5-740">Это свойство будет устаревшим в 2019 мая и будет заменено свойством Девицегуардсекуребутвисдма.</span><span class="sxs-lookup"><span data-stu-id="99cd5-740">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="99cd5-741">Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="99cd5-741">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="99cd5-742">девицегуардсекуребутвисдма</span><span class="sxs-lookup"><span data-stu-id="99cd5-742">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="99cd5-743">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="99cd5-743">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="99cd5-744">Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="99cd5-744">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="99cd5-745">Возможные значения: `notConfigured`, `withoutDMA`, `withDMA`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-745">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="99cd5-746">девицегуардлаунчсистемгуард</span><span class="sxs-lookup"><span data-stu-id="99cd5-746">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="99cd5-747">Включение</span><span class="sxs-lookup"><span data-stu-id="99cd5-747">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="99cd5-748">Позволяет ИТ – администратору настраивать запуск системы защиты системы.</span><span class="sxs-lookup"><span data-stu-id="99cd5-748">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="99cd5-749">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-749">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="99cd5-750">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="99cd5-750">smartScreenEnableInShell</span></span>|<span data-ttu-id="99cd5-751">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-751">Boolean</span></span>|<span data-ttu-id="99cd5-752">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="99cd5-752">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="99cd5-753">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="99cd5-753">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="99cd5-754">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-754">Boolean</span></span>|<span data-ttu-id="99cd5-755">Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="99cd5-755">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="99cd5-756">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="99cd5-756">applicationGuardEnabled</span></span>|<span data-ttu-id="99cd5-757">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-757">Boolean</span></span>|<span data-ttu-id="99cd5-758">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="99cd5-758">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="99cd5-759">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="99cd5-759">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="99cd5-760">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="99cd5-760">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="99cd5-761">Включение Application Guard в Защитнике Windows для более новых сборок Windows.</span><span class="sxs-lookup"><span data-stu-id="99cd5-761">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="99cd5-762">Возможные значения: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-762">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="99cd5-763">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="99cd5-763">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="99cd5-764">аппликатионгуардблоккфилетрансфертипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-764">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="99cd5-765">Блокировать буфер обмена для передачи файла изображения, текстового файла или ни одного из них.</span><span class="sxs-lookup"><span data-stu-id="99cd5-765">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="99cd5-766">Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-766">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="99cd5-767">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="99cd5-767">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="99cd5-768">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-768">Boolean</span></span>|<span data-ttu-id="99cd5-769">Позволяет заблокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="99cd5-769">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="99cd5-770">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="99cd5-770">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="99cd5-771">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-771">Boolean</span></span>|<span data-ttu-id="99cd5-772">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="99cd5-772">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="99cd5-773">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="99cd5-773">applicationGuardForceAuditing</span></span>|<span data-ttu-id="99cd5-774">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-774">Boolean</span></span>|<span data-ttu-id="99cd5-775">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="99cd5-775">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="99cd5-776">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="99cd5-776">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="99cd5-777">аппликатионгуардблоккклипбоардшарингтипе</span><span class="sxs-lookup"><span data-stu-id="99cd5-777">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="99cd5-778">Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="99cd5-778">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="99cd5-779">Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-779">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="99cd5-780">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="99cd5-780">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="99cd5-781">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-781">Boolean</span></span>|<span data-ttu-id="99cd5-782">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="99cd5-782">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="99cd5-783">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="99cd5-783">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="99cd5-784">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-784">Boolean</span></span>|<span data-ttu-id="99cd5-785">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="99cd5-785">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="99cd5-786">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="99cd5-786">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="99cd5-787">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-787">Boolean</span></span>|<span data-ttu-id="99cd5-788">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="99cd5-788">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="99cd5-789">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="99cd5-789">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="99cd5-790">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-790">Boolean</span></span>|<span data-ttu-id="99cd5-791">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="99cd5-791">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="99cd5-792">аппликатионгуардалловвиртуалгпу</span><span class="sxs-lookup"><span data-stu-id="99cd5-792">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="99cd5-793">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-793">Boolean</span></span>|<span data-ttu-id="99cd5-794">Разрешить приложению Application Guard использовать виртуальный GPU</span><span class="sxs-lookup"><span data-stu-id="99cd5-794">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="99cd5-795">аппликатионгуардалловфилесавеонхост</span><span class="sxs-lookup"><span data-stu-id="99cd5-795">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="99cd5-796">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-796">Boolean</span></span>|<span data-ttu-id="99cd5-797">Разрешить пользователям скачивать файлы из EDGE в контейнере Application Guard и сохранять их в файловой системе узла</span><span class="sxs-lookup"><span data-stu-id="99cd5-797">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="99cd5-798">битлоккералловстандардусеренкриптион</span><span class="sxs-lookup"><span data-stu-id="99cd5-798">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="99cd5-799">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-799">Boolean</span></span>|<span data-ttu-id="99cd5-800">Позволяет администратору разрешить обычным пользователям включать енкрпитион во время присоединения к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="99cd5-800">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="99cd5-801">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="99cd5-801">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="99cd5-802">Логический</span><span class="sxs-lookup"><span data-stu-id="99cd5-802">Boolean</span></span>|<span data-ttu-id="99cd5-803">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="99cd5-803">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="99cd5-804">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="99cd5-804">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="99cd5-805">Boolean</span><span class="sxs-lookup"><span data-stu-id="99cd5-805">Boolean</span></span>|<span data-ttu-id="99cd5-806">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="99cd5-806">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="99cd5-807">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="99cd5-807">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="99cd5-808">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="99cd5-808">bitLockerEncryptDevice</span></span>|<span data-ttu-id="99cd5-809">Boolean</span><span class="sxs-lookup"><span data-stu-id="99cd5-809">Boolean</span></span>|<span data-ttu-id="99cd5-810">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="99cd5-810">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="99cd5-811">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="99cd5-811">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="99cd5-812">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="99cd5-812">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="99cd5-813">Политика системного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="99cd5-813">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="99cd5-814">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="99cd5-814">bitLockerFixedDrivePolicy</span></span>|<span data-ttu-id="99cd5-815">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md);</span><span class="sxs-lookup"><span data-stu-id="99cd5-815">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)</span></span>|<span data-ttu-id="99cd5-816">Политика фиксированного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="99cd5-816">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="99cd5-817">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="99cd5-817">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="99cd5-818">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="99cd5-818">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="99cd5-819">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="99cd5-819">BitLocker Removable Drive Policy.</span></span>|
|<span data-ttu-id="99cd5-820">битлоккеррековерипассвордротатион</span><span class="sxs-lookup"><span data-stu-id="99cd5-820">bitLockerRecoveryPasswordRotation</span></span>|[<span data-ttu-id="99cd5-821">bitLockerRecoveryPasswordRotationType</span><span class="sxs-lookup"><span data-stu-id="99cd5-821">bitLockerRecoveryPasswordRotationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|<span data-ttu-id="99cd5-822">Этот параметр инициирует поворот пароля восстановления на основе клиента после восстановления диска ОС (с помощью BOOTMGR или WinRE).</span><span class="sxs-lookup"><span data-stu-id="99cd5-822">This setting initiates a client-driven recovery password rotation after an OS drive recovery (either by using bootmgr or WinRE).</span></span> <span data-ttu-id="99cd5-823">Возможные значения: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span><span class="sxs-lookup"><span data-stu-id="99cd5-823">Possible values are: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span></span>|



## <a name="response"></a><span data-ttu-id="99cd5-824">Отклик</span><span class="sxs-lookup"><span data-stu-id="99cd5-824">Response</span></span>
<span data-ttu-id="99cd5-825">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="99cd5-825">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99cd5-826">Пример</span><span class="sxs-lookup"><span data-stu-id="99cd5-826">Example</span></span>

### <a name="request"></a><span data-ttu-id="99cd5-827">Запрос</span><span class="sxs-lookup"><span data-stu-id="99cd5-827">Request</span></span>
<span data-ttu-id="99cd5-828">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99cd5-828">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 28588

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
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
  "dmaGuardDeviceEnumerationPolicy": "blockAll",
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "displayName": "Display Name value",
      "description": "Description value",
      "packageFamilyName": "Package Family Name value",
      "filePath": "File Path value",
      "serviceName": "Service Name value",
      "protocol": 8,
      "localPortRanges": [
        "Local Port Ranges value"
      ],
      "remotePortRanges": [
        "Remote Port Ranges value"
      ],
      "localAddressRanges": [
        "Local Address Ranges value"
      ],
      "remoteAddressRanges": [
        "Remote Address Ranges value"
      ],
      "profileTypes": "domain",
      "action": "blocked",
      "trafficDirection": "out",
      "interfaceTypes": "remoteAccess",
      "edgeTraversal": "blocked",
      "localUserAuthorizations": "Local User Authorizations value"
    }
  ],
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDenyLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "automatic",
  "xboxServicesLiveAuthManagerServiceStartupMode": "automatic",
  "xboxServicesLiveGameSaveServiceStartupMode": "automatic",
  "xboxServicesLiveNetworkingServiceStartupMode": "automatic",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsDisableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "Local Security Options Guest Account Name value",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "administrators",
  "localSecurityOptionsMachineInactivityLimit": 10,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 3,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "Local Security Options Log On Message Title value",
  "localSecurityOptionsLogOnMessageText": "Local Security Options Log On Message Text value",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "Local Security Options Allow Remote Calls To Security Accounts Manager value",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "requireNtmlV2SessionSecurity",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "requireNtmlV2SessionSecurity",
  "lanManagerAuthenticationLevel": "lmNtlmAndNtlmV2",
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "elevateWithoutPrompting",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "automaticallyDenyElevationRequests",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "userDisplayNameDomainUser",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "administrators",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "noAction",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "Defender Security Center Organization Display Name value",
  "defenderSecurityCenterHelpEmail": "Defender Security Center Help Email value",
  "defenderSecurityCenterHelpPhone": "Defender Security Center Help Phone value",
  "defenderSecurityCenterHelpURL": "Defender Security Center Help URL value",
  "defenderSecurityCenterNotificationsFromApp": "blockNoncriticalNotifications",
  "defenderSecurityCenterITContactDisplay": "displayInAppAndInNotifications",
  "windowsDefenderTamperProtection": "enable",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "defenderAdobeReaderLaunchChildProcess": "enable",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "enable",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "block",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "enable",
  "defenderOfficeAppsLaunchChildProcessType": "block",
  "defenderOfficeAppsLaunchChildProcess": "enable",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "block",
  "defenderOfficeMacroCodeAllowWin32Imports": "enable",
  "defenderScriptObfuscatedMacroCodeType": "block",
  "defenderScriptObfuscatedMacroCode": "enable",
  "defenderScriptDownloadedPayloadExecutionType": "block",
  "defenderScriptDownloadedPayloadExecution": "enable",
  "defenderPreventCredentialStealingType": "enable",
  "defenderProcessCreationType": "block",
  "defenderProcessCreation": "enable",
  "defenderUntrustedUSBProcessType": "block",
  "defenderUntrustedUSBProcess": "enable",
  "defenderUntrustedExecutableType": "block",
  "defenderUntrustedExecutable": "enable",
  "defenderEmailContentExecutionType": "block",
  "defenderEmailContentExecution": "enable",
  "defenderAdvancedRansomewareProtectionType": "enable",
  "defenderGuardMyFoldersType": "enable",
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderNetworkProtectionType": "enable",
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "enableWithUEFILock",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "deviceGuardSecureBootWithDMA": "withoutDMA",
  "deviceGuardLaunchSystemGuard": "enabled",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "enabledForEdge",
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "bitLockerAllowStandardUserEncryption": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "required",
    "startupAuthenticationTpmPinUsage": "required",
    "startupAuthenticationTpmKeyUsage": "required",
    "startupAuthenticationTpmPinAndKeyUsage": "required",
    "minimumPinLength": 0,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "Preboot Recovery Message value",
    "prebootRecoveryUrl": "https://example.com/prebootRecoveryUrl/"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  },
  "bitLockerRecoveryPasswordRotation": "disabled"
}
```

### <a name="response"></a><span data-ttu-id="99cd5-829">Отклик</span><span class="sxs-lookup"><span data-stu-id="99cd5-829">Response</span></span>
<span data-ttu-id="99cd5-p206">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="99cd5-p206">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 28760

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "09709403-9403-0970-0394-700903947009",
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
  "dmaGuardDeviceEnumerationPolicy": "blockAll",
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "displayName": "Display Name value",
      "description": "Description value",
      "packageFamilyName": "Package Family Name value",
      "filePath": "File Path value",
      "serviceName": "Service Name value",
      "protocol": 8,
      "localPortRanges": [
        "Local Port Ranges value"
      ],
      "remotePortRanges": [
        "Remote Port Ranges value"
      ],
      "localAddressRanges": [
        "Local Address Ranges value"
      ],
      "remoteAddressRanges": [
        "Remote Address Ranges value"
      ],
      "profileTypes": "domain",
      "action": "blocked",
      "trafficDirection": "out",
      "interfaceTypes": "remoteAccess",
      "edgeTraversal": "blocked",
      "localUserAuthorizations": "Local User Authorizations value"
    }
  ],
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDenyLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "automatic",
  "xboxServicesLiveAuthManagerServiceStartupMode": "automatic",
  "xboxServicesLiveGameSaveServiceStartupMode": "automatic",
  "xboxServicesLiveNetworkingServiceStartupMode": "automatic",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsDisableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "Local Security Options Guest Account Name value",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "administrators",
  "localSecurityOptionsMachineInactivityLimit": 10,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 3,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "Local Security Options Log On Message Title value",
  "localSecurityOptionsLogOnMessageText": "Local Security Options Log On Message Text value",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "Local Security Options Allow Remote Calls To Security Accounts Manager value",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "requireNtmlV2SessionSecurity",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "requireNtmlV2SessionSecurity",
  "lanManagerAuthenticationLevel": "lmNtlmAndNtlmV2",
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "elevateWithoutPrompting",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "automaticallyDenyElevationRequests",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "userDisplayNameDomainUser",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "administrators",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "noAction",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "Defender Security Center Organization Display Name value",
  "defenderSecurityCenterHelpEmail": "Defender Security Center Help Email value",
  "defenderSecurityCenterHelpPhone": "Defender Security Center Help Phone value",
  "defenderSecurityCenterHelpURL": "Defender Security Center Help URL value",
  "defenderSecurityCenterNotificationsFromApp": "blockNoncriticalNotifications",
  "defenderSecurityCenterITContactDisplay": "displayInAppAndInNotifications",
  "windowsDefenderTamperProtection": "enable",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "defenderAdobeReaderLaunchChildProcess": "enable",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "enable",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "block",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "enable",
  "defenderOfficeAppsLaunchChildProcessType": "block",
  "defenderOfficeAppsLaunchChildProcess": "enable",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "block",
  "defenderOfficeMacroCodeAllowWin32Imports": "enable",
  "defenderScriptObfuscatedMacroCodeType": "block",
  "defenderScriptObfuscatedMacroCode": "enable",
  "defenderScriptDownloadedPayloadExecutionType": "block",
  "defenderScriptDownloadedPayloadExecution": "enable",
  "defenderPreventCredentialStealingType": "enable",
  "defenderProcessCreationType": "block",
  "defenderProcessCreation": "enable",
  "defenderUntrustedUSBProcessType": "block",
  "defenderUntrustedUSBProcess": "enable",
  "defenderUntrustedExecutableType": "block",
  "defenderUntrustedExecutable": "enable",
  "defenderEmailContentExecutionType": "block",
  "defenderEmailContentExecution": "enable",
  "defenderAdvancedRansomewareProtectionType": "enable",
  "defenderGuardMyFoldersType": "enable",
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderNetworkProtectionType": "enable",
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "enableWithUEFILock",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "deviceGuardSecureBootWithDMA": "withoutDMA",
  "deviceGuardLaunchSystemGuard": "enabled",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "enabledForEdge",
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "bitLockerAllowStandardUserEncryption": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "required",
    "startupAuthenticationTpmPinUsage": "required",
    "startupAuthenticationTpmKeyUsage": "required",
    "startupAuthenticationTpmPinAndKeyUsage": "required",
    "minimumPinLength": 0,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "Preboot Recovery Message value",
    "prebootRecoveryUrl": "https://example.com/prebootRecoveryUrl/"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  },
  "bitLockerRecoveryPasswordRotation": "disabled"
}
```






