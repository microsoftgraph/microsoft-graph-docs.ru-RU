---
title: Создание windows10EndpointProtectionConfiguration
description: Создание объекта windows10EndpointProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 01f5393b9fd91336c7711931f46ecfa50195e889
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137044"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="ec12b-103">Создание windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec12b-103">Create windows10EndpointProtectionConfiguration</span></span>

<span data-ttu-id="ec12b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec12b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec12b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec12b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec12b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec12b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec12b-107">Создание объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec12b-107">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec12b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ec12b-108">Prerequisites</span></span>
<span data-ttu-id="ec12b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec12b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec12b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec12b-111">Permission type</span></span>|<span data-ttu-id="ec12b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec12b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec12b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec12b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec12b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec12b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ec12b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec12b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec12b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec12b-116">Not supported.</span></span>|
|<span data-ttu-id="ec12b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ec12b-117">Application</span></span>|<span data-ttu-id="ec12b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec12b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec12b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec12b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ec12b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ec12b-120">Request headers</span></span>
|<span data-ttu-id="ec12b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ec12b-121">Header</span></span>|<span data-ttu-id="ec12b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ec12b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec12b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec12b-123">Authorization</span></span>|<span data-ttu-id="ec12b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec12b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec12b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ec12b-125">Accept</span></span>|<span data-ttu-id="ec12b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ec12b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec12b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec12b-127">Request body</span></span>
<span data-ttu-id="ec12b-128">В теле запроса добавьте представление объекта windows10EndpointProtectionConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec12b-128">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="ec12b-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ec12b-129">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="ec12b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec12b-130">Property</span></span>|<span data-ttu-id="ec12b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ec12b-131">Type</span></span>|<span data-ttu-id="ec12b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ec12b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec12b-133">id</span><span class="sxs-lookup"><span data-stu-id="ec12b-133">id</span></span>|<span data-ttu-id="ec12b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ec12b-134">String</span></span>|<span data-ttu-id="ec12b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ec12b-135">Key of the entity.</span></span> <span data-ttu-id="ec12b-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec12b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec12b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec12b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ec12b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec12b-138">DateTimeOffset</span></span>|<span data-ttu-id="ec12b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ec12b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ec12b-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec12b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec12b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ec12b-141">roleScopeTagIds</span></span>|<span data-ttu-id="ec12b-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ec12b-142">String collection</span></span>|<span data-ttu-id="ec12b-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="ec12b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ec12b-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec12b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec12b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ec12b-145">supportsScopeTags</span></span>|<span data-ttu-id="ec12b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-146">Boolean</span></span>|<span data-ttu-id="ec12b-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ec12b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ec12b-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="ec12b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ec12b-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ec12b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ec12b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec12b-150">This property is read-only.</span></span> <span data-ttu-id="ec12b-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec12b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec12b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ec12b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ec12b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ec12b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ec12b-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ec12b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ec12b-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec12b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec12b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ec12b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ec12b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ec12b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ec12b-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ec12b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ec12b-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec12b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec12b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ec12b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ec12b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ec12b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ec12b-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ec12b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ec12b-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec12b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec12b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ec12b-164">createdDateTime</span></span>|<span data-ttu-id="ec12b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec12b-165">DateTimeOffset</span></span>|<span data-ttu-id="ec12b-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ec12b-166">DateTime the object was created.</span></span> <span data-ttu-id="ec12b-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec12b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec12b-168">description</span><span class="sxs-lookup"><span data-stu-id="ec12b-168">description</span></span>|<span data-ttu-id="ec12b-169">Строка</span><span class="sxs-lookup"><span data-stu-id="ec12b-169">String</span></span>|<span data-ttu-id="ec12b-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ec12b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ec12b-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec12b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec12b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ec12b-172">displayName</span></span>|<span data-ttu-id="ec12b-173">Строка</span><span class="sxs-lookup"><span data-stu-id="ec12b-173">String</span></span>|<span data-ttu-id="ec12b-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ec12b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ec12b-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec12b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec12b-176">version</span><span class="sxs-lookup"><span data-stu-id="ec12b-176">version</span></span>|<span data-ttu-id="ec12b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ec12b-177">Int32</span></span>|<span data-ttu-id="ec12b-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ec12b-178">Version of the device configuration.</span></span> <span data-ttu-id="ec12b-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec12b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec12b-180">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="ec12b-180">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="ec12b-181">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="ec12b-181">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="ec12b-182">Эта политика предназначена для обеспечения дополнительной защиты от внешних устройств, способных к DMA.</span><span class="sxs-lookup"><span data-stu-id="ec12b-182">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="ec12b-183">Это позволяет больше контролировать переумывление внешних устройств, способных к DMA, несовместимых с DMA Remapping/device memory isolation and sandboxing.</span><span class="sxs-lookup"><span data-stu-id="ec12b-183">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="ec12b-184">Эта политика вступает в силу только тогда, когда защита DMA ядра поддерживается и включена программным обеспечением системы.</span><span class="sxs-lookup"><span data-stu-id="ec12b-184">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="ec12b-185">Защита DMA ядра — это функция платформы, которая не может управляться с помощью политики или конечным пользователем.</span><span class="sxs-lookup"><span data-stu-id="ec12b-185">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="ec12b-186">Она должна поддерживаться системой во время производства.</span><span class="sxs-lookup"><span data-stu-id="ec12b-186">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="ec12b-187">Чтобы проверить, поддерживает ли система защиту DMA ядра, ознакомьтесь с полем Защиты DMA ядра на странице Сводка MSINFO32.exe.</span><span class="sxs-lookup"><span data-stu-id="ec12b-187">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="ec12b-188">Возможные значения: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-188">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="ec12b-189">firewallRules</span><span class="sxs-lookup"><span data-stu-id="ec12b-189">firewallRules</span></span>|<span data-ttu-id="ec12b-190">[коллекция windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)</span><span class="sxs-lookup"><span data-stu-id="ec12b-190">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="ec12b-191">Настраивает параметры правил брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="ec12b-191">Configures the firewall rule settings.</span></span> <span data-ttu-id="ec12b-192">Эта коллекция может содержать не более 150 элементов.</span><span class="sxs-lookup"><span data-stu-id="ec12b-192">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="ec12b-193">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="ec12b-193">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="ec12b-194">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-194">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-195">Это право пользователя используется диспетчером учетных данных во время резервного копирования и восстановления.</span><span class="sxs-lookup"><span data-stu-id="ec12b-195">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="ec12b-196">Сохраненные учетные данные пользователей могут быть скомпрометированы, если эта привилегия будет предоставлена другим сущностям.</span><span class="sxs-lookup"><span data-stu-id="ec12b-196">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="ec12b-197">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="ec12b-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="ec12b-198">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="ec12b-198">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="ec12b-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-200">Это право пользователя определяет, какие пользователи и группы могут подключаться к компьютеру по сети.</span><span class="sxs-lookup"><span data-stu-id="ec12b-200">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="ec12b-201">Разрешено состояние поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec12b-201">State Allowed is supported.</span></span>|
|<span data-ttu-id="ec12b-202">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="ec12b-202">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="ec12b-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-204">Это право пользователя определяет, какие пользователи и группы блокируют подключение к компьютеру по сети.</span><span class="sxs-lookup"><span data-stu-id="ec12b-204">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="ec12b-205">Поддерживается государственный блок.</span><span class="sxs-lookup"><span data-stu-id="ec12b-205">State Block is supported.</span></span>|
|<span data-ttu-id="ec12b-206">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ec12b-206">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="ec12b-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-208">Это право пользователя позволяет процессу выдать себя любому пользователю без проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ec12b-208">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="ec12b-209">Таким образом, этот процесс может получить доступ к тем же локальным ресурсам, что и этот пользователь.</span><span class="sxs-lookup"><span data-stu-id="ec12b-209">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="ec12b-210">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="ec12b-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="ec12b-211">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="ec12b-211">userRightsLocalLogOn</span></span>|[<span data-ttu-id="ec12b-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-213">Это право пользователя определяет, какие пользователи могут войти на компьютер.</span><span class="sxs-lookup"><span data-stu-id="ec12b-213">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="ec12b-214">Состояния NotConfigured, Разрешенные поддерживаются</span><span class="sxs-lookup"><span data-stu-id="ec12b-214">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="ec12b-215">userRightsDenyLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="ec12b-215">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="ec12b-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-217">Это право пользователя определяет, какие пользователи не могут войти на компьютер.</span><span class="sxs-lookup"><span data-stu-id="ec12b-217">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="ec12b-218">Поддерживаются состояния NotConfigured, Blocked</span><span class="sxs-lookup"><span data-stu-id="ec12b-218">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="ec12b-219">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="ec12b-219">userRightsBackupData</span></span>|[<span data-ttu-id="ec12b-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-221">Это право пользователя определяет, какие пользователи могут обходить разрешения файлов, каталогов, реестров и других постоянных объектов при архивов и каталогах.</span><span class="sxs-lookup"><span data-stu-id="ec12b-221">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="ec12b-222">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="ec12b-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="ec12b-223">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="ec12b-223">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="ec12b-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-225">Это право пользователя определяет, какие пользователи и группы могут изменять время и дату на внутренних часах компьютера.</span><span class="sxs-lookup"><span data-stu-id="ec12b-225">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="ec12b-226">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="ec12b-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="ec12b-227">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="ec12b-227">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="ec12b-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-229">Этот параметр безопасности определяет, могут ли пользователи создавать глобальные объекты, доступные для всех сеансов.</span><span class="sxs-lookup"><span data-stu-id="ec12b-229">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="ec12b-230">Пользователи, которые могут создавать глобальные объекты, могут влиять на процессы, которые запускаются в сеансах других пользователей, что может привести к сбою приложения или повреждениям данных.</span><span class="sxs-lookup"><span data-stu-id="ec12b-230">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="ec12b-231">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="ec12b-231">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="ec12b-232">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="ec12b-232">userRightsCreatePageFile</span></span>|[<span data-ttu-id="ec12b-233">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-233">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-234">Это право пользователя определяет, какие пользователи и группы могут вызывать внутренний API для создания и изменения размера файла страницы.</span><span class="sxs-lookup"><span data-stu-id="ec12b-234">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="ec12b-235">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="ec12b-235">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="ec12b-236">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="ec12b-236">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="ec12b-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-238">Это право пользователя определяет, какие учетные записи можно использовать в процессах для создания объекта каталога с помощью объекта-диспетчера.</span><span class="sxs-lookup"><span data-stu-id="ec12b-238">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="ec12b-239">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="ec12b-239">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="ec12b-240">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="ec12b-240">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="ec12b-241">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-241">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-242">Это право пользователя определяет, может ли пользователь создать символическую ссылку с компьютера, на который он вошел.</span><span class="sxs-lookup"><span data-stu-id="ec12b-242">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="ec12b-243">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="ec12b-243">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="ec12b-244">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="ec12b-244">userRightsCreateToken</span></span>|[<span data-ttu-id="ec12b-245">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-245">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-246">Это право пользователя определяет, какие пользователи/группы могут использоваться процессами для создания маркера, который затем можно использовать для получения доступа к любым локальным ресурсам, когда процесс использует внутренний API для создания маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="ec12b-246">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="ec12b-247">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="ec12b-247">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="ec12b-248">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="ec12b-248">userRightsDebugPrograms</span></span>|[<span data-ttu-id="ec12b-249">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-249">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-250">Это право пользователя определяет, какие пользователи могут прикрепить отладка к любому процессу или к ядру.</span><span class="sxs-lookup"><span data-stu-id="ec12b-250">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="ec12b-251">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="ec12b-251">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="ec12b-252">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="ec12b-252">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="ec12b-253">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-253">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-254">Это право пользователя определяет, какие пользователи и группы не могут войти в систему в качестве клиента служб удаленного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="ec12b-254">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="ec12b-255">Поддерживаются только состояния NotConfigured и Blocked</span><span class="sxs-lookup"><span data-stu-id="ec12b-255">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="ec12b-256">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="ec12b-256">userRightsDelegation</span></span>|[<span data-ttu-id="ec12b-257">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-257">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-258">Это право пользователя определяет, какие пользователи могут установить параметр Доверенный для делегирования на объект пользователя или компьютера.</span><span class="sxs-lookup"><span data-stu-id="ec12b-258">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="ec12b-259">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="ec12b-259">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="ec12b-260">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="ec12b-260">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="ec12b-261">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-261">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-262">Это право пользователя определяет, какие учетные записи можно использовать для добавления записей в журнал безопасности.</span><span class="sxs-lookup"><span data-stu-id="ec12b-262">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="ec12b-263">Журнал безопасности используется для отслеживания несанкционированного доступа к системе.</span><span class="sxs-lookup"><span data-stu-id="ec12b-263">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="ec12b-264">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="ec12b-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="ec12b-265">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="ec12b-265">userRightsImpersonateClient</span></span>|[<span data-ttu-id="ec12b-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-267">Назначение этого права пользователю позволяет программам, работающим от имени этого пользователя, выдать себя за клиента.</span><span class="sxs-lookup"><span data-stu-id="ec12b-267">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="ec12b-268">Требование этого права пользователя для такого обезличения не позволяет неавторизованному пользователю убедить клиента подключиться к созданной им службе, а затем выдать себя за этого клиента, что может привести к повышению разрешений неавторизованного пользователя до административных или системных уровней.</span><span class="sxs-lookup"><span data-stu-id="ec12b-268">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="ec12b-269">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="ec12b-269">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="ec12b-270">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="ec12b-270">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="ec12b-271">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-271">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-272">Это право пользователя определяет, какие учетные записи могут использовать процесс с доступом write Property к другому процессу для увеличения приоритета выполнения, назначенного другому процессу.</span><span class="sxs-lookup"><span data-stu-id="ec12b-272">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="ec12b-273">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="ec12b-273">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="ec12b-274">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="ec12b-274">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="ec12b-275">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-275">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-276">Это право пользователя определяет, какие пользователи могут динамически загружать и разгружать драйверы устройств или другой код в режиме ядра.</span><span class="sxs-lookup"><span data-stu-id="ec12b-276">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="ec12b-277">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="ec12b-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="ec12b-278">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="ec12b-278">userRightsLockMemory</span></span>|[<span data-ttu-id="ec12b-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-280">Это право пользователя определяет, какие учетные записи могут использовать процесс для хранения данных в физической памяти, что не позволяет системе использовать данные в виртуальную память на диске.</span><span class="sxs-lookup"><span data-stu-id="ec12b-280">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="ec12b-281">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="ec12b-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="ec12b-282">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="ec12b-282">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="ec12b-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-284">Это право пользователя определяет, какие пользователи могут указывать параметры аудита доступа к объекту для отдельных ресурсов, таких как файлы, объекты Active Directory и ключи реестра.</span><span class="sxs-lookup"><span data-stu-id="ec12b-284">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="ec12b-285">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="ec12b-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="ec12b-286">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="ec12b-286">userRightsManageVolumes</span></span>|[<span data-ttu-id="ec12b-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-288">Это право пользователя определяет, какие пользователи и группы могут выполнять задачи технического обслуживания на томе, например удаленное дефрагментирование.</span><span class="sxs-lookup"><span data-stu-id="ec12b-288">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="ec12b-289">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="ec12b-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="ec12b-290">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="ec12b-290">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="ec12b-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-292">Это право пользователя определяет, кто может изменять значения среды прошивки.</span><span class="sxs-lookup"><span data-stu-id="ec12b-292">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="ec12b-293">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="ec12b-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="ec12b-294">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="ec12b-294">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="ec12b-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-296">Это право пользователя определяет, какие учетные записи пользователей могут изменять метку целостности объектов, таких как файлы, ключи реестра или процессы, которыми владеют другие пользователи.</span><span class="sxs-lookup"><span data-stu-id="ec12b-296">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="ec12b-297">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="ec12b-297">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="ec12b-298">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="ec12b-298">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="ec12b-299">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-299">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-300">Это право пользователя определяет, какие пользователи могут использовать средства мониторинга производительности для мониторинга производительности системных процессов.</span><span class="sxs-lookup"><span data-stu-id="ec12b-300">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="ec12b-301">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="ec12b-301">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="ec12b-302">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="ec12b-302">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="ec12b-303">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-303">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-304">Это право пользователя определяет, какие пользователи могут отключить компьютер из удаленного расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="ec12b-304">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="ec12b-305">Неправильное использование этого права пользователя может привести к отказу в обслуживании.</span><span class="sxs-lookup"><span data-stu-id="ec12b-305">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="ec12b-306">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="ec12b-306">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="ec12b-307">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="ec12b-307">userRightsRestoreData</span></span>|[<span data-ttu-id="ec12b-308">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-308">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-309">Это право пользователя определяет, какие пользователи могут обходить разрешения файлов, каталогов, реестров и других постоянных объектов при восстановлении архивных файлов и каталогов, а также определяет, какие пользователи могут установить любой допустимый принцип безопасности в качестве владельца объекта.</span><span class="sxs-lookup"><span data-stu-id="ec12b-309">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="ec12b-310">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="ec12b-310">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="ec12b-311">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="ec12b-311">userRightsTakeOwnership</span></span>|[<span data-ttu-id="ec12b-312">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="ec12b-312">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="ec12b-313">Это право пользователя определяет, какие пользователи могут взять на себя право собственности на любой защищаемый объект в системе, включая объекты Active Directory, файлы и папки, принтеры, ключи реестра, процессы и потоки.</span><span class="sxs-lookup"><span data-stu-id="ec12b-313">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="ec12b-314">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="ec12b-314">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="ec12b-315">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="ec12b-315">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="ec12b-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-316">Boolean</span></span>|<span data-ttu-id="ec12b-317">Этот параметр определяет, включено ли сохранение игры xbox (1) или отключено (0).</span><span class="sxs-lookup"><span data-stu-id="ec12b-317">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="ec12b-318">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="ec12b-318">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="ec12b-319">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="ec12b-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="ec12b-320">Этот параметр определяет, является ли тип запуска службы управления аксессуарами автоматическим (2), ручным (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="ec12b-320">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="ec12b-321">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="ec12b-321">Default: Manual.</span></span> <span data-ttu-id="ec12b-322">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="ec12b-323">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="ec12b-323">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="ec12b-324">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="ec12b-324">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="ec12b-325">Этот параметр определяет, является ли тип запуска службы Live Auth Manager автоматическим (2), ручным (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="ec12b-325">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="ec12b-326">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="ec12b-326">Default: Manual.</span></span> <span data-ttu-id="ec12b-327">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-327">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="ec12b-328">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="ec12b-328">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="ec12b-329">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="ec12b-329">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="ec12b-330">Этот параметр определяет, является ли тип запуска службы сохранения Live Game автоматическим (2), ручным (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="ec12b-330">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="ec12b-331">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="ec12b-331">Default: Manual.</span></span> <span data-ttu-id="ec12b-332">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-332">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="ec12b-333">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="ec12b-333">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="ec12b-334">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="ec12b-334">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="ec12b-335">Этот параметр определяет, является ли тип запуска сетевой службы автоматическим (2), ручным (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="ec12b-335">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="ec12b-336">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="ec12b-336">Default: Manual.</span></span> <span data-ttu-id="ec12b-337">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-337">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="ec12b-338">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="ec12b-338">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="ec12b-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-339">Boolean</span></span>|<span data-ttu-id="ec12b-340">Запретить пользователям добавлять на этот компьютер новые учетные записи Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ec12b-340">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="ec12b-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="ec12b-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="ec12b-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-342">Boolean</span></span>|<span data-ttu-id="ec12b-343">Включить локальные учетные записи, которые не защищены паролем, для входа из других местоположений, кроме физического устройства. Включено значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="ec12b-343">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="ec12b-344">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="ec12b-344">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="ec12b-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-345">Boolean</span></span>|<span data-ttu-id="ec12b-346">Определяет, включена или отключена учетная запись локального администратора.</span><span class="sxs-lookup"><span data-stu-id="ec12b-346">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="ec12b-347">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="ec12b-347">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="ec12b-348">Строка</span><span class="sxs-lookup"><span data-stu-id="ec12b-348">String</span></span>|<span data-ttu-id="ec12b-349">Определите другое имя учетной записи, связанное с идентификатором безопасности (SID) для учетной записи "Администратор".</span><span class="sxs-lookup"><span data-stu-id="ec12b-349">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="ec12b-350">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="ec12b-350">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="ec12b-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-351">Boolean</span></span>|<span data-ttu-id="ec12b-352">Определяет, включена или отключена учетная запись гостевой.</span><span class="sxs-lookup"><span data-stu-id="ec12b-352">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="ec12b-353">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="ec12b-353">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="ec12b-354">Строка</span><span class="sxs-lookup"><span data-stu-id="ec12b-354">String</span></span>|<span data-ttu-id="ec12b-355">Определите другое имя учетной записи, связанное с идентификатором безопасности (SID) для учетной записи "Гость".</span><span class="sxs-lookup"><span data-stu-id="ec12b-355">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="ec12b-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="ec12b-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="ec12b-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-357">Boolean</span></span>|<span data-ttu-id="ec12b-358">Запретить отсоединовку портативного компьютера без входа.</span><span class="sxs-lookup"><span data-stu-id="ec12b-358">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="ec12b-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="ec12b-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="ec12b-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-360">Boolean</span></span>|<span data-ttu-id="ec12b-361">Ограничить установку драйверов принтера в рамках подключения к общему принтеру только администраторам.</span><span class="sxs-lookup"><span data-stu-id="ec12b-361">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="ec12b-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="ec12b-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="ec12b-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-363">Boolean</span></span>|<span data-ttu-id="ec12b-364">Включение этого параметра позволяет только в интерактивном режиме войти в систему пользователю, чтобы получить доступ к CD-ROM-носителю.</span><span class="sxs-lookup"><span data-stu-id="ec12b-364">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="ec12b-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="ec12b-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="ec12b-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="ec12b-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="ec12b-367">Определите, кому разрешено форматирование и удаление съемных носители NTFS.</span><span class="sxs-lookup"><span data-stu-id="ec12b-367">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="ec12b-368">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-368">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="ec12b-369">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="ec12b-369">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="ec12b-370">Int32</span><span class="sxs-lookup"><span data-stu-id="ec12b-370">Int32</span></span>|<span data-ttu-id="ec12b-371">Определите максимальные минуты бездействия на экране входа на интерактивном рабочем столе до тех пор, пока не будет работать замотивник экрана.</span><span class="sxs-lookup"><span data-stu-id="ec12b-371">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="ec12b-372">Допустимые значения от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="ec12b-372">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="ec12b-373">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="ec12b-373">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="ec12b-374">Int32</span><span class="sxs-lookup"><span data-stu-id="ec12b-374">Int32</span></span>|<span data-ttu-id="ec12b-375">Определите максимальные минуты бездействия на экране входа на интерактивном рабочем столе до тех пор, пока не будет работать замотивник экрана.</span><span class="sxs-lookup"><span data-stu-id="ec12b-375">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="ec12b-376">Допустимые значения от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="ec12b-376">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="ec12b-377">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="ec12b-377">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="ec12b-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-378">Boolean</span></span>|<span data-ttu-id="ec12b-379">Перед входом в систему необходимо нажать на CTRL+ALT+DEL.</span><span class="sxs-lookup"><span data-stu-id="ec12b-379">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="ec12b-380">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="ec12b-380">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="ec12b-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-381">Boolean</span></span>|<span data-ttu-id="ec12b-382">Не отображать имя пользователя последнего человека, который вписался на этом устройстве.</span><span class="sxs-lookup"><span data-stu-id="ec12b-382">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="ec12b-383">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="ec12b-383">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="ec12b-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-384">Boolean</span></span>|<span data-ttu-id="ec12b-385">Не отображать имя пользователя пользователя, вписавшись на это устройство после входа учетных данных и до отображения рабочего стола устройства.</span><span class="sxs-lookup"><span data-stu-id="ec12b-385">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="ec12b-386">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="ec12b-386">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="ec12b-387">Строка</span><span class="sxs-lookup"><span data-stu-id="ec12b-387">String</span></span>|<span data-ttu-id="ec12b-388">Установите название сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="ec12b-388">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="ec12b-389">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="ec12b-389">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="ec12b-390">Строка</span><span class="sxs-lookup"><span data-stu-id="ec12b-390">String</span></span>|<span data-ttu-id="ec12b-391">Установите текст сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="ec12b-391">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="ec12b-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="ec12b-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="ec12b-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-393">Boolean</span></span>|<span data-ttu-id="ec12b-394">Блокировать запросы на проверку подлинности PKU2U на этом устройстве для использования удостоверений в Интернете.</span><span class="sxs-lookup"><span data-stu-id="ec12b-394">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="ec12b-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="ec12b-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="ec12b-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-396">Boolean</span></span>|<span data-ttu-id="ec12b-397">Помощник пользовательского интерфейса для подразделения LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="ec12b-397">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="ec12b-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="ec12b-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="ec12b-399">Строка</span><span class="sxs-lookup"><span data-stu-id="ec12b-399">String</span></span>|<span data-ttu-id="ec12b-400">Изменить строку определения определения дескриптора безопасности по умолчанию, чтобы разрешить пользователям и группам делать удаленные вызовы в SAM.</span><span class="sxs-lookup"><span data-stu-id="ec12b-400">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="ec12b-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="ec12b-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="ec12b-402">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="ec12b-402">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="ec12b-403">Этот параметр безопасности позволяет клиенту требовать согласования 128-битного шифрования и/или безопасности сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="ec12b-403">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="ec12b-404">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-404">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="ec12b-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="ec12b-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="ec12b-406">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="ec12b-406">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="ec12b-407">Этот параметр безопасности позволяет серверу требовать согласования 128-битного шифрования и/или безопасности сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="ec12b-407">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="ec12b-408">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-408">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="ec12b-409">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="ec12b-409">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="ec12b-410">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="ec12b-410">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="ec12b-411">Этот параметр безопасности определяет, какой протокол проверки подлинности вызовов и ответов используется для сетевых логотипов.</span><span class="sxs-lookup"><span data-stu-id="ec12b-411">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="ec12b-412">Возможные значения: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-412">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="ec12b-413">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="ec12b-413">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="ec12b-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-414">Boolean</span></span>|<span data-ttu-id="ec12b-415">Если включено, клиент SMB позволит использовать небезопасные гостевых логотипы.</span><span class="sxs-lookup"><span data-stu-id="ec12b-415">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="ec12b-416">Если он не настроен, клиент SMB отклоняет небезопасные гостевых логотипы.</span><span class="sxs-lookup"><span data-stu-id="ec12b-416">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="ec12b-417">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="ec12b-417">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="ec12b-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-418">Boolean</span></span>|<span data-ttu-id="ec12b-419">Этот параметр безопасности определяет, очищается ли виртуальная страница памяти при отключении системы.</span><span class="sxs-lookup"><span data-stu-id="ec12b-419">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="ec12b-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="ec12b-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="ec12b-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-421">Boolean</span></span>|<span data-ttu-id="ec12b-422">Этот параметр безопасности определяет, можно ли отключить компьютер без входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="ec12b-422">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="ec12b-423">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="ec12b-423">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="ec12b-424">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-424">Boolean</span></span>|<span data-ttu-id="ec12b-425">Разрешить приложениям UIAccess подсказок для повышения без использования безопасного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="ec12b-425">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="ec12b-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="ec12b-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="ec12b-427">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-427">Boolean</span></span>|<span data-ttu-id="ec12b-428">Виртуализация сбоев записи файлов и реестра для каждого пользователя</span><span class="sxs-lookup"><span data-stu-id="ec12b-428">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="ec12b-429">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="ec12b-429">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="ec12b-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-430">Boolean</span></span>|<span data-ttu-id="ec12b-431">Принудительное выполнение проверки пути сертификации PKI для заданного исполняемого файла до разрешения на запуск.</span><span class="sxs-lookup"><span data-stu-id="ec12b-431">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="ec12b-432">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="ec12b-432">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="ec12b-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="ec12b-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="ec12b-434">Определите поведение запроса на повышение для администраторов в режиме утверждения администратора.</span><span class="sxs-lookup"><span data-stu-id="ec12b-434">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="ec12b-435">Возможные значения: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-435">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="ec12b-436">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="ec12b-436">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="ec12b-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="ec12b-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="ec12b-438">Определите поведение запроса высоты для стандартных пользователей.</span><span class="sxs-lookup"><span data-stu-id="ec12b-438">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="ec12b-439">Возможные значения: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-439">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="ec12b-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="ec12b-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="ec12b-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-441">Boolean</span></span>|<span data-ttu-id="ec12b-442">Включить все запросы на повышение, чтобы перейти на рабочий стол интерактивного пользователя, а не на безопасный рабочий стол.</span><span class="sxs-lookup"><span data-stu-id="ec12b-442">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="ec12b-443">Используются оперативные параметры политики поведения для администраторов и стандартных пользователей.</span><span class="sxs-lookup"><span data-stu-id="ec12b-443">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="ec12b-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="ec12b-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="ec12b-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-445">Boolean</span></span>|<span data-ttu-id="ec12b-446">Установки приложений, требующие повышенных привилегий, будут подсказок для учетных данных администратора. Включено значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="ec12b-446">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="ec12b-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="ec12b-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="ec12b-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-448">Boolean</span></span>|<span data-ttu-id="ec12b-449">Разрешить приложениям UIAccess подсказок для повышения без использования безопасного рабочего стола. Включено значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="ec12b-449">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="ec12b-450">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="ec12b-450">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="ec12b-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-451">Boolean</span></span>|<span data-ttu-id="ec12b-452">Определяет, использует ли встроенная учетная запись администратора режим утверждения администратора или запускает все приложения с полными привилегиями администратора. Включено значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="ec12b-452">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="ec12b-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="ec12b-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="ec12b-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-454">Boolean</span></span>|<span data-ttu-id="ec12b-455">Определите, включен ли режим утверждения администрирования и все параметры политики UAC по умолчанию</span><span class="sxs-lookup"><span data-stu-id="ec12b-455">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="ec12b-456">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="ec12b-456">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="ec12b-457">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="ec12b-457">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="ec12b-458">Настройка пользовательских сведений, отображаемых при блокировке сеанса.</span><span class="sxs-lookup"><span data-stu-id="ec12b-458">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="ec12b-459">Если они не настроены, отображается имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="ec12b-459">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="ec12b-460">Возможные значения: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-460">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="ec12b-461">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="ec12b-461">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="ec12b-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="ec12b-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="ec12b-463">Настройка пользовательских сведений, отображаемых при блокировке сеанса.</span><span class="sxs-lookup"><span data-stu-id="ec12b-463">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="ec12b-464">Если они не настроены, отображается имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="ec12b-464">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="ec12b-465">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-465">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="ec12b-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="ec12b-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="ec12b-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-467">Boolean</span></span>|<span data-ttu-id="ec12b-468">Этот параметр безопасности определяет, пытается ли клиент SMB договориться о подписании пакета SMB.</span><span class="sxs-lookup"><span data-stu-id="ec12b-468">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="ec12b-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="ec12b-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="ec12b-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-470">Boolean</span></span>|<span data-ttu-id="ec12b-471">Этот параметр безопасности определяет, требуется ли подписывать пакет клиентского компонента SMB.</span><span class="sxs-lookup"><span data-stu-id="ec12b-471">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="ec12b-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="ec12b-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="ec12b-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-473">Boolean</span></span>|<span data-ttu-id="ec12b-474">Если этот параметр безопасности включен, перенаправлению Блока сообщений сервера (SMB) разрешается отправлять простые пароли на серверы SMB, не включаемые в Microsoft, которые не поддерживают шифрование паролей во время проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ec12b-474">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="ec12b-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="ec12b-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="ec12b-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-476">Boolean</span></span>|<span data-ttu-id="ec12b-477">Этот параметр безопасности определяет, требуется ли подписание пакета компонентом сервера SMB.</span><span class="sxs-lookup"><span data-stu-id="ec12b-477">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="ec12b-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="ec12b-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="ec12b-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-479">Boolean</span></span>|<span data-ttu-id="ec12b-480">Этот параметр безопасности определяет, будет ли SMB-сервер согласовывать подписание пакетов SMB с клиентами, которые его запрашивают.</span><span class="sxs-lookup"><span data-stu-id="ec12b-480">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="ec12b-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="ec12b-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="ec12b-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-482">Boolean</span></span>|<span data-ttu-id="ec12b-483">По умолчанию этот параметр безопасности ограничивает анонимный доступ к акциям и трубам к настройкам именных труб, к которые можно получить анонимный доступ, а также к акциям, к которые можно получить анонимный доступ.</span><span class="sxs-lookup"><span data-stu-id="ec12b-483">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="ec12b-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="ec12b-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="ec12b-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-485">Boolean</span></span>|<span data-ttu-id="ec12b-486">Этот параметр безопасности определяет, какие дополнительные разрешения будут предоставлены для анонимных подключений к компьютеру.</span><span class="sxs-lookup"><span data-stu-id="ec12b-486">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="ec12b-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="ec12b-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="ec12b-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-488">Boolean</span></span>|<span data-ttu-id="ec12b-489">Этот параметр безопасности определяет, разрешает ли анонимным пользователям выполнять определенные действия, такие как список имен учетных записей домена и сетевых акций.</span><span class="sxs-lookup"><span data-stu-id="ec12b-489">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="ec12b-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="ec12b-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="ec12b-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-491">Boolean</span></span>|<span data-ttu-id="ec12b-492">Этот параметр безопасности определяет, сохраняется ли при следующем изменении пароля значение hash-значения lan Manager (LM) для нового пароля.</span><span class="sxs-lookup"><span data-stu-id="ec12b-492">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="ec12b-493">Он не хранится по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec12b-493">It’s not stored by default.</span></span>|
|<span data-ttu-id="ec12b-494">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="ec12b-494">localSecurityOptionsSmartCardRemovalBehavior</span></span>|<span data-ttu-id="ec12b-495">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md);</span><span class="sxs-lookup"><span data-stu-id="ec12b-495">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)</span></span>|<span data-ttu-id="ec12b-496">Этот параметр безопасности определяет, что происходит, когда смарт-карта для зарегистрированного пользователя удаляется из чтения смарт-карт.</span><span class="sxs-lookup"><span data-stu-id="ec12b-496">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="ec12b-497">Возможные значения: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-497">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="ec12b-498">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="ec12b-498">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="ec12b-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-499">Boolean</span></span>|<span data-ttu-id="ec12b-500">Используется для отключения отображения области защиты приложения и браузера.</span><span class="sxs-lookup"><span data-stu-id="ec12b-500">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="ec12b-501">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="ec12b-501">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="ec12b-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-502">Boolean</span></span>|<span data-ttu-id="ec12b-503">Используется для отключения отображения области семейных параметров.</span><span class="sxs-lookup"><span data-stu-id="ec12b-503">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="ec12b-504">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="ec12b-504">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="ec12b-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-505">Boolean</span></span>|<span data-ttu-id="ec12b-506">Используется для отключения отображения производительности устройства и области работоспособности.</span><span class="sxs-lookup"><span data-stu-id="ec12b-506">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="ec12b-507">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="ec12b-507">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="ec12b-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-508">Boolean</span></span>|<span data-ttu-id="ec12b-509">Используется для отключения отображения брандмауэра и области защиты сети.</span><span class="sxs-lookup"><span data-stu-id="ec12b-509">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="ec12b-510">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="ec12b-510">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="ec12b-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-511">Boolean</span></span>|<span data-ttu-id="ec12b-512">Используется для отключения отображения области защиты от вирусов и угроз.</span><span class="sxs-lookup"><span data-stu-id="ec12b-512">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="ec12b-513">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="ec12b-513">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="ec12b-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-514">Boolean</span></span>|<span data-ttu-id="ec12b-515">Используется для отключения отображения области защиты учетной записи.</span><span class="sxs-lookup"><span data-stu-id="ec12b-515">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="ec12b-516">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="ec12b-516">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="ec12b-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-517">Boolean</span></span>|<span data-ttu-id="ec12b-518">Используется для отключения отображения кнопки Clear TPM.</span><span class="sxs-lookup"><span data-stu-id="ec12b-518">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="ec12b-519">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="ec12b-519">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="ec12b-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-520">Boolean</span></span>|<span data-ttu-id="ec12b-521">Используется для отключения отображения области защиты оборудования.</span><span class="sxs-lookup"><span data-stu-id="ec12b-521">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="ec12b-522">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="ec12b-522">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="ec12b-523">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-523">Boolean</span></span>|<span data-ttu-id="ec12b-524">Используется для отключения отображения управления областью уведомлений.</span><span class="sxs-lookup"><span data-stu-id="ec12b-524">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="ec12b-525">Чтобы этот параметр вступил в силу, пользователю необходимо либо выйти, либо войти, либо перезагрустить компьютер.</span><span class="sxs-lookup"><span data-stu-id="ec12b-525">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="ec12b-526">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="ec12b-526">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="ec12b-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-527">Boolean</span></span>|<span data-ttu-id="ec12b-528">Используется для отключения отображения области защиты вымогателей.</span><span class="sxs-lookup"><span data-stu-id="ec12b-528">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="ec12b-529">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="ec12b-529">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="ec12b-530">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-530">Boolean</span></span>|<span data-ttu-id="ec12b-531">Используется для отключения отображения безопасной области загрузки под безопасностью устройства.</span><span class="sxs-lookup"><span data-stu-id="ec12b-531">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="ec12b-532">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="ec12b-532">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="ec12b-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-533">Boolean</span></span>|<span data-ttu-id="ec12b-534">Используется для отключения отображения устранения неполадок процесса безопасности в области безопасности устройства.</span><span class="sxs-lookup"><span data-stu-id="ec12b-534">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="ec12b-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="ec12b-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="ec12b-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-536">Boolean</span></span>|<span data-ttu-id="ec12b-537">Используется для отключения отображения обновления прошивки TPM при обнаружении уязвимого прошивки.</span><span class="sxs-lookup"><span data-stu-id="ec12b-537">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="ec12b-538">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="ec12b-538">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="ec12b-539">Строка</span><span class="sxs-lookup"><span data-stu-id="ec12b-539">String</span></span>|<span data-ttu-id="ec12b-540">Имя компании, отображаемая пользователям.</span><span class="sxs-lookup"><span data-stu-id="ec12b-540">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="ec12b-541">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="ec12b-541">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="ec12b-542">Строка</span><span class="sxs-lookup"><span data-stu-id="ec12b-542">String</span></span>|<span data-ttu-id="ec12b-543">Адрес электронной почты, отображаемой пользователям.</span><span class="sxs-lookup"><span data-stu-id="ec12b-543">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="ec12b-544">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="ec12b-544">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="ec12b-545">Строка</span><span class="sxs-lookup"><span data-stu-id="ec12b-545">String</span></span>|<span data-ttu-id="ec12b-546">Номер телефона или Skype ID, отображаемый пользователям.</span><span class="sxs-lookup"><span data-stu-id="ec12b-546">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="ec12b-547">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="ec12b-547">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="ec12b-548">Строка</span><span class="sxs-lookup"><span data-stu-id="ec12b-548">String</span></span>|<span data-ttu-id="ec12b-549">URL-адрес портала справки, отображаемый пользователями.</span><span class="sxs-lookup"><span data-stu-id="ec12b-549">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="ec12b-550">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="ec12b-550">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="ec12b-551">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="ec12b-551">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="ec12b-552">Уведомления, отображаемые из отображаемой области приложения.</span><span class="sxs-lookup"><span data-stu-id="ec12b-552">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="ec12b-553">Возможные значения: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-553">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="ec12b-554">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="ec12b-554">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="ec12b-555">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="ec12b-555">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="ec12b-556">Настройка отображения контактных данных ИТ для конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="ec12b-556">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="ec12b-557">Возможные значения: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-557">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="ec12b-558">windowsDefenderTamperProtection</span><span class="sxs-lookup"><span data-stu-id="ec12b-558">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="ec12b-559">windowsDefenderTamperProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="ec12b-559">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="ec12b-560">Настройка параметров защитника Windows TamperProtection.</span><span class="sxs-lookup"><span data-stu-id="ec12b-560">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="ec12b-561">Возможные значения: `notConfigured`, `enable`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-561">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="ec12b-562">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="ec12b-562">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="ec12b-563">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-563">Boolean</span></span>|<span data-ttu-id="ec12b-564">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="ec12b-564">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="ec12b-565">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="ec12b-565">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="ec12b-566">Int32</span><span class="sxs-lookup"><span data-stu-id="ec12b-566">Int32</span></span>|<span data-ttu-id="ec12b-567">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="ec12b-567">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="ec12b-568">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="ec12b-568">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="ec12b-569">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="ec12b-569">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="ec12b-570">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="ec12b-570">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="ec12b-571">брандмауэрPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="ec12b-571">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="ec12b-572">Выберите кодику предварительного ключа, которая будет использоваться.</span><span class="sxs-lookup"><span data-stu-id="ec12b-572">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="ec12b-573">Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-573">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="ec12b-574">firewallIPSecExemptionsNone</span><span class="sxs-lookup"><span data-stu-id="ec12b-574">firewallIPSecExemptionsNone</span></span>|<span data-ttu-id="ec12b-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-575">Boolean</span></span>|<span data-ttu-id="ec12b-576">Настройка исключений IPSec без исключений</span><span class="sxs-lookup"><span data-stu-id="ec12b-576">Configures IPSec exemptions to no exemptions</span></span>|
|<span data-ttu-id="ec12b-577">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="ec12b-577">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="ec12b-578">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-578">Boolean</span></span>|<span data-ttu-id="ec12b-579">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="ec12b-579">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="ec12b-580">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="ec12b-580">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="ec12b-581">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-581">Boolean</span></span>|<span data-ttu-id="ec12b-582">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="ec12b-582">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="ec12b-583">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="ec12b-583">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="ec12b-584">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-584">Boolean</span></span>|<span data-ttu-id="ec12b-585">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="ec12b-585">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="ec12b-586">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="ec12b-586">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="ec12b-587">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-587">Boolean</span></span>|<span data-ttu-id="ec12b-588">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="ec12b-588">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="ec12b-589">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="ec12b-589">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="ec12b-590">брандмауэрCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="ec12b-590">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="ec12b-591">Укажите, как будет применяться список отзывов сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ec12b-591">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="ec12b-592">Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-592">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="ec12b-593">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="ec12b-593">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="ec12b-594">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-594">Boolean</span></span>|<span data-ttu-id="ec12b-595">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="ec12b-595">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="ec12b-596">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="ec12b-596">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="ec12b-597">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="ec12b-597">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="ec12b-598">Настраивает, как следует применять очереди пакетов в сценарии шлюза туннеля.</span><span class="sxs-lookup"><span data-stu-id="ec12b-598">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="ec12b-599">Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-599">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="ec12b-600">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="ec12b-600">firewallProfileDomain</span></span>|[<span data-ttu-id="ec12b-601">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="ec12b-601">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="ec12b-602">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="ec12b-602">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="ec12b-603">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="ec12b-603">firewallProfilePublic</span></span>|[<span data-ttu-id="ec12b-604">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="ec12b-604">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="ec12b-605">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="ec12b-605">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="ec12b-606">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="ec12b-606">firewallProfilePrivate</span></span>|[<span data-ttu-id="ec12b-607">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="ec12b-607">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="ec12b-608">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="ec12b-608">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="ec12b-609">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="ec12b-609">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="ec12b-610">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-610">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="ec12b-611">Значение, указывающее поведение Adobe Reader при создании детских процессов.</span><span class="sxs-lookup"><span data-stu-id="ec12b-611">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="ec12b-612">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-612">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="ec12b-613">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="ec12b-613">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="ec12b-614">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ec12b-614">String collection</span></span>|<span data-ttu-id="ec12b-615">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="ec12b-615">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="ec12b-616">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-616">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="ec12b-617">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="ec12b-617">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="ec12b-618">Значение, указывающее поведение приложений Office, впрыскивающихся в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="ec12b-618">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="ec12b-619">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-619">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="ec12b-620">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="ec12b-620">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="ec12b-621">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-621">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="ec12b-622">Значение, указывающее поведение приложений Office, впрыскивающихся в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="ec12b-622">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="ec12b-623">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-623">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="ec12b-624">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="ec12b-624">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="ec12b-625">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-625">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="ec12b-626">Значение, указывающее поведение приложений связи Office, в том числе Microsoft Outlook, от создания детских процессов.</span><span class="sxs-lookup"><span data-stu-id="ec12b-626">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="ec12b-627">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-627">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="ec12b-628">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="ec12b-628">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="ec12b-629">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="ec12b-629">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="ec12b-630">Значение, указывающее поведение приложений Office/макрос, создаваемых или запускаемых исполняемого контента.</span><span class="sxs-lookup"><span data-stu-id="ec12b-630">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="ec12b-631">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-631">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="ec12b-632">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="ec12b-632">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="ec12b-633">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-633">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="ec12b-634">Значение, указывающее поведение приложений Office/макрос, создаваемых или запускаемых исполняемого контента.</span><span class="sxs-lookup"><span data-stu-id="ec12b-634">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="ec12b-635">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-635">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="ec12b-636">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="ec12b-636">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="ec12b-637">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="ec12b-637">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="ec12b-638">Значение, указывающее поведение приложения Office, запускающее детские процессы.</span><span class="sxs-lookup"><span data-stu-id="ec12b-638">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="ec12b-639">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-639">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="ec12b-640">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="ec12b-640">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="ec12b-641">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-641">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="ec12b-642">Значение, указывающее поведение приложения Office, запускающее детские процессы.</span><span class="sxs-lookup"><span data-stu-id="ec12b-642">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="ec12b-643">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-643">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="ec12b-644">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="ec12b-644">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="ec12b-645">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="ec12b-645">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="ec12b-646">Значение, указывающее поведение импорта Win32 из кода Макроса в Office.</span><span class="sxs-lookup"><span data-stu-id="ec12b-646">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="ec12b-647">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-647">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="ec12b-648">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="ec12b-648">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="ec12b-649">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-649">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="ec12b-650">Значение, указывающее поведение импорта Win32 из кода Макроса в Office.</span><span class="sxs-lookup"><span data-stu-id="ec12b-650">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="ec12b-651">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-651">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="ec12b-652">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="ec12b-652">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="ec12b-653">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="ec12b-653">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="ec12b-654">Значение, указывающее поведение запутываемого кода js/vbs/ps/macro.</span><span class="sxs-lookup"><span data-stu-id="ec12b-654">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="ec12b-655">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-655">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="ec12b-656">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="ec12b-656">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="ec12b-657">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-657">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="ec12b-658">Значение, указывающее поведение запутываемого кода js/vbs/ps/macro.</span><span class="sxs-lookup"><span data-stu-id="ec12b-658">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="ec12b-659">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-659">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="ec12b-660">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-660">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="ec12b-661">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="ec12b-661">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="ec12b-662">Значение, указывающее поведение js/vbs для выполнения полезной нагрузки, скачанных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="ec12b-662">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="ec12b-663">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-663">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="ec12b-664">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="ec12b-664">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="ec12b-665">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-665">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="ec12b-666">Значение, указывающее поведение js/vbs для выполнения полезной нагрузки, скачанных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="ec12b-666">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="ec12b-667">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-667">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="ec12b-668">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="ec12b-668">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="ec12b-669">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-669">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="ec12b-670">Значение, указывающее, разрешен ли кража учетных данных из подсистемы локального органа безопасности Windows.</span><span class="sxs-lookup"><span data-stu-id="ec12b-670">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="ec12b-671">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-671">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="ec12b-672">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="ec12b-672">defenderProcessCreationType</span></span>|[<span data-ttu-id="ec12b-673">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="ec12b-673">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="ec12b-674">Значение, указывающее отклик на создание процессов, происходящих из команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="ec12b-674">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="ec12b-675">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-675">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="ec12b-676">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="ec12b-676">defenderProcessCreation</span></span>|[<span data-ttu-id="ec12b-677">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-677">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="ec12b-678">Значение, указывающее отклик на создание процессов, происходящих из команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="ec12b-678">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="ec12b-679">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-679">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="ec12b-680">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="ec12b-680">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="ec12b-681">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="ec12b-681">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="ec12b-682">Значение, указывающее ответ на ненарушимые и неподписаные процессы, которые запускают из USB.</span><span class="sxs-lookup"><span data-stu-id="ec12b-682">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="ec12b-683">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-683">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="ec12b-684">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="ec12b-684">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="ec12b-685">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-685">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="ec12b-686">Значение, указывающее ответ на ненарушимые и неподписаные процессы, которые запускают из USB.</span><span class="sxs-lookup"><span data-stu-id="ec12b-686">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="ec12b-687">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-687">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="ec12b-688">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="ec12b-688">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="ec12b-689">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="ec12b-689">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="ec12b-690">Значение, указывающее ответ на исполняемые, которые не соответствуют критериям распространенности, возраста или доверенного списка.</span><span class="sxs-lookup"><span data-stu-id="ec12b-690">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="ec12b-691">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-691">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="ec12b-692">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="ec12b-692">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="ec12b-693">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-693">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="ec12b-694">Значение, указывающее ответ на исполняемые, которые не соответствуют критериям распространенности, возраста или доверенного списка.</span><span class="sxs-lookup"><span data-stu-id="ec12b-694">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="ec12b-695">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-695">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="ec12b-696">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-696">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="ec12b-697">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="ec12b-697">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="ec12b-698">Значение, указывающее, что выполнение исполняемого контента (exe, dll, ps, js, vbs и т.д.) должно быть отброшено из электронной почты (веб-почта/почтовый клиент).</span><span class="sxs-lookup"><span data-stu-id="ec12b-698">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="ec12b-699">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-699">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="ec12b-700">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="ec12b-700">defenderEmailContentExecution</span></span>|[<span data-ttu-id="ec12b-701">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-701">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="ec12b-702">Значение, указывающее, что выполнение исполняемого контента (exe, dll, ps, js, vbs и т.д.) должно быть отброшено из электронной почты (веб-почта/почтовый клиент).</span><span class="sxs-lookup"><span data-stu-id="ec12b-702">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="ec12b-703">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-703">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="ec12b-704">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-704">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="ec12b-705">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-705">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="ec12b-706">Значение, указывающее использование передовой защиты от программ-вымогателей.</span><span class="sxs-lookup"><span data-stu-id="ec12b-706">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="ec12b-707">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-707">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="ec12b-708">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="ec12b-708">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="ec12b-709">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-709">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="ec12b-710">Значение, указывающее поведение защищенных папок.</span><span class="sxs-lookup"><span data-stu-id="ec12b-710">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="ec12b-711">Возможные значения: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-711">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="ec12b-712">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="ec12b-712">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="ec12b-713">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ec12b-713">String collection</span></span>|<span data-ttu-id="ec12b-714">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="ec12b-714">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="ec12b-715">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="ec12b-715">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="ec12b-716">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ec12b-716">String collection</span></span>|<span data-ttu-id="ec12b-717">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="ec12b-717">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="ec12b-718">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-718">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="ec12b-719">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-719">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="ec12b-720">Значение, указывающее поведение NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="ec12b-720">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="ec12b-721">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-721">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="ec12b-722">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="ec12b-722">defenderExploitProtectionXml</span></span>|<span data-ttu-id="ec12b-723">Binary</span><span class="sxs-lookup"><span data-stu-id="ec12b-723">Binary</span></span>|<span data-ttu-id="ec12b-724">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="ec12b-724">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="ec12b-725">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="ec12b-725">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="ec12b-726">String</span><span class="sxs-lookup"><span data-stu-id="ec12b-726">String</span></span>|<span data-ttu-id="ec12b-727">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="ec12b-727">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="ec12b-728">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="ec12b-728">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="ec12b-729">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-729">Boolean</span></span>|<span data-ttu-id="ec12b-730">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="ec12b-730">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="ec12b-731">defenderBlockPersistenceThroughWmiType</span><span class="sxs-lookup"><span data-stu-id="ec12b-731">defenderBlockPersistenceThroughWmiType</span></span>|[<span data-ttu-id="ec12b-732">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="ec12b-732">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="ec12b-733">Значение, указывающее поведение сохраняемого блока с помощью подписки на события WMI.</span><span class="sxs-lookup"><span data-stu-id="ec12b-733">Value indicating the behavior of Block persistence through WMI event subscription.</span></span> <span data-ttu-id="ec12b-734">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-734">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="ec12b-735">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="ec12b-735">appLockerApplicationControl</span></span>|[<span data-ttu-id="ec12b-736">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="ec12b-736">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="ec12b-737">Позволяет администратору выбирать разрешенные типы приложений для устройств.</span><span class="sxs-lookup"><span data-stu-id="ec12b-737">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="ec12b-738">Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-738">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="ec12b-739">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="ec12b-739">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="ec12b-740">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="ec12b-740">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="ec12b-741">Включай учетную защиту, когда включен уровень безопасности платформы с безопасностью безопасной загрузки и безопасностью на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="ec12b-741">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="ec12b-742">Возможные значения: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-742">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`, `disable`.</span></span>|
|<span data-ttu-id="ec12b-743">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="ec12b-743">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="ec12b-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-744">Boolean</span></span>|<span data-ttu-id="ec12b-745">Включает безопасность на основе виртуализации (VBS).</span><span class="sxs-lookup"><span data-stu-id="ec12b-745">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="ec12b-746">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="ec12b-746">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="ec12b-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-747">Boolean</span></span>|<span data-ttu-id="ec12b-748">Это свойство будет обесценилось в мае 2019 г. и будет заменено свойством DeviceGuardSecureBootWithDMA.</span><span class="sxs-lookup"><span data-stu-id="ec12b-748">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="ec12b-749">Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="ec12b-749">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="ec12b-750">deviceGuardSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="ec12b-750">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="ec12b-751">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="ec12b-751">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="ec12b-752">Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="ec12b-752">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="ec12b-753">Возможные значения: `notConfigured`, `withoutDMA`, `withDMA`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-753">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="ec12b-754">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="ec12b-754">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="ec12b-755">включить</span><span class="sxs-lookup"><span data-stu-id="ec12b-755">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ec12b-756">Позволяет ИТ-администратору настроить запуск System Guard.</span><span class="sxs-lookup"><span data-stu-id="ec12b-756">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="ec12b-757">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-757">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ec12b-758">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="ec12b-758">smartScreenEnableInShell</span></span>|<span data-ttu-id="ec12b-759">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-759">Boolean</span></span>|<span data-ttu-id="ec12b-760">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="ec12b-760">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="ec12b-761">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="ec12b-761">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="ec12b-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-762">Boolean</span></span>|<span data-ttu-id="ec12b-763">Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="ec12b-763">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="ec12b-764">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="ec12b-764">applicationGuardEnabled</span></span>|<span data-ttu-id="ec12b-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-765">Boolean</span></span>|<span data-ttu-id="ec12b-766">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="ec12b-766">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="ec12b-767">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="ec12b-767">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="ec12b-768">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="ec12b-768">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="ec12b-769">Включить Защитник Windows для более новых сборки Windows.</span><span class="sxs-lookup"><span data-stu-id="ec12b-769">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="ec12b-770">Возможные значения: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-770">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="ec12b-771">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="ec12b-771">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="ec12b-772">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="ec12b-772">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="ec12b-773">Блокировка буфера обмена для передачи файла изображений, текстового файла или ни одного из них.</span><span class="sxs-lookup"><span data-stu-id="ec12b-773">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="ec12b-774">Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-774">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="ec12b-775">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="ec12b-775">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="ec12b-776">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-776">Boolean</span></span>|<span data-ttu-id="ec12b-777">Позволяет заблокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="ec12b-777">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="ec12b-778">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="ec12b-778">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="ec12b-779">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-779">Boolean</span></span>|<span data-ttu-id="ec12b-780">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="ec12b-780">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="ec12b-781">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="ec12b-781">applicationGuardForceAuditing</span></span>|<span data-ttu-id="ec12b-782">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-782">Boolean</span></span>|<span data-ttu-id="ec12b-783">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="ec12b-783">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="ec12b-784">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="ec12b-784">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="ec12b-785">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="ec12b-785">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="ec12b-786">Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="ec12b-786">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="ec12b-787">Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-787">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="ec12b-788">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="ec12b-788">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="ec12b-789">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-789">Boolean</span></span>|<span data-ttu-id="ec12b-790">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="ec12b-790">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="ec12b-791">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="ec12b-791">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="ec12b-792">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-792">Boolean</span></span>|<span data-ttu-id="ec12b-793">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="ec12b-793">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="ec12b-794">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="ec12b-794">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="ec12b-795">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-795">Boolean</span></span>|<span data-ttu-id="ec12b-796">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="ec12b-796">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="ec12b-797">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="ec12b-797">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="ec12b-798">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-798">Boolean</span></span>|<span data-ttu-id="ec12b-799">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="ec12b-799">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="ec12b-800">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="ec12b-800">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="ec12b-801">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-801">Boolean</span></span>|<span data-ttu-id="ec12b-802">Разрешить охраннику приложения использовать виртуальный GPU</span><span class="sxs-lookup"><span data-stu-id="ec12b-802">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="ec12b-803">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="ec12b-803">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="ec12b-804">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-804">Boolean</span></span>|<span data-ttu-id="ec12b-805">Разрешить пользователям скачивать файлы из Edge в контейнере охраны приложений и сохранять их в файловой системе хост</span><span class="sxs-lookup"><span data-stu-id="ec12b-805">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="ec12b-806">applicationGuardAllowCameraMicrophoneRedirection</span><span class="sxs-lookup"><span data-stu-id="ec12b-806">applicationGuardAllowCameraMicrophoneRedirection</span></span>|<span data-ttu-id="ec12b-807">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-807">Boolean</span></span>|<span data-ttu-id="ec12b-808">Получает или задает, могут ли приложения в Microsoft Defender Application Guard получить доступ к камере и микрофону устройства.</span><span class="sxs-lookup"><span data-stu-id="ec12b-808">Gets or sets whether applications inside Microsoft Defender Application Guard can access the device’s camera and microphone.</span></span>|
|<span data-ttu-id="ec12b-809">applicationGuardCertificateThumbprints</span><span class="sxs-lookup"><span data-stu-id="ec12b-809">applicationGuardCertificateThumbprints</span></span>|<span data-ttu-id="ec12b-810">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ec12b-810">String collection</span></span>|<span data-ttu-id="ec12b-811">Позволяет использовать корневые сертификаты определенного уровня устройств в контейнере Microsoft Defender Application Guard.</span><span class="sxs-lookup"><span data-stu-id="ec12b-811">Allows certain device level Root Certificates to be shared with the Microsoft Defender Application Guard container.</span></span>|
|<span data-ttu-id="ec12b-812">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="ec12b-812">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="ec12b-813">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-813">Boolean</span></span>|<span data-ttu-id="ec12b-814">Позволяет администратору разрешить стандартным пользователям включить encrpytion во время azure AD Join.</span><span class="sxs-lookup"><span data-stu-id="ec12b-814">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="ec12b-815">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="ec12b-815">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="ec12b-816">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-816">Boolean</span></span>|<span data-ttu-id="ec12b-817">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="ec12b-817">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="ec12b-818">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="ec12b-818">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="ec12b-819">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-819">Boolean</span></span>|<span data-ttu-id="ec12b-820">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="ec12b-820">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="ec12b-821">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="ec12b-821">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="ec12b-822">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="ec12b-822">bitLockerEncryptDevice</span></span>|<span data-ttu-id="ec12b-823">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-823">Boolean</span></span>|<span data-ttu-id="ec12b-824">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="ec12b-824">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="ec12b-825">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="ec12b-825">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="ec12b-826">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="ec12b-826">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="ec12b-827">Политика привода системы BitLocker.</span><span class="sxs-lookup"><span data-stu-id="ec12b-827">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="ec12b-828">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="ec12b-828">bitLockerFixedDrivePolicy</span></span>|<span data-ttu-id="ec12b-829">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md);</span><span class="sxs-lookup"><span data-stu-id="ec12b-829">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)</span></span>|<span data-ttu-id="ec12b-830">Политика фиксированного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="ec12b-830">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="ec12b-831">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="ec12b-831">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="ec12b-832">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="ec12b-832">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="ec12b-833">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="ec12b-833">BitLocker Removable Drive Policy.</span></span>|
|<span data-ttu-id="ec12b-834">bitLockerRecoveryPasswordRotation</span><span class="sxs-lookup"><span data-stu-id="ec12b-834">bitLockerRecoveryPasswordRotation</span></span>|[<span data-ttu-id="ec12b-835">bitLockerRecoveryPasswordRotationType</span><span class="sxs-lookup"><span data-stu-id="ec12b-835">bitLockerRecoveryPasswordRotationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|<span data-ttu-id="ec12b-836">Этот параметр инициирует вращение пароля на основе клиента после восстановления диска ОС (с помощью bootmgr или WinRE).</span><span class="sxs-lookup"><span data-stu-id="ec12b-836">This setting initiates a client-driven recovery password rotation after an OS drive recovery (either by using bootmgr or WinRE).</span></span> <span data-ttu-id="ec12b-837">Возможные значения: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-837">Possible values are: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span></span>|
|<span data-ttu-id="ec12b-838">defenderDisableScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="ec12b-838">defenderDisableScanArchiveFiles</span></span>|<span data-ttu-id="ec12b-839">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-839">Boolean</span></span>|<span data-ttu-id="ec12b-840">Позволяет или не разрешает сканирование архивов.</span><span class="sxs-lookup"><span data-stu-id="ec12b-840">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="ec12b-841">defenderAllowScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="ec12b-841">defenderAllowScanArchiveFiles</span></span>|<span data-ttu-id="ec12b-842">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-842">Boolean</span></span>|<span data-ttu-id="ec12b-843">Позволяет или не разрешает сканирование архивов.</span><span class="sxs-lookup"><span data-stu-id="ec12b-843">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="ec12b-844">defenderDisableBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="ec12b-844">defenderDisableBehaviorMonitoring</span></span>|<span data-ttu-id="ec12b-845">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-845">Boolean</span></span>|<span data-ttu-id="ec12b-846">Позволяет или не разрешает Защитник Windows функции мониторинга поведения.</span><span class="sxs-lookup"><span data-stu-id="ec12b-846">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="ec12b-847">defenderAllowBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="ec12b-847">defenderAllowBehaviorMonitoring</span></span>|<span data-ttu-id="ec12b-848">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-848">Boolean</span></span>|<span data-ttu-id="ec12b-849">Позволяет или не разрешает Защитник Windows функции мониторинга поведения.</span><span class="sxs-lookup"><span data-stu-id="ec12b-849">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="ec12b-850">defenderDisableCloudProtection</span><span class="sxs-lookup"><span data-stu-id="ec12b-850">defenderDisableCloudProtection</span></span>|<span data-ttu-id="ec12b-851">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-851">Boolean</span></span>|<span data-ttu-id="ec12b-852">Чтобы лучше защитить компьютер, Защитник Windows отправляет в Корпорацию Майкрософт сведения о любых проблемах, которые он находит.</span><span class="sxs-lookup"><span data-stu-id="ec12b-852">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="ec12b-853">Корпорация Майкрософт проанализирует эту информацию, узнает больше о проблемах, затрагивающих вас и других клиентов, и предложит улучшенные решения.</span><span class="sxs-lookup"><span data-stu-id="ec12b-853">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="ec12b-854">defenderAllowCloudProtection</span><span class="sxs-lookup"><span data-stu-id="ec12b-854">defenderAllowCloudProtection</span></span>|<span data-ttu-id="ec12b-855">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-855">Boolean</span></span>|<span data-ttu-id="ec12b-856">Чтобы лучше защитить компьютер, Защитник Windows отправляет в Корпорацию Майкрософт сведения о любых проблемах, которые он находит.</span><span class="sxs-lookup"><span data-stu-id="ec12b-856">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="ec12b-857">Корпорация Майкрософт проанализирует эту информацию, узнает больше о проблемах, затрагивающих вас и других клиентов, и предложит улучшенные решения.</span><span class="sxs-lookup"><span data-stu-id="ec12b-857">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="ec12b-858">defenderEnableScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="ec12b-858">defenderEnableScanIncomingMail</span></span>|<span data-ttu-id="ec12b-859">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-859">Boolean</span></span>|<span data-ttu-id="ec12b-860">Позволяет или не разрешает сканирование электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ec12b-860">Allows or disallows scanning of email.</span></span>|
|<span data-ttu-id="ec12b-861">defenderEnableScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="ec12b-861">defenderEnableScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="ec12b-862">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-862">Boolean</span></span>|<span data-ttu-id="ec12b-863">Позволяет или не разрешает полное сканирование картографифицированных сетевых дисков.</span><span class="sxs-lookup"><span data-stu-id="ec12b-863">Allows or disallows a full scan of mapped network drives.</span></span>|
|<span data-ttu-id="ec12b-864">defenderDisableScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="ec12b-864">defenderDisableScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="ec12b-865">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-865">Boolean</span></span>|<span data-ttu-id="ec12b-866">Позволяет или отстраняет полное сканирование съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="ec12b-866">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="ec12b-867">Во время быстрого сканирования съемные диски могут по-прежнему проверяться.</span><span class="sxs-lookup"><span data-stu-id="ec12b-867">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="ec12b-868">defenderAllowScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="ec12b-868">defenderAllowScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="ec12b-869">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-869">Boolean</span></span>|<span data-ttu-id="ec12b-870">Позволяет или отстраняет полное сканирование съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="ec12b-870">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="ec12b-871">Во время быстрого сканирования съемные диски могут по-прежнему проверяться.</span><span class="sxs-lookup"><span data-stu-id="ec12b-871">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="ec12b-872">defenderDisableScanDownloads</span><span class="sxs-lookup"><span data-stu-id="ec12b-872">defenderDisableScanDownloads</span></span>|<span data-ttu-id="ec12b-873">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-873">Boolean</span></span>|<span data-ttu-id="ec12b-874">Позволяет или не разрешает Защитник Windows IOAVP Protection.</span><span class="sxs-lookup"><span data-stu-id="ec12b-874">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="ec12b-875">defenderAllowScanDownloads</span><span class="sxs-lookup"><span data-stu-id="ec12b-875">defenderAllowScanDownloads</span></span>|<span data-ttu-id="ec12b-876">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-876">Boolean</span></span>|<span data-ttu-id="ec12b-877">Позволяет или не разрешает Защитник Windows IOAVP Protection.</span><span class="sxs-lookup"><span data-stu-id="ec12b-877">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="ec12b-878">defenderDisableIntrusionPreventionSystem</span><span class="sxs-lookup"><span data-stu-id="ec12b-878">defenderDisableIntrusionPreventionSystem</span></span>|<span data-ttu-id="ec12b-879">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-879">Boolean</span></span>|<span data-ttu-id="ec12b-880">Позволяет или не разрешает Защитник Windows функции предотвращения вторжений.</span><span class="sxs-lookup"><span data-stu-id="ec12b-880">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="ec12b-881">defenderAllowIntrusionPreventionSystem</span><span class="sxs-lookup"><span data-stu-id="ec12b-881">defenderAllowIntrusionPreventionSystem</span></span>|<span data-ttu-id="ec12b-882">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-882">Boolean</span></span>|<span data-ttu-id="ec12b-883">Позволяет или не разрешает Защитник Windows функции предотвращения вторжений.</span><span class="sxs-lookup"><span data-stu-id="ec12b-883">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="ec12b-884">defenderDisableOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="ec12b-884">defenderDisableOnAccessProtection</span></span>|<span data-ttu-id="ec12b-885">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-885">Boolean</span></span>|<span data-ttu-id="ec12b-886">Позволяет или не разрешает Защитник Windows функции защиты доступа.</span><span class="sxs-lookup"><span data-stu-id="ec12b-886">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="ec12b-887">defenderAllowOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="ec12b-887">defenderAllowOnAccessProtection</span></span>|<span data-ttu-id="ec12b-888">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-888">Boolean</span></span>|<span data-ttu-id="ec12b-889">Позволяет или не разрешает Защитник Windows функции защиты доступа.</span><span class="sxs-lookup"><span data-stu-id="ec12b-889">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="ec12b-890">defenderDisableRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="ec12b-890">defenderDisableRealTimeMonitoring</span></span>|<span data-ttu-id="ec12b-891">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-891">Boolean</span></span>|<span data-ttu-id="ec12b-892">Позволяет или не разрешает Защитник Windows функции мониторинга реального времени.</span><span class="sxs-lookup"><span data-stu-id="ec12b-892">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="ec12b-893">defenderAllowRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="ec12b-893">defenderAllowRealTimeMonitoring</span></span>|<span data-ttu-id="ec12b-894">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-894">Boolean</span></span>|<span data-ttu-id="ec12b-895">Позволяет или не разрешает Защитник Windows функции мониторинга реального времени.</span><span class="sxs-lookup"><span data-stu-id="ec12b-895">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="ec12b-896">defenderDisableScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="ec12b-896">defenderDisableScanNetworkFiles</span></span>|<span data-ttu-id="ec12b-897">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-897">Boolean</span></span>|<span data-ttu-id="ec12b-898">Позволяет или не разрешает сканирование сетевых файлов.</span><span class="sxs-lookup"><span data-stu-id="ec12b-898">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="ec12b-899">defenderAllowScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="ec12b-899">defenderAllowScanNetworkFiles</span></span>|<span data-ttu-id="ec12b-900">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-900">Boolean</span></span>|<span data-ttu-id="ec12b-901">Позволяет или не разрешает сканирование сетевых файлов.</span><span class="sxs-lookup"><span data-stu-id="ec12b-901">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="ec12b-902">defenderDisableScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="ec12b-902">defenderDisableScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="ec12b-903">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-903">Boolean</span></span>|<span data-ttu-id="ec12b-904">Позволяет или не разрешает Защитник Windows скриптов.</span><span class="sxs-lookup"><span data-stu-id="ec12b-904">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="ec12b-905">defenderAllowScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="ec12b-905">defenderAllowScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="ec12b-906">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-906">Boolean</span></span>|<span data-ttu-id="ec12b-907">Позволяет или не разрешает Защитник Windows скриптов.</span><span class="sxs-lookup"><span data-stu-id="ec12b-907">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="ec12b-908">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="ec12b-908">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="ec12b-909">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-909">Boolean</span></span>|<span data-ttu-id="ec12b-910">Позволяет или не разрешает пользователю доступ к пользовательскому Защитник Windows пользовательскому интерфейсу.</span><span class="sxs-lookup"><span data-stu-id="ec12b-910">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="ec12b-911">Если они будут отложены, Защитник Windows уведомления также будут подавлены.</span><span class="sxs-lookup"><span data-stu-id="ec12b-911">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="ec12b-912">defenderAllowEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="ec12b-912">defenderAllowEndUserAccess</span></span>|<span data-ttu-id="ec12b-913">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-913">Boolean</span></span>|<span data-ttu-id="ec12b-914">Позволяет или не разрешает пользователю доступ к пользовательскому Защитник Windows пользовательскому интерфейсу.</span><span class="sxs-lookup"><span data-stu-id="ec12b-914">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="ec12b-915">Если они будут отложены, Защитник Windows уведомления также будут подавлены.</span><span class="sxs-lookup"><span data-stu-id="ec12b-915">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="ec12b-916">defenderScanMaxCpuPercentage</span><span class="sxs-lookup"><span data-stu-id="ec12b-916">defenderScanMaxCpuPercentage</span></span>|<span data-ttu-id="ec12b-917">Int32</span><span class="sxs-lookup"><span data-stu-id="ec12b-917">Int32</span></span>|<span data-ttu-id="ec12b-918">Представляет средний коэффициент нагрузки ЦП для Защитник Windows проверки (в процентах).</span><span class="sxs-lookup"><span data-stu-id="ec12b-918">Represents the average CPU load factor for the Windows Defender scan (in percent).</span></span> <span data-ttu-id="ec12b-919">Значение по умолчанию равно 50.</span><span class="sxs-lookup"><span data-stu-id="ec12b-919">The default value is 50.</span></span> <span data-ttu-id="ec12b-920">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="ec12b-920">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ec12b-921">defenderCheckForSignaturesBeforeRunningScan</span><span class="sxs-lookup"><span data-stu-id="ec12b-921">defenderCheckForSignaturesBeforeRunningScan</span></span>|<span data-ttu-id="ec12b-922">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-922">Boolean</span></span>|<span data-ttu-id="ec12b-923">Этот параметр политики позволяет управлять проверкой новых определений вирусов и программ-шпионов перед запуском сканирования.</span><span class="sxs-lookup"><span data-stu-id="ec12b-923">This policy setting allows you to manage whether a check for new virus and spyware definitions will occur before running a scan.</span></span>|
|<span data-ttu-id="ec12b-924">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="ec12b-924">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="ec12b-925">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="ec12b-925">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="ec12b-926">Добавлена в Windows 10 версии 1709.</span><span class="sxs-lookup"><span data-stu-id="ec12b-926">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="ec12b-927">Этот параметр политики определяет, насколько Защитник Windows антивирус будет блокировать и сканировать подозрительные файлы.</span><span class="sxs-lookup"><span data-stu-id="ec12b-927">This policy setting determines how aggressive Windows Defender Antivirus will be in blocking and scanning suspicious files.</span></span> <span data-ttu-id="ec12b-928">Тип значения является integer.</span><span class="sxs-lookup"><span data-stu-id="ec12b-928">Value type is integer.</span></span> <span data-ttu-id="ec12b-929">Для этой функции требуется включить параметр "Присоединиться к Microsoft MAPS".</span><span class="sxs-lookup"><span data-stu-id="ec12b-929">This feature requires the "Join Microsoft MAPS" setting enabled in order to function.</span></span> <span data-ttu-id="ec12b-930">Возможные значения: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-930">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="ec12b-931">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="ec12b-931">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="ec12b-932">Int32</span><span class="sxs-lookup"><span data-stu-id="ec12b-932">Int32</span></span>|<span data-ttu-id="ec12b-933">Добавлена в Windows 10 версии 1709.</span><span class="sxs-lookup"><span data-stu-id="ec12b-933">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="ec12b-934">Эта функция позволяет Защитник Windows антивирусу блокировать подозрительный файл на срок до 60 секунд и сканировать его в облаке, чтобы убедиться, что он является безопасным.</span><span class="sxs-lookup"><span data-stu-id="ec12b-934">This feature allows Windows Defender Antivirus to block a suspicious file for up to 60 seconds, and scan it in the cloud to make sure it's safe.</span></span> <span data-ttu-id="ec12b-935">Тип значения является наборным, диапазон — 0 — 50.</span><span class="sxs-lookup"><span data-stu-id="ec12b-935">Value type is integer, range is 0 - 50.</span></span> <span data-ttu-id="ec12b-936">Эта функция зависит от трех других параметров MAPS, которые необходимо включить: "Настройка функции "Блок с первого взгляда"; " Присоединяйтесь к Microsoft MAPS"; "Отправка образцов файлов при необходимости дальнейшего анализа".</span><span class="sxs-lookup"><span data-stu-id="ec12b-936">This feature depends on three other MAPS settings the must all be enabled- "Configure the 'Block at First Sight' feature; "Join Microsoft MAPS"; "Send file samples when further analysis is required".</span></span> <span data-ttu-id="ec12b-937">Допустимые значения: от 0 до 50.</span><span class="sxs-lookup"><span data-stu-id="ec12b-937">Valid values 0 to 50</span></span>|
|<span data-ttu-id="ec12b-938">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="ec12b-938">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="ec12b-939">Int32</span><span class="sxs-lookup"><span data-stu-id="ec12b-939">Int32</span></span>|<span data-ttu-id="ec12b-940">Период времени (в днях), когда элементы карантина будут храниться в системе.</span><span class="sxs-lookup"><span data-stu-id="ec12b-940">Time period (in days) that quarantine items will be stored on the system.</span></span> <span data-ttu-id="ec12b-941">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="ec12b-941">Valid values 0 to 90</span></span>|
|<span data-ttu-id="ec12b-942">defenderDisableCatchupFullScan</span><span class="sxs-lookup"><span data-stu-id="ec12b-942">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="ec12b-943">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-943">Boolean</span></span>|<span data-ttu-id="ec12b-944">Этот параметр политики позволяет настроить проверки наверстать упущенное для запланированных полных сканов.</span><span class="sxs-lookup"><span data-stu-id="ec12b-944">This policy setting allows you to configure catch-up scans for scheduled full scans.</span></span> <span data-ttu-id="ec12b-945">Проверка наверстать упущенное — это проверка, которая инициируется из-за пропущенного регулярно запланированного сканирования.</span><span class="sxs-lookup"><span data-stu-id="ec12b-945">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="ec12b-946">Обычно эти запланированные проверки пропускаются из-за отключения компьютера в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="ec12b-946">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="ec12b-947">defenderDisableCatchupQuickScan</span><span class="sxs-lookup"><span data-stu-id="ec12b-947">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="ec12b-948">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-948">Boolean</span></span>|<span data-ttu-id="ec12b-949">Этот параметр политики позволяет настроить проверки наверстать упущенное для запланированных быстрых сканирований.</span><span class="sxs-lookup"><span data-stu-id="ec12b-949">This policy setting allows you to configure catch-up scans for scheduled quick scans.</span></span> <span data-ttu-id="ec12b-950">Проверка наверстать упущенное — это проверка, которая инициируется из-за пропущенного регулярно запланированного сканирования.</span><span class="sxs-lookup"><span data-stu-id="ec12b-950">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="ec12b-951">Обычно эти запланированные проверки пропускаются из-за отключения компьютера в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="ec12b-951">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="ec12b-952">defenderEnableLowCpuPriority</span><span class="sxs-lookup"><span data-stu-id="ec12b-952">defenderEnableLowCpuPriority</span></span>|<span data-ttu-id="ec12b-953">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec12b-953">Boolean</span></span>|<span data-ttu-id="ec12b-954">Этот параметр политики позволяет включить или отключить низкий приоритет ЦП для запланированных сканов.</span><span class="sxs-lookup"><span data-stu-id="ec12b-954">This policy setting allows you to enable or disable low CPU priority for scheduled scans.</span></span>|
|<span data-ttu-id="ec12b-955">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="ec12b-955">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="ec12b-956">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ec12b-956">String collection</span></span>|<span data-ttu-id="ec12b-957">Расширения файлов, которые необходимо исключить из проверки и защиты в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="ec12b-957">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="ec12b-958">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="ec12b-958">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="ec12b-959">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ec12b-959">String collection</span></span>|<span data-ttu-id="ec12b-960">Файлы и папки, которые необходимо исключить из проверки и защиты в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="ec12b-960">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="ec12b-961">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="ec12b-961">defenderProcessesToExclude</span></span>|<span data-ttu-id="ec12b-962">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ec12b-962">String collection</span></span>|<span data-ttu-id="ec12b-963">Процессы, которые необходимо исключить из проверки и защиты в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="ec12b-963">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="ec12b-964">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="ec12b-964">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="ec12b-965">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="ec12b-965">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="ec12b-966">Добавлено в Windows 10 версии 1607.</span><span class="sxs-lookup"><span data-stu-id="ec12b-966">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="ec12b-967">Указывает уровень обнаружения для потенциально нежелательных приложений (PUAs).</span><span class="sxs-lookup"><span data-stu-id="ec12b-967">Specifies the level of detection for potentially unwanted applications (PUAs).</span></span> <span data-ttu-id="ec12b-968">Защитник Windows оповещает вас о скачиве потенциально нежелательного программного обеспечения или попытках установить себя на компьютере.</span><span class="sxs-lookup"><span data-stu-id="ec12b-968">Windows Defender alerts you when potentially unwanted software is being downloaded or attempts to install itself on your computer.</span></span> <span data-ttu-id="ec12b-969">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-969">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="ec12b-970">defenderScanDirection</span><span class="sxs-lookup"><span data-stu-id="ec12b-970">defenderScanDirection</span></span>|[<span data-ttu-id="ec12b-971">defenderRealtimeScanDirection</span><span class="sxs-lookup"><span data-stu-id="ec12b-971">defenderRealtimeScanDirection</span></span>](../resources/intune-deviceconfig-defenderrealtimescandirection.md)|<span data-ttu-id="ec12b-972">Контролирует, какие наборы файлов следует отслеживать.</span><span class="sxs-lookup"><span data-stu-id="ec12b-972">Controls which sets of files should be monitored.</span></span> <span data-ttu-id="ec12b-973">Возможные значения: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-973">Possible values are: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="ec12b-974">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="ec12b-974">defenderScanType</span></span>|[<span data-ttu-id="ec12b-975">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="ec12b-975">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="ec12b-976">Выбирает, следует ли выполнять быстрое сканирование или полное сканирование.</span><span class="sxs-lookup"><span data-stu-id="ec12b-976">Selects whether to perform a quick scan or full scan.</span></span> <span data-ttu-id="ec12b-977">Возможные значения: `userDefined`, `disabled`, `quick`, `full`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-977">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="ec12b-978">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="ec12b-978">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="ec12b-979">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ec12b-979">TimeOfDay</span></span>|<span data-ttu-id="ec12b-980">Выбирает время суток, когда Защитник Windows быстрое сканирование.</span><span class="sxs-lookup"><span data-stu-id="ec12b-980">Selects the time of day that the Windows Defender quick scan should run.</span></span> <span data-ttu-id="ec12b-981">Например, значение 0=12:00AM, значение 60=1:00AM, значение 120=2:00 и так далее, до значения 1380=11:00PM.</span><span class="sxs-lookup"><span data-stu-id="ec12b-981">For example, a value of 0=12:00AM, a value of 60=1:00AM, a value of 120=2:00, and so on, up to a value of 1380=11:00PM.</span></span> <span data-ttu-id="ec12b-982">Значение по умолчанию — 120</span><span class="sxs-lookup"><span data-stu-id="ec12b-982">The default value is 120</span></span>|
|<span data-ttu-id="ec12b-983">defenderScheduledScanDay</span><span class="sxs-lookup"><span data-stu-id="ec12b-983">defenderScheduledScanDay</span></span>|[<span data-ttu-id="ec12b-984">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="ec12b-984">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="ec12b-985">Выбирает день запуска Защитник Windows проверки.</span><span class="sxs-lookup"><span data-stu-id="ec12b-985">Selects the day that the Windows Defender scan should run.</span></span> <span data-ttu-id="ec12b-986">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-986">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="ec12b-987">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="ec12b-987">defenderScheduledScanTime</span></span>|<span data-ttu-id="ec12b-988">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ec12b-988">TimeOfDay</span></span>|<span data-ttu-id="ec12b-989">Выбирает время суток, когда должна Защитник Windows проверка.</span><span class="sxs-lookup"><span data-stu-id="ec12b-989">Selects the time of day that the Windows Defender scan should run.</span></span>|
|<span data-ttu-id="ec12b-990">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="ec12b-990">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="ec12b-991">Int32</span><span class="sxs-lookup"><span data-stu-id="ec12b-991">Int32</span></span>|<span data-ttu-id="ec12b-992">Указывает интервал (в часах), который будет использоваться для проверки подписей, поэтому вместо использования ScheduleDay и ScheduleTime проверка новых подписей будет задана в соответствии с интервалом.</span><span class="sxs-lookup"><span data-stu-id="ec12b-992">Specifies the interval (in hours) that will be used to check for signatures, so instead of using the ScheduleDay and ScheduleTime the check for new signatures will be set according to the interval.</span></span> <span data-ttu-id="ec12b-993">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="ec12b-993">Valid values 0 to 24</span></span>|
|<span data-ttu-id="ec12b-994">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="ec12b-994">defenderSubmitSamplesConsentType</span></span>|<span data-ttu-id="ec12b-995">[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md);</span><span class="sxs-lookup"><span data-stu-id="ec12b-995">[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)</span></span>|<span data-ttu-id="ec12b-996">Проверка уровня согласия пользователя в Защитник Windows для отправки данных.</span><span class="sxs-lookup"><span data-stu-id="ec12b-996">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="ec12b-997">Возможные значения: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span><span class="sxs-lookup"><span data-stu-id="ec12b-997">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="ec12b-998">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="ec12b-998">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="ec12b-999">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="ec12b-999">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="ec12b-1000">Позволяет администратору указать допустимые уровни серьезности угрозы и соответствующий ИД действий по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec12b-1000">Allows an administrator to specify any valid threat severity levels and the corresponding default action ID to take.</span></span>|



## <a name="response"></a><span data-ttu-id="ec12b-1001">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec12b-1001">Response</span></span>
<span data-ttu-id="ec12b-1002">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ec12b-1002">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec12b-1003">Пример</span><span class="sxs-lookup"><span data-stu-id="ec12b-1003">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec12b-1004">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec12b-1004">Request</span></span>
<span data-ttu-id="ec12b-1005">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec12b-1005">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 31268

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
  "defenderBlockPersistenceThroughWmiType": "block",
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
  "applicationGuardAllowCameraMicrophoneRedirection": true,
  "applicationGuardCertificateThumbprints": [
    "Application Guard Certificate Thumbprints value"
  ],
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

### <a name="response"></a><span data-ttu-id="ec12b-1006">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec12b-1006">Response</span></span>
<span data-ttu-id="ec12b-p226">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec12b-p226">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 31440

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
  "defenderBlockPersistenceThroughWmiType": "block",
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
  "applicationGuardAllowCameraMicrophoneRedirection": true,
  "applicationGuardCertificateThumbprints": [
    "Application Guard Certificate Thumbprints value"
  ],
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




