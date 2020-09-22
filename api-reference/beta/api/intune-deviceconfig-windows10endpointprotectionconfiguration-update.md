---
title: Обновление объекта windows10EndpointProtectionConfiguration
description: Обновляет свойства объекта windows10EndpointProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2c36ac4ef440d0548730048413c4a32a59c68b1a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48068800"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="6e70b-103">Обновление объекта windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e70b-103">Update windows10EndpointProtectionConfiguration</span></span>

<span data-ttu-id="6e70b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e70b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e70b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e70b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e70b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e70b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e70b-107">Обновляет свойства объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e70b-107">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e70b-108">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="6e70b-108">Prerequisites</span></span>
<span data-ttu-id="6e70b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e70b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e70b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e70b-111">Permission type</span></span>|<span data-ttu-id="6e70b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e70b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e70b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e70b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e70b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e70b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e70b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e70b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e70b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e70b-116">Not supported.</span></span>|
|<span data-ttu-id="6e70b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e70b-117">Application</span></span>|<span data-ttu-id="6e70b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e70b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e70b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e70b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6e70b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6e70b-120">Request headers</span></span>
|<span data-ttu-id="6e70b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e70b-121">Header</span></span>|<span data-ttu-id="6e70b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6e70b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e70b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e70b-123">Authorization</span></span>|<span data-ttu-id="6e70b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e70b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e70b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6e70b-125">Accept</span></span>|<span data-ttu-id="6e70b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e70b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e70b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e70b-127">Request body</span></span>
<span data-ttu-id="6e70b-128">В теле запроса добавьте представление объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e70b-128">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="6e70b-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e70b-129">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="6e70b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e70b-130">Property</span></span>|<span data-ttu-id="6e70b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6e70b-131">Type</span></span>|<span data-ttu-id="6e70b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6e70b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e70b-133">id</span><span class="sxs-lookup"><span data-stu-id="6e70b-133">id</span></span>|<span data-ttu-id="6e70b-134">String</span><span class="sxs-lookup"><span data-stu-id="6e70b-134">String</span></span>|<span data-ttu-id="6e70b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6e70b-135">Key of the entity.</span></span> <span data-ttu-id="6e70b-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e70b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e70b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e70b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6e70b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e70b-138">DateTimeOffset</span></span>|<span data-ttu-id="6e70b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6e70b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6e70b-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e70b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e70b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6e70b-141">roleScopeTagIds</span></span>|<span data-ttu-id="6e70b-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6e70b-142">String collection</span></span>|<span data-ttu-id="6e70b-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6e70b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6e70b-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e70b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e70b-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="6e70b-145">supportsScopeTags</span></span>|<span data-ttu-id="6e70b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-146">Boolean</span></span>|<span data-ttu-id="6e70b-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="6e70b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6e70b-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="6e70b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6e70b-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6e70b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6e70b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e70b-150">This property is read-only.</span></span> <span data-ttu-id="6e70b-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e70b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e70b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6e70b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6e70b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6e70b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6e70b-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6e70b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6e70b-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e70b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e70b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6e70b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6e70b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6e70b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6e70b-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6e70b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6e70b-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e70b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e70b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6e70b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6e70b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6e70b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6e70b-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6e70b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6e70b-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e70b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e70b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e70b-164">createdDateTime</span></span>|<span data-ttu-id="6e70b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e70b-165">DateTimeOffset</span></span>|<span data-ttu-id="6e70b-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6e70b-166">DateTime the object was created.</span></span> <span data-ttu-id="6e70b-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e70b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e70b-168">description</span><span class="sxs-lookup"><span data-stu-id="6e70b-168">description</span></span>|<span data-ttu-id="6e70b-169">String</span><span class="sxs-lookup"><span data-stu-id="6e70b-169">String</span></span>|<span data-ttu-id="6e70b-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6e70b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6e70b-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e70b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e70b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="6e70b-172">displayName</span></span>|<span data-ttu-id="6e70b-173">String</span><span class="sxs-lookup"><span data-stu-id="6e70b-173">String</span></span>|<span data-ttu-id="6e70b-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6e70b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6e70b-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e70b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e70b-176">version</span><span class="sxs-lookup"><span data-stu-id="6e70b-176">version</span></span>|<span data-ttu-id="6e70b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6e70b-177">Int32</span></span>|<span data-ttu-id="6e70b-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6e70b-178">Version of the device configuration.</span></span> <span data-ttu-id="6e70b-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e70b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e70b-180">дмагуарддевицеенумератионполици</span><span class="sxs-lookup"><span data-stu-id="6e70b-180">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="6e70b-181">дмагуарддевицеенумератионполицитипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-181">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="6e70b-182">Эта политика предназначена для обеспечения дополнительной защиты от внешних устройств с поддержкой прямого доступа к памяти.</span><span class="sxs-lookup"><span data-stu-id="6e70b-182">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="6e70b-183">Он обеспечивает более полный контроль над перечислением устройств с поддержкой внешних устройств с поддержкой прямого доступа к памяти, несовместимых с пересопоставлением и изоляцией памяти устройств и изолированной средой.</span><span class="sxs-lookup"><span data-stu-id="6e70b-183">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="6e70b-184">Эта политика вступает в силу только тогда, когда система защиты DMA поддерживается и включена встроенным встроенным по.</span><span class="sxs-lookup"><span data-stu-id="6e70b-184">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="6e70b-185">Защита от DMA ядра — это компонент платформы, который невозможно контролировать с помощью политики или конечным пользователем.</span><span class="sxs-lookup"><span data-stu-id="6e70b-185">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="6e70b-186">Она должна поддерживаться системой на момент производства.</span><span class="sxs-lookup"><span data-stu-id="6e70b-186">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="6e70b-187">Чтобы проверить, поддерживает ли система защиту DMA, проверьте поле Защита ядра DMA на странице сводки MSINFO32.exe.</span><span class="sxs-lookup"><span data-stu-id="6e70b-187">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="6e70b-188">Возможные значения: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-188">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="6e70b-189">фиреваллрулес</span><span class="sxs-lookup"><span data-stu-id="6e70b-189">firewallRules</span></span>|<span data-ttu-id="6e70b-190">Коллекция [виндовсфиреваллруле](../resources/intune-deviceconfig-windowsfirewallrule.md)</span><span class="sxs-lookup"><span data-stu-id="6e70b-190">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="6e70b-191">Настраивает параметры правила брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="6e70b-191">Configures the firewall rule settings.</span></span> <span data-ttu-id="6e70b-192">Эта коллекция может содержать не более 150 элементов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-192">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="6e70b-193">усерригхтсакцесскредентиалманажераструстедкаллер</span><span class="sxs-lookup"><span data-stu-id="6e70b-193">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="6e70b-194">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-194">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-195">Это право пользователя используется диспетчером учетных данных во время резервного копирования и восстановления.</span><span class="sxs-lookup"><span data-stu-id="6e70b-195">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="6e70b-196">Сохраненные учетные данные пользователей могут быть скомпрометированы, если эта привилегия передана другим субъектам.</span><span class="sxs-lookup"><span data-stu-id="6e70b-196">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="6e70b-197">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e70b-198">усерригхтсалловакцессфромнетворк</span><span class="sxs-lookup"><span data-stu-id="6e70b-198">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="6e70b-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-200">Это право пользователя определяет, какие пользователи и группы могут подключаться к компьютеру через сеть.</span><span class="sxs-lookup"><span data-stu-id="6e70b-200">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="6e70b-201">Допустимое состояние — Supported.</span><span class="sxs-lookup"><span data-stu-id="6e70b-201">State Allowed is supported.</span></span>|
|<span data-ttu-id="6e70b-202">усерригхтсблоккакцессфромнетворк</span><span class="sxs-lookup"><span data-stu-id="6e70b-202">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="6e70b-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-204">Это право пользователя определяет, каким пользователям и группам запрещается подключаться к компьютеру через сеть.</span><span class="sxs-lookup"><span data-stu-id="6e70b-204">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="6e70b-205">Блок состояния поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e70b-205">State Block is supported.</span></span>|
|<span data-ttu-id="6e70b-206">усерригхтсактаспартофсеоператингсистем</span><span class="sxs-lookup"><span data-stu-id="6e70b-206">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="6e70b-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-208">Это право пользователя позволяет процессу олицетворять любого пользователя без проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="6e70b-208">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="6e70b-209">Таким образом, процесс может получить доступ к тем же локальным ресурсам, что и пользователь.</span><span class="sxs-lookup"><span data-stu-id="6e70b-209">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="6e70b-210">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e70b-211">усерригхтслокаллогон</span><span class="sxs-lookup"><span data-stu-id="6e70b-211">userRightsLocalLogOn</span></span>|[<span data-ttu-id="6e70b-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-213">Это право пользователя определяет, какие пользователи могут входить на компьютер.</span><span class="sxs-lookup"><span data-stu-id="6e70b-213">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="6e70b-214">Допустимые состояния NotConfigured, Поддерживаемые</span><span class="sxs-lookup"><span data-stu-id="6e70b-214">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="6e70b-215">усерригхтсденилокаллогон</span><span class="sxs-lookup"><span data-stu-id="6e70b-215">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="6e70b-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-217">Это право пользователя определяет, какие пользователи не могут войти на компьютер.</span><span class="sxs-lookup"><span data-stu-id="6e70b-217">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="6e70b-218">Состояния NotConfigured, блокировки поддерживаются</span><span class="sxs-lookup"><span data-stu-id="6e70b-218">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="6e70b-219">усерригхтсбаккупдата</span><span class="sxs-lookup"><span data-stu-id="6e70b-219">userRightsBackupData</span></span>|[<span data-ttu-id="6e70b-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-221">Это право пользователя определяет, какие пользователи могут обходить разрешения для файлов, каталогов, реестра и других постоянных объектов при резервном копировании файлов и каталогов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-221">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="6e70b-222">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e70b-223">усерригхтсчанжесистемтиме</span><span class="sxs-lookup"><span data-stu-id="6e70b-223">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="6e70b-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-225">Это право пользователя определяет, какие пользователи и группы могут изменять время и дату на внутреннем часовом компьютере.</span><span class="sxs-lookup"><span data-stu-id="6e70b-225">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="6e70b-226">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e70b-227">усерригхтскреатеглобалобжектс</span><span class="sxs-lookup"><span data-stu-id="6e70b-227">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="6e70b-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-229">Этот параметр безопасности определяет, могут ли пользователи создавать глобальные объекты, доступные для всех сеансов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-229">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="6e70b-230">Пользователи, которые могут создавать глобальные объекты, могут повлиять на процессы, выполняемые в сеансах других пользователей, что может привести к сбою приложения или повреждению данных.</span><span class="sxs-lookup"><span data-stu-id="6e70b-230">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="6e70b-231">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-231">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e70b-232">усерригхтскреатепажефиле</span><span class="sxs-lookup"><span data-stu-id="6e70b-232">userRightsCreatePageFile</span></span>|[<span data-ttu-id="6e70b-233">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-233">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-234">Это право пользователя определяет, какие пользователи и группы могут вызывать внутренний API, чтобы создать и изменить размер файла подкачки.</span><span class="sxs-lookup"><span data-stu-id="6e70b-234">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="6e70b-235">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-235">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e70b-236">усерригхтскреатеперманентшаредобжектс</span><span class="sxs-lookup"><span data-stu-id="6e70b-236">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="6e70b-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-238">Это право пользователя определяет, какие учетные записи могут использоваться процессами для создания объекта каталога с помощью диспетчера объектов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-238">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="6e70b-239">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-239">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e70b-240">усерригхтскреатесимболиклинкс</span><span class="sxs-lookup"><span data-stu-id="6e70b-240">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="6e70b-241">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-241">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-242">Это право пользователя определяет, может ли пользователь создать символическую ссылку с компьютера, на который они входили.</span><span class="sxs-lookup"><span data-stu-id="6e70b-242">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="6e70b-243">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-243">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e70b-244">усерригхтскреатетокен</span><span class="sxs-lookup"><span data-stu-id="6e70b-244">userRightsCreateToken</span></span>|[<span data-ttu-id="6e70b-245">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-245">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-246">Это право пользователя определяет, какие пользователи и группы могут использоваться процессами для создания маркера, который можно использовать для получения доступа к любому локальному ресурсу, когда процесс использует внутренний API для создания маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="6e70b-246">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="6e70b-247">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-247">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e70b-248">усерригхтсдебугпрограмс</span><span class="sxs-lookup"><span data-stu-id="6e70b-248">userRightsDebugPrograms</span></span>|[<span data-ttu-id="6e70b-249">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-249">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-250">Это право пользователя определяет, какие пользователи могут прикреплять отладчик к любому процессу или ядру.</span><span class="sxs-lookup"><span data-stu-id="6e70b-250">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="6e70b-251">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-251">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e70b-252">усерригхтсремотедесктопсервицеслогон</span><span class="sxs-lookup"><span data-stu-id="6e70b-252">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="6e70b-253">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-253">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-254">Это право пользователя определяет, каким пользователям и группам запрещается вход в систему в качестве клиента служб удаленных рабочих столов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-254">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="6e70b-255">Поддерживаются только состояния NotConfigured и Block</span><span class="sxs-lookup"><span data-stu-id="6e70b-255">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="6e70b-256">усерригхтсделегатион</span><span class="sxs-lookup"><span data-stu-id="6e70b-256">userRightsDelegation</span></span>|[<span data-ttu-id="6e70b-257">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-257">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-258">Это право пользователя определяет, какие пользователи могут устанавливать параметр "доверять для делегирования" для объекта пользователя или компьютера.</span><span class="sxs-lookup"><span data-stu-id="6e70b-258">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="6e70b-259">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-259">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e70b-260">усерригхтсженератесекуритяудитс</span><span class="sxs-lookup"><span data-stu-id="6e70b-260">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="6e70b-261">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-261">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-262">Это право пользователя определяет, какие учетные записи могут использоваться процессом для добавления записей в журнал безопасности.</span><span class="sxs-lookup"><span data-stu-id="6e70b-262">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="6e70b-263">Журнал безопасности используется для трассировки несанкционированного доступа к системе.</span><span class="sxs-lookup"><span data-stu-id="6e70b-263">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="6e70b-264">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e70b-265">усерригхтсимперсонатеклиент</span><span class="sxs-lookup"><span data-stu-id="6e70b-265">userRightsImpersonateClient</span></span>|[<span data-ttu-id="6e70b-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-267">Назначение этого права пользователю позволяет программам, выполняемым от имени этого пользователя, олицетворять клиента.</span><span class="sxs-lookup"><span data-stu-id="6e70b-267">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="6e70b-268">Требование этого пользователя для такого рода олицетворения запрещает несанкционированному пользователю подключаться к созданной им службе, а затем олицетворять этого клиента, что может повысить уровень разрешений неавторизованного пользователя до уровня администратора или уровня системы.</span><span class="sxs-lookup"><span data-stu-id="6e70b-268">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="6e70b-269">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-269">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e70b-270">усерригхтсинкреасесчедулингприорити</span><span class="sxs-lookup"><span data-stu-id="6e70b-270">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="6e70b-271">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-271">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-272">Это право пользователя определяет, какие учетные записи могут использовать процесс с доступом к свойствам Write для другого процесса, чтобы увеличить приоритет выполнения, назначенный другому процессу.</span><span class="sxs-lookup"><span data-stu-id="6e70b-272">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="6e70b-273">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-273">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e70b-274">усерригхтслоадунлоаддриверс</span><span class="sxs-lookup"><span data-stu-id="6e70b-274">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="6e70b-275">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-275">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-276">Это право пользователя определяет, какие пользователи могут динамически загружать и выгружать драйверы устройств или другой код в режиме ядра.</span><span class="sxs-lookup"><span data-stu-id="6e70b-276">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="6e70b-277">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e70b-278">усерригхтслоккмемори</span><span class="sxs-lookup"><span data-stu-id="6e70b-278">userRightsLockMemory</span></span>|[<span data-ttu-id="6e70b-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-280">Это право пользователя определяет, какие учетные записи могут использовать процесс для хранения данных в физической памяти, что предотвращает их разбиение данных на виртуальную память на диске.</span><span class="sxs-lookup"><span data-stu-id="6e70b-280">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="6e70b-281">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e70b-282">усерригхтсманажеаудитингандсекуритилогс</span><span class="sxs-lookup"><span data-stu-id="6e70b-282">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="6e70b-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-284">Это право пользователя определяет, какие пользователи могут задавать параметры аудита доступа к объектам для отдельных ресурсов, таких как файлы, объекты Active Directory и разделы реестра.</span><span class="sxs-lookup"><span data-stu-id="6e70b-284">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="6e70b-285">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e70b-286">усерригхтсманажеволумес</span><span class="sxs-lookup"><span data-stu-id="6e70b-286">userRightsManageVolumes</span></span>|[<span data-ttu-id="6e70b-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-288">Это право пользователя определяет, какие пользователи и группы могут выполнять задачи обслуживания для тома, такие как удаленная дефрагментация.</span><span class="sxs-lookup"><span data-stu-id="6e70b-288">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="6e70b-289">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e70b-290">усерригхтсмодифифирмваринвиронмент</span><span class="sxs-lookup"><span data-stu-id="6e70b-290">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="6e70b-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-292">Это право пользователя определяет, кто может изменять значения в аппаратной среде.</span><span class="sxs-lookup"><span data-stu-id="6e70b-292">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="6e70b-293">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e70b-294">усерригхтсмодифйобжектлабелс</span><span class="sxs-lookup"><span data-stu-id="6e70b-294">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="6e70b-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-296">Это право пользователя определяет, какие учетные записи пользователей могут изменять метки целостности объектов, таких как файлы, разделы реестра или процессы, принадлежащие другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="6e70b-296">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="6e70b-297">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-297">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e70b-298">усерригхтспрофилесинглепроцесс</span><span class="sxs-lookup"><span data-stu-id="6e70b-298">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="6e70b-299">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-299">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-300">Это право пользователя определяет, какие пользователи могут использовать средства мониторинга производительности для наблюдения за производительностью системных процессов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-300">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="6e70b-301">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-301">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e70b-302">усерригхтсремотешутдовн</span><span class="sxs-lookup"><span data-stu-id="6e70b-302">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="6e70b-303">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-303">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-304">Это право пользователя определяет, каким пользователям разрешено завершать работу компьютера из удаленного расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="6e70b-304">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="6e70b-305">Неправильное использование этого права пользователя может привести к отказу в обслуживании.</span><span class="sxs-lookup"><span data-stu-id="6e70b-305">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="6e70b-306">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-306">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e70b-307">усерригхтсресторедата</span><span class="sxs-lookup"><span data-stu-id="6e70b-307">userRightsRestoreData</span></span>|[<span data-ttu-id="6e70b-308">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-308">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-309">Это право пользователя определяет, какие пользователи могут обходить разрешения для файлов, каталогов, реестра и других постоянных объектов при восстановлении резервных копий файлов и каталогов, и определяет, какие пользователи могут устанавливать любой действительный субъект безопасности в качестве владельца объекта.</span><span class="sxs-lookup"><span data-stu-id="6e70b-309">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="6e70b-310">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-310">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e70b-311">усерригхтстакеовнершип</span><span class="sxs-lookup"><span data-stu-id="6e70b-311">userRightsTakeOwnership</span></span>|[<span data-ttu-id="6e70b-312">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e70b-312">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e70b-313">Это право пользователя определяет, какие пользователи могут становиться владельцами любого защищаемого объекта в системе, включая объекты Active Directory, файлы и папки, принтеры, разделы реестра, процессы и потоки.</span><span class="sxs-lookup"><span data-stu-id="6e70b-313">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="6e70b-314">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="6e70b-314">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e70b-315">ксбокссервицесенаблексбоксгамесаветаск</span><span class="sxs-lookup"><span data-stu-id="6e70b-315">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="6e70b-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-316">Boolean</span></span>|<span data-ttu-id="6e70b-317">Этот параметр определяет, включена ли функция сохранения игры Xbox (1) или отключена (0).</span><span class="sxs-lookup"><span data-stu-id="6e70b-317">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="6e70b-318">ксбокссервицесакцессориманажементсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="6e70b-318">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="6e70b-319">сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="6e70b-320">Этот параметр определяет, является ли тип запуска службы управления принадлежностью автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="6e70b-320">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="6e70b-321">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="6e70b-321">Default: Manual.</span></span> <span data-ttu-id="6e70b-322">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="6e70b-323">ксбокссервицесливеаусманажерсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="6e70b-323">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="6e70b-324">сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-324">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="6e70b-325">Этот параметр определяет, является ли тип запуска службы диспетчера Live auth автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="6e70b-325">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="6e70b-326">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="6e70b-326">Default: Manual.</span></span> <span data-ttu-id="6e70b-327">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-327">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="6e70b-328">ксбокссервицесливегамесавесервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="6e70b-328">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="6e70b-329">сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-329">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="6e70b-330">Этот параметр определяет, является ли тип запуска службы Live Save Service автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="6e70b-330">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="6e70b-331">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="6e70b-331">Default: Manual.</span></span> <span data-ttu-id="6e70b-332">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-332">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="6e70b-333">ксбокссервицесливенетворкингсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="6e70b-333">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="6e70b-334">сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-334">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="6e70b-335">Этот параметр определяет, является ли тип запуска сетевой службы автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="6e70b-335">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="6e70b-336">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="6e70b-336">Default: Manual.</span></span> <span data-ttu-id="6e70b-337">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-337">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="6e70b-338">локалсекуритйоптионсблоккмикрософтаккаунтс</span><span class="sxs-lookup"><span data-stu-id="6e70b-338">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="6e70b-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-339">Boolean</span></span>|<span data-ttu-id="6e70b-340">Запретить пользователям добавлять новые учетные записи Майкрософт на этот компьютер.</span><span class="sxs-lookup"><span data-stu-id="6e70b-340">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="6e70b-341">локалсекуритйоптионсблоккремотелогонвисбланкпассворд</span><span class="sxs-lookup"><span data-stu-id="6e70b-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="6e70b-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-342">Boolean</span></span>|<span data-ttu-id="6e70b-343">Включите локальные учетные записи, не защищенные паролем, для входа в систему из расположений, отличных от физического устройства. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="6e70b-343">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="6e70b-344">локалсекуритйоптионсдисаблеадминистратораккаунт</span><span class="sxs-lookup"><span data-stu-id="6e70b-344">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="6e70b-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-345">Boolean</span></span>|<span data-ttu-id="6e70b-346">Определяет, включена или отключена учетная запись локального администратора.</span><span class="sxs-lookup"><span data-stu-id="6e70b-346">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="6e70b-347">локалсекуритйоптионсадминистратораккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="6e70b-347">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="6e70b-348">String</span><span class="sxs-lookup"><span data-stu-id="6e70b-348">String</span></span>|<span data-ttu-id="6e70b-349">Определите имя другой учетной записи, которая будет связана с идентификатором безопасности (SID) учетной записи "Administrator".</span><span class="sxs-lookup"><span data-stu-id="6e70b-349">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="6e70b-350">локалсекуритйоптионсдисаблегуестаккаунт</span><span class="sxs-lookup"><span data-stu-id="6e70b-350">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="6e70b-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-351">Boolean</span></span>|<span data-ttu-id="6e70b-352">Определяет, включена или отключена Гостевая учетная запись.</span><span class="sxs-lookup"><span data-stu-id="6e70b-352">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="6e70b-353">локалсекуритйоптионсгуестаккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="6e70b-353">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="6e70b-354">String</span><span class="sxs-lookup"><span data-stu-id="6e70b-354">String</span></span>|<span data-ttu-id="6e70b-355">Определите имя другой учетной записи, которая будет связана с идентификатором безопасности (SID) для учетной записи "гость".</span><span class="sxs-lookup"><span data-stu-id="6e70b-355">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="6e70b-356">локалсекуритйоптионсалловундокквисаусавингтологон</span><span class="sxs-lookup"><span data-stu-id="6e70b-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="6e70b-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-357">Boolean</span></span>|<span data-ttu-id="6e70b-358">Запретите отстыковку портативного компьютера без необходимости входа в систему.</span><span class="sxs-lookup"><span data-stu-id="6e70b-358">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="6e70b-359">локалсекуритйоптионсблоккусерсинсталлингпринтердриверс</span><span class="sxs-lookup"><span data-stu-id="6e70b-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="6e70b-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-360">Boolean</span></span>|<span data-ttu-id="6e70b-361">Ограничьте установку драйверов принтеров в рамках подключения к общему принтеру только для администраторов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-361">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="6e70b-362">локалсекуритйоптионсблоккремотеоптикалдривеакцесс</span><span class="sxs-lookup"><span data-stu-id="6e70b-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="6e70b-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-363">Boolean</span></span>|<span data-ttu-id="6e70b-364">Включение этого параметра позволяет интерактивно вошедший в систему пользователь получать доступ к устройству чтения компакт-дисков.</span><span class="sxs-lookup"><span data-stu-id="6e70b-364">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="6e70b-365">локалсекуритйоптионсформатандежектофремоваблемедиаалловедусер</span><span class="sxs-lookup"><span data-stu-id="6e70b-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="6e70b-366">локалсекуритйоптионсформатандежектофремоваблемедиаалловедусертипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="6e70b-367">Определите, кому разрешено форматировать и извлекать съемные носители NTFS.</span><span class="sxs-lookup"><span data-stu-id="6e70b-367">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="6e70b-368">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-368">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="6e70b-369">локалсекуритйоптионсмачинеинактивитилимит</span><span class="sxs-lookup"><span data-stu-id="6e70b-369">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="6e70b-370">Int32</span><span class="sxs-lookup"><span data-stu-id="6e70b-370">Int32</span></span>|<span data-ttu-id="6e70b-371">Определите максимальное количество минут отсутствия активности на экране входа интерактивного рабочего стола, пока не запустится экранная заставка.</span><span class="sxs-lookup"><span data-stu-id="6e70b-371">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="6e70b-372">Допустимые значения — от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="6e70b-372">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="6e70b-373">локалсекуритйоптионсмачинеинактивитилимитинминутес</span><span class="sxs-lookup"><span data-stu-id="6e70b-373">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="6e70b-374">Int32</span><span class="sxs-lookup"><span data-stu-id="6e70b-374">Int32</span></span>|<span data-ttu-id="6e70b-375">Определите максимальное количество минут отсутствия активности на экране входа интерактивного рабочего стола, пока не запустится экранная заставка.</span><span class="sxs-lookup"><span data-stu-id="6e70b-375">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="6e70b-376">Допустимые значения — от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="6e70b-376">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="6e70b-377">локалсекуритйоптионсдонотрекуиректрлалтдел</span><span class="sxs-lookup"><span data-stu-id="6e70b-377">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="6e70b-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-378">Boolean</span></span>|<span data-ttu-id="6e70b-379">Требовать нажатия клавиш CTRL + ALT + DEL, прежде чем пользователь сможет войти в систему.</span><span class="sxs-lookup"><span data-stu-id="6e70b-379">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="6e70b-380">локалсекуритйоптионшиделастсигнединусер</span><span class="sxs-lookup"><span data-stu-id="6e70b-380">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="6e70b-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-381">Boolean</span></span>|<span data-ttu-id="6e70b-382">Не отображать имя последнего пользователя, выполнившего вход на это устройство.</span><span class="sxs-lookup"><span data-stu-id="6e70b-382">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="6e70b-383">локалсекуритйоптионшидеусернамеатсигнин</span><span class="sxs-lookup"><span data-stu-id="6e70b-383">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="6e70b-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-384">Boolean</span></span>|<span data-ttu-id="6e70b-385">Не отображать имя пользователя, выполняющего вход на это устройство, после ввода учетных данных и отображения рабочего стола на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6e70b-385">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="6e70b-386">локалсекуритйоптионслогонмессажетитле</span><span class="sxs-lookup"><span data-stu-id="6e70b-386">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="6e70b-387">String</span><span class="sxs-lookup"><span data-stu-id="6e70b-387">String</span></span>|<span data-ttu-id="6e70b-388">Задайте заголовок сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="6e70b-388">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="6e70b-389">локалсекуритйоптионслогонмессажетекст</span><span class="sxs-lookup"><span data-stu-id="6e70b-389">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="6e70b-390">String</span><span class="sxs-lookup"><span data-stu-id="6e70b-390">String</span></span>|<span data-ttu-id="6e70b-391">Задайте текст сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="6e70b-391">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="6e70b-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="6e70b-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="6e70b-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-393">Boolean</span></span>|<span data-ttu-id="6e70b-394">Блокировать запросы проверки подлинности PKU2U на этом устройстве для использования сетевых удостоверений.</span><span class="sxs-lookup"><span data-stu-id="6e70b-394">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="6e70b-395">локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажерхелпербул</span><span class="sxs-lookup"><span data-stu-id="6e70b-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="6e70b-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-396">Boolean</span></span>|<span data-ttu-id="6e70b-397">Помощник по пользовательскому интерфейсу Boolean для объекта Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажер</span><span class="sxs-lookup"><span data-stu-id="6e70b-397">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="6e70b-398">локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажер</span><span class="sxs-lookup"><span data-stu-id="6e70b-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="6e70b-399">String</span><span class="sxs-lookup"><span data-stu-id="6e70b-399">String</span></span>|<span data-ttu-id="6e70b-400">Измените строку языка определения дескрипторов безопасности по умолчанию, чтобы разрешить или запретить пользователям и группам совершать удаленные вызовы в SAM.</span><span class="sxs-lookup"><span data-stu-id="6e70b-400">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="6e70b-401">локалсекуритйоптионсминимумсессионсекуритифорнтлмсспбаседклиентс</span><span class="sxs-lookup"><span data-stu-id="6e70b-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="6e70b-402">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="6e70b-402">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="6e70b-403">Этот параметр безопасности позволяет клиенту требовать согласование 128-разрядного шифрования и/или сеанса защиты сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="6e70b-403">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="6e70b-404">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-404">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="6e70b-405">локалсекуритйоптионсминимумсессионсекуритифорнтлмсспбаседсерверс</span><span class="sxs-lookup"><span data-stu-id="6e70b-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="6e70b-406">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="6e70b-406">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="6e70b-407">Этот параметр безопасности позволяет серверу требовать согласование 128-разрядного шифрования и/или сеанса защиты сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="6e70b-407">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="6e70b-408">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-408">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="6e70b-409">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="6e70b-409">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="6e70b-410">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="6e70b-410">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="6e70b-411">Этот параметр безопасности определяет, какой протокол проверки подлинности "запрос/ответ" используется для входа в сеть.</span><span class="sxs-lookup"><span data-stu-id="6e70b-411">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="6e70b-412">Возможные значения: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-412">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="6e70b-413">ланманажерворкстатиондисаблеинсекурегуестлогонс</span><span class="sxs-lookup"><span data-stu-id="6e70b-413">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="6e70b-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-414">Boolean</span></span>|<span data-ttu-id="6e70b-415">Если этот параметр включен, клиент SMB будет разрешать небезопасные гостевые входы.</span><span class="sxs-lookup"><span data-stu-id="6e70b-415">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="6e70b-416">Если этот параметр не настроен, клиент SMB будет отклонять небезопасные гостевые входы.</span><span class="sxs-lookup"><span data-stu-id="6e70b-416">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="6e70b-417">локалсекуритйоптионсклеарвиртуалмеморипажефиле</span><span class="sxs-lookup"><span data-stu-id="6e70b-417">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="6e70b-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-418">Boolean</span></span>|<span data-ttu-id="6e70b-419">Этот параметр безопасности определяет, будет ли очищаться файл подкачки виртуальной памяти при завершении работы системы.</span><span class="sxs-lookup"><span data-stu-id="6e70b-419">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="6e70b-420">локалсекуритйоптионсалловсистемтобешутдовнвисаусавингтологон</span><span class="sxs-lookup"><span data-stu-id="6e70b-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="6e70b-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-421">Boolean</span></span>|<span data-ttu-id="6e70b-422">Этот параметр безопасности определяет, можно ли завершить работу компьютера, не выполняя вход в Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-422">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="6e70b-423">локалсекуритйоптионсалловуиакцессаппликатионелеватион</span><span class="sxs-lookup"><span data-stu-id="6e70b-423">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="6e70b-424">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-424">Boolean</span></span>|<span data-ttu-id="6e70b-425">Разрешить UIAccess Apps запрос на повышение прав без использования безопасного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="6e70b-425">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="6e70b-426">локалсекуритйоптионсвиртуализефилеандрегистривритефаилурестоперусерлокатионс</span><span class="sxs-lookup"><span data-stu-id="6e70b-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="6e70b-427">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-427">Boolean</span></span>|<span data-ttu-id="6e70b-428">Виртуализация сбоев записи в файл и реестр для отдельных расположений пользователей</span><span class="sxs-lookup"><span data-stu-id="6e70b-428">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="6e70b-429">локалсекуритйоптионсонлелеватесигнедексекутаблес</span><span class="sxs-lookup"><span data-stu-id="6e70b-429">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="6e70b-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-430">Boolean</span></span>|<span data-ttu-id="6e70b-431">Принудительная проверка пути сертификации PKI для указанного исполняемого файла перед тем, как он будет разрешен для запуска.</span><span class="sxs-lookup"><span data-stu-id="6e70b-431">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="6e70b-432">локалсекуритйоптионсадминистраторелеватионпромптбехавиор</span><span class="sxs-lookup"><span data-stu-id="6e70b-432">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="6e70b-433">локалсекуритйоптионсадминистраторелеватионпромптбехавиортипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="6e70b-434">Определите поведение запросов на повышение прав для администраторов в режиме одобрения администратором.</span><span class="sxs-lookup"><span data-stu-id="6e70b-434">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="6e70b-435">Возможные значения: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-435">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="6e70b-436">локалсекуритйоптионсстандардусерелеватионпромптбехавиор</span><span class="sxs-lookup"><span data-stu-id="6e70b-436">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="6e70b-437">локалсекуритйоптионсстандардусерелеватионпромптбехавиортипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="6e70b-438">Определите поведение запросов на повышение прав для стандартных пользователей.</span><span class="sxs-lookup"><span data-stu-id="6e70b-438">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="6e70b-439">Возможные значения: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-439">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="6e70b-440">локалсекуритйоптионссвитчтосекуредесктопвхенпромптингфорелеватион</span><span class="sxs-lookup"><span data-stu-id="6e70b-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="6e70b-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-441">Boolean</span></span>|<span data-ttu-id="6e70b-442">Разрешить всем запросам на повышение прав доступ к рабочему столу интерактивного пользователя, а не к безопасному рабочему столу.</span><span class="sxs-lookup"><span data-stu-id="6e70b-442">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="6e70b-443">Используются параметры политики поведения запросов для администраторов и стандартных пользователей.</span><span class="sxs-lookup"><span data-stu-id="6e70b-443">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="6e70b-444">локалсекуритйоптионсдетектаппликатионинсталлатионсандпромптфорелеватион</span><span class="sxs-lookup"><span data-stu-id="6e70b-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="6e70b-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-445">Boolean</span></span>|<span data-ttu-id="6e70b-446">При установке приложений, требующих повышенных привилегий, запрашиваются учетные данные администратора. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="6e70b-446">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="6e70b-447">локалсекуритйоптионсалловуиакцессаппликатионсфорсекурелокатионс</span><span class="sxs-lookup"><span data-stu-id="6e70b-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="6e70b-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-448">Boolean</span></span>|<span data-ttu-id="6e70b-449">Разрешить UIAccess Apps запрос на повышение прав без использования безопасного рабочего стола. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="6e70b-449">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="6e70b-450">локалсекуритйоптионсусеадминаппровалмоде</span><span class="sxs-lookup"><span data-stu-id="6e70b-450">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="6e70b-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-451">Boolean</span></span>|<span data-ttu-id="6e70b-452">Определяет, использует ли встроенная учетная запись администратора режим одобрения администратором или выполняет все приложения с правами полного администратора. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="6e70b-452">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="6e70b-453">локалсекуритйоптионсусеадминаппровалмодефорадминистраторс</span><span class="sxs-lookup"><span data-stu-id="6e70b-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="6e70b-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-454">Boolean</span></span>|<span data-ttu-id="6e70b-455">Определить, включен ли режим одобрения администратором и все параметры политики контроля учетных записей, по умолчанию включено</span><span class="sxs-lookup"><span data-stu-id="6e70b-455">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="6e70b-456">локалсекуритйоптионсинформатионшовнонлоккскрин</span><span class="sxs-lookup"><span data-stu-id="6e70b-456">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="6e70b-457">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="6e70b-457">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="6e70b-458">Настройте сведения о пользователе, которые отображаются, когда сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="6e70b-458">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="6e70b-459">Если этот флажок не установлен, отображаются отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e70b-459">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="6e70b-460">Возможные значения: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-460">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="6e70b-461">локалсекуритйоптионсинформатиондисплайедонлоккскрин</span><span class="sxs-lookup"><span data-stu-id="6e70b-461">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="6e70b-462">локалсекуритйоптионсинформатиондисплайедонлоккскринтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="6e70b-463">Настройте сведения о пользователе, которые отображаются, когда сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="6e70b-463">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="6e70b-464">Если этот флажок не установлен, отображаются отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e70b-464">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="6e70b-465">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-465">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="6e70b-466">локалсекуритйоптионсдисаблеклиентдигиталлисигнкоммуникатионсифсерверагрис</span><span class="sxs-lookup"><span data-stu-id="6e70b-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="6e70b-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-467">Boolean</span></span>|<span data-ttu-id="6e70b-468">Этот параметр безопасности определяет, будет ли клиент SMB пытаться согласовать подписывание SMB пакетов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-468">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="6e70b-469">локалсекуритйоптионсклиентдигиталлисигнкоммуникатионсалвайс</span><span class="sxs-lookup"><span data-stu-id="6e70b-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="6e70b-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-470">Boolean</span></span>|<span data-ttu-id="6e70b-471">Этот параметр безопасности определяет, требуется ли Подписывание пакетов для клиентского SMB-компонента.</span><span class="sxs-lookup"><span data-stu-id="6e70b-471">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="6e70b-472">локалсекуритйоптионсклиентсендуненкриптедпассвордтосирдпартисмбсерверс</span><span class="sxs-lookup"><span data-stu-id="6e70b-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="6e70b-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-473">Boolean</span></span>|<span data-ttu-id="6e70b-474">Если этот параметр безопасности включен, перенаправителем SMB (Server Message Block) разрешено отправлять пароли открытым текстом на серверы SMB сторонних производителей, не поддерживающие шифрование паролей во время проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="6e70b-474">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="6e70b-475">локалсекуритйоптионсдисаблесервердигиталлисигнкоммуникатионсалвайс</span><span class="sxs-lookup"><span data-stu-id="6e70b-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="6e70b-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-476">Boolean</span></span>|<span data-ttu-id="6e70b-477">Этот параметр безопасности определяет, требуется ли подписи пакетов для SMB-компонентов сервера.</span><span class="sxs-lookup"><span data-stu-id="6e70b-477">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="6e70b-478">локалсекуритйоптионсдисаблесервердигиталлисигнкоммуникатионсифклиентагрис</span><span class="sxs-lookup"><span data-stu-id="6e70b-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="6e70b-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-479">Boolean</span></span>|<span data-ttu-id="6e70b-480">Этот параметр безопасности определяет, будет ли SMB согласовывать подпись SMB Packet с клиентами, которые их запрашивают.</span><span class="sxs-lookup"><span data-stu-id="6e70b-480">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="6e70b-481">локалсекуритйоптионсрестриктанонимаусакцесстонамедпипесандшарес</span><span class="sxs-lookup"><span data-stu-id="6e70b-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="6e70b-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-482">Boolean</span></span>|<span data-ttu-id="6e70b-483">По умолчанию этот параметр безопасности запрещает анонимный доступ к ресурсам и каналам к параметрам именованных каналов, к которым возможен анонимный доступ, и к общедоступным ресурсам, к которым возможен анонимный доступ</span><span class="sxs-lookup"><span data-stu-id="6e70b-483">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="6e70b-484">локалсекуритйоптионсдоноталлованонимаусенумератионофсамаккаунтс</span><span class="sxs-lookup"><span data-stu-id="6e70b-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="6e70b-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-485">Boolean</span></span>|<span data-ttu-id="6e70b-486">Этот параметр безопасности определяет, какие дополнительные разрешения будут предоставлены анонимным подключениям к компьютеру.</span><span class="sxs-lookup"><span data-stu-id="6e70b-486">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="6e70b-487">локалсекуритйоптионсаллованонимаусенумератионофсамаккаунтсандшарес</span><span class="sxs-lookup"><span data-stu-id="6e70b-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="6e70b-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-488">Boolean</span></span>|<span data-ttu-id="6e70b-489">Этот параметр безопасности определяет, разрешено ли анонимным пользователям выполнять определенные действия, например перечислять имена доменных учетных записей и сетевые общие папки.</span><span class="sxs-lookup"><span data-stu-id="6e70b-489">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="6e70b-490">локалсекуритйоптионсдонотстореланманажерхашвалуеоннекстпассвордчанже</span><span class="sxs-lookup"><span data-stu-id="6e70b-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="6e70b-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-491">Boolean</span></span>|<span data-ttu-id="6e70b-492">Этот параметр безопасности определяет, будет ли сохраняться значение хэша LAN Manager (LM) для нового пароля при следующем изменении пароля.</span><span class="sxs-lookup"><span data-stu-id="6e70b-492">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="6e70b-493">По умолчанию он не хранится.</span><span class="sxs-lookup"><span data-stu-id="6e70b-493">It’s not stored by default.</span></span>|
|<span data-ttu-id="6e70b-494">локалсекуритйоптионссмарткардремовалбехавиор</span><span class="sxs-lookup"><span data-stu-id="6e70b-494">localSecurityOptionsSmartCardRemovalBehavior</span></span>|<span data-ttu-id="6e70b-495">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md);</span><span class="sxs-lookup"><span data-stu-id="6e70b-495">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)</span></span>|<span data-ttu-id="6e70b-496">Этот параметр безопасности определяет, что происходит при удалении смарт-карты пользователя, выполнившего вход в систему, из устройства чтения смарт-карт.</span><span class="sxs-lookup"><span data-stu-id="6e70b-496">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="6e70b-497">Возможные значения: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-497">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="6e70b-498">дефендерсекуритицентердисаблеаппбровсеруи</span><span class="sxs-lookup"><span data-stu-id="6e70b-498">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="6e70b-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-499">Boolean</span></span>|<span data-ttu-id="6e70b-500">Используется для отключения отображения области защиты приложений и браузера.</span><span class="sxs-lookup"><span data-stu-id="6e70b-500">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="6e70b-501">дефендерсекуритицентердисаблефамилюи</span><span class="sxs-lookup"><span data-stu-id="6e70b-501">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="6e70b-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-502">Boolean</span></span>|<span data-ttu-id="6e70b-503">Используется для отключения отображения области семьи.</span><span class="sxs-lookup"><span data-stu-id="6e70b-503">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="6e70b-504">дефендерсекуритицентердисаблехеалсуи</span><span class="sxs-lookup"><span data-stu-id="6e70b-504">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="6e70b-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-505">Boolean</span></span>|<span data-ttu-id="6e70b-506">Используется для отключения отображения области производительности и работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="6e70b-506">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="6e70b-507">дефендерсекуритицентердисабленетворкуи</span><span class="sxs-lookup"><span data-stu-id="6e70b-507">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="6e70b-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-508">Boolean</span></span>|<span data-ttu-id="6e70b-509">Используется для отключения отображения зоны "брандмауэр" и "Защита сети".</span><span class="sxs-lookup"><span data-stu-id="6e70b-509">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="6e70b-510">дефендерсекуритицентердисаблевирусуи</span><span class="sxs-lookup"><span data-stu-id="6e70b-510">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="6e70b-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-511">Boolean</span></span>|<span data-ttu-id="6e70b-512">Используется для отключения отображения области защиты от вирусов и угроз.</span><span class="sxs-lookup"><span data-stu-id="6e70b-512">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="6e70b-513">дефендерсекуритицентердисаблеаккаунтуи</span><span class="sxs-lookup"><span data-stu-id="6e70b-513">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="6e70b-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-514">Boolean</span></span>|<span data-ttu-id="6e70b-515">Используется для отключения отображения области защиты учетных записей.</span><span class="sxs-lookup"><span data-stu-id="6e70b-515">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="6e70b-516">дефендерсекуритицентердисаблеклеартпмуи</span><span class="sxs-lookup"><span data-stu-id="6e70b-516">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="6e70b-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-517">Boolean</span></span>|<span data-ttu-id="6e70b-518">Используется для отключения отображения кнопки Очистить доверенный платформенный модуль.</span><span class="sxs-lookup"><span data-stu-id="6e70b-518">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="6e70b-519">дефендерсекуритицентердисаблехардвареуи</span><span class="sxs-lookup"><span data-stu-id="6e70b-519">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="6e70b-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-520">Boolean</span></span>|<span data-ttu-id="6e70b-521">Используется для отключения отображения области аппаратной защиты.</span><span class="sxs-lookup"><span data-stu-id="6e70b-521">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="6e70b-522">дефендерсекуритицентердисабленотификатионареауи</span><span class="sxs-lookup"><span data-stu-id="6e70b-522">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="6e70b-523">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-523">Boolean</span></span>|<span data-ttu-id="6e70b-524">Используется для отключения отображения элемента управления "область уведомлений".</span><span class="sxs-lookup"><span data-stu-id="6e70b-524">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="6e70b-525">Для вступления этого параметра в силу пользователю необходимо выйти из системы и войти в нее, а затем перезагрузить компьютер.</span><span class="sxs-lookup"><span data-stu-id="6e70b-525">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="6e70b-526">дефендерсекуритицентердисаблерансомвареуи</span><span class="sxs-lookup"><span data-stu-id="6e70b-526">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="6e70b-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-527">Boolean</span></span>|<span data-ttu-id="6e70b-528">Используется для отключения отображения области защиты от пошантажистом.</span><span class="sxs-lookup"><span data-stu-id="6e70b-528">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="6e70b-529">дефендерсекуритицентердисаблесекуребутуи</span><span class="sxs-lookup"><span data-stu-id="6e70b-529">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="6e70b-530">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-530">Boolean</span></span>|<span data-ttu-id="6e70b-531">Используется для отключения отображения области безопасной загрузки в разделе Безопасность устройства.</span><span class="sxs-lookup"><span data-stu-id="6e70b-531">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="6e70b-532">дефендерсекуритицентердисаблетраублешутингуи</span><span class="sxs-lookup"><span data-stu-id="6e70b-532">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="6e70b-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-533">Boolean</span></span>|<span data-ttu-id="6e70b-534">Используется для отключения отображения устранения неполадок процесса безопасности в разделе Безопасность устройства.</span><span class="sxs-lookup"><span data-stu-id="6e70b-534">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="6e70b-535">дефендерсекуритицентердисаблевулнераблетпмфирмвареупдатеуи</span><span class="sxs-lookup"><span data-stu-id="6e70b-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="6e70b-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-536">Boolean</span></span>|<span data-ttu-id="6e70b-537">Используется для отключения отображения обновления микропрограммы доверенного платформенного модуля при обнаружении уязвимого программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="6e70b-537">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="6e70b-538">дефендерсекуритицентерорганизатиондисплайнаме</span><span class="sxs-lookup"><span data-stu-id="6e70b-538">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="6e70b-539">String</span><span class="sxs-lookup"><span data-stu-id="6e70b-539">String</span></span>|<span data-ttu-id="6e70b-540">Имя компании, которое отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="6e70b-540">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="6e70b-541">дефендерсекуритицентерхелпемаил</span><span class="sxs-lookup"><span data-stu-id="6e70b-541">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="6e70b-542">String</span><span class="sxs-lookup"><span data-stu-id="6e70b-542">String</span></span>|<span data-ttu-id="6e70b-543">Адрес электронной почты, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="6e70b-543">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="6e70b-544">дефендерсекуритицентерхелпфоне</span><span class="sxs-lookup"><span data-stu-id="6e70b-544">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="6e70b-545">String</span><span class="sxs-lookup"><span data-stu-id="6e70b-545">String</span></span>|<span data-ttu-id="6e70b-546">Номер телефона или идентификатор Skype, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="6e70b-546">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="6e70b-547">дефендерсекуритицентерхелпурл</span><span class="sxs-lookup"><span data-stu-id="6e70b-547">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="6e70b-548">String</span><span class="sxs-lookup"><span data-stu-id="6e70b-548">String</span></span>|<span data-ttu-id="6e70b-549">URL-адрес портала справки это отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="6e70b-549">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="6e70b-550">дефендерсекуритицентернотификатионсфромапп</span><span class="sxs-lookup"><span data-stu-id="6e70b-550">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="6e70b-551">дефендерсекуритицентернотификатионсфромапптипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-551">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="6e70b-552">Уведомления, отображаемые в отображаемых областях приложения.</span><span class="sxs-lookup"><span data-stu-id="6e70b-552">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="6e70b-553">Возможные значения: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-553">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="6e70b-554">дефендерсекуритицентеритконтактдисплай</span><span class="sxs-lookup"><span data-stu-id="6e70b-554">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="6e70b-555">дефендерсекуритицентеритконтактдисплайтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-555">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="6e70b-556">Настройка места отображения контактной информации для конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="6e70b-556">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="6e70b-557">Возможные значения: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-557">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="6e70b-558">виндовсдефендертамперпротектион</span><span class="sxs-lookup"><span data-stu-id="6e70b-558">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="6e70b-559">windowsDefenderTamperProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="6e70b-559">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="6e70b-560">Настройка параметров Тамперпротектион для защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-560">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="6e70b-561">Возможные значения: `notConfigured`, `enable`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-561">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="6e70b-562">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="6e70b-562">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="6e70b-563">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-563">Boolean</span></span>|<span data-ttu-id="6e70b-564">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="6e70b-564">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="6e70b-565">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="6e70b-565">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="6e70b-566">Int32</span><span class="sxs-lookup"><span data-stu-id="6e70b-566">Int32</span></span>|<span data-ttu-id="6e70b-567">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="6e70b-567">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="6e70b-568">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="6e70b-568">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="6e70b-569">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="6e70b-569">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="6e70b-570">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="6e70b-570">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="6e70b-571">фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-571">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="6e70b-572">Выберите используемую кодировку с общим ключом.</span><span class="sxs-lookup"><span data-stu-id="6e70b-572">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="6e70b-573">Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-573">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="6e70b-574">фиреваллипсецексемптионсноне</span><span class="sxs-lookup"><span data-stu-id="6e70b-574">firewallIPSecExemptionsNone</span></span>|<span data-ttu-id="6e70b-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-575">Boolean</span></span>|<span data-ttu-id="6e70b-576">Настраивает исключения IPSec без исключений</span><span class="sxs-lookup"><span data-stu-id="6e70b-576">Configures IPSec exemptions to no exemptions</span></span>|
|<span data-ttu-id="6e70b-577">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="6e70b-577">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="6e70b-578">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-578">Boolean</span></span>|<span data-ttu-id="6e70b-579">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="6e70b-579">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="6e70b-580">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="6e70b-580">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="6e70b-581">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-581">Boolean</span></span>|<span data-ttu-id="6e70b-582">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="6e70b-582">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="6e70b-583">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="6e70b-583">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="6e70b-584">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-584">Boolean</span></span>|<span data-ttu-id="6e70b-585">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="6e70b-585">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="6e70b-586">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="6e70b-586">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="6e70b-587">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-587">Boolean</span></span>|<span data-ttu-id="6e70b-588">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="6e70b-588">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="6e70b-589">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="6e70b-589">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="6e70b-590">фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-590">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="6e70b-591">Укажите способ применения списка отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-591">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="6e70b-592">Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-592">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="6e70b-593">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="6e70b-593">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="6e70b-594">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-594">Boolean</span></span>|<span data-ttu-id="6e70b-595">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="6e70b-595">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="6e70b-596">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="6e70b-596">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="6e70b-597">фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-597">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="6e70b-598">Настраивает способ применения очередей пакетов в сценарии туннельного шлюза.</span><span class="sxs-lookup"><span data-stu-id="6e70b-598">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="6e70b-599">Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-599">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="6e70b-600">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="6e70b-600">firewallProfileDomain</span></span>|[<span data-ttu-id="6e70b-601">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6e70b-601">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="6e70b-602">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="6e70b-602">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="6e70b-603">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="6e70b-603">firewallProfilePublic</span></span>|[<span data-ttu-id="6e70b-604">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6e70b-604">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="6e70b-605">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="6e70b-605">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="6e70b-606">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="6e70b-606">firewallProfilePrivate</span></span>|[<span data-ttu-id="6e70b-607">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6e70b-607">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="6e70b-608">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="6e70b-608">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="6e70b-609">дефендерадобереадерлаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="6e70b-609">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="6e70b-610">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-610">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e70b-611">Значение, указывающее поведение Adobe Reader при создании дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-611">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="6e70b-612">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-612">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-613">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="6e70b-613">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="6e70b-614">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6e70b-614">String collection</span></span>|<span data-ttu-id="6e70b-615">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="6e70b-615">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="6e70b-616">дефендероффицеаппсосерпроцессинжектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-616">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="6e70b-617">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-617">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e70b-618">Значение, указывающее поведение приложений Office, добавляемых в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="6e70b-618">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="6e70b-619">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-619">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-620">дефендероффицеаппсосерпроцессинжектион</span><span class="sxs-lookup"><span data-stu-id="6e70b-620">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="6e70b-621">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-621">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e70b-622">Значение, указывающее поведение приложений Office, добавляемых в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="6e70b-622">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="6e70b-623">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-623">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-624">дефендероффицекоммуникатионаппслаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="6e70b-624">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="6e70b-625">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-625">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e70b-626">Значение, определяющее поведение приложений для связи с Office, включая Microsoft Outlook, от создания дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-626">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="6e70b-627">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-627">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-628">дефендероффицеаппсексекутаблеконтенткреатионорлаунчтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-628">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="6e70b-629">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-629">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e70b-630">Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого контента.</span><span class="sxs-lookup"><span data-stu-id="6e70b-630">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="6e70b-631">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-631">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-632">дефендероффицеаппсексекутаблеконтенткреатионорлаунч</span><span class="sxs-lookup"><span data-stu-id="6e70b-632">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="6e70b-633">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-633">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e70b-634">Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого контента.</span><span class="sxs-lookup"><span data-stu-id="6e70b-634">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="6e70b-635">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-635">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-636">дефендероффицеаппслаунччилдпроцесстипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-636">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="6e70b-637">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-637">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e70b-638">Значение, указывающее поведение запуска приложения Office для дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-638">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="6e70b-639">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-639">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-640">дефендероффицеаппслаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="6e70b-640">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="6e70b-641">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-641">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e70b-642">Значение, указывающее поведение запуска приложения Office для дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-642">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="6e70b-643">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-643">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-644">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="6e70b-644">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="6e70b-645">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-645">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e70b-646">Значение, указывающее поведение импорта Win32 из кода макросов в Office.</span><span class="sxs-lookup"><span data-stu-id="6e70b-646">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="6e70b-647">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-647">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-648">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="6e70b-648">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="6e70b-649">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-649">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e70b-650">Значение, указывающее поведение импорта Win32 из кода макросов в Office.</span><span class="sxs-lookup"><span data-stu-id="6e70b-650">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="6e70b-651">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-651">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-652">дефендерскриптобфускатедмакрокодетипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-652">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="6e70b-653">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-653">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e70b-654">Значение, определяющее поведение кода "замаскированный JS/VBS/PS/макрос".</span><span class="sxs-lookup"><span data-stu-id="6e70b-654">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="6e70b-655">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-655">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-656">дефендерскриптобфускатедмакрокоде</span><span class="sxs-lookup"><span data-stu-id="6e70b-656">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="6e70b-657">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-657">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e70b-658">Значение, определяющее поведение кода "замаскированный JS/VBS/PS/макрос".</span><span class="sxs-lookup"><span data-stu-id="6e70b-658">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="6e70b-659">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-659">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-660">дефендерскриптдовнлоадедпайлоадексекутионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-660">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="6e70b-661">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-661">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e70b-662">Значение, определяющее поведение JS-и VBS-данных, загруженных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="6e70b-662">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="6e70b-663">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-663">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-664">дефендерскриптдовнлоадедпайлоадексекутион</span><span class="sxs-lookup"><span data-stu-id="6e70b-664">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="6e70b-665">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-665">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e70b-666">Значение, определяющее поведение JS-и VBS-данных, загруженных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="6e70b-666">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="6e70b-667">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-667">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-668">дефендерпревенткредентиалстеалингтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-668">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="6e70b-669">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-669">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e70b-670">Значение, указывающее, разрешено ли перенос учетных данных из подсистемы локального центра безопасности Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-670">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="6e70b-671">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-671">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-672">дефендерпроцесскреатионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-672">defenderProcessCreationType</span></span>|[<span data-ttu-id="6e70b-673">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-673">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e70b-674">Значение, указывающее ответ на создание процессов, исходящих от команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="6e70b-674">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="6e70b-675">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-675">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-676">дефендерпроцесскреатион</span><span class="sxs-lookup"><span data-stu-id="6e70b-676">defenderProcessCreation</span></span>|[<span data-ttu-id="6e70b-677">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-677">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e70b-678">Значение, указывающее ответ на создание процессов, исходящих от команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="6e70b-678">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="6e70b-679">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-679">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-680">дефендерунтрустедусбпроцесстипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-680">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="6e70b-681">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-681">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e70b-682">Значение, указывающее ответ на недоверенные и неподписанные процессы, которые запускаются с USB.</span><span class="sxs-lookup"><span data-stu-id="6e70b-682">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="6e70b-683">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-683">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-684">дефендерунтрустедусбпроцесс</span><span class="sxs-lookup"><span data-stu-id="6e70b-684">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="6e70b-685">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-685">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e70b-686">Значение, указывающее ответ на недоверенные и неподписанные процессы, которые запускаются с USB.</span><span class="sxs-lookup"><span data-stu-id="6e70b-686">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="6e70b-687">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-687">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-688">дефендерунтрустедексекутаблетипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-688">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="6e70b-689">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-689">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e70b-690">Значение, указывающее ответ на исполняемые файлы, которые не отвечают условиям преобладание, возраст или доверенного списка.</span><span class="sxs-lookup"><span data-stu-id="6e70b-690">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="6e70b-691">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-691">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-692">дефендерунтрустедексекутабле</span><span class="sxs-lookup"><span data-stu-id="6e70b-692">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="6e70b-693">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-693">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e70b-694">Значение, указывающее ответ на исполняемые файлы, которые не отвечают условиям преобладание, возраст или доверенного списка.</span><span class="sxs-lookup"><span data-stu-id="6e70b-694">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="6e70b-695">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-695">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-696">дефендеремаилконтентексекутионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-696">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="6e70b-697">дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-697">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e70b-698">Значение, указывающее, следует ли удалять исполняемые файлы (exe, DLL, PS, JS, VBS и т. д.) из электронной почты (почтовая или почтовая программа).</span><span class="sxs-lookup"><span data-stu-id="6e70b-698">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="6e70b-699">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-699">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-700">дефендеремаилконтентексекутион</span><span class="sxs-lookup"><span data-stu-id="6e70b-700">defenderEmailContentExecution</span></span>|[<span data-ttu-id="6e70b-701">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-701">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e70b-702">Значение, указывающее, следует ли удалять исполняемые файлы (exe, DLL, PS, JS, VBS и т. д.) из электронной почты (почтовая или почтовая программа).</span><span class="sxs-lookup"><span data-stu-id="6e70b-702">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="6e70b-703">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-703">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-704">дефендерадванцедрансомеварепротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-704">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="6e70b-705">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-705">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e70b-706">Значение, указывающее на использование расширенной защиты в рансомеваре.</span><span class="sxs-lookup"><span data-stu-id="6e70b-706">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="6e70b-707">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-707">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-708">дефендергуардмифолдерстипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-708">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="6e70b-709">фолдерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-709">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="6e70b-710">Значение, указывающее поведение защищенных папок.</span><span class="sxs-lookup"><span data-stu-id="6e70b-710">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="6e70b-711">Возможные значения: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-711">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="6e70b-712">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="6e70b-712">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="6e70b-713">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6e70b-713">String collection</span></span>|<span data-ttu-id="6e70b-714">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="6e70b-714">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="6e70b-715">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="6e70b-715">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="6e70b-716">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6e70b-716">String collection</span></span>|<span data-ttu-id="6e70b-717">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="6e70b-717">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="6e70b-718">дефендернетворкпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-718">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="6e70b-719">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-719">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e70b-720">Значение, указывающее поведение Нетворкпротектион.</span><span class="sxs-lookup"><span data-stu-id="6e70b-720">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="6e70b-721">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-721">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-722">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="6e70b-722">defenderExploitProtectionXml</span></span>|<span data-ttu-id="6e70b-723">Binary</span><span class="sxs-lookup"><span data-stu-id="6e70b-723">Binary</span></span>|<span data-ttu-id="6e70b-724">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-724">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="6e70b-725">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="6e70b-725">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="6e70b-726">String</span><span class="sxs-lookup"><span data-stu-id="6e70b-726">String</span></span>|<span data-ttu-id="6e70b-727">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="6e70b-727">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="6e70b-728">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="6e70b-728">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="6e70b-729">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-729">Boolean</span></span>|<span data-ttu-id="6e70b-730">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-730">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="6e70b-731">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="6e70b-731">appLockerApplicationControl</span></span>|[<span data-ttu-id="6e70b-732">апплоккераппликатионконтролтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-732">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="6e70b-733">Позволяет администратору выбирать разрешенные типы приложений для устройств.</span><span class="sxs-lookup"><span data-stu-id="6e70b-733">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="6e70b-734">Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-734">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="6e70b-735">девицегуардлокалсистемаусоритикредентиалгуардсеттингс</span><span class="sxs-lookup"><span data-stu-id="6e70b-735">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="6e70b-736">девицегуардлокалсистемаусоритикредентиалгуардтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-736">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="6e70b-737">Включите Guard в учетных данных, когда включен уровень безопасности платформы с безопасной загрузкой и безопасностью на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="6e70b-737">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="6e70b-738">Возможные значения: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-738">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`, `disable`.</span></span>|
|<span data-ttu-id="6e70b-739">девицегуарденаблевиртуализатионбаседсекурити</span><span class="sxs-lookup"><span data-stu-id="6e70b-739">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="6e70b-740">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-740">Boolean</span></span>|<span data-ttu-id="6e70b-741">Включает безопасность на основе виртуализации (VBS).</span><span class="sxs-lookup"><span data-stu-id="6e70b-741">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="6e70b-742">девицегуарденаблесекуребутвисдма</span><span class="sxs-lookup"><span data-stu-id="6e70b-742">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="6e70b-743">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-743">Boolean</span></span>|<span data-ttu-id="6e70b-744">Это свойство будет устаревшим в 2019 мая и будет заменено свойством Девицегуардсекуребутвисдма.</span><span class="sxs-lookup"><span data-stu-id="6e70b-744">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="6e70b-745">Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="6e70b-745">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="6e70b-746">девицегуардсекуребутвисдма</span><span class="sxs-lookup"><span data-stu-id="6e70b-746">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="6e70b-747">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="6e70b-747">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="6e70b-748">Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="6e70b-748">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="6e70b-749">Возможные значения: `notConfigured`, `withoutDMA`, `withDMA`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-749">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="6e70b-750">девицегуардлаунчсистемгуард</span><span class="sxs-lookup"><span data-stu-id="6e70b-750">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="6e70b-751">Включение</span><span class="sxs-lookup"><span data-stu-id="6e70b-751">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="6e70b-752">Позволяет ИТ – администратору настраивать запуск системы защиты системы.</span><span class="sxs-lookup"><span data-stu-id="6e70b-752">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="6e70b-753">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-753">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="6e70b-754">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="6e70b-754">smartScreenEnableInShell</span></span>|<span data-ttu-id="6e70b-755">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-755">Boolean</span></span>|<span data-ttu-id="6e70b-756">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-756">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="6e70b-757">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="6e70b-757">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="6e70b-758">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-758">Boolean</span></span>|<span data-ttu-id="6e70b-759">Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="6e70b-759">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="6e70b-760">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="6e70b-760">applicationGuardEnabled</span></span>|<span data-ttu-id="6e70b-761">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-761">Boolean</span></span>|<span data-ttu-id="6e70b-762">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="6e70b-762">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="6e70b-763">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="6e70b-763">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="6e70b-764">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="6e70b-764">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="6e70b-765">Включение Application Guard в Защитнике Windows для более новых сборок Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-765">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="6e70b-766">Возможные значения: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-766">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="6e70b-767">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="6e70b-767">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="6e70b-768">аппликатионгуардблоккфилетрансфертипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-768">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="6e70b-769">Блокировать буфер обмена для передачи файла изображения, текстового файла или ни одного из них.</span><span class="sxs-lookup"><span data-stu-id="6e70b-769">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="6e70b-770">Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-770">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="6e70b-771">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="6e70b-771">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="6e70b-772">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-772">Boolean</span></span>|<span data-ttu-id="6e70b-773">Позволяет заблокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="6e70b-773">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="6e70b-774">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="6e70b-774">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="6e70b-775">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-775">Boolean</span></span>|<span data-ttu-id="6e70b-776">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="6e70b-776">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="6e70b-777">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="6e70b-777">applicationGuardForceAuditing</span></span>|<span data-ttu-id="6e70b-778">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-778">Boolean</span></span>|<span data-ttu-id="6e70b-779">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="6e70b-779">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="6e70b-780">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="6e70b-780">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="6e70b-781">аппликатионгуардблоккклипбоардшарингтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-781">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="6e70b-782">Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="6e70b-782">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="6e70b-783">Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-783">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="6e70b-784">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="6e70b-784">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="6e70b-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-785">Boolean</span></span>|<span data-ttu-id="6e70b-786">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="6e70b-786">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="6e70b-787">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="6e70b-787">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="6e70b-788">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-788">Boolean</span></span>|<span data-ttu-id="6e70b-789">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="6e70b-789">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="6e70b-790">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="6e70b-790">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="6e70b-791">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-791">Boolean</span></span>|<span data-ttu-id="6e70b-792">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="6e70b-792">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="6e70b-793">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="6e70b-793">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="6e70b-794">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-794">Boolean</span></span>|<span data-ttu-id="6e70b-795">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="6e70b-795">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="6e70b-796">аппликатионгуардалловвиртуалгпу</span><span class="sxs-lookup"><span data-stu-id="6e70b-796">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="6e70b-797">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-797">Boolean</span></span>|<span data-ttu-id="6e70b-798">Разрешить приложению Application Guard использовать виртуальный GPU</span><span class="sxs-lookup"><span data-stu-id="6e70b-798">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="6e70b-799">аппликатионгуардалловфилесавеонхост</span><span class="sxs-lookup"><span data-stu-id="6e70b-799">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="6e70b-800">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-800">Boolean</span></span>|<span data-ttu-id="6e70b-801">Разрешить пользователям скачивать файлы из EDGE в контейнере Application Guard и сохранять их в файловой системе узла</span><span class="sxs-lookup"><span data-stu-id="6e70b-801">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="6e70b-802">битлоккералловстандардусеренкриптион</span><span class="sxs-lookup"><span data-stu-id="6e70b-802">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="6e70b-803">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-803">Boolean</span></span>|<span data-ttu-id="6e70b-804">Позволяет администратору разрешить обычным пользователям включать енкрпитион во время присоединения к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6e70b-804">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="6e70b-805">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="6e70b-805">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="6e70b-806">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-806">Boolean</span></span>|<span data-ttu-id="6e70b-807">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="6e70b-807">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="6e70b-808">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="6e70b-808">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="6e70b-809">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-809">Boolean</span></span>|<span data-ttu-id="6e70b-810">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="6e70b-810">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="6e70b-811">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="6e70b-811">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="6e70b-812">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="6e70b-812">bitLockerEncryptDevice</span></span>|<span data-ttu-id="6e70b-813">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-813">Boolean</span></span>|<span data-ttu-id="6e70b-814">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="6e70b-814">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="6e70b-815">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6e70b-815">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="6e70b-816">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6e70b-816">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="6e70b-817">Политика системного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="6e70b-817">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="6e70b-818">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6e70b-818">bitLockerFixedDrivePolicy</span></span>|<span data-ttu-id="6e70b-819">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md);</span><span class="sxs-lookup"><span data-stu-id="6e70b-819">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)</span></span>|<span data-ttu-id="6e70b-820">Политика фиксированного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="6e70b-820">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="6e70b-821">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6e70b-821">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="6e70b-822">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6e70b-822">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="6e70b-823">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="6e70b-823">BitLocker Removable Drive Policy.</span></span>|
|<span data-ttu-id="6e70b-824">битлоккеррековерипассвордротатион</span><span class="sxs-lookup"><span data-stu-id="6e70b-824">bitLockerRecoveryPasswordRotation</span></span>|[<span data-ttu-id="6e70b-825">bitLockerRecoveryPasswordRotationType</span><span class="sxs-lookup"><span data-stu-id="6e70b-825">bitLockerRecoveryPasswordRotationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|<span data-ttu-id="6e70b-826">Этот параметр инициирует поворот пароля восстановления на основе клиента после восстановления диска ОС (с помощью BOOTMGR или WinRE).</span><span class="sxs-lookup"><span data-stu-id="6e70b-826">This setting initiates a client-driven recovery password rotation after an OS drive recovery (either by using bootmgr or WinRE).</span></span> <span data-ttu-id="6e70b-827">Возможные значения: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-827">Possible values are: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span></span>|
|<span data-ttu-id="6e70b-828">дефендердисаблесканарчивефилес</span><span class="sxs-lookup"><span data-stu-id="6e70b-828">defenderDisableScanArchiveFiles</span></span>|<span data-ttu-id="6e70b-829">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-829">Boolean</span></span>|<span data-ttu-id="6e70b-830">Разрешает или запрещает сканирование архивов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-830">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="6e70b-831">дефендералловсканарчивефилес</span><span class="sxs-lookup"><span data-stu-id="6e70b-831">defenderAllowScanArchiveFiles</span></span>|<span data-ttu-id="6e70b-832">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-832">Boolean</span></span>|<span data-ttu-id="6e70b-833">Разрешает или запрещает сканирование архивов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-833">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="6e70b-834">дефендердисаблебехавиормониторинг</span><span class="sxs-lookup"><span data-stu-id="6e70b-834">defenderDisableBehaviorMonitoring</span></span>|<span data-ttu-id="6e70b-835">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-835">Boolean</span></span>|<span data-ttu-id="6e70b-836">Разрешает или запрещает функции мониторинга режима защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-836">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="6e70b-837">дефендералловбехавиормониторинг</span><span class="sxs-lookup"><span data-stu-id="6e70b-837">defenderAllowBehaviorMonitoring</span></span>|<span data-ttu-id="6e70b-838">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-838">Boolean</span></span>|<span data-ttu-id="6e70b-839">Разрешает или запрещает функции мониторинга режима защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-839">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="6e70b-840">дефендердисаблеклаудпротектион</span><span class="sxs-lookup"><span data-stu-id="6e70b-840">defenderDisableCloudProtection</span></span>|<span data-ttu-id="6e70b-841">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-841">Boolean</span></span>|<span data-ttu-id="6e70b-842">Чтобы лучше защитить компьютер, защитник Windows будет отправлять в корпорацию Майкрософт сведения обо всех обнаруженных неполадках.</span><span class="sxs-lookup"><span data-stu-id="6e70b-842">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="6e70b-843">Корпорация Майкрософт проанализирует эти сведения, Узнайте больше об ошибках, которые могут повлиять на ваших клиентов и других пользователей, и предложит улучшенные решения.</span><span class="sxs-lookup"><span data-stu-id="6e70b-843">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="6e70b-844">дефендералловклаудпротектион</span><span class="sxs-lookup"><span data-stu-id="6e70b-844">defenderAllowCloudProtection</span></span>|<span data-ttu-id="6e70b-845">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-845">Boolean</span></span>|<span data-ttu-id="6e70b-846">Чтобы лучше защитить компьютер, защитник Windows будет отправлять в корпорацию Майкрософт сведения обо всех обнаруженных неполадках.</span><span class="sxs-lookup"><span data-stu-id="6e70b-846">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="6e70b-847">Корпорация Майкрософт проанализирует эти сведения, Узнайте больше об ошибках, которые могут повлиять на ваших клиентов и других пользователей, и предложит улучшенные решения.</span><span class="sxs-lookup"><span data-stu-id="6e70b-847">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="6e70b-848">дефендеренаблесканинкомингмаил</span><span class="sxs-lookup"><span data-stu-id="6e70b-848">defenderEnableScanIncomingMail</span></span>|<span data-ttu-id="6e70b-849">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-849">Boolean</span></span>|<span data-ttu-id="6e70b-850">Разрешает или запрещает сканирование электронной почты.</span><span class="sxs-lookup"><span data-stu-id="6e70b-850">Allows or disallows scanning of email.</span></span>|
|<span data-ttu-id="6e70b-851">дефендеренаблесканмаппеднетворкдривесдурингфуллскан</span><span class="sxs-lookup"><span data-stu-id="6e70b-851">defenderEnableScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="6e70b-852">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-852">Boolean</span></span>|<span data-ttu-id="6e70b-853">Разрешает или запрещает полное сканирование подключенных сетевых дисков.</span><span class="sxs-lookup"><span data-stu-id="6e70b-853">Allows or disallows a full scan of mapped network drives.</span></span>|
|<span data-ttu-id="6e70b-854">дефендердисаблесканремовабледривесдурингфуллскан</span><span class="sxs-lookup"><span data-stu-id="6e70b-854">defenderDisableScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="6e70b-855">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-855">Boolean</span></span>|<span data-ttu-id="6e70b-856">Разрешает или запрещает полное сканирование съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="6e70b-856">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="6e70b-857">Во время быстрого сканирования съемные диски все еще могут сканироваться.</span><span class="sxs-lookup"><span data-stu-id="6e70b-857">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="6e70b-858">дефендералловсканремовабледривесдурингфуллскан</span><span class="sxs-lookup"><span data-stu-id="6e70b-858">defenderAllowScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="6e70b-859">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-859">Boolean</span></span>|<span data-ttu-id="6e70b-860">Разрешает или запрещает полное сканирование съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="6e70b-860">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="6e70b-861">Во время быстрого сканирования съемные диски все еще могут сканироваться.</span><span class="sxs-lookup"><span data-stu-id="6e70b-861">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="6e70b-862">дефендердисаблескандовнлоадс</span><span class="sxs-lookup"><span data-stu-id="6e70b-862">defenderDisableScanDownloads</span></span>|<span data-ttu-id="6e70b-863">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-863">Boolean</span></span>|<span data-ttu-id="6e70b-864">Разрешает или запрещает функции защиты ИОАВП защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-864">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="6e70b-865">дефендералловскандовнлоадс</span><span class="sxs-lookup"><span data-stu-id="6e70b-865">defenderAllowScanDownloads</span></span>|<span data-ttu-id="6e70b-866">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-866">Boolean</span></span>|<span data-ttu-id="6e70b-867">Разрешает или запрещает функции защиты ИОАВП защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-867">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="6e70b-868">дефендердисаблеинтрусионпревентионсистем</span><span class="sxs-lookup"><span data-stu-id="6e70b-868">defenderDisableIntrusionPreventionSystem</span></span>|<span data-ttu-id="6e70b-869">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-869">Boolean</span></span>|<span data-ttu-id="6e70b-870">Разрешает или запрещает функции предотвращения вторжения в Защитнике Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-870">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="6e70b-871">дефендералловинтрусионпревентионсистем</span><span class="sxs-lookup"><span data-stu-id="6e70b-871">defenderAllowIntrusionPreventionSystem</span></span>|<span data-ttu-id="6e70b-872">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-872">Boolean</span></span>|<span data-ttu-id="6e70b-873">Разрешает или запрещает функции предотвращения вторжения в Защитнике Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-873">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="6e70b-874">дефендердисаблеонакцесспротектион</span><span class="sxs-lookup"><span data-stu-id="6e70b-874">defenderDisableOnAccessProtection</span></span>|<span data-ttu-id="6e70b-875">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-875">Boolean</span></span>|<span data-ttu-id="6e70b-876">Разрешает или запрещает защитник Windows для функций защиты доступа.</span><span class="sxs-lookup"><span data-stu-id="6e70b-876">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="6e70b-877">дефендералловонакцесспротектион</span><span class="sxs-lookup"><span data-stu-id="6e70b-877">defenderAllowOnAccessProtection</span></span>|<span data-ttu-id="6e70b-878">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-878">Boolean</span></span>|<span data-ttu-id="6e70b-879">Разрешает или запрещает защитник Windows для функций защиты доступа.</span><span class="sxs-lookup"><span data-stu-id="6e70b-879">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="6e70b-880">дефендердисаблереалтимемониторинг</span><span class="sxs-lookup"><span data-stu-id="6e70b-880">defenderDisableRealTimeMonitoring</span></span>|<span data-ttu-id="6e70b-881">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-881">Boolean</span></span>|<span data-ttu-id="6e70b-882">Разрешает или запрещает функции мониторинга в режиме реального времени защитник Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-882">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="6e70b-883">дефендералловреалтимемониторинг</span><span class="sxs-lookup"><span data-stu-id="6e70b-883">defenderAllowRealTimeMonitoring</span></span>|<span data-ttu-id="6e70b-884">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-884">Boolean</span></span>|<span data-ttu-id="6e70b-885">Разрешает или запрещает функции мониторинга в режиме реального времени защитник Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-885">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="6e70b-886">дефендердисаблесканнетворкфилес</span><span class="sxs-lookup"><span data-stu-id="6e70b-886">defenderDisableScanNetworkFiles</span></span>|<span data-ttu-id="6e70b-887">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-887">Boolean</span></span>|<span data-ttu-id="6e70b-888">Разрешает или запрещает сканирование сетевых файлов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-888">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="6e70b-889">дефендералловсканнетворкфилес</span><span class="sxs-lookup"><span data-stu-id="6e70b-889">defenderAllowScanNetworkFiles</span></span>|<span data-ttu-id="6e70b-890">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-890">Boolean</span></span>|<span data-ttu-id="6e70b-891">Разрешает или запрещает сканирование сетевых файлов.</span><span class="sxs-lookup"><span data-stu-id="6e70b-891">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="6e70b-892">дефендердисаблесканскриптслоадедининтернетексплорер</span><span class="sxs-lookup"><span data-stu-id="6e70b-892">defenderDisableScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="6e70b-893">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-893">Boolean</span></span>|<span data-ttu-id="6e70b-894">Разрешает или запрещает функцию сканирования сценариев защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-894">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="6e70b-895">дефендералловсканскриптслоадедининтернетексплорер</span><span class="sxs-lookup"><span data-stu-id="6e70b-895">defenderAllowScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="6e70b-896">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-896">Boolean</span></span>|<span data-ttu-id="6e70b-897">Разрешает или запрещает функцию сканирования сценариев защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-897">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="6e70b-898">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="6e70b-898">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="6e70b-899">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-899">Boolean</span></span>|<span data-ttu-id="6e70b-900">Разрешает или запрещает пользователям доступ к пользовательскому интерфейсу защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-900">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="6e70b-901">Если этот флажок не разрешен, все уведомления защитника Windows также будут подавляться.</span><span class="sxs-lookup"><span data-stu-id="6e70b-901">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="6e70b-902">дефендералловендусеракцесс</span><span class="sxs-lookup"><span data-stu-id="6e70b-902">defenderAllowEndUserAccess</span></span>|<span data-ttu-id="6e70b-903">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-903">Boolean</span></span>|<span data-ttu-id="6e70b-904">Разрешает или запрещает пользователям доступ к пользовательскому интерфейсу защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-904">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="6e70b-905">Если этот флажок не разрешен, все уведомления защитника Windows также будут подавляться.</span><span class="sxs-lookup"><span data-stu-id="6e70b-905">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="6e70b-906">дефендерсканмакскпуперцентаже</span><span class="sxs-lookup"><span data-stu-id="6e70b-906">defenderScanMaxCpuPercentage</span></span>|<span data-ttu-id="6e70b-907">Int32</span><span class="sxs-lookup"><span data-stu-id="6e70b-907">Int32</span></span>|<span data-ttu-id="6e70b-908">Представляет средний коэффициент загрузки ЦП для сканирования защитником Windows (в процентах).</span><span class="sxs-lookup"><span data-stu-id="6e70b-908">Represents the average CPU load factor for the Windows Defender scan (in percent).</span></span> <span data-ttu-id="6e70b-909">Значение по умолчанию равно 50.</span><span class="sxs-lookup"><span data-stu-id="6e70b-909">The default value is 50.</span></span> <span data-ttu-id="6e70b-910">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="6e70b-910">Valid values 0 to 100</span></span>|
|<span data-ttu-id="6e70b-911">дефендерчеккфорсигнатуресбефореруннингскан</span><span class="sxs-lookup"><span data-stu-id="6e70b-911">defenderCheckForSignaturesBeforeRunningScan</span></span>|<span data-ttu-id="6e70b-912">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-912">Boolean</span></span>|<span data-ttu-id="6e70b-913">Этот параметр политики позволяет управлять тем, будет ли выполняться проверка новых определений вирусов и программ-шпионов перед выполнением проверки.</span><span class="sxs-lookup"><span data-stu-id="6e70b-913">This policy setting allows you to manage whether a check for new virus and spyware definitions will occur before running a scan.</span></span>|
|<span data-ttu-id="6e70b-914">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="6e70b-914">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="6e70b-915">дефендерклаудблокклевелтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-915">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="6e70b-916">Добавлено в Windows 10 версии 1709.</span><span class="sxs-lookup"><span data-stu-id="6e70b-916">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="6e70b-917">Этот параметр политики определяет, как активно антивирусная программа "Защитник Windows" будет блокировать и сканировать подозрительные файлы.</span><span class="sxs-lookup"><span data-stu-id="6e70b-917">This policy setting determines how aggressive Windows Defender Antivirus will be in blocking and scanning suspicious files.</span></span> <span data-ttu-id="6e70b-918">Тип значения: целое число.</span><span class="sxs-lookup"><span data-stu-id="6e70b-918">Value type is integer.</span></span> <span data-ttu-id="6e70b-919">Для работы этой функции необходимо включить параметр "присоединение к Microsoft MAPS".</span><span class="sxs-lookup"><span data-stu-id="6e70b-919">This feature requires the "Join Microsoft MAPS" setting enabled in order to function.</span></span> <span data-ttu-id="6e70b-920">Возможные значения: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-920">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="6e70b-921">дефендерклаудекстендедтимеаутинсекондс</span><span class="sxs-lookup"><span data-stu-id="6e70b-921">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="6e70b-922">Int32</span><span class="sxs-lookup"><span data-stu-id="6e70b-922">Int32</span></span>|<span data-ttu-id="6e70b-923">Добавлено в Windows 10 версии 1709.</span><span class="sxs-lookup"><span data-stu-id="6e70b-923">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="6e70b-924">Эта функция позволяет антивирусной программе "Защитник Windows" заблокировать подозрительный файл размером до 60 секунд и проверить его в облаке, чтобы убедиться, что он безопасен.</span><span class="sxs-lookup"><span data-stu-id="6e70b-924">This feature allows Windows Defender Antivirus to block a suspicious file for up to 60 seconds, and scan it in the cloud to make sure it's safe.</span></span> <span data-ttu-id="6e70b-925">Тип значения: целое число, Range — 0-50.</span><span class="sxs-lookup"><span data-stu-id="6e70b-925">Value type is integer, range is 0 - 50.</span></span> <span data-ttu-id="6e70b-926">Эта функция зависит от трех других параметров карт, которые должны быть включены — "Настройка блока при первом пошаговом отображении"; " Присоединяйтесь к Microsoft MAPS "; "Отправлять образцы файлов, когда необходим дальнейший анализ".</span><span class="sxs-lookup"><span data-stu-id="6e70b-926">This feature depends on three other MAPS settings the must all be enabled- "Configure the 'Block at First Sight' feature; "Join Microsoft MAPS"; "Send file samples when further analysis is required".</span></span> <span data-ttu-id="6e70b-927">Допустимые значения: от 0 до 50.</span><span class="sxs-lookup"><span data-stu-id="6e70b-927">Valid values 0 to 50</span></span>|
|<span data-ttu-id="6e70b-928">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="6e70b-928">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="6e70b-929">Int32</span><span class="sxs-lookup"><span data-stu-id="6e70b-929">Int32</span></span>|<span data-ttu-id="6e70b-930">Период времени (в днях), в течение которого элементы, помещенные в карантин, будут храниться в системе.</span><span class="sxs-lookup"><span data-stu-id="6e70b-930">Time period (in days) that quarantine items will be stored on the system.</span></span> <span data-ttu-id="6e70b-931">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="6e70b-931">Valid values 0 to 90</span></span>|
|<span data-ttu-id="6e70b-932">дефендердисаблекатчупфуллскан</span><span class="sxs-lookup"><span data-stu-id="6e70b-932">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="6e70b-933">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-933">Boolean</span></span>|<span data-ttu-id="6e70b-934">Этот параметр политики позволяет настроить поиск по расписанию для полного сканирования.</span><span class="sxs-lookup"><span data-stu-id="6e70b-934">This policy setting allows you to configure catch-up scans for scheduled full scans.</span></span> <span data-ttu-id="6e70b-935">Вторичное сканирование — это сканирование, которое инициируется из-за пропускной ошибки запланированной проверки.</span><span class="sxs-lookup"><span data-stu-id="6e70b-935">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="6e70b-936">Обычно эти запланированные проверки пропущены, так как компьютер был отключен в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="6e70b-936">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="6e70b-937">дефендердисаблекатчупкуиккскан</span><span class="sxs-lookup"><span data-stu-id="6e70b-937">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="6e70b-938">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-938">Boolean</span></span>|<span data-ttu-id="6e70b-939">Этот параметр политики позволяет настроить дополнительные проверки для запланированных быстрых проверок.</span><span class="sxs-lookup"><span data-stu-id="6e70b-939">This policy setting allows you to configure catch-up scans for scheduled quick scans.</span></span> <span data-ttu-id="6e70b-940">Вторичное сканирование — это сканирование, которое инициируется из-за пропускной ошибки запланированной проверки.</span><span class="sxs-lookup"><span data-stu-id="6e70b-940">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="6e70b-941">Обычно эти запланированные проверки пропущены, так как компьютер был отключен в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="6e70b-941">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="6e70b-942">дефендеренаблеловкпуприорити</span><span class="sxs-lookup"><span data-stu-id="6e70b-942">defenderEnableLowCpuPriority</span></span>|<span data-ttu-id="6e70b-943">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e70b-943">Boolean</span></span>|<span data-ttu-id="6e70b-944">Этот параметр политики позволяет включать или отключать минимальный приоритет ЦП для запланированных проверок.</span><span class="sxs-lookup"><span data-stu-id="6e70b-944">This policy setting allows you to enable or disable low CPU priority for scheduled scans.</span></span>|
|<span data-ttu-id="6e70b-945">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="6e70b-945">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="6e70b-946">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6e70b-946">String collection</span></span>|<span data-ttu-id="6e70b-947">Расширения файлов, которые необходимо исключить из проверки и защиты в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="6e70b-947">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="6e70b-948">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="6e70b-948">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="6e70b-949">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6e70b-949">String collection</span></span>|<span data-ttu-id="6e70b-950">Файлы и папки, которые необходимо исключить из проверки и защиты в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="6e70b-950">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="6e70b-951">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="6e70b-951">defenderProcessesToExclude</span></span>|<span data-ttu-id="6e70b-952">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6e70b-952">String collection</span></span>|<span data-ttu-id="6e70b-953">Процессы, которые необходимо исключить из проверки и защиты в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="6e70b-953">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="6e70b-954">дефендерпотентиаллюнвантедаппактион</span><span class="sxs-lookup"><span data-stu-id="6e70b-954">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="6e70b-955">дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="6e70b-955">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e70b-956">Добавлено в Windows 10 версии 1607.</span><span class="sxs-lookup"><span data-stu-id="6e70b-956">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="6e70b-957">Задает уровень обнаружения для потенциально нежелательных приложений (Пуас).</span><span class="sxs-lookup"><span data-stu-id="6e70b-957">Specifies the level of detection for potentially unwanted applications (PUAs).</span></span> <span data-ttu-id="6e70b-958">Защитник Windows предупреждает вас о том, что загружается потенциально нежелательное программное обеспечение, или пытается установить себя на компьютер.</span><span class="sxs-lookup"><span data-stu-id="6e70b-958">Windows Defender alerts you when potentially unwanted software is being downloaded or attempts to install itself on your computer.</span></span> <span data-ttu-id="6e70b-959">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-959">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e70b-960">дефендерскандиректион</span><span class="sxs-lookup"><span data-stu-id="6e70b-960">defenderScanDirection</span></span>|[<span data-ttu-id="6e70b-961">defenderRealtimeScanDirection</span><span class="sxs-lookup"><span data-stu-id="6e70b-961">defenderRealtimeScanDirection</span></span>](../resources/intune-deviceconfig-defenderrealtimescandirection.md)|<span data-ttu-id="6e70b-962">Определяет, какие наборы файлов следует отслеживать.</span><span class="sxs-lookup"><span data-stu-id="6e70b-962">Controls which sets of files should be monitored.</span></span> <span data-ttu-id="6e70b-963">Возможные значения: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-963">Possible values are: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="6e70b-964">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="6e70b-964">defenderScanType</span></span>|[<span data-ttu-id="6e70b-965">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="6e70b-965">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="6e70b-966">Позволяет выбрать, следует ли выполнять быструю или полную проверку.</span><span class="sxs-lookup"><span data-stu-id="6e70b-966">Selects whether to perform a quick scan or full scan.</span></span> <span data-ttu-id="6e70b-967">Возможные значения: `userDefined`, `disabled`, `quick`, `full`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-967">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="6e70b-968">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="6e70b-968">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="6e70b-969">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6e70b-969">TimeOfDay</span></span>|<span data-ttu-id="6e70b-970">Выбирает время суток, которое должно выполняться при запуске быстрого сканирования защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-970">Selects the time of day that the Windows Defender quick scan should run.</span></span> <span data-ttu-id="6e70b-971">Например, значение 0 = 12:00AM, значение 60 = 1:00AM, значение 120 = 2:00 и т. д., вплоть до значения 1380 = 11:00PM.</span><span class="sxs-lookup"><span data-stu-id="6e70b-971">For example, a value of 0=12:00AM, a value of 60=1:00AM, a value of 120=2:00, and so on, up to a value of 1380=11:00PM.</span></span> <span data-ttu-id="6e70b-972">Значение по умолчанию — 120</span><span class="sxs-lookup"><span data-stu-id="6e70b-972">The default value is 120</span></span>|
|<span data-ttu-id="6e70b-973">дефендерсчедуледскандай</span><span class="sxs-lookup"><span data-stu-id="6e70b-973">defenderScheduledScanDay</span></span>|[<span data-ttu-id="6e70b-974">виклисчедуле</span><span class="sxs-lookup"><span data-stu-id="6e70b-974">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="6e70b-975">Выбирает день запуска проверки защитником Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-975">Selects the day that the Windows Defender scan should run.</span></span> <span data-ttu-id="6e70b-976">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-976">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="6e70b-977">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="6e70b-977">defenderScheduledScanTime</span></span>|<span data-ttu-id="6e70b-978">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6e70b-978">TimeOfDay</span></span>|<span data-ttu-id="6e70b-979">Выбирает время суток, в течение которого должно выполняться сканирование защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="6e70b-979">Selects the time of day that the Windows Defender scan should run.</span></span>|
|<span data-ttu-id="6e70b-980">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="6e70b-980">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="6e70b-981">Int32</span><span class="sxs-lookup"><span data-stu-id="6e70b-981">Int32</span></span>|<span data-ttu-id="6e70b-982">Указывает интервал (в часах), который будет использоваться для проверки подписей, поэтому вместо использования Счедуледай и Счедулетиме проверка новых подписей будет установлена в соответствии с интервалом.</span><span class="sxs-lookup"><span data-stu-id="6e70b-982">Specifies the interval (in hours) that will be used to check for signatures, so instead of using the ScheduleDay and ScheduleTime the check for new signatures will be set according to the interval.</span></span> <span data-ttu-id="6e70b-983">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="6e70b-983">Valid values 0 to 24</span></span>|
|<span data-ttu-id="6e70b-984">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="6e70b-984">defenderSubmitSamplesConsentType</span></span>|<span data-ttu-id="6e70b-985">[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md);</span><span class="sxs-lookup"><span data-stu-id="6e70b-985">[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)</span></span>|<span data-ttu-id="6e70b-986">Проверка уровня согласия пользователя в Защитнике Windows для отправки данных.</span><span class="sxs-lookup"><span data-stu-id="6e70b-986">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="6e70b-987">Возможные значения: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span><span class="sxs-lookup"><span data-stu-id="6e70b-987">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="6e70b-988">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="6e70b-988">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="6e70b-989">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="6e70b-989">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="6e70b-990">Позволяет администратору указать допустимые уровни серьезности угроз и соответствующий идентификатор действия по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6e70b-990">Allows an administrator to specify any valid threat severity levels and the corresponding default action ID to take.</span></span>|



## <a name="response"></a><span data-ttu-id="6e70b-991">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e70b-991">Response</span></span>
<span data-ttu-id="6e70b-992">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6e70b-992">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e70b-993">Пример</span><span class="sxs-lookup"><span data-stu-id="6e70b-993">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e70b-994">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e70b-994">Request</span></span>
<span data-ttu-id="6e70b-995">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e70b-995">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 31045

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
  "firewallIPSecExemptionsNone": true,
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
  "defenderAllowScanArchiveFiles": true,
  "defenderDisableBehaviorMonitoring": true,
  "defenderAllowBehaviorMonitoring": true,
  "defenderDisableCloudProtection": true,
  "defenderAllowCloudProtection": true,
  "defenderEnableScanIncomingMail": true,
  "defenderEnableScanMappedNetworkDrivesDuringFullScan": true,
  "defenderDisableScanRemovableDrivesDuringFullScan": true,
  "defenderAllowScanRemovableDrivesDuringFullScan": true,
  "defenderDisableScanDownloads": true,
  "defenderAllowScanDownloads": true,
  "defenderDisableIntrusionPreventionSystem": true,
  "defenderAllowIntrusionPreventionSystem": true,
  "defenderDisableOnAccessProtection": true,
  "defenderAllowOnAccessProtection": true,
  "defenderDisableRealTimeMonitoring": true,
  "defenderAllowRealTimeMonitoring": true,
  "defenderDisableScanNetworkFiles": true,
  "defenderAllowScanNetworkFiles": true,
  "defenderDisableScanScriptsLoadedInInternetExplorer": true,
  "defenderAllowScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderAllowEndUserAccess": true,
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
  "defenderSignatureUpdateIntervalInHours": 6,
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

### <a name="response"></a><span data-ttu-id="6e70b-996">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e70b-996">Response</span></span>
<span data-ttu-id="6e70b-p225">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e70b-p225">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 31217

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
  "firewallIPSecExemptionsNone": true,
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
  "defenderAllowScanArchiveFiles": true,
  "defenderDisableBehaviorMonitoring": true,
  "defenderAllowBehaviorMonitoring": true,
  "defenderDisableCloudProtection": true,
  "defenderAllowCloudProtection": true,
  "defenderEnableScanIncomingMail": true,
  "defenderEnableScanMappedNetworkDrivesDuringFullScan": true,
  "defenderDisableScanRemovableDrivesDuringFullScan": true,
  "defenderAllowScanRemovableDrivesDuringFullScan": true,
  "defenderDisableScanDownloads": true,
  "defenderAllowScanDownloads": true,
  "defenderDisableIntrusionPreventionSystem": true,
  "defenderAllowIntrusionPreventionSystem": true,
  "defenderDisableOnAccessProtection": true,
  "defenderAllowOnAccessProtection": true,
  "defenderDisableRealTimeMonitoring": true,
  "defenderAllowRealTimeMonitoring": true,
  "defenderDisableScanNetworkFiles": true,
  "defenderAllowScanNetworkFiles": true,
  "defenderDisableScanScriptsLoadedInInternetExplorer": true,
  "defenderAllowScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderAllowEndUserAccess": true,
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
  "defenderSignatureUpdateIntervalInHours": 6,
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






