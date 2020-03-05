---
title: Обновление объекта windows10EndpointProtectionConfiguration
description: Обновляет свойства объекта windows10EndpointProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 852130090080da70034df5642822da812d74d79d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42480391"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="15f6f-103">Обновление объекта windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="15f6f-103">Update windows10EndpointProtectionConfiguration</span></span>

<span data-ttu-id="15f6f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="15f6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15f6f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15f6f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15f6f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15f6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15f6f-107">Обновляет свойства объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15f6f-107">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15f6f-108">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="15f6f-108">Prerequisites</span></span>
<span data-ttu-id="15f6f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15f6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15f6f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15f6f-111">Permission type</span></span>|<span data-ttu-id="15f6f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="15f6f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15f6f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15f6f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15f6f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15f6f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="15f6f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15f6f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15f6f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15f6f-116">Not supported.</span></span>|
|<span data-ttu-id="15f6f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15f6f-117">Application</span></span>|<span data-ttu-id="15f6f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15f6f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15f6f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15f6f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="15f6f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="15f6f-120">Request headers</span></span>
|<span data-ttu-id="15f6f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15f6f-121">Header</span></span>|<span data-ttu-id="15f6f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="15f6f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15f6f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="15f6f-123">Authorization</span></span>|<span data-ttu-id="15f6f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15f6f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15f6f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="15f6f-125">Accept</span></span>|<span data-ttu-id="15f6f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15f6f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15f6f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15f6f-127">Request body</span></span>
<span data-ttu-id="15f6f-128">В теле запроса добавьте представление объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15f6f-128">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="15f6f-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15f6f-129">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="15f6f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="15f6f-130">Property</span></span>|<span data-ttu-id="15f6f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="15f6f-131">Type</span></span>|<span data-ttu-id="15f6f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="15f6f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15f6f-133">id</span><span class="sxs-lookup"><span data-stu-id="15f6f-133">id</span></span>|<span data-ttu-id="15f6f-134">String</span><span class="sxs-lookup"><span data-stu-id="15f6f-134">String</span></span>|<span data-ttu-id="15f6f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="15f6f-135">Key of the entity.</span></span> <span data-ttu-id="15f6f-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15f6f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15f6f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15f6f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="15f6f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15f6f-138">DateTimeOffset</span></span>|<span data-ttu-id="15f6f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="15f6f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="15f6f-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15f6f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15f6f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="15f6f-141">roleScopeTagIds</span></span>|<span data-ttu-id="15f6f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="15f6f-142">String collection</span></span>|<span data-ttu-id="15f6f-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="15f6f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="15f6f-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15f6f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15f6f-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="15f6f-145">supportsScopeTags</span></span>|<span data-ttu-id="15f6f-146">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-146">Boolean</span></span>|<span data-ttu-id="15f6f-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="15f6f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="15f6f-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="15f6f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="15f6f-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="15f6f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="15f6f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="15f6f-150">This property is read-only.</span></span> <span data-ttu-id="15f6f-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15f6f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15f6f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="15f6f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="15f6f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="15f6f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="15f6f-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="15f6f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="15f6f-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15f6f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15f6f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="15f6f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="15f6f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="15f6f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="15f6f-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="15f6f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="15f6f-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15f6f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15f6f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="15f6f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="15f6f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="15f6f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="15f6f-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="15f6f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="15f6f-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15f6f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15f6f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15f6f-164">createdDateTime</span></span>|<span data-ttu-id="15f6f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15f6f-165">DateTimeOffset</span></span>|<span data-ttu-id="15f6f-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="15f6f-166">DateTime the object was created.</span></span> <span data-ttu-id="15f6f-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15f6f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15f6f-168">description</span><span class="sxs-lookup"><span data-stu-id="15f6f-168">description</span></span>|<span data-ttu-id="15f6f-169">String</span><span class="sxs-lookup"><span data-stu-id="15f6f-169">String</span></span>|<span data-ttu-id="15f6f-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="15f6f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="15f6f-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15f6f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15f6f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="15f6f-172">displayName</span></span>|<span data-ttu-id="15f6f-173">Строка</span><span class="sxs-lookup"><span data-stu-id="15f6f-173">String</span></span>|<span data-ttu-id="15f6f-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="15f6f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="15f6f-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15f6f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15f6f-176">version</span><span class="sxs-lookup"><span data-stu-id="15f6f-176">version</span></span>|<span data-ttu-id="15f6f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="15f6f-177">Int32</span></span>|<span data-ttu-id="15f6f-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="15f6f-178">Version of the device configuration.</span></span> <span data-ttu-id="15f6f-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15f6f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15f6f-180">дмагуарддевицеенумератионполици</span><span class="sxs-lookup"><span data-stu-id="15f6f-180">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="15f6f-181">дмагуарддевицеенумератионполицитипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-181">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="15f6f-182">Эта политика предназначена для обеспечения дополнительной защиты от внешних устройств с поддержкой прямого доступа к памяти.</span><span class="sxs-lookup"><span data-stu-id="15f6f-182">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="15f6f-183">Он обеспечивает более полный контроль над перечислением устройств с поддержкой внешних устройств с поддержкой прямого доступа к памяти, несовместимых с пересопоставлением и изоляцией памяти устройств и изолированной средой.</span><span class="sxs-lookup"><span data-stu-id="15f6f-183">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="15f6f-184">Эта политика вступает в силу только тогда, когда система защиты DMA поддерживается и включена встроенным встроенным по.</span><span class="sxs-lookup"><span data-stu-id="15f6f-184">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="15f6f-185">Защита от DMA ядра — это компонент платформы, который невозможно контролировать с помощью политики или конечным пользователем.</span><span class="sxs-lookup"><span data-stu-id="15f6f-185">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="15f6f-186">Она должна поддерживаться системой на момент производства.</span><span class="sxs-lookup"><span data-stu-id="15f6f-186">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="15f6f-187">Чтобы проверить, поддерживает ли система защиту DMA, проверьте поле Защита ядра DMA на странице Сводка объекта MSINFO32. exe.</span><span class="sxs-lookup"><span data-stu-id="15f6f-187">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="15f6f-188">Возможные значения: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-188">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="15f6f-189">фиреваллрулес</span><span class="sxs-lookup"><span data-stu-id="15f6f-189">firewallRules</span></span>|<span data-ttu-id="15f6f-190">Коллекция [виндовсфиреваллруле](../resources/intune-deviceconfig-windowsfirewallrule.md)</span><span class="sxs-lookup"><span data-stu-id="15f6f-190">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="15f6f-191">Настраивает параметры правила брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="15f6f-191">Configures the firewall rule settings.</span></span> <span data-ttu-id="15f6f-192">Эта коллекция может содержать не более 150 элементов.</span><span class="sxs-lookup"><span data-stu-id="15f6f-192">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="15f6f-193">усерригхтсакцесскредентиалманажераструстедкаллер</span><span class="sxs-lookup"><span data-stu-id="15f6f-193">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="15f6f-194">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-194">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-195">Это право пользователя используется диспетчером учетных данных во время резервного копирования и восстановления.</span><span class="sxs-lookup"><span data-stu-id="15f6f-195">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="15f6f-196">Сохраненные учетные данные пользователей могут быть скомпрометированы, если эта привилегия передана другим субъектам.</span><span class="sxs-lookup"><span data-stu-id="15f6f-196">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="15f6f-197">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="15f6f-198">усерригхтсалловакцессфромнетворк</span><span class="sxs-lookup"><span data-stu-id="15f6f-198">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="15f6f-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-200">Это право пользователя определяет, какие пользователи и группы могут подключаться к компьютеру через сеть.</span><span class="sxs-lookup"><span data-stu-id="15f6f-200">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="15f6f-201">Допустимое состояние — Supported.</span><span class="sxs-lookup"><span data-stu-id="15f6f-201">State Allowed is supported.</span></span>|
|<span data-ttu-id="15f6f-202">усерригхтсблоккакцессфромнетворк</span><span class="sxs-lookup"><span data-stu-id="15f6f-202">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="15f6f-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-204">Это право пользователя определяет, каким пользователям и группам запрещается подключаться к компьютеру через сеть.</span><span class="sxs-lookup"><span data-stu-id="15f6f-204">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="15f6f-205">Блок состояния поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15f6f-205">State Block is supported.</span></span>|
|<span data-ttu-id="15f6f-206">усерригхтсактаспартофсеоператингсистем</span><span class="sxs-lookup"><span data-stu-id="15f6f-206">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="15f6f-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-208">Это право пользователя позволяет процессу олицетворять любого пользователя без проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="15f6f-208">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="15f6f-209">Таким образом, процесс может получить доступ к тем же локальным ресурсам, что и пользователь.</span><span class="sxs-lookup"><span data-stu-id="15f6f-209">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="15f6f-210">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="15f6f-211">усерригхтслокаллогон</span><span class="sxs-lookup"><span data-stu-id="15f6f-211">userRightsLocalLogOn</span></span>|[<span data-ttu-id="15f6f-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-213">Это право пользователя определяет, какие пользователи могут входить на компьютер.</span><span class="sxs-lookup"><span data-stu-id="15f6f-213">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="15f6f-214">Допустимые состояния NotConfigured, Поддерживаемые</span><span class="sxs-lookup"><span data-stu-id="15f6f-214">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="15f6f-215">усерригхтсденилокаллогон</span><span class="sxs-lookup"><span data-stu-id="15f6f-215">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="15f6f-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-217">Это право пользователя определяет, какие пользователи не могут войти на компьютер.</span><span class="sxs-lookup"><span data-stu-id="15f6f-217">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="15f6f-218">Состояния NotConfigured, блокировки поддерживаются</span><span class="sxs-lookup"><span data-stu-id="15f6f-218">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="15f6f-219">усерригхтсбаккупдата</span><span class="sxs-lookup"><span data-stu-id="15f6f-219">userRightsBackupData</span></span>|[<span data-ttu-id="15f6f-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-221">Это право пользователя определяет, какие пользователи могут обходить разрешения для файлов, каталогов, реестра и других постоянных объектов при резервном копировании файлов и каталогов.</span><span class="sxs-lookup"><span data-stu-id="15f6f-221">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="15f6f-222">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="15f6f-223">усерригхтсчанжесистемтиме</span><span class="sxs-lookup"><span data-stu-id="15f6f-223">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="15f6f-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-225">Это право пользователя определяет, какие пользователи и группы могут изменять время и дату на внутреннем часовом компьютере.</span><span class="sxs-lookup"><span data-stu-id="15f6f-225">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="15f6f-226">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="15f6f-227">усерригхтскреатеглобалобжектс</span><span class="sxs-lookup"><span data-stu-id="15f6f-227">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="15f6f-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-229">Этот параметр безопасности определяет, могут ли пользователи создавать глобальные объекты, доступные для всех сеансов.</span><span class="sxs-lookup"><span data-stu-id="15f6f-229">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="15f6f-230">Пользователи, которые могут создавать глобальные объекты, могут повлиять на процессы, выполняемые в сеансах других пользователей, что может привести к сбою приложения или повреждению данных.</span><span class="sxs-lookup"><span data-stu-id="15f6f-230">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="15f6f-231">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-231">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="15f6f-232">усерригхтскреатепажефиле</span><span class="sxs-lookup"><span data-stu-id="15f6f-232">userRightsCreatePageFile</span></span>|[<span data-ttu-id="15f6f-233">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-233">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-234">Это право пользователя определяет, какие пользователи и группы могут вызывать внутренний API, чтобы создать и изменить размер файла подкачки.</span><span class="sxs-lookup"><span data-stu-id="15f6f-234">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="15f6f-235">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-235">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="15f6f-236">усерригхтскреатеперманентшаредобжектс</span><span class="sxs-lookup"><span data-stu-id="15f6f-236">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="15f6f-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-238">Это право пользователя определяет, какие учетные записи могут использоваться процессами для создания объекта каталога с помощью диспетчера объектов.</span><span class="sxs-lookup"><span data-stu-id="15f6f-238">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="15f6f-239">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-239">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="15f6f-240">усерригхтскреатесимболиклинкс</span><span class="sxs-lookup"><span data-stu-id="15f6f-240">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="15f6f-241">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-241">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-242">Это право пользователя определяет, может ли пользователь создать символическую ссылку с компьютера, на который они входили.</span><span class="sxs-lookup"><span data-stu-id="15f6f-242">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="15f6f-243">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-243">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="15f6f-244">усерригхтскреатетокен</span><span class="sxs-lookup"><span data-stu-id="15f6f-244">userRightsCreateToken</span></span>|[<span data-ttu-id="15f6f-245">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-245">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-246">Это право пользователя определяет, какие пользователи и группы могут использоваться процессами для создания маркера, который можно использовать для получения доступа к любому локальному ресурсу, когда процесс использует внутренний API для создания маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="15f6f-246">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="15f6f-247">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-247">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="15f6f-248">усерригхтсдебугпрограмс</span><span class="sxs-lookup"><span data-stu-id="15f6f-248">userRightsDebugPrograms</span></span>|[<span data-ttu-id="15f6f-249">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-249">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-250">Это право пользователя определяет, какие пользователи могут прикреплять отладчик к любому процессу или ядру.</span><span class="sxs-lookup"><span data-stu-id="15f6f-250">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="15f6f-251">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-251">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="15f6f-252">усерригхтсремотедесктопсервицеслогон</span><span class="sxs-lookup"><span data-stu-id="15f6f-252">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="15f6f-253">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-253">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-254">Это право пользователя определяет, каким пользователям и группам запрещается вход в систему в качестве клиента служб удаленных рабочих столов.</span><span class="sxs-lookup"><span data-stu-id="15f6f-254">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="15f6f-255">Поддерживаются только состояния NotConfigured и Block</span><span class="sxs-lookup"><span data-stu-id="15f6f-255">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="15f6f-256">усерригхтсделегатион</span><span class="sxs-lookup"><span data-stu-id="15f6f-256">userRightsDelegation</span></span>|[<span data-ttu-id="15f6f-257">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-257">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-258">Это право пользователя определяет, какие пользователи могут устанавливать параметр "доверять для делегирования" для объекта пользователя или компьютера.</span><span class="sxs-lookup"><span data-stu-id="15f6f-258">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="15f6f-259">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-259">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="15f6f-260">усерригхтсженератесекуритяудитс</span><span class="sxs-lookup"><span data-stu-id="15f6f-260">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="15f6f-261">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-261">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-262">Это право пользователя определяет, какие учетные записи могут использоваться процессом для добавления записей в журнал безопасности.</span><span class="sxs-lookup"><span data-stu-id="15f6f-262">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="15f6f-263">Журнал безопасности используется для трассировки несанкционированного доступа к системе.</span><span class="sxs-lookup"><span data-stu-id="15f6f-263">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="15f6f-264">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="15f6f-265">усерригхтсимперсонатеклиент</span><span class="sxs-lookup"><span data-stu-id="15f6f-265">userRightsImpersonateClient</span></span>|[<span data-ttu-id="15f6f-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-267">Назначение этого права пользователю позволяет программам, выполняемым от имени этого пользователя, олицетворять клиента.</span><span class="sxs-lookup"><span data-stu-id="15f6f-267">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="15f6f-268">Требование этого пользователя для такого рода олицетворения запрещает несанкционированному пользователю подключаться к созданной им службе, а затем олицетворять этого клиента, что может повысить уровень разрешений неавторизованного пользователя до Уровни администрирования или системы.</span><span class="sxs-lookup"><span data-stu-id="15f6f-268">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="15f6f-269">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-269">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="15f6f-270">усерригхтсинкреасесчедулингприорити</span><span class="sxs-lookup"><span data-stu-id="15f6f-270">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="15f6f-271">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-271">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-272">Это право пользователя определяет, какие учетные записи могут использовать процесс с доступом к свойствам Write для другого процесса, чтобы увеличить приоритет выполнения, назначенный другому процессу.</span><span class="sxs-lookup"><span data-stu-id="15f6f-272">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="15f6f-273">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-273">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="15f6f-274">усерригхтслоадунлоаддриверс</span><span class="sxs-lookup"><span data-stu-id="15f6f-274">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="15f6f-275">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-275">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-276">Это право пользователя определяет, какие пользователи могут динамически загружать и выгружать драйверы устройств или другой код в режиме ядра.</span><span class="sxs-lookup"><span data-stu-id="15f6f-276">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="15f6f-277">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="15f6f-278">усерригхтслоккмемори</span><span class="sxs-lookup"><span data-stu-id="15f6f-278">userRightsLockMemory</span></span>|[<span data-ttu-id="15f6f-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-280">Это право пользователя определяет, какие учетные записи могут использовать процесс для хранения данных в физической памяти, что предотвращает их разбиение данных на виртуальную память на диске.</span><span class="sxs-lookup"><span data-stu-id="15f6f-280">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="15f6f-281">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="15f6f-282">усерригхтсманажеаудитингандсекуритилогс</span><span class="sxs-lookup"><span data-stu-id="15f6f-282">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="15f6f-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-284">Это право пользователя определяет, какие пользователи могут задавать параметры аудита доступа к объектам для отдельных ресурсов, таких как файлы, объекты Active Directory и разделы реестра.</span><span class="sxs-lookup"><span data-stu-id="15f6f-284">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="15f6f-285">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="15f6f-286">усерригхтсманажеволумес</span><span class="sxs-lookup"><span data-stu-id="15f6f-286">userRightsManageVolumes</span></span>|[<span data-ttu-id="15f6f-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-288">Это право пользователя определяет, какие пользователи и группы могут выполнять задачи обслуживания для тома, такие как удаленная дефрагментация.</span><span class="sxs-lookup"><span data-stu-id="15f6f-288">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="15f6f-289">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="15f6f-290">усерригхтсмодифифирмваринвиронмент</span><span class="sxs-lookup"><span data-stu-id="15f6f-290">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="15f6f-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-292">Это право пользователя определяет, кто может изменять значения в аппаратной среде.</span><span class="sxs-lookup"><span data-stu-id="15f6f-292">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="15f6f-293">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="15f6f-294">усерригхтсмодифйобжектлабелс</span><span class="sxs-lookup"><span data-stu-id="15f6f-294">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="15f6f-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-296">Это право пользователя определяет, какие учетные записи пользователей могут изменять метки целостности объектов, таких как файлы, разделы реестра или процессы, принадлежащие другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="15f6f-296">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="15f6f-297">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-297">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="15f6f-298">усерригхтспрофилесинглепроцесс</span><span class="sxs-lookup"><span data-stu-id="15f6f-298">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="15f6f-299">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-299">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-300">Это право пользователя определяет, какие пользователи могут использовать средства мониторинга производительности для наблюдения за производительностью системных процессов.</span><span class="sxs-lookup"><span data-stu-id="15f6f-300">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="15f6f-301">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-301">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="15f6f-302">усерригхтсремотешутдовн</span><span class="sxs-lookup"><span data-stu-id="15f6f-302">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="15f6f-303">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-303">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-304">Это право пользователя определяет, каким пользователям разрешено завершать работу компьютера из удаленного расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="15f6f-304">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="15f6f-305">Неправильное использование этого права пользователя может привести к отказу в обслуживании.</span><span class="sxs-lookup"><span data-stu-id="15f6f-305">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="15f6f-306">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-306">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="15f6f-307">усерригхтсресторедата</span><span class="sxs-lookup"><span data-stu-id="15f6f-307">userRightsRestoreData</span></span>|[<span data-ttu-id="15f6f-308">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-308">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-309">Это право пользователя определяет, какие пользователи могут обходить разрешения для файлов, каталогов, реестра и других постоянных объектов при восстановлении резервных копий файлов и каталогов, и определяет, какие пользователи могут устанавливать любой действительный субъект безопасности в качестве владельца объекта.</span><span class="sxs-lookup"><span data-stu-id="15f6f-309">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="15f6f-310">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-310">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="15f6f-311">усерригхтстакеовнершип</span><span class="sxs-lookup"><span data-stu-id="15f6f-311">userRightsTakeOwnership</span></span>|[<span data-ttu-id="15f6f-312">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="15f6f-312">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="15f6f-313">Это право пользователя определяет, какие пользователи могут становиться владельцами любого защищаемого объекта в системе, включая объекты Active Directory, файлы и папки, принтеры, разделы реестра, процессы и потоки.</span><span class="sxs-lookup"><span data-stu-id="15f6f-313">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="15f6f-314">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="15f6f-314">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="15f6f-315">ксбокссервицесенаблексбоксгамесаветаск</span><span class="sxs-lookup"><span data-stu-id="15f6f-315">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="15f6f-316">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-316">Boolean</span></span>|<span data-ttu-id="15f6f-317">Этот параметр определяет, включена ли функция сохранения игры Xbox (1) или отключена (0).</span><span class="sxs-lookup"><span data-stu-id="15f6f-317">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="15f6f-318">ксбокссервицесакцессориманажементсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="15f6f-318">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="15f6f-319">сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="15f6f-320">Этот параметр определяет, является ли тип запуска службы управления принадлежностью автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="15f6f-320">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="15f6f-321">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="15f6f-321">Default: Manual.</span></span> <span data-ttu-id="15f6f-322">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="15f6f-323">ксбокссервицесливеаусманажерсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="15f6f-323">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="15f6f-324">сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-324">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="15f6f-325">Этот параметр определяет, является ли тип запуска службы диспетчера Live auth автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="15f6f-325">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="15f6f-326">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="15f6f-326">Default: Manual.</span></span> <span data-ttu-id="15f6f-327">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-327">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="15f6f-328">ксбокссервицесливегамесавесервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="15f6f-328">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="15f6f-329">сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-329">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="15f6f-330">Этот параметр определяет, является ли тип запуска службы Live Save Service автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="15f6f-330">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="15f6f-331">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="15f6f-331">Default: Manual.</span></span> <span data-ttu-id="15f6f-332">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-332">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="15f6f-333">ксбокссервицесливенетворкингсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="15f6f-333">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="15f6f-334">сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-334">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="15f6f-335">Этот параметр определяет, является ли тип запуска сетевой службы автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="15f6f-335">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="15f6f-336">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="15f6f-336">Default: Manual.</span></span> <span data-ttu-id="15f6f-337">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-337">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="15f6f-338">локалсекуритйоптионсблоккмикрософтаккаунтс</span><span class="sxs-lookup"><span data-stu-id="15f6f-338">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="15f6f-339">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-339">Boolean</span></span>|<span data-ttu-id="15f6f-340">Запретить пользователям добавлять новые учетные записи Майкрософт на этот компьютер.</span><span class="sxs-lookup"><span data-stu-id="15f6f-340">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="15f6f-341">локалсекуритйоптионсблоккремотелогонвисбланкпассворд</span><span class="sxs-lookup"><span data-stu-id="15f6f-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="15f6f-342">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-342">Boolean</span></span>|<span data-ttu-id="15f6f-343">Включите локальные учетные записи, не защищенные паролем, для входа в систему из расположений, отличных от физического устройства. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="15f6f-343">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="15f6f-344">локалсекуритйоптионсдисаблеадминистратораккаунт</span><span class="sxs-lookup"><span data-stu-id="15f6f-344">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="15f6f-345">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-345">Boolean</span></span>|<span data-ttu-id="15f6f-346">Определяет, включена или отключена учетная запись локального администратора.</span><span class="sxs-lookup"><span data-stu-id="15f6f-346">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="15f6f-347">локалсекуритйоптионсадминистратораккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="15f6f-347">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="15f6f-348">String</span><span class="sxs-lookup"><span data-stu-id="15f6f-348">String</span></span>|<span data-ttu-id="15f6f-349">Определите имя другой учетной записи, которая будет связана с идентификатором безопасности (SID) учетной записи "Administrator".</span><span class="sxs-lookup"><span data-stu-id="15f6f-349">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="15f6f-350">локалсекуритйоптионсдисаблегуестаккаунт</span><span class="sxs-lookup"><span data-stu-id="15f6f-350">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="15f6f-351">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-351">Boolean</span></span>|<span data-ttu-id="15f6f-352">Определяет, включена или отключена Гостевая учетная запись.</span><span class="sxs-lookup"><span data-stu-id="15f6f-352">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="15f6f-353">локалсекуритйоптионсгуестаккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="15f6f-353">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="15f6f-354">String</span><span class="sxs-lookup"><span data-stu-id="15f6f-354">String</span></span>|<span data-ttu-id="15f6f-355">Определите имя другой учетной записи, которая будет связана с идентификатором безопасности (SID) для учетной записи "гость".</span><span class="sxs-lookup"><span data-stu-id="15f6f-355">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="15f6f-356">локалсекуритйоптионсалловундокквисаусавингтологон</span><span class="sxs-lookup"><span data-stu-id="15f6f-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="15f6f-357">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-357">Boolean</span></span>|<span data-ttu-id="15f6f-358">Запретите отстыковку портативного компьютера без необходимости входа в систему.</span><span class="sxs-lookup"><span data-stu-id="15f6f-358">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="15f6f-359">локалсекуритйоптионсблоккусерсинсталлингпринтердриверс</span><span class="sxs-lookup"><span data-stu-id="15f6f-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="15f6f-360">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-360">Boolean</span></span>|<span data-ttu-id="15f6f-361">Ограничьте установку драйверов принтеров в рамках подключения к общему принтеру только для администраторов.</span><span class="sxs-lookup"><span data-stu-id="15f6f-361">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="15f6f-362">локалсекуритйоптионсблоккремотеоптикалдривеакцесс</span><span class="sxs-lookup"><span data-stu-id="15f6f-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="15f6f-363">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-363">Boolean</span></span>|<span data-ttu-id="15f6f-364">Включение этого параметра позволяет интерактивно вошедший в систему пользователь получать доступ к устройству чтения компакт-дисков.</span><span class="sxs-lookup"><span data-stu-id="15f6f-364">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="15f6f-365">локалсекуритйоптионсформатандежектофремоваблемедиаалловедусер</span><span class="sxs-lookup"><span data-stu-id="15f6f-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="15f6f-366">локалсекуритйоптионсформатандежектофремоваблемедиаалловедусертипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="15f6f-367">Определите, кому разрешено форматировать и извлекать съемные носители NTFS.</span><span class="sxs-lookup"><span data-stu-id="15f6f-367">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="15f6f-368">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-368">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="15f6f-369">локалсекуритйоптионсмачинеинактивитилимит</span><span class="sxs-lookup"><span data-stu-id="15f6f-369">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="15f6f-370">Int32</span><span class="sxs-lookup"><span data-stu-id="15f6f-370">Int32</span></span>|<span data-ttu-id="15f6f-371">Определите максимальное количество минут отсутствия активности на экране входа интерактивного рабочего стола, пока не запустится экранная заставка.</span><span class="sxs-lookup"><span data-stu-id="15f6f-371">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="15f6f-372">Допустимые значения — от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="15f6f-372">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="15f6f-373">локалсекуритйоптионсмачинеинактивитилимитинминутес</span><span class="sxs-lookup"><span data-stu-id="15f6f-373">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="15f6f-374">Int32</span><span class="sxs-lookup"><span data-stu-id="15f6f-374">Int32</span></span>|<span data-ttu-id="15f6f-375">Определите максимальное количество минут отсутствия активности на экране входа интерактивного рабочего стола, пока не запустится экранная заставка.</span><span class="sxs-lookup"><span data-stu-id="15f6f-375">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="15f6f-376">Допустимые значения — от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="15f6f-376">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="15f6f-377">локалсекуритйоптионсдонотрекуиректрлалтдел</span><span class="sxs-lookup"><span data-stu-id="15f6f-377">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="15f6f-378">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-378">Boolean</span></span>|<span data-ttu-id="15f6f-379">Требовать нажатия клавиш CTRL + ALT + DEL, прежде чем пользователь сможет войти в систему.</span><span class="sxs-lookup"><span data-stu-id="15f6f-379">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="15f6f-380">локалсекуритйоптионшиделастсигнединусер</span><span class="sxs-lookup"><span data-stu-id="15f6f-380">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="15f6f-381">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-381">Boolean</span></span>|<span data-ttu-id="15f6f-382">Не отображать имя последнего пользователя, выполнившего вход на это устройство.</span><span class="sxs-lookup"><span data-stu-id="15f6f-382">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="15f6f-383">локалсекуритйоптионшидеусернамеатсигнин</span><span class="sxs-lookup"><span data-stu-id="15f6f-383">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="15f6f-384">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-384">Boolean</span></span>|<span data-ttu-id="15f6f-385">Не отображать имя пользователя, выполняющего вход на это устройство, после ввода учетных данных и отображения рабочего стола на устройстве.</span><span class="sxs-lookup"><span data-stu-id="15f6f-385">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="15f6f-386">локалсекуритйоптионслогонмессажетитле</span><span class="sxs-lookup"><span data-stu-id="15f6f-386">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="15f6f-387">String</span><span class="sxs-lookup"><span data-stu-id="15f6f-387">String</span></span>|<span data-ttu-id="15f6f-388">Задайте заголовок сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="15f6f-388">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="15f6f-389">локалсекуритйоптионслогонмессажетекст</span><span class="sxs-lookup"><span data-stu-id="15f6f-389">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="15f6f-390">String</span><span class="sxs-lookup"><span data-stu-id="15f6f-390">String</span></span>|<span data-ttu-id="15f6f-391">Задайте текст сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="15f6f-391">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="15f6f-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="15f6f-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="15f6f-393">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-393">Boolean</span></span>|<span data-ttu-id="15f6f-394">Блокировать запросы проверки подлинности PKU2U на этом устройстве для использования сетевых удостоверений.</span><span class="sxs-lookup"><span data-stu-id="15f6f-394">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="15f6f-395">локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажерхелпербул</span><span class="sxs-lookup"><span data-stu-id="15f6f-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="15f6f-396">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-396">Boolean</span></span>|<span data-ttu-id="15f6f-397">Помощник по пользовательскому интерфейсу Boolean для объекта Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажер</span><span class="sxs-lookup"><span data-stu-id="15f6f-397">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="15f6f-398">локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажер</span><span class="sxs-lookup"><span data-stu-id="15f6f-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="15f6f-399">String</span><span class="sxs-lookup"><span data-stu-id="15f6f-399">String</span></span>|<span data-ttu-id="15f6f-400">Измените строку языка определения дескрипторов безопасности по умолчанию, чтобы разрешить или запретить пользователям и группам совершать удаленные вызовы в SAM.</span><span class="sxs-lookup"><span data-stu-id="15f6f-400">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="15f6f-401">локалсекуритйоптионсминимумсессионсекуритифорнтлмсспбаседклиентс</span><span class="sxs-lookup"><span data-stu-id="15f6f-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="15f6f-402">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="15f6f-402">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="15f6f-403">Этот параметр безопасности позволяет клиенту требовать согласование 128-разрядного шифрования и/или сеанса защиты сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="15f6f-403">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="15f6f-404">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-404">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="15f6f-405">локалсекуритйоптионсминимумсессионсекуритифорнтлмсспбаседсерверс</span><span class="sxs-lookup"><span data-stu-id="15f6f-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="15f6f-406">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="15f6f-406">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="15f6f-407">Этот параметр безопасности позволяет серверу требовать согласование 128-разрядного шифрования и/или сеанса защиты сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="15f6f-407">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="15f6f-408">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-408">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="15f6f-409">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="15f6f-409">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="15f6f-410">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="15f6f-410">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="15f6f-411">Этот параметр безопасности определяет, какой протокол проверки подлинности "запрос/ответ" используется для входа в сеть.</span><span class="sxs-lookup"><span data-stu-id="15f6f-411">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="15f6f-412">Возможные значения: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-412">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="15f6f-413">ланманажерворкстатиондисаблеинсекурегуестлогонс</span><span class="sxs-lookup"><span data-stu-id="15f6f-413">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="15f6f-414">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-414">Boolean</span></span>|<span data-ttu-id="15f6f-415">Если этот параметр включен, клиент SMB будет разрешать небезопасные гостевые входы.</span><span class="sxs-lookup"><span data-stu-id="15f6f-415">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="15f6f-416">Если этот параметр не настроен, клиент SMB будет отклонять небезопасные гостевые входы.</span><span class="sxs-lookup"><span data-stu-id="15f6f-416">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="15f6f-417">локалсекуритйоптионсклеарвиртуалмеморипажефиле</span><span class="sxs-lookup"><span data-stu-id="15f6f-417">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="15f6f-418">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-418">Boolean</span></span>|<span data-ttu-id="15f6f-419">Этот параметр безопасности определяет, будет ли очищаться файл подкачки виртуальной памяти при завершении работы системы.</span><span class="sxs-lookup"><span data-stu-id="15f6f-419">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="15f6f-420">локалсекуритйоптионсалловсистемтобешутдовнвисаусавингтологон</span><span class="sxs-lookup"><span data-stu-id="15f6f-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="15f6f-421">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-421">Boolean</span></span>|<span data-ttu-id="15f6f-422">Этот параметр безопасности определяет, можно ли завершить работу компьютера, не выполняя вход в Windows.</span><span class="sxs-lookup"><span data-stu-id="15f6f-422">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="15f6f-423">локалсекуритйоптионсалловуиакцессаппликатионелеватион</span><span class="sxs-lookup"><span data-stu-id="15f6f-423">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="15f6f-424">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-424">Boolean</span></span>|<span data-ttu-id="15f6f-425">Разрешить UIAccess Apps запрос на повышение прав без использования безопасного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="15f6f-425">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="15f6f-426">локалсекуритйоптионсвиртуализефилеандрегистривритефаилурестоперусерлокатионс</span><span class="sxs-lookup"><span data-stu-id="15f6f-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="15f6f-427">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-427">Boolean</span></span>|<span data-ttu-id="15f6f-428">Виртуализация сбоев записи в файл и реестр для отдельных расположений пользователей</span><span class="sxs-lookup"><span data-stu-id="15f6f-428">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="15f6f-429">локалсекуритйоптионсонлелеватесигнедексекутаблес</span><span class="sxs-lookup"><span data-stu-id="15f6f-429">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="15f6f-430">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-430">Boolean</span></span>|<span data-ttu-id="15f6f-431">Принудительная проверка пути сертификации PKI для указанного исполняемого файла перед тем, как он будет разрешен для запуска.</span><span class="sxs-lookup"><span data-stu-id="15f6f-431">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="15f6f-432">локалсекуритйоптионсадминистраторелеватионпромптбехавиор</span><span class="sxs-lookup"><span data-stu-id="15f6f-432">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="15f6f-433">локалсекуритйоптионсадминистраторелеватионпромптбехавиортипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="15f6f-434">Определите поведение запросов на повышение прав для администраторов в режиме одобрения администратором.</span><span class="sxs-lookup"><span data-stu-id="15f6f-434">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="15f6f-435">Возможные значения: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-435">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="15f6f-436">локалсекуритйоптионсстандардусерелеватионпромптбехавиор</span><span class="sxs-lookup"><span data-stu-id="15f6f-436">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="15f6f-437">локалсекуритйоптионсстандардусерелеватионпромптбехавиортипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="15f6f-438">Определите поведение запросов на повышение прав для стандартных пользователей.</span><span class="sxs-lookup"><span data-stu-id="15f6f-438">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="15f6f-439">Возможные значения: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-439">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="15f6f-440">локалсекуритйоптионссвитчтосекуредесктопвхенпромптингфорелеватион</span><span class="sxs-lookup"><span data-stu-id="15f6f-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="15f6f-441">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-441">Boolean</span></span>|<span data-ttu-id="15f6f-442">Разрешить всем запросам на повышение прав доступ к рабочему столу интерактивного пользователя, а не к безопасному рабочему столу.</span><span class="sxs-lookup"><span data-stu-id="15f6f-442">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="15f6f-443">Используются параметры политики поведения запросов для администраторов и стандартных пользователей.</span><span class="sxs-lookup"><span data-stu-id="15f6f-443">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="15f6f-444">локалсекуритйоптионсдетектаппликатионинсталлатионсандпромптфорелеватион</span><span class="sxs-lookup"><span data-stu-id="15f6f-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="15f6f-445">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-445">Boolean</span></span>|<span data-ttu-id="15f6f-446">При установке приложений, требующих повышенных привилегий, запрашиваются учетные данные администратора. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="15f6f-446">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="15f6f-447">локалсекуритйоптионсалловуиакцессаппликатионсфорсекурелокатионс</span><span class="sxs-lookup"><span data-stu-id="15f6f-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="15f6f-448">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-448">Boolean</span></span>|<span data-ttu-id="15f6f-449">Разрешить UIAccess Apps запрос на повышение прав без использования безопасного рабочего стола. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="15f6f-449">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="15f6f-450">локалсекуритйоптионсусеадминаппровалмоде</span><span class="sxs-lookup"><span data-stu-id="15f6f-450">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="15f6f-451">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-451">Boolean</span></span>|<span data-ttu-id="15f6f-452">Определяет, использует ли встроенная учетная запись администратора режим одобрения администратором или выполняет все приложения с правами полного администратора. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="15f6f-452">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="15f6f-453">локалсекуритйоптионсусеадминаппровалмодефорадминистраторс</span><span class="sxs-lookup"><span data-stu-id="15f6f-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="15f6f-454">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-454">Boolean</span></span>|<span data-ttu-id="15f6f-455">Определить, включен ли режим одобрения администратором и все параметры политики контроля учетных записей, по умолчанию включено</span><span class="sxs-lookup"><span data-stu-id="15f6f-455">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="15f6f-456">локалсекуритйоптионсинформатионшовнонлоккскрин</span><span class="sxs-lookup"><span data-stu-id="15f6f-456">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="15f6f-457">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="15f6f-457">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="15f6f-458">Настройте сведения о пользователе, которые отображаются, когда сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="15f6f-458">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="15f6f-459">Если этот флажок не установлен, отображаются отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="15f6f-459">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="15f6f-460">Возможные значения: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-460">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="15f6f-461">локалсекуритйоптионсинформатиондисплайедонлоккскрин</span><span class="sxs-lookup"><span data-stu-id="15f6f-461">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="15f6f-462">локалсекуритйоптионсинформатиондисплайедонлоккскринтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="15f6f-463">Настройте сведения о пользователе, которые отображаются, когда сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="15f6f-463">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="15f6f-464">Если этот флажок не установлен, отображаются отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="15f6f-464">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="15f6f-465">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-465">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="15f6f-466">локалсекуритйоптионсдисаблеклиентдигиталлисигнкоммуникатионсифсерверагрис</span><span class="sxs-lookup"><span data-stu-id="15f6f-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="15f6f-467">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-467">Boolean</span></span>|<span data-ttu-id="15f6f-468">Этот параметр безопасности определяет, будет ли клиент SMB пытаться согласовать подписывание SMB пакетов.</span><span class="sxs-lookup"><span data-stu-id="15f6f-468">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="15f6f-469">локалсекуритйоптионсклиентдигиталлисигнкоммуникатионсалвайс</span><span class="sxs-lookup"><span data-stu-id="15f6f-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="15f6f-470">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-470">Boolean</span></span>|<span data-ttu-id="15f6f-471">Этот параметр безопасности определяет, требуется ли Подписывание пакетов для клиентского SMB-компонента.</span><span class="sxs-lookup"><span data-stu-id="15f6f-471">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="15f6f-472">локалсекуритйоптионсклиентсендуненкриптедпассвордтосирдпартисмбсерверс</span><span class="sxs-lookup"><span data-stu-id="15f6f-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="15f6f-473">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-473">Boolean</span></span>|<span data-ttu-id="15f6f-474">Если этот параметр безопасности включен, перенаправителем SMB (Server Message Block) разрешено отправлять пароли открытым текстом на серверы SMB сторонних производителей, не поддерживающие шифрование паролей во время проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="15f6f-474">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="15f6f-475">локалсекуритйоптионсдисаблесервердигиталлисигнкоммуникатионсалвайс</span><span class="sxs-lookup"><span data-stu-id="15f6f-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="15f6f-476">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-476">Boolean</span></span>|<span data-ttu-id="15f6f-477">Этот параметр безопасности определяет, требуется ли подписи пакетов для SMB-компонентов сервера.</span><span class="sxs-lookup"><span data-stu-id="15f6f-477">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="15f6f-478">локалсекуритйоптионсдисаблесервердигиталлисигнкоммуникатионсифклиентагрис</span><span class="sxs-lookup"><span data-stu-id="15f6f-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="15f6f-479">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-479">Boolean</span></span>|<span data-ttu-id="15f6f-480">Этот параметр безопасности определяет, будет ли SMB согласовывать подпись SMB Packet с клиентами, которые их запрашивают.</span><span class="sxs-lookup"><span data-stu-id="15f6f-480">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="15f6f-481">локалсекуритйоптионсрестриктанонимаусакцесстонамедпипесандшарес</span><span class="sxs-lookup"><span data-stu-id="15f6f-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="15f6f-482">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-482">Boolean</span></span>|<span data-ttu-id="15f6f-483">По умолчанию этот параметр безопасности запрещает анонимный доступ к ресурсам и каналам к параметрам именованных каналов, к которым возможен анонимный доступ, и к общедоступным ресурсам, к которым возможен анонимный доступ</span><span class="sxs-lookup"><span data-stu-id="15f6f-483">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="15f6f-484">локалсекуритйоптионсдоноталлованонимаусенумератионофсамаккаунтс</span><span class="sxs-lookup"><span data-stu-id="15f6f-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="15f6f-485">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-485">Boolean</span></span>|<span data-ttu-id="15f6f-486">Этот параметр безопасности определяет, какие дополнительные разрешения будут предоставлены анонимным подключениям к компьютеру.</span><span class="sxs-lookup"><span data-stu-id="15f6f-486">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="15f6f-487">локалсекуритйоптионсаллованонимаусенумератионофсамаккаунтсандшарес</span><span class="sxs-lookup"><span data-stu-id="15f6f-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="15f6f-488">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-488">Boolean</span></span>|<span data-ttu-id="15f6f-489">Этот параметр безопасности определяет, разрешено ли анонимным пользователям выполнять определенные действия, например перечислять имена доменных учетных записей и сетевые общие папки.</span><span class="sxs-lookup"><span data-stu-id="15f6f-489">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="15f6f-490">локалсекуритйоптионсдонотстореланманажерхашвалуеоннекстпассвордчанже</span><span class="sxs-lookup"><span data-stu-id="15f6f-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="15f6f-491">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-491">Boolean</span></span>|<span data-ttu-id="15f6f-492">Этот параметр безопасности определяет, будет ли сохраняться значение хэша LAN Manager (LM) для нового пароля при следующем изменении пароля.</span><span class="sxs-lookup"><span data-stu-id="15f6f-492">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="15f6f-493">По умолчанию он не хранится.</span><span class="sxs-lookup"><span data-stu-id="15f6f-493">It’s not stored by default.</span></span>|
|<span data-ttu-id="15f6f-494">локалсекуритйоптионссмарткардремовалбехавиор</span><span class="sxs-lookup"><span data-stu-id="15f6f-494">localSecurityOptionsSmartCardRemovalBehavior</span></span>|<span data-ttu-id="15f6f-495">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md);</span><span class="sxs-lookup"><span data-stu-id="15f6f-495">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)</span></span>|<span data-ttu-id="15f6f-496">Этот параметр безопасности определяет, что происходит при удалении смарт-карты пользователя, выполнившего вход в систему, из устройства чтения смарт-карт.</span><span class="sxs-lookup"><span data-stu-id="15f6f-496">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="15f6f-497">Возможные значения: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-497">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="15f6f-498">дефендерсекуритицентердисаблеаппбровсеруи</span><span class="sxs-lookup"><span data-stu-id="15f6f-498">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="15f6f-499">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-499">Boolean</span></span>|<span data-ttu-id="15f6f-500">Используется для отключения отображения области защиты приложений и браузера.</span><span class="sxs-lookup"><span data-stu-id="15f6f-500">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="15f6f-501">дефендерсекуритицентердисаблефамилюи</span><span class="sxs-lookup"><span data-stu-id="15f6f-501">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="15f6f-502">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-502">Boolean</span></span>|<span data-ttu-id="15f6f-503">Используется для отключения отображения области семьи.</span><span class="sxs-lookup"><span data-stu-id="15f6f-503">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="15f6f-504">дефендерсекуритицентердисаблехеалсуи</span><span class="sxs-lookup"><span data-stu-id="15f6f-504">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="15f6f-505">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-505">Boolean</span></span>|<span data-ttu-id="15f6f-506">Используется для отключения отображения области производительности и работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="15f6f-506">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="15f6f-507">дефендерсекуритицентердисабленетворкуи</span><span class="sxs-lookup"><span data-stu-id="15f6f-507">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="15f6f-508">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-508">Boolean</span></span>|<span data-ttu-id="15f6f-509">Используется для отключения отображения зоны "брандмауэр" и "Защита сети".</span><span class="sxs-lookup"><span data-stu-id="15f6f-509">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="15f6f-510">дефендерсекуритицентердисаблевирусуи</span><span class="sxs-lookup"><span data-stu-id="15f6f-510">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="15f6f-511">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-511">Boolean</span></span>|<span data-ttu-id="15f6f-512">Используется для отключения отображения области защиты от вирусов и угроз.</span><span class="sxs-lookup"><span data-stu-id="15f6f-512">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="15f6f-513">дефендерсекуритицентердисаблеаккаунтуи</span><span class="sxs-lookup"><span data-stu-id="15f6f-513">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="15f6f-514">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-514">Boolean</span></span>|<span data-ttu-id="15f6f-515">Используется для отключения отображения области защиты учетных записей.</span><span class="sxs-lookup"><span data-stu-id="15f6f-515">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="15f6f-516">дефендерсекуритицентердисаблеклеартпмуи</span><span class="sxs-lookup"><span data-stu-id="15f6f-516">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="15f6f-517">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-517">Boolean</span></span>|<span data-ttu-id="15f6f-518">Используется для отключения отображения кнопки Очистить доверенный платформенный модуль.</span><span class="sxs-lookup"><span data-stu-id="15f6f-518">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="15f6f-519">дефендерсекуритицентердисаблехардвареуи</span><span class="sxs-lookup"><span data-stu-id="15f6f-519">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="15f6f-520">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-520">Boolean</span></span>|<span data-ttu-id="15f6f-521">Используется для отключения отображения области аппаратной защиты.</span><span class="sxs-lookup"><span data-stu-id="15f6f-521">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="15f6f-522">дефендерсекуритицентердисабленотификатионареауи</span><span class="sxs-lookup"><span data-stu-id="15f6f-522">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="15f6f-523">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-523">Boolean</span></span>|<span data-ttu-id="15f6f-524">Используется для отключения отображения элемента управления "область уведомлений".</span><span class="sxs-lookup"><span data-stu-id="15f6f-524">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="15f6f-525">Для вступления этого параметра в силу пользователю необходимо выйти из системы и войти в нее, а затем перезагрузить компьютер.</span><span class="sxs-lookup"><span data-stu-id="15f6f-525">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="15f6f-526">дефендерсекуритицентердисаблерансомвареуи</span><span class="sxs-lookup"><span data-stu-id="15f6f-526">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="15f6f-527">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-527">Boolean</span></span>|<span data-ttu-id="15f6f-528">Используется для отключения отображения области защиты от пошантажистом.</span><span class="sxs-lookup"><span data-stu-id="15f6f-528">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="15f6f-529">дефендерсекуритицентердисаблесекуребутуи</span><span class="sxs-lookup"><span data-stu-id="15f6f-529">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="15f6f-530">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-530">Boolean</span></span>|<span data-ttu-id="15f6f-531">Используется для отключения отображения области безопасной загрузки в разделе Безопасность устройства.</span><span class="sxs-lookup"><span data-stu-id="15f6f-531">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="15f6f-532">дефендерсекуритицентердисаблетраублешутингуи</span><span class="sxs-lookup"><span data-stu-id="15f6f-532">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="15f6f-533">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-533">Boolean</span></span>|<span data-ttu-id="15f6f-534">Используется для отключения отображения устранения неполадок процесса безопасности в разделе Безопасность устройства.</span><span class="sxs-lookup"><span data-stu-id="15f6f-534">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="15f6f-535">дефендерсекуритицентердисаблевулнераблетпмфирмвареупдатеуи</span><span class="sxs-lookup"><span data-stu-id="15f6f-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="15f6f-536">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-536">Boolean</span></span>|<span data-ttu-id="15f6f-537">Используется для отключения отображения обновления микропрограммы доверенного платформенного модуля при обнаружении уязвимого программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="15f6f-537">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="15f6f-538">дефендерсекуритицентерорганизатиондисплайнаме</span><span class="sxs-lookup"><span data-stu-id="15f6f-538">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="15f6f-539">String</span><span class="sxs-lookup"><span data-stu-id="15f6f-539">String</span></span>|<span data-ttu-id="15f6f-540">Имя компании, которое отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="15f6f-540">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="15f6f-541">дефендерсекуритицентерхелпемаил</span><span class="sxs-lookup"><span data-stu-id="15f6f-541">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="15f6f-542">String</span><span class="sxs-lookup"><span data-stu-id="15f6f-542">String</span></span>|<span data-ttu-id="15f6f-543">Адрес электронной почты, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="15f6f-543">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="15f6f-544">дефендерсекуритицентерхелпфоне</span><span class="sxs-lookup"><span data-stu-id="15f6f-544">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="15f6f-545">String</span><span class="sxs-lookup"><span data-stu-id="15f6f-545">String</span></span>|<span data-ttu-id="15f6f-546">Номер телефона или идентификатор Skype, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="15f6f-546">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="15f6f-547">дефендерсекуритицентерхелпурл</span><span class="sxs-lookup"><span data-stu-id="15f6f-547">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="15f6f-548">String</span><span class="sxs-lookup"><span data-stu-id="15f6f-548">String</span></span>|<span data-ttu-id="15f6f-549">URL-адрес портала справки это отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="15f6f-549">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="15f6f-550">дефендерсекуритицентернотификатионсфромапп</span><span class="sxs-lookup"><span data-stu-id="15f6f-550">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="15f6f-551">дефендерсекуритицентернотификатионсфромапптипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-551">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="15f6f-552">Уведомления, отображаемые в отображаемых областях приложения.</span><span class="sxs-lookup"><span data-stu-id="15f6f-552">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="15f6f-553">Возможные значения: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-553">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="15f6f-554">дефендерсекуритицентеритконтактдисплай</span><span class="sxs-lookup"><span data-stu-id="15f6f-554">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="15f6f-555">дефендерсекуритицентеритконтактдисплайтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-555">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="15f6f-556">Настройка места отображения контактной информации для конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="15f6f-556">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="15f6f-557">Возможные значения: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-557">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="15f6f-558">виндовсдефендертамперпротектион</span><span class="sxs-lookup"><span data-stu-id="15f6f-558">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="15f6f-559">windowsDefenderTamperProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="15f6f-559">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="15f6f-560">Настройка параметров Тамперпротектион для защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="15f6f-560">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="15f6f-561">Возможные значения: `notConfigured`, `enable`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-561">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="15f6f-562">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="15f6f-562">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="15f6f-563">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-563">Boolean</span></span>|<span data-ttu-id="15f6f-564">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="15f6f-564">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="15f6f-565">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="15f6f-565">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="15f6f-566">Int32</span><span class="sxs-lookup"><span data-stu-id="15f6f-566">Int32</span></span>|<span data-ttu-id="15f6f-567">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="15f6f-567">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="15f6f-568">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="15f6f-568">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="15f6f-569">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="15f6f-569">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="15f6f-570">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="15f6f-570">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="15f6f-571">фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-571">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="15f6f-572">Выберите используемую кодировку с общим ключом.</span><span class="sxs-lookup"><span data-stu-id="15f6f-572">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="15f6f-573">Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-573">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="15f6f-574">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="15f6f-574">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="15f6f-575">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-575">Boolean</span></span>|<span data-ttu-id="15f6f-576">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="15f6f-576">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="15f6f-577">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="15f6f-577">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="15f6f-578">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-578">Boolean</span></span>|<span data-ttu-id="15f6f-579">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="15f6f-579">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="15f6f-580">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="15f6f-580">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="15f6f-581">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-581">Boolean</span></span>|<span data-ttu-id="15f6f-582">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="15f6f-582">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="15f6f-583">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="15f6f-583">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="15f6f-584">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-584">Boolean</span></span>|<span data-ttu-id="15f6f-585">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="15f6f-585">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="15f6f-586">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="15f6f-586">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="15f6f-587">фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-587">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="15f6f-588">Укажите способ применения списка отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="15f6f-588">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="15f6f-589">Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-589">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="15f6f-590">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="15f6f-590">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="15f6f-591">Boolean</span><span class="sxs-lookup"><span data-stu-id="15f6f-591">Boolean</span></span>|<span data-ttu-id="15f6f-592">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="15f6f-592">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="15f6f-593">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="15f6f-593">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="15f6f-594">фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-594">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="15f6f-595">Настраивает способ применения очередей пакетов в сценарии туннельного шлюза.</span><span class="sxs-lookup"><span data-stu-id="15f6f-595">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="15f6f-596">Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-596">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="15f6f-597">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="15f6f-597">firewallProfileDomain</span></span>|[<span data-ttu-id="15f6f-598">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="15f6f-598">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="15f6f-599">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="15f6f-599">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="15f6f-600">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="15f6f-600">firewallProfilePublic</span></span>|[<span data-ttu-id="15f6f-601">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="15f6f-601">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="15f6f-602">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="15f6f-602">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="15f6f-603">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="15f6f-603">firewallProfilePrivate</span></span>|[<span data-ttu-id="15f6f-604">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="15f6f-604">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="15f6f-605">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="15f6f-605">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="15f6f-606">дефендерадобереадерлаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="15f6f-606">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="15f6f-607">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-607">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="15f6f-608">Значение, указывающее поведение Adobe Reader при создании дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="15f6f-608">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="15f6f-609">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-609">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-610">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="15f6f-610">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="15f6f-611">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="15f6f-611">String collection</span></span>|<span data-ttu-id="15f6f-612">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="15f6f-612">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="15f6f-613">дефендероффицеаппсосерпроцессинжектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-613">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="15f6f-614">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-614">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="15f6f-615">Значение, указывающее поведение приложений Office, добавляемых в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="15f6f-615">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="15f6f-616">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-616">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-617">дефендероффицеаппсосерпроцессинжектион</span><span class="sxs-lookup"><span data-stu-id="15f6f-617">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="15f6f-618">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-618">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="15f6f-619">Значение, указывающее поведение приложений Office, добавляемых в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="15f6f-619">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="15f6f-620">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-620">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-621">дефендероффицекоммуникатионаппслаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="15f6f-621">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="15f6f-622">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-622">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="15f6f-623">Значение, определяющее поведение приложений для связи с Office, включая Microsoft Outlook, от создания дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="15f6f-623">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="15f6f-624">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-624">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-625">дефендероффицеаппсексекутаблеконтенткреатионорлаунчтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-625">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="15f6f-626">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-626">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="15f6f-627">Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого контента.</span><span class="sxs-lookup"><span data-stu-id="15f6f-627">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="15f6f-628">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-628">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-629">дефендероффицеаппсексекутаблеконтенткреатионорлаунч</span><span class="sxs-lookup"><span data-stu-id="15f6f-629">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="15f6f-630">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-630">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="15f6f-631">Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого контента.</span><span class="sxs-lookup"><span data-stu-id="15f6f-631">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="15f6f-632">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-632">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-633">дефендероффицеаппслаунччилдпроцесстипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-633">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="15f6f-634">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-634">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="15f6f-635">Значение, указывающее поведение запуска приложения Office для дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="15f6f-635">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="15f6f-636">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-636">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-637">дефендероффицеаппслаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="15f6f-637">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="15f6f-638">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-638">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="15f6f-639">Значение, указывающее поведение запуска приложения Office для дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="15f6f-639">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="15f6f-640">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-640">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-641">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="15f6f-641">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="15f6f-642">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-642">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="15f6f-643">Значение, указывающее поведение импорта Win32 из кода макросов в Office.</span><span class="sxs-lookup"><span data-stu-id="15f6f-643">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="15f6f-644">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-644">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-645">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="15f6f-645">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="15f6f-646">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-646">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="15f6f-647">Значение, указывающее поведение импорта Win32 из кода макросов в Office.</span><span class="sxs-lookup"><span data-stu-id="15f6f-647">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="15f6f-648">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-648">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-649">дефендерскриптобфускатедмакрокодетипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-649">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="15f6f-650">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-650">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="15f6f-651">Значение, определяющее поведение кода "замаскированный JS/VBS/PS/макрос".</span><span class="sxs-lookup"><span data-stu-id="15f6f-651">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="15f6f-652">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-652">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-653">дефендерскриптобфускатедмакрокоде</span><span class="sxs-lookup"><span data-stu-id="15f6f-653">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="15f6f-654">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-654">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="15f6f-655">Значение, определяющее поведение кода "замаскированный JS/VBS/PS/макрос".</span><span class="sxs-lookup"><span data-stu-id="15f6f-655">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="15f6f-656">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-656">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-657">дефендерскриптдовнлоадедпайлоадексекутионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-657">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="15f6f-658">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-658">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="15f6f-659">Значение, определяющее поведение JS-и VBS-данных, загруженных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="15f6f-659">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="15f6f-660">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-660">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-661">дефендерскриптдовнлоадедпайлоадексекутион</span><span class="sxs-lookup"><span data-stu-id="15f6f-661">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="15f6f-662">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-662">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="15f6f-663">Значение, определяющее поведение JS-и VBS-данных, загруженных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="15f6f-663">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="15f6f-664">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-664">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-665">дефендерпревенткредентиалстеалингтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-665">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="15f6f-666">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-666">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="15f6f-667">Значение, указывающее, разрешено ли перенос учетных данных из подсистемы локального центра безопасности Windows.</span><span class="sxs-lookup"><span data-stu-id="15f6f-667">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="15f6f-668">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-668">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-669">дефендерпроцесскреатионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-669">defenderProcessCreationType</span></span>|[<span data-ttu-id="15f6f-670">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-670">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="15f6f-671">Значение, указывающее ответ на создание процессов, исходящих от команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="15f6f-671">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="15f6f-672">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-672">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-673">дефендерпроцесскреатион</span><span class="sxs-lookup"><span data-stu-id="15f6f-673">defenderProcessCreation</span></span>|[<span data-ttu-id="15f6f-674">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-674">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="15f6f-675">Значение, указывающее ответ на создание процессов, исходящих от команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="15f6f-675">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="15f6f-676">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-676">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-677">дефендерунтрустедусбпроцесстипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-677">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="15f6f-678">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-678">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="15f6f-679">Значение, указывающее ответ на недоверенные и неподписанные процессы, которые запускаются с USB.</span><span class="sxs-lookup"><span data-stu-id="15f6f-679">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="15f6f-680">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-680">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-681">дефендерунтрустедусбпроцесс</span><span class="sxs-lookup"><span data-stu-id="15f6f-681">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="15f6f-682">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-682">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="15f6f-683">Значение, указывающее ответ на недоверенные и неподписанные процессы, которые запускаются с USB.</span><span class="sxs-lookup"><span data-stu-id="15f6f-683">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="15f6f-684">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-684">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-685">дефендерунтрустедексекутаблетипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-685">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="15f6f-686">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-686">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="15f6f-687">Значение, указывающее ответ на исполняемые файлы, которые не отвечают условиям преобладание, возраст или доверенного списка.</span><span class="sxs-lookup"><span data-stu-id="15f6f-687">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="15f6f-688">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-688">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-689">дефендерунтрустедексекутабле</span><span class="sxs-lookup"><span data-stu-id="15f6f-689">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="15f6f-690">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-690">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="15f6f-691">Значение, указывающее ответ на исполняемые файлы, которые не отвечают условиям преобладание, возраст или доверенного списка.</span><span class="sxs-lookup"><span data-stu-id="15f6f-691">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="15f6f-692">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-692">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-693">дефендеремаилконтентексекутионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-693">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="15f6f-694">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-694">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="15f6f-695">Значение, указывающее, следует ли удалять исполняемые файлы (exe, DLL, PS, JS, VBS и т. д.) из электронной почты (почтовая или почтовая программа).</span><span class="sxs-lookup"><span data-stu-id="15f6f-695">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="15f6f-696">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-696">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-697">дефендеремаилконтентексекутион</span><span class="sxs-lookup"><span data-stu-id="15f6f-697">defenderEmailContentExecution</span></span>|[<span data-ttu-id="15f6f-698">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-698">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="15f6f-699">Значение, указывающее, следует ли удалять исполняемые файлы (exe, DLL, PS, JS, VBS и т. д.) из электронной почты (почтовая или почтовая программа).</span><span class="sxs-lookup"><span data-stu-id="15f6f-699">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="15f6f-700">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-700">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-701">дефендерадванцедрансомеварепротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-701">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="15f6f-702">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-702">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="15f6f-703">Значение, указывающее на использование расширенной защиты в рансомеваре.</span><span class="sxs-lookup"><span data-stu-id="15f6f-703">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="15f6f-704">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-704">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-705">дефендергуардмифолдерстипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-705">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="15f6f-706">фолдерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-706">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="15f6f-707">Значение, указывающее поведение защищенных папок.</span><span class="sxs-lookup"><span data-stu-id="15f6f-707">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="15f6f-708">Возможные значения: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-708">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="15f6f-709">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="15f6f-709">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="15f6f-710">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="15f6f-710">String collection</span></span>|<span data-ttu-id="15f6f-711">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="15f6f-711">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="15f6f-712">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="15f6f-712">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="15f6f-713">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="15f6f-713">String collection</span></span>|<span data-ttu-id="15f6f-714">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="15f6f-714">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="15f6f-715">дефендернетворкпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-715">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="15f6f-716">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-716">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="15f6f-717">Значение, указывающее поведение Нетворкпротектион.</span><span class="sxs-lookup"><span data-stu-id="15f6f-717">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="15f6f-718">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-718">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-719">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="15f6f-719">defenderExploitProtectionXml</span></span>|<span data-ttu-id="15f6f-720">Binary</span><span class="sxs-lookup"><span data-stu-id="15f6f-720">Binary</span></span>|<span data-ttu-id="15f6f-721">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="15f6f-721">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="15f6f-722">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="15f6f-722">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="15f6f-723">String</span><span class="sxs-lookup"><span data-stu-id="15f6f-723">String</span></span>|<span data-ttu-id="15f6f-724">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="15f6f-724">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="15f6f-725">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="15f6f-725">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="15f6f-726">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-726">Boolean</span></span>|<span data-ttu-id="15f6f-727">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="15f6f-727">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="15f6f-728">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="15f6f-728">appLockerApplicationControl</span></span>|[<span data-ttu-id="15f6f-729">апплоккераппликатионконтролтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-729">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="15f6f-730">Позволяет администратору выбирать разрешенные типы приложений для устройств.</span><span class="sxs-lookup"><span data-stu-id="15f6f-730">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="15f6f-731">Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-731">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="15f6f-732">девицегуардлокалсистемаусоритикредентиалгуардсеттингс</span><span class="sxs-lookup"><span data-stu-id="15f6f-732">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="15f6f-733">девицегуардлокалсистемаусоритикредентиалгуардтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-733">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="15f6f-734">Включите Guard в учетных данных, когда включен уровень безопасности платформы с безопасной загрузкой и безопасностью на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="15f6f-734">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="15f6f-735">Возможные значения: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-735">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="15f6f-736">девицегуарденаблевиртуализатионбаседсекурити</span><span class="sxs-lookup"><span data-stu-id="15f6f-736">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="15f6f-737">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-737">Boolean</span></span>|<span data-ttu-id="15f6f-738">Включает безопасность на основе виртуализации (VBS).</span><span class="sxs-lookup"><span data-stu-id="15f6f-738">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="15f6f-739">девицегуарденаблесекуребутвисдма</span><span class="sxs-lookup"><span data-stu-id="15f6f-739">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="15f6f-740">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-740">Boolean</span></span>|<span data-ttu-id="15f6f-741">Это свойство будет устаревшим в 2019 мая и будет заменено свойством Девицегуардсекуребутвисдма.</span><span class="sxs-lookup"><span data-stu-id="15f6f-741">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="15f6f-742">Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="15f6f-742">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="15f6f-743">девицегуардсекуребутвисдма</span><span class="sxs-lookup"><span data-stu-id="15f6f-743">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="15f6f-744">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="15f6f-744">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="15f6f-745">Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="15f6f-745">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="15f6f-746">Возможные значения: `notConfigured`, `withoutDMA`, `withDMA`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-746">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="15f6f-747">девицегуардлаунчсистемгуард</span><span class="sxs-lookup"><span data-stu-id="15f6f-747">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="15f6f-748">Включение</span><span class="sxs-lookup"><span data-stu-id="15f6f-748">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="15f6f-749">Позволяет ИТ – администратору настраивать запуск системы защиты системы.</span><span class="sxs-lookup"><span data-stu-id="15f6f-749">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="15f6f-750">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-750">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="15f6f-751">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="15f6f-751">smartScreenEnableInShell</span></span>|<span data-ttu-id="15f6f-752">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-752">Boolean</span></span>|<span data-ttu-id="15f6f-753">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="15f6f-753">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="15f6f-754">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="15f6f-754">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="15f6f-755">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-755">Boolean</span></span>|<span data-ttu-id="15f6f-756">Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="15f6f-756">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="15f6f-757">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="15f6f-757">applicationGuardEnabled</span></span>|<span data-ttu-id="15f6f-758">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-758">Boolean</span></span>|<span data-ttu-id="15f6f-759">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="15f6f-759">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="15f6f-760">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="15f6f-760">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="15f6f-761">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="15f6f-761">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="15f6f-762">Включение Application Guard в Защитнике Windows для более новых сборок Windows.</span><span class="sxs-lookup"><span data-stu-id="15f6f-762">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="15f6f-763">Возможные значения: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-763">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="15f6f-764">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="15f6f-764">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="15f6f-765">аппликатионгуардблоккфилетрансфертипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-765">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="15f6f-766">Блокировать буфер обмена для передачи файла изображения, текстового файла или ни одного из них.</span><span class="sxs-lookup"><span data-stu-id="15f6f-766">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="15f6f-767">Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-767">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="15f6f-768">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="15f6f-768">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="15f6f-769">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-769">Boolean</span></span>|<span data-ttu-id="15f6f-770">Позволяет заблокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="15f6f-770">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="15f6f-771">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="15f6f-771">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="15f6f-772">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-772">Boolean</span></span>|<span data-ttu-id="15f6f-773">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="15f6f-773">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="15f6f-774">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="15f6f-774">applicationGuardForceAuditing</span></span>|<span data-ttu-id="15f6f-775">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-775">Boolean</span></span>|<span data-ttu-id="15f6f-776">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="15f6f-776">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="15f6f-777">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="15f6f-777">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="15f6f-778">аппликатионгуардблоккклипбоардшарингтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-778">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="15f6f-779">Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="15f6f-779">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="15f6f-780">Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-780">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="15f6f-781">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="15f6f-781">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="15f6f-782">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-782">Boolean</span></span>|<span data-ttu-id="15f6f-783">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="15f6f-783">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="15f6f-784">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="15f6f-784">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="15f6f-785">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-785">Boolean</span></span>|<span data-ttu-id="15f6f-786">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="15f6f-786">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="15f6f-787">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="15f6f-787">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="15f6f-788">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-788">Boolean</span></span>|<span data-ttu-id="15f6f-789">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="15f6f-789">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="15f6f-790">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="15f6f-790">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="15f6f-791">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-791">Boolean</span></span>|<span data-ttu-id="15f6f-792">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="15f6f-792">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="15f6f-793">аппликатионгуардалловвиртуалгпу</span><span class="sxs-lookup"><span data-stu-id="15f6f-793">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="15f6f-794">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-794">Boolean</span></span>|<span data-ttu-id="15f6f-795">Разрешить приложению Application Guard использовать виртуальный GPU</span><span class="sxs-lookup"><span data-stu-id="15f6f-795">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="15f6f-796">аппликатионгуардалловфилесавеонхост</span><span class="sxs-lookup"><span data-stu-id="15f6f-796">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="15f6f-797">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-797">Boolean</span></span>|<span data-ttu-id="15f6f-798">Разрешить пользователям скачивать файлы из EDGE в контейнере Application Guard и сохранять их в файловой системе узла</span><span class="sxs-lookup"><span data-stu-id="15f6f-798">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="15f6f-799">битлоккералловстандардусеренкриптион</span><span class="sxs-lookup"><span data-stu-id="15f6f-799">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="15f6f-800">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-800">Boolean</span></span>|<span data-ttu-id="15f6f-801">Позволяет администратору разрешить обычным пользователям включать енкрпитион во время присоединения к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="15f6f-801">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="15f6f-802">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="15f6f-802">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="15f6f-803">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-803">Boolean</span></span>|<span data-ttu-id="15f6f-804">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="15f6f-804">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="15f6f-805">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="15f6f-805">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="15f6f-806">Boolean</span><span class="sxs-lookup"><span data-stu-id="15f6f-806">Boolean</span></span>|<span data-ttu-id="15f6f-807">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="15f6f-807">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="15f6f-808">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="15f6f-808">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="15f6f-809">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="15f6f-809">bitLockerEncryptDevice</span></span>|<span data-ttu-id="15f6f-810">Boolean</span><span class="sxs-lookup"><span data-stu-id="15f6f-810">Boolean</span></span>|<span data-ttu-id="15f6f-811">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="15f6f-811">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="15f6f-812">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="15f6f-812">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="15f6f-813">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="15f6f-813">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="15f6f-814">Политика системного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="15f6f-814">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="15f6f-815">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="15f6f-815">bitLockerFixedDrivePolicy</span></span>|<span data-ttu-id="15f6f-816">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md);</span><span class="sxs-lookup"><span data-stu-id="15f6f-816">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)</span></span>|<span data-ttu-id="15f6f-817">Политика фиксированного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="15f6f-817">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="15f6f-818">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="15f6f-818">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="15f6f-819">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="15f6f-819">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="15f6f-820">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="15f6f-820">BitLocker Removable Drive Policy.</span></span>|
|<span data-ttu-id="15f6f-821">битлоккеррековерипассвордротатион</span><span class="sxs-lookup"><span data-stu-id="15f6f-821">bitLockerRecoveryPasswordRotation</span></span>|[<span data-ttu-id="15f6f-822">bitLockerRecoveryPasswordRotationType</span><span class="sxs-lookup"><span data-stu-id="15f6f-822">bitLockerRecoveryPasswordRotationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|<span data-ttu-id="15f6f-823">Этот параметр инициирует поворот пароля восстановления на основе клиента после восстановления диска ОС (с помощью BOOTMGR или WinRE).</span><span class="sxs-lookup"><span data-stu-id="15f6f-823">This setting initiates a client-driven recovery password rotation after an OS drive recovery (either by using bootmgr or WinRE).</span></span> <span data-ttu-id="15f6f-824">Возможные значения: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-824">Possible values are: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span></span>|
|<span data-ttu-id="15f6f-825">дефендердисаблесканарчивефилес</span><span class="sxs-lookup"><span data-stu-id="15f6f-825">defenderDisableScanArchiveFiles</span></span>|<span data-ttu-id="15f6f-826">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-826">Boolean</span></span>|<span data-ttu-id="15f6f-827">Разрешает или запрещает сканирование архивов.</span><span class="sxs-lookup"><span data-stu-id="15f6f-827">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="15f6f-828">дефендердисаблебехавиормониторинг</span><span class="sxs-lookup"><span data-stu-id="15f6f-828">defenderDisableBehaviorMonitoring</span></span>|<span data-ttu-id="15f6f-829">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-829">Boolean</span></span>|<span data-ttu-id="15f6f-830">Разрешает или запрещает функции мониторинга режима защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="15f6f-830">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="15f6f-831">дефендердисаблеклаудпротектион</span><span class="sxs-lookup"><span data-stu-id="15f6f-831">defenderDisableCloudProtection</span></span>|<span data-ttu-id="15f6f-832">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-832">Boolean</span></span>|<span data-ttu-id="15f6f-833">Чтобы лучше защитить компьютер, защитник Windows будет отправлять в корпорацию Майкрософт сведения обо всех обнаруженных неполадках.</span><span class="sxs-lookup"><span data-stu-id="15f6f-833">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="15f6f-834">Корпорация Майкрософт проанализирует эти сведения, Узнайте больше об ошибках, которые могут повлиять на ваших клиентов и других пользователей, и предложит улучшенные решения.</span><span class="sxs-lookup"><span data-stu-id="15f6f-834">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="15f6f-835">дефендеренаблесканинкомингмаил</span><span class="sxs-lookup"><span data-stu-id="15f6f-835">defenderEnableScanIncomingMail</span></span>|<span data-ttu-id="15f6f-836">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-836">Boolean</span></span>|<span data-ttu-id="15f6f-837">Разрешает или запрещает сканирование электронной почты.</span><span class="sxs-lookup"><span data-stu-id="15f6f-837">Allows or disallows scanning of email.</span></span>|
|<span data-ttu-id="15f6f-838">дефендеренаблесканмаппеднетворкдривесдурингфуллскан</span><span class="sxs-lookup"><span data-stu-id="15f6f-838">defenderEnableScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="15f6f-839">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-839">Boolean</span></span>|<span data-ttu-id="15f6f-840">Разрешает или запрещает полное сканирование подключенных сетевых дисков.</span><span class="sxs-lookup"><span data-stu-id="15f6f-840">Allows or disallows a full scan of mapped network drives.</span></span>|
|<span data-ttu-id="15f6f-841">дефендердисаблесканремовабледривесдурингфуллскан</span><span class="sxs-lookup"><span data-stu-id="15f6f-841">defenderDisableScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="15f6f-842">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-842">Boolean</span></span>|<span data-ttu-id="15f6f-843">Разрешает или запрещает полное сканирование съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="15f6f-843">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="15f6f-844">Во время быстрого сканирования съемные диски все еще могут сканироваться.</span><span class="sxs-lookup"><span data-stu-id="15f6f-844">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="15f6f-845">дефендердисаблескандовнлоадс</span><span class="sxs-lookup"><span data-stu-id="15f6f-845">defenderDisableScanDownloads</span></span>|<span data-ttu-id="15f6f-846">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-846">Boolean</span></span>|<span data-ttu-id="15f6f-847">Разрешает или запрещает функции защиты ИОАВП защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="15f6f-847">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="15f6f-848">дефендердисаблеинтрусионпревентионсистем</span><span class="sxs-lookup"><span data-stu-id="15f6f-848">defenderDisableIntrusionPreventionSystem</span></span>|<span data-ttu-id="15f6f-849">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-849">Boolean</span></span>|<span data-ttu-id="15f6f-850">Разрешает или запрещает функции предотвращения вторжения в Защитнике Windows.</span><span class="sxs-lookup"><span data-stu-id="15f6f-850">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="15f6f-851">дефендердисаблеонакцесспротектион</span><span class="sxs-lookup"><span data-stu-id="15f6f-851">defenderDisableOnAccessProtection</span></span>|<span data-ttu-id="15f6f-852">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-852">Boolean</span></span>|<span data-ttu-id="15f6f-853">Разрешает или запрещает защитник Windows для функций защиты доступа.</span><span class="sxs-lookup"><span data-stu-id="15f6f-853">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="15f6f-854">дефендердисаблереалтимемониторинг</span><span class="sxs-lookup"><span data-stu-id="15f6f-854">defenderDisableRealTimeMonitoring</span></span>|<span data-ttu-id="15f6f-855">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-855">Boolean</span></span>|<span data-ttu-id="15f6f-856">Разрешает или запрещает функции мониторинга в режиме реального времени защитник Windows.</span><span class="sxs-lookup"><span data-stu-id="15f6f-856">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="15f6f-857">дефендердисаблесканнетворкфилес</span><span class="sxs-lookup"><span data-stu-id="15f6f-857">defenderDisableScanNetworkFiles</span></span>|<span data-ttu-id="15f6f-858">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-858">Boolean</span></span>|<span data-ttu-id="15f6f-859">Разрешает или запрещает сканирование сетевых файлов.</span><span class="sxs-lookup"><span data-stu-id="15f6f-859">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="15f6f-860">дефендердисаблесканскриптслоадедининтернетексплорер</span><span class="sxs-lookup"><span data-stu-id="15f6f-860">defenderDisableScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="15f6f-861">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-861">Boolean</span></span>|<span data-ttu-id="15f6f-862">Разрешает или запрещает функцию сканирования сценариев защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="15f6f-862">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="15f6f-863">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="15f6f-863">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="15f6f-864">Boolean</span><span class="sxs-lookup"><span data-stu-id="15f6f-864">Boolean</span></span>|<span data-ttu-id="15f6f-865">Разрешает или запрещает пользователям доступ к пользовательскому интерфейсу защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="15f6f-865">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="15f6f-866">Если этот флажок не разрешен, все уведомления защитника Windows также будут подавляться.</span><span class="sxs-lookup"><span data-stu-id="15f6f-866">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="15f6f-867">дефендерсканмакскпуперцентаже</span><span class="sxs-lookup"><span data-stu-id="15f6f-867">defenderScanMaxCpuPercentage</span></span>|<span data-ttu-id="15f6f-868">Int32</span><span class="sxs-lookup"><span data-stu-id="15f6f-868">Int32</span></span>|<span data-ttu-id="15f6f-869">Представляет средний коэффициент загрузки ЦП для сканирования защитником Windows (в процентах).</span><span class="sxs-lookup"><span data-stu-id="15f6f-869">Represents the average CPU load factor for the Windows Defender scan (in percent).</span></span> <span data-ttu-id="15f6f-870">Значение по умолчанию равно 50.</span><span class="sxs-lookup"><span data-stu-id="15f6f-870">The default value is 50.</span></span> <span data-ttu-id="15f6f-871">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="15f6f-871">Valid values 0 to 100</span></span>|
|<span data-ttu-id="15f6f-872">дефендерчеккфорсигнатуресбефореруннингскан</span><span class="sxs-lookup"><span data-stu-id="15f6f-872">defenderCheckForSignaturesBeforeRunningScan</span></span>|<span data-ttu-id="15f6f-873">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-873">Boolean</span></span>|<span data-ttu-id="15f6f-874">Этот параметр политики позволяет управлять тем, будет ли выполняться проверка новых определений вирусов и программ-шпионов перед выполнением проверки.</span><span class="sxs-lookup"><span data-stu-id="15f6f-874">This policy setting allows you to manage whether a check for new virus and spyware definitions will occur before running a scan.</span></span>|
|<span data-ttu-id="15f6f-875">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="15f6f-875">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="15f6f-876">дефендерклаудблокклевелтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-876">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="15f6f-877">Добавлено в Windows 10 версии 1709.</span><span class="sxs-lookup"><span data-stu-id="15f6f-877">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="15f6f-878">Этот параметр политики определяет, как активно антивирусная программа "Защитник Windows" будет блокировать и сканировать подозрительные файлы.</span><span class="sxs-lookup"><span data-stu-id="15f6f-878">This policy setting determines how aggressive Windows Defender Antivirus will be in blocking and scanning suspicious files.</span></span> <span data-ttu-id="15f6f-879">Тип значения: целое число.</span><span class="sxs-lookup"><span data-stu-id="15f6f-879">Value type is integer.</span></span> <span data-ttu-id="15f6f-880">Для работы этой функции необходимо включить параметр "присоединение к Microsoft MAPS".</span><span class="sxs-lookup"><span data-stu-id="15f6f-880">This feature requires the "Join Microsoft MAPS" setting enabled in order to function.</span></span> <span data-ttu-id="15f6f-881">Возможные значения: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-881">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="15f6f-882">дефендерклаудекстендедтимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="15f6f-882">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="15f6f-883">Int32</span><span class="sxs-lookup"><span data-stu-id="15f6f-883">Int32</span></span>|<span data-ttu-id="15f6f-884">Добавлено в Windows 10 версии 1709.</span><span class="sxs-lookup"><span data-stu-id="15f6f-884">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="15f6f-885">Эта функция позволяет антивирусной программе "Защитник Windows" заблокировать подозрительный файл размером до 60 секунд и проверить его в облаке, чтобы убедиться, что он безопасен.</span><span class="sxs-lookup"><span data-stu-id="15f6f-885">This feature allows Windows Defender Antivirus to block a suspicious file for up to 60 seconds, and scan it in the cloud to make sure it's safe.</span></span> <span data-ttu-id="15f6f-886">Тип значения: целое число, Range — 0-50.</span><span class="sxs-lookup"><span data-stu-id="15f6f-886">Value type is integer, range is 0 - 50.</span></span> <span data-ttu-id="15f6f-887">Эта функция зависит от трех других параметров карт, которые должны быть включены — "Настройка блока при первом пошаговом отображении"; " Присоединяйтесь к Microsoft MAPS "; "Отправлять образцы файлов, когда необходим дальнейший анализ".</span><span class="sxs-lookup"><span data-stu-id="15f6f-887">This feature depends on three other MAPS settings the must all be enabled- "Configure the 'Block at First Sight' feature; "Join Microsoft MAPS"; "Send file samples when further analysis is required".</span></span> <span data-ttu-id="15f6f-888">Допустимые значения: от 0 до 50.</span><span class="sxs-lookup"><span data-stu-id="15f6f-888">Valid values 0 to 50</span></span>|
|<span data-ttu-id="15f6f-889">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="15f6f-889">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="15f6f-890">Int32</span><span class="sxs-lookup"><span data-stu-id="15f6f-890">Int32</span></span>|<span data-ttu-id="15f6f-891">Период времени (в днях), в течение которого элементы, помещенные в карантин, будут храниться в системе.</span><span class="sxs-lookup"><span data-stu-id="15f6f-891">Time period (in days) that quarantine items will be stored on the system.</span></span> <span data-ttu-id="15f6f-892">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="15f6f-892">Valid values 0 to 90</span></span>|
|<span data-ttu-id="15f6f-893">дефендердисаблекатчупфуллскан</span><span class="sxs-lookup"><span data-stu-id="15f6f-893">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="15f6f-894">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-894">Boolean</span></span>|<span data-ttu-id="15f6f-895">Этот параметр политики позволяет настроить поиск по расписанию для полного сканирования.</span><span class="sxs-lookup"><span data-stu-id="15f6f-895">This policy setting allows you to configure catch-up scans for scheduled full scans.</span></span> <span data-ttu-id="15f6f-896">Вторичное сканирование — это сканирование, которое инициируется из-за пропускной ошибки запланированной проверки.</span><span class="sxs-lookup"><span data-stu-id="15f6f-896">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="15f6f-897">Обычно эти запланированные проверки пропущены, так как компьютер был отключен в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="15f6f-897">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="15f6f-898">дефендердисаблекатчупкуиккскан</span><span class="sxs-lookup"><span data-stu-id="15f6f-898">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="15f6f-899">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-899">Boolean</span></span>|<span data-ttu-id="15f6f-900">Этот параметр политики позволяет настроить дополнительные проверки для запланированных быстрых проверок.</span><span class="sxs-lookup"><span data-stu-id="15f6f-900">This policy setting allows you to configure catch-up scans for scheduled quick scans.</span></span> <span data-ttu-id="15f6f-901">Вторичное сканирование — это сканирование, которое инициируется из-за пропускной ошибки запланированной проверки.</span><span class="sxs-lookup"><span data-stu-id="15f6f-901">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="15f6f-902">Обычно эти запланированные проверки пропущены, так как компьютер был отключен в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="15f6f-902">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="15f6f-903">дефендеренаблеловкпуприорити</span><span class="sxs-lookup"><span data-stu-id="15f6f-903">defenderEnableLowCpuPriority</span></span>|<span data-ttu-id="15f6f-904">Логический</span><span class="sxs-lookup"><span data-stu-id="15f6f-904">Boolean</span></span>|<span data-ttu-id="15f6f-905">Этот параметр политики позволяет включать или отключать минимальный приоритет ЦП для запланированных проверок.</span><span class="sxs-lookup"><span data-stu-id="15f6f-905">This policy setting allows you to enable or disable low CPU priority for scheduled scans.</span></span>|
|<span data-ttu-id="15f6f-906">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="15f6f-906">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="15f6f-907">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="15f6f-907">String collection</span></span>|<span data-ttu-id="15f6f-908">Расширения файлов, которые необходимо исключить из проверки и защиты в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="15f6f-908">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="15f6f-909">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="15f6f-909">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="15f6f-910">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="15f6f-910">String collection</span></span>|<span data-ttu-id="15f6f-911">Файлы и папки, которые необходимо исключить из проверки и защиты в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="15f6f-911">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="15f6f-912">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="15f6f-912">defenderProcessesToExclude</span></span>|<span data-ttu-id="15f6f-913">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="15f6f-913">String collection</span></span>|<span data-ttu-id="15f6f-914">Процессы, которые необходимо исключить из проверки и защиты в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="15f6f-914">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="15f6f-915">дефендерпотентиаллюнвантедаппактион</span><span class="sxs-lookup"><span data-stu-id="15f6f-915">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="15f6f-916">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="15f6f-916">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="15f6f-917">Добавлено в Windows 10 версии 1607.</span><span class="sxs-lookup"><span data-stu-id="15f6f-917">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="15f6f-918">Задает уровень обнаружения для потенциально нежелательных приложений (Пуас).</span><span class="sxs-lookup"><span data-stu-id="15f6f-918">Specifies the level of detection for potentially unwanted applications (PUAs).</span></span> <span data-ttu-id="15f6f-919">Защитник Windows предупреждает вас о том, что загружается потенциально нежелательное программное обеспечение, или пытается установить себя на компьютер.</span><span class="sxs-lookup"><span data-stu-id="15f6f-919">Windows Defender alerts you when potentially unwanted software is being downloaded or attempts to install itself on your computer.</span></span> <span data-ttu-id="15f6f-920">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-920">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="15f6f-921">дефендерскандиректион</span><span class="sxs-lookup"><span data-stu-id="15f6f-921">defenderScanDirection</span></span>|[<span data-ttu-id="15f6f-922">defenderRealtimeScanDirection</span><span class="sxs-lookup"><span data-stu-id="15f6f-922">defenderRealtimeScanDirection</span></span>](../resources/intune-deviceconfig-defenderrealtimescandirection.md)|<span data-ttu-id="15f6f-923">Определяет, какие наборы файлов следует отслеживать.</span><span class="sxs-lookup"><span data-stu-id="15f6f-923">Controls which sets of files should be monitored.</span></span> <span data-ttu-id="15f6f-924">Возможные значения: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-924">Possible values are: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="15f6f-925">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="15f6f-925">defenderScanType</span></span>|[<span data-ttu-id="15f6f-926">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="15f6f-926">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="15f6f-927">Позволяет выбрать, следует ли выполнять быструю или полную проверку.</span><span class="sxs-lookup"><span data-stu-id="15f6f-927">Selects whether to perform a quick scan or full scan.</span></span> <span data-ttu-id="15f6f-928">Возможные значения: `userDefined`, `disabled`, `quick`, `full`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-928">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="15f6f-929">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="15f6f-929">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="15f6f-930">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="15f6f-930">TimeOfDay</span></span>|<span data-ttu-id="15f6f-931">Выбирает время суток, которое должно выполняться при запуске быстрого сканирования защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="15f6f-931">Selects the time of day that the Windows Defender quick scan should run.</span></span> <span data-ttu-id="15f6f-932">Например, значение 0 = 12:00AM, значение 60 = 1:00AM, значение 120 = 2:00 и т. д., вплоть до значения 1380 = 11:00PM.</span><span class="sxs-lookup"><span data-stu-id="15f6f-932">For example, a value of 0=12:00AM, a value of 60=1:00AM, a value of 120=2:00, and so on, up to a value of 1380=11:00PM.</span></span> <span data-ttu-id="15f6f-933">Значение по умолчанию — 120</span><span class="sxs-lookup"><span data-stu-id="15f6f-933">The default value is 120</span></span>|
|<span data-ttu-id="15f6f-934">дефендерсчедуледскандай</span><span class="sxs-lookup"><span data-stu-id="15f6f-934">defenderScheduledScanDay</span></span>|[<span data-ttu-id="15f6f-935">виклисчедуле</span><span class="sxs-lookup"><span data-stu-id="15f6f-935">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="15f6f-936">Выбирает день запуска проверки защитником Windows.</span><span class="sxs-lookup"><span data-stu-id="15f6f-936">Selects the day that the Windows Defender scan should run.</span></span> <span data-ttu-id="15f6f-937">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-937">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="15f6f-938">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="15f6f-938">defenderScheduledScanTime</span></span>|<span data-ttu-id="15f6f-939">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="15f6f-939">TimeOfDay</span></span>|<span data-ttu-id="15f6f-940">Выбирает время суток, в течение которого должно выполняться сканирование защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="15f6f-940">Selects the time of day that the Windows Defender scan should run.</span></span>|
|<span data-ttu-id="15f6f-941">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="15f6f-941">defenderSubmitSamplesConsentType</span></span>|<span data-ttu-id="15f6f-942">[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md);</span><span class="sxs-lookup"><span data-stu-id="15f6f-942">[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)</span></span>|<span data-ttu-id="15f6f-943">Проверка уровня согласия пользователя в Защитнике Windows для отправки данных.</span><span class="sxs-lookup"><span data-stu-id="15f6f-943">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="15f6f-944">Возможные значения: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span><span class="sxs-lookup"><span data-stu-id="15f6f-944">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="15f6f-945">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="15f6f-945">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="15f6f-946">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="15f6f-946">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="15f6f-947">Позволяет администратору указать допустимые уровни серьезности угроз и соответствующий идентификатор действия по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="15f6f-947">Allows an administrator to specify any valid threat severity levels and the corresponding default action ID to take.</span></span>|



## <a name="response"></a><span data-ttu-id="15f6f-948">Отклик</span><span class="sxs-lookup"><span data-stu-id="15f6f-948">Response</span></span>
<span data-ttu-id="15f6f-949">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="15f6f-949">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15f6f-950">Пример</span><span class="sxs-lookup"><span data-stu-id="15f6f-950">Example</span></span>

### <a name="request"></a><span data-ttu-id="15f6f-951">Запрос</span><span class="sxs-lookup"><span data-stu-id="15f6f-951">Request</span></span>
<span data-ttu-id="15f6f-952">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15f6f-952">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 30451

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
  "bitLockerRecoveryPasswordRotation": "disabled",
  "defenderDisableScanArchiveFiles": true,
  "defenderDisableBehaviorMonitoring": true,
  "defenderDisableCloudProtection": true,
  "defenderEnableScanIncomingMail": true,
  "defenderEnableScanMappedNetworkDrivesDuringFullScan": true,
  "defenderDisableScanRemovableDrivesDuringFullScan": true,
  "defenderDisableScanDownloads": true,
  "defenderDisableIntrusionPreventionSystem": true,
  "defenderDisableOnAccessProtection": true,
  "defenderDisableRealTimeMonitoring": true,
  "defenderDisableScanNetworkFiles": true,
  "defenderDisableScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderScanMaxCpuPercentage": 12,
  "defenderCheckForSignaturesBeforeRunningScan": true,
  "defenderCloudBlockLevel": "high",
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDisableCatchupFullScan": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderEnableLowCpuPriority": true,
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPotentiallyUnwantedAppAction": "enable",
  "defenderScanDirection": "monitorIncomingFilesOnly",
  "defenderScanType": "disabled",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderScheduledScanDay": "everyday",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  }
}
```

### <a name="response"></a><span data-ttu-id="15f6f-953">Отклик</span><span class="sxs-lookup"><span data-stu-id="15f6f-953">Response</span></span>
<span data-ttu-id="15f6f-p221">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15f6f-p221">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 30623

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
  "bitLockerRecoveryPasswordRotation": "disabled",
  "defenderDisableScanArchiveFiles": true,
  "defenderDisableBehaviorMonitoring": true,
  "defenderDisableCloudProtection": true,
  "defenderEnableScanIncomingMail": true,
  "defenderEnableScanMappedNetworkDrivesDuringFullScan": true,
  "defenderDisableScanRemovableDrivesDuringFullScan": true,
  "defenderDisableScanDownloads": true,
  "defenderDisableIntrusionPreventionSystem": true,
  "defenderDisableOnAccessProtection": true,
  "defenderDisableRealTimeMonitoring": true,
  "defenderDisableScanNetworkFiles": true,
  "defenderDisableScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderScanMaxCpuPercentage": 12,
  "defenderCheckForSignaturesBeforeRunningScan": true,
  "defenderCloudBlockLevel": "high",
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDisableCatchupFullScan": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderEnableLowCpuPriority": true,
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPotentiallyUnwantedAppAction": "enable",
  "defenderScanDirection": "monitorIncomingFilesOnly",
  "defenderScanType": "disabled",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderScheduledScanDay": "everyday",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  }
}
```





