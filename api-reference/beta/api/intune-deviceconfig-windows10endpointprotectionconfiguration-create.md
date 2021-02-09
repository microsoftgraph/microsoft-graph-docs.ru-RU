---
title: Создание windows10EndpointProtectionConfiguration
description: Создание объекта windows10EndpointProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 04b1e1a7567d7a2ab63803097c9c84b2046ab411
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154574"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="66130-103">Создание windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="66130-103">Create windows10EndpointProtectionConfiguration</span></span>

<span data-ttu-id="66130-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66130-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66130-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66130-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66130-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66130-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66130-107">Создание объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66130-107">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66130-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="66130-108">Prerequisites</span></span>
<span data-ttu-id="66130-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66130-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66130-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66130-111">Permission type</span></span>|<span data-ttu-id="66130-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="66130-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66130-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66130-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66130-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66130-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="66130-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66130-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66130-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66130-116">Not supported.</span></span>|
|<span data-ttu-id="66130-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66130-117">Application</span></span>|<span data-ttu-id="66130-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66130-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66130-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66130-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="66130-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="66130-120">Request headers</span></span>
|<span data-ttu-id="66130-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="66130-121">Header</span></span>|<span data-ttu-id="66130-122">Значение</span><span class="sxs-lookup"><span data-stu-id="66130-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66130-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66130-123">Authorization</span></span>|<span data-ttu-id="66130-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66130-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66130-125">Accept</span><span class="sxs-lookup"><span data-stu-id="66130-125">Accept</span></span>|<span data-ttu-id="66130-126">application/json</span><span class="sxs-lookup"><span data-stu-id="66130-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66130-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66130-127">Request body</span></span>
<span data-ttu-id="66130-128">В теле запроса добавьте представление объекта windows10EndpointProtectionConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66130-128">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="66130-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="66130-129">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="66130-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="66130-130">Property</span></span>|<span data-ttu-id="66130-131">Тип</span><span class="sxs-lookup"><span data-stu-id="66130-131">Type</span></span>|<span data-ttu-id="66130-132">Описание</span><span class="sxs-lookup"><span data-stu-id="66130-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66130-133">id</span><span class="sxs-lookup"><span data-stu-id="66130-133">id</span></span>|<span data-ttu-id="66130-134">String</span><span class="sxs-lookup"><span data-stu-id="66130-134">String</span></span>|<span data-ttu-id="66130-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="66130-135">Key of the entity.</span></span> <span data-ttu-id="66130-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66130-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66130-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66130-137">lastModifiedDateTime</span></span>|<span data-ttu-id="66130-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66130-138">DateTimeOffset</span></span>|<span data-ttu-id="66130-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="66130-139">DateTime the object was last modified.</span></span> <span data-ttu-id="66130-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66130-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66130-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="66130-141">roleScopeTagIds</span></span>|<span data-ttu-id="66130-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="66130-142">String collection</span></span>|<span data-ttu-id="66130-143">Список тегов области для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="66130-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="66130-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66130-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66130-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="66130-145">supportsScopeTags</span></span>|<span data-ttu-id="66130-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-146">Boolean</span></span>|<span data-ttu-id="66130-147">Указывает, поддерживает ли конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="66130-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="66130-148">Назначение свойству ScopeTags не допускается, если это значение имеет значение false, а сущности не будут видны пользователям с заданной областью действия.</span><span class="sxs-lookup"><span data-stu-id="66130-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="66130-149">Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="66130-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="66130-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="66130-150">This property is read-only.</span></span> <span data-ttu-id="66130-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66130-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66130-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="66130-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="66130-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="66130-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="66130-154">Применимость выпуска ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="66130-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="66130-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66130-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66130-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="66130-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="66130-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="66130-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="66130-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="66130-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="66130-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66130-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66130-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="66130-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="66130-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="66130-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="66130-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="66130-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="66130-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66130-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66130-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66130-164">createdDateTime</span></span>|<span data-ttu-id="66130-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66130-165">DateTimeOffset</span></span>|<span data-ttu-id="66130-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="66130-166">DateTime the object was created.</span></span> <span data-ttu-id="66130-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66130-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66130-168">description</span><span class="sxs-lookup"><span data-stu-id="66130-168">description</span></span>|<span data-ttu-id="66130-169">String</span><span class="sxs-lookup"><span data-stu-id="66130-169">String</span></span>|<span data-ttu-id="66130-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="66130-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="66130-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66130-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66130-172">displayName</span><span class="sxs-lookup"><span data-stu-id="66130-172">displayName</span></span>|<span data-ttu-id="66130-173">String</span><span class="sxs-lookup"><span data-stu-id="66130-173">String</span></span>|<span data-ttu-id="66130-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="66130-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="66130-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66130-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66130-176">version</span><span class="sxs-lookup"><span data-stu-id="66130-176">version</span></span>|<span data-ttu-id="66130-177">Int32</span><span class="sxs-lookup"><span data-stu-id="66130-177">Int32</span></span>|<span data-ttu-id="66130-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="66130-178">Version of the device configuration.</span></span> <span data-ttu-id="66130-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66130-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66130-180">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="66130-180">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="66130-181">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="66130-181">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="66130-182">Эта политика предназначена для обеспечения дополнительной защиты от внешних устройств с DMA.</span><span class="sxs-lookup"><span data-stu-id="66130-182">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="66130-183">Он обеспечивает более полный контроль над нумерацией внешних устройств с DMA, несовместимых с DMA Remapping/изоляцией памяти устройства и изолированием.</span><span class="sxs-lookup"><span data-stu-id="66130-183">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="66130-184">Эта политика вступает в силу только в том случае, если защита DMA ядра поддерживается и включена системным программным обеспечением.</span><span class="sxs-lookup"><span data-stu-id="66130-184">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="66130-185">Защита DMA ядра — это функция платформы, которой невозможно управлять с помощью политики или конечным пользователем.</span><span class="sxs-lookup"><span data-stu-id="66130-185">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="66130-186">Оно должно поддерживаться системой во время производства.</span><span class="sxs-lookup"><span data-stu-id="66130-186">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="66130-187">Чтобы проверить, поддерживает ли система защиту DMA ядра, проверьте поле "Защита DMA ядра" на странице сводки MSINFO32.exe.</span><span class="sxs-lookup"><span data-stu-id="66130-187">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="66130-188">Возможные значения: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="66130-188">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="66130-189">firewallRules</span><span class="sxs-lookup"><span data-stu-id="66130-189">firewallRules</span></span>|<span data-ttu-id="66130-190">[Коллекция windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)</span><span class="sxs-lookup"><span data-stu-id="66130-190">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="66130-191">Настраивает параметры правила брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="66130-191">Configures the firewall rule settings.</span></span> <span data-ttu-id="66130-192">Эта коллекция может содержать не более 150 элементов.</span><span class="sxs-lookup"><span data-stu-id="66130-192">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="66130-193">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="66130-193">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="66130-194">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-194">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-195">Это право пользователя используется диспетчером учетных данных во время резервного копирования и восстановления.</span><span class="sxs-lookup"><span data-stu-id="66130-195">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="66130-196">Сохраненные учетные данные пользователей могут быть скомпрометированы, если эта привилегия предоставляется другим сущностям.</span><span class="sxs-lookup"><span data-stu-id="66130-196">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="66130-197">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="66130-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="66130-198">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="66130-198">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="66130-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-200">Это право пользователя определяет, какие пользователи и группы могут подключаться к компьютеру по сети.</span><span class="sxs-lookup"><span data-stu-id="66130-200">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="66130-201">Поддерживается состояние "Разрешено".</span><span class="sxs-lookup"><span data-stu-id="66130-201">State Allowed is supported.</span></span>|
|<span data-ttu-id="66130-202">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="66130-202">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="66130-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-204">Это право пользователя определяет, какие пользователи и группы не могут подключаться к компьютеру по сети.</span><span class="sxs-lookup"><span data-stu-id="66130-204">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="66130-205">Блокировка состояния поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66130-205">State Block is supported.</span></span>|
|<span data-ttu-id="66130-206">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="66130-206">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="66130-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-208">Это право пользователя позволяет процессу подавлять любого пользователя без проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="66130-208">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="66130-209">Таким образом, этот процесс может получить доступ к тем же локальным ресурсам, что и этот пользователь.</span><span class="sxs-lookup"><span data-stu-id="66130-209">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="66130-210">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="66130-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="66130-211">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="66130-211">userRightsLocalLogOn</span></span>|[<span data-ttu-id="66130-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-213">Это право пользователя определяет, какие пользователи могут войти на компьютер.</span><span class="sxs-lookup"><span data-stu-id="66130-213">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="66130-214">Поддерживаются состояния NotConfigured, Allowed</span><span class="sxs-lookup"><span data-stu-id="66130-214">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="66130-215">userRightsDenyLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="66130-215">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="66130-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-217">Это право пользователя определяет, какие пользователи не могут войти на компьютер.</span><span class="sxs-lookup"><span data-stu-id="66130-217">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="66130-218">Поддерживаются состояния NotConfigured, Blocked</span><span class="sxs-lookup"><span data-stu-id="66130-218">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="66130-219">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="66130-219">userRightsBackupData</span></span>|[<span data-ttu-id="66130-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-221">Это право пользователя определяет, какие пользователи могут обходить разрешения файлов, каталогов, реестра и других постоянных объектов при архивирования файлов и каталогов.</span><span class="sxs-lookup"><span data-stu-id="66130-221">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="66130-222">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="66130-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="66130-223">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="66130-223">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="66130-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-225">Это право пользователя определяет, какие пользователи и группы могут изменять время и дату во внутренних часах компьютера.</span><span class="sxs-lookup"><span data-stu-id="66130-225">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="66130-226">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="66130-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="66130-227">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="66130-227">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="66130-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-229">Этот параметр безопасности определяет, могут ли пользователи создавать глобальные объекты, доступные для всех сеансов.</span><span class="sxs-lookup"><span data-stu-id="66130-229">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="66130-230">Пользователи, которые могут создавать глобальные объекты, могут влиять на процессы, которые запускаются в сеансах других пользователей, что может привести к сбою приложения или повреждения данных.</span><span class="sxs-lookup"><span data-stu-id="66130-230">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="66130-231">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="66130-231">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="66130-232">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="66130-232">userRightsCreatePageFile</span></span>|[<span data-ttu-id="66130-233">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-233">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-234">Это право пользователя определяет, какие пользователи и группы могут вызывать внутренний API для создания и изменения размера файла страницы.</span><span class="sxs-lookup"><span data-stu-id="66130-234">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="66130-235">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="66130-235">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="66130-236">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="66130-236">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="66130-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-238">Это право пользователя определяет, какие учетные записи могут использоваться процессами для создания объекта каталога с помощью диспетчера объектов.</span><span class="sxs-lookup"><span data-stu-id="66130-238">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="66130-239">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="66130-239">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="66130-240">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="66130-240">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="66130-241">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-241">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-242">Это право пользователя определяет, может ли пользователь создать символьную ссылку с компьютера, на который он вошел.</span><span class="sxs-lookup"><span data-stu-id="66130-242">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="66130-243">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="66130-243">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="66130-244">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="66130-244">userRightsCreateToken</span></span>|[<span data-ttu-id="66130-245">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-245">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-246">Это право пользователя определяет, какие пользователи или группы могут использоваться процессами для создания маркера, который затем можно использовать для получения доступа к любым локальным ресурсам, когда процесс использует внутренний API для создания маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="66130-246">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="66130-247">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="66130-247">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="66130-248">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="66130-248">userRightsDebugPrograms</span></span>|[<span data-ttu-id="66130-249">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-249">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-250">Это право пользователя определяет, какие пользователи могут прикрепить отладок к любому процессу или ядру.</span><span class="sxs-lookup"><span data-stu-id="66130-250">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="66130-251">Поддерживаются только состояния NotConfigured и Allowed</span><span class="sxs-lookup"><span data-stu-id="66130-251">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="66130-252">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="66130-252">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="66130-253">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-253">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-254">Это право пользователя определяет, какие пользователи и группы не могут войти в качестве клиента служб удаленных рабочих стола.</span><span class="sxs-lookup"><span data-stu-id="66130-254">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="66130-255">Поддерживаются только состояния NotConfigured и Blocked</span><span class="sxs-lookup"><span data-stu-id="66130-255">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="66130-256">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="66130-256">userRightsDelegation</span></span>|[<span data-ttu-id="66130-257">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-257">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-258">Это право пользователя определяет, какие пользователи могут установить параметр "Доверенный для делегирования" для объекта пользователя или компьютера.</span><span class="sxs-lookup"><span data-stu-id="66130-258">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="66130-259">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="66130-259">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="66130-260">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="66130-260">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="66130-261">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-261">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-262">Это право пользователя определяет, какие учетные записи могут использоваться процессом для добавления записей в журнал безопасности.</span><span class="sxs-lookup"><span data-stu-id="66130-262">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="66130-263">Журнал безопасности используется для трассировки несанкционированного доступа к системе.</span><span class="sxs-lookup"><span data-stu-id="66130-263">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="66130-264">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="66130-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="66130-265">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="66130-265">userRightsImpersonateClient</span></span>|[<span data-ttu-id="66130-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-267">Назначение этого права пользователю позволяет программам, запущенным от имени этого пользователя, выдать себя за клиента.</span><span class="sxs-lookup"><span data-stu-id="66130-267">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="66130-268">Требование этого права пользователя для такого типа поднаправления не позволяет неавторизованному пользователю подключиться к созданной им службе, а затем под видом этого клиента, что может повысить уровень разрешений неавторизованного пользователя до административных или системных уровней.</span><span class="sxs-lookup"><span data-stu-id="66130-268">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="66130-269">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="66130-269">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="66130-270">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="66130-270">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="66130-271">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-271">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-272">Это право пользователя определяет, какие учетные записи могут использовать процесс с доступом на запись свойств к другому процессу для повышения приоритета выполнения, назначенного другому процессу.</span><span class="sxs-lookup"><span data-stu-id="66130-272">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="66130-273">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="66130-273">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="66130-274">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="66130-274">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="66130-275">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-275">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-276">Это право пользователя определяет, какие пользователи могут динамически загружать и выгружать драйверы устройств или другой код в режиме ядра.</span><span class="sxs-lookup"><span data-stu-id="66130-276">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="66130-277">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="66130-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="66130-278">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="66130-278">userRightsLockMemory</span></span>|[<span data-ttu-id="66130-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-280">Это право пользователя определяет, какие учетные записи могут использовать процесс для хранения данных в физической памяти, что не позволяет системе разгона данных в виртуальную память на диске.</span><span class="sxs-lookup"><span data-stu-id="66130-280">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="66130-281">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="66130-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="66130-282">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="66130-282">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="66130-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-284">Это право пользователя определяет, какие пользователи могут указывать параметры аудита доступа к объектам для отдельных ресурсов, таких как файлы, объекты Active Directory и ключи реестра.</span><span class="sxs-lookup"><span data-stu-id="66130-284">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="66130-285">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="66130-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="66130-286">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="66130-286">userRightsManageVolumes</span></span>|[<span data-ttu-id="66130-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-288">Это право пользователя определяет, какие пользователи и группы могут выполнять задачи обслуживания на томе, например удаленную дефрагментацию.</span><span class="sxs-lookup"><span data-stu-id="66130-288">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="66130-289">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="66130-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="66130-290">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="66130-290">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="66130-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-292">Это право пользователя определяет, кто может изменять значения среды микропрограмм.</span><span class="sxs-lookup"><span data-stu-id="66130-292">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="66130-293">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="66130-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="66130-294">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="66130-294">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="66130-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-296">Это право пользователя определяет, какие учетные записи пользователей могут изменять метку целостности объектов, таких как файлы, ключи реестра или процессы, которые принадлежат другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="66130-296">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="66130-297">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="66130-297">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="66130-298">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="66130-298">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="66130-299">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-299">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-300">Это право пользователя определяет, какие пользователи могут использовать средства мониторинга производительности для отслеживания производительности системных процессов.</span><span class="sxs-lookup"><span data-stu-id="66130-300">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="66130-301">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="66130-301">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="66130-302">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="66130-302">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="66130-303">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-303">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-304">Это право пользователя определяет, какие пользователи могут отключить компьютер из удаленного расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="66130-304">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="66130-305">Неправильное использование этого права пользователя может привести к отказу в обслуживании.</span><span class="sxs-lookup"><span data-stu-id="66130-305">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="66130-306">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="66130-306">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="66130-307">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="66130-307">userRightsRestoreData</span></span>|[<span data-ttu-id="66130-308">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-308">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-309">Это право пользователя определяет, какие пользователи могут обходить разрешения файлов, каталогов, реестра и других постоянных объектов при восстановлении архивных файлов и каталогов, а также определяет, какие пользователи могут установить любого допустимого участников безопасности в качестве владельца объекта.</span><span class="sxs-lookup"><span data-stu-id="66130-309">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="66130-310">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="66130-310">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="66130-311">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="66130-311">userRightsTakeOwnership</span></span>|[<span data-ttu-id="66130-312">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="66130-312">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="66130-313">Это право пользователя определяет, какие пользователи могут стать владельцем любого защищаемого объекта в системе, включая объекты Active Directory, файлы и папки, принтеры, ключи реестра, процессы и потоки.</span><span class="sxs-lookup"><span data-stu-id="66130-313">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="66130-314">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="66130-314">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="66130-315">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="66130-315">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="66130-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-316">Boolean</span></span>|<span data-ttu-id="66130-317">Этот параметр определяет, включено ли сохранение игры xbox (1) или отключено (0).</span><span class="sxs-lookup"><span data-stu-id="66130-317">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="66130-318">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="66130-318">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="66130-319">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="66130-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="66130-320">Этот параметр определяет тип запуска службы управления "Метод доступа": Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="66130-320">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="66130-321">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="66130-321">Default: Manual.</span></span> <span data-ttu-id="66130-322">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="66130-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="66130-323">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="66130-323">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="66130-324">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="66130-324">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="66130-325">Этот параметр определяет тип запуска службы Live Auth Manager — Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="66130-325">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="66130-326">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="66130-326">Default: Manual.</span></span> <span data-ttu-id="66130-327">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="66130-327">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="66130-328">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="66130-328">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="66130-329">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="66130-329">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="66130-330">Этот параметр определяет тип запуска службы сохранения live Game — Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="66130-330">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="66130-331">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="66130-331">Default: Manual.</span></span> <span data-ttu-id="66130-332">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="66130-332">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="66130-333">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="66130-333">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="66130-334">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="66130-334">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="66130-335">Этот параметр определяет тип запуска сетевой службы Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="66130-335">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="66130-336">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="66130-336">Default: Manual.</span></span> <span data-ttu-id="66130-337">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="66130-337">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="66130-338">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="66130-338">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="66130-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-339">Boolean</span></span>|<span data-ttu-id="66130-340">Запретить пользователям добавлять новые учетные записи Майкрософт на этот компьютер.</span><span class="sxs-lookup"><span data-stu-id="66130-340">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="66130-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="66130-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="66130-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-342">Boolean</span></span>|<span data-ttu-id="66130-343">Включить локальные учетные записи, которые не защищены паролем, для входа в систему из местоположений, кроме физического устройства. По умолчанию включено</span><span class="sxs-lookup"><span data-stu-id="66130-343">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="66130-344">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="66130-344">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="66130-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-345">Boolean</span></span>|<span data-ttu-id="66130-346">Определяет, включена ли учетная запись локального администратора.</span><span class="sxs-lookup"><span data-stu-id="66130-346">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="66130-347">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="66130-347">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="66130-348">String</span><span class="sxs-lookup"><span data-stu-id="66130-348">String</span></span>|<span data-ttu-id="66130-349">Определите другое имя учетной записи, которое будет связано с идентификатором безопасности (SID) для учетной записи "Администратор".</span><span class="sxs-lookup"><span data-stu-id="66130-349">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="66130-350">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="66130-350">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="66130-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-351">Boolean</span></span>|<span data-ttu-id="66130-352">Определяет, включена ли гостевая учетная запись.</span><span class="sxs-lookup"><span data-stu-id="66130-352">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="66130-353">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="66130-353">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="66130-354">String</span><span class="sxs-lookup"><span data-stu-id="66130-354">String</span></span>|<span data-ttu-id="66130-355">Определите другое имя учетной записи, которое будет связано с идентификатором безопасности (SID) для учетной записи "Гость".</span><span class="sxs-lookup"><span data-stu-id="66130-355">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="66130-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="66130-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="66130-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-357">Boolean</span></span>|<span data-ttu-id="66130-358">Запретить отсоединую от портативного компьютера без необходимости входа в систему.</span><span class="sxs-lookup"><span data-stu-id="66130-358">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="66130-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="66130-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="66130-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-360">Boolean</span></span>|<span data-ttu-id="66130-361">Ограничить установку драйверов принтера при подключении к общему принтеру только администраторам.</span><span class="sxs-lookup"><span data-stu-id="66130-361">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="66130-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="66130-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="66130-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-363">Boolean</span></span>|<span data-ttu-id="66130-364">Включение этого параметра позволяет пользователю получать доступ к компакт-дисководным носителю только в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="66130-364">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="66130-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="66130-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="66130-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="66130-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="66130-367">Определите, кому разрешено форматирование и извлечение съемных носитеев NTFS.</span><span class="sxs-lookup"><span data-stu-id="66130-367">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="66130-368">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="66130-368">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="66130-369">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="66130-369">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="66130-370">Int32</span><span class="sxs-lookup"><span data-stu-id="66130-370">Int32</span></span>|<span data-ttu-id="66130-371">Определите максимальное время бездействия в минутах на экране входа интерактивного рабочего стола до тех пор, пока не будет работать экранная программа сохранения.</span><span class="sxs-lookup"><span data-stu-id="66130-371">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="66130-372">Допустимые значения: от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="66130-372">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="66130-373">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="66130-373">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="66130-374">Int32</span><span class="sxs-lookup"><span data-stu-id="66130-374">Int32</span></span>|<span data-ttu-id="66130-375">Определите максимальное время бездействия в минутах на экране входа интерактивного рабочего стола, пока не будет работать экранная программа сохранения.</span><span class="sxs-lookup"><span data-stu-id="66130-375">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="66130-376">Допустимые значения: от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="66130-376">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="66130-377">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="66130-377">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="66130-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-378">Boolean</span></span>|<span data-ttu-id="66130-379">Прежде чем пользователь сможет войти в систему, необходимо нажать CTRL+ALT+DEL.</span><span class="sxs-lookup"><span data-stu-id="66130-379">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="66130-380">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="66130-380">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="66130-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-381">Boolean</span></span>|<span data-ttu-id="66130-382">Не отображать имя пользователя последнего пользователя, выписавшегося на этом устройстве.</span><span class="sxs-lookup"><span data-stu-id="66130-382">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="66130-383">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="66130-383">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="66130-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-384">Boolean</span></span>|<span data-ttu-id="66130-385">Не отображать имя пользователя, войдя на это устройство, после в введены учетных данных и до отображения рабочего стола устройства.</span><span class="sxs-lookup"><span data-stu-id="66130-385">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="66130-386">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="66130-386">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="66130-387">String</span><span class="sxs-lookup"><span data-stu-id="66130-387">String</span></span>|<span data-ttu-id="66130-388">Заголовок сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="66130-388">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="66130-389">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="66130-389">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="66130-390">String</span><span class="sxs-lookup"><span data-stu-id="66130-390">String</span></span>|<span data-ttu-id="66130-391">Установите текст сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="66130-391">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="66130-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="66130-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="66130-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-393">Boolean</span></span>|<span data-ttu-id="66130-394">Блокировать запросы проверки подлинности PKU2U на этом устройстве для использования сетевых удостоверений.</span><span class="sxs-lookup"><span data-stu-id="66130-394">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="66130-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="66130-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="66130-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-396">Boolean</span></span>|<span data-ttu-id="66130-397">Ui helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span><span class="sxs-lookup"><span data-stu-id="66130-397">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="66130-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="66130-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="66130-399">String</span><span class="sxs-lookup"><span data-stu-id="66130-399">String</span></span>|<span data-ttu-id="66130-400">Изменить строку языка определения дескриптора безопасности по умолчанию, чтобы разрешить или запретить пользователям и группам делать удаленные вызовы SAM.</span><span class="sxs-lookup"><span data-stu-id="66130-400">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="66130-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="66130-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="66130-402">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="66130-402">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="66130-403">Этот параметр безопасности позволяет клиенту требовать согласования 128-битного шифрования и/или безопасности сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="66130-403">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="66130-404">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="66130-404">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="66130-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="66130-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="66130-406">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="66130-406">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="66130-407">Этот параметр безопасности позволяет серверу требовать согласования 128-битного шифрования и/или безопасности сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="66130-407">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="66130-408">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="66130-408">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="66130-409">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="66130-409">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="66130-410">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="66130-410">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="66130-411">Этот параметр безопасности определяет, какой протокол проверки подлинности запроса/ответа используется для сетевых учетных данных.</span><span class="sxs-lookup"><span data-stu-id="66130-411">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="66130-412">Возможные значения: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="66130-412">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="66130-413">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="66130-413">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="66130-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-414">Boolean</span></span>|<span data-ttu-id="66130-415">Если этот список включен, клиент SMB разрешит незащищенные гостевых входа.</span><span class="sxs-lookup"><span data-stu-id="66130-415">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="66130-416">Если он не настроен, клиент SMB отклоняет незащищенные гостевых логов.</span><span class="sxs-lookup"><span data-stu-id="66130-416">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="66130-417">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="66130-417">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="66130-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-418">Boolean</span></span>|<span data-ttu-id="66130-419">Этот параметр безопасности определяет, очищается ли страница виртуальной памяти при отключке системы.</span><span class="sxs-lookup"><span data-stu-id="66130-419">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="66130-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="66130-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="66130-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-421">Boolean</span></span>|<span data-ttu-id="66130-422">Этот параметр безопасности определяет, можно ли отключить компьютер без необходимости входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="66130-422">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="66130-423">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="66130-423">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="66130-424">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-424">Boolean</span></span>|<span data-ttu-id="66130-425">Разрешить приложениям UIAccess запрос повышения прав без использования безопасного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="66130-425">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="66130-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="66130-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="66130-427">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-427">Boolean</span></span>|<span data-ttu-id="66130-428">Виртуализация сбоев записи файлов и реестра для каждого расположения пользователя</span><span class="sxs-lookup"><span data-stu-id="66130-428">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="66130-429">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="66130-429">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="66130-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-430">Boolean</span></span>|<span data-ttu-id="66130-431">Принудительное выполнение проверки пути сертификации PKI для заданного исполняемого файла перед разрешением на запуск.</span><span class="sxs-lookup"><span data-stu-id="66130-431">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="66130-432">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="66130-432">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="66130-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="66130-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="66130-434">Определите поведение запроса на повышение прав для администраторов в режиме утверждения администратором.</span><span class="sxs-lookup"><span data-stu-id="66130-434">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="66130-435">Возможные значения: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="66130-435">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="66130-436">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="66130-436">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="66130-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="66130-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="66130-438">Определите поведение запроса на повышение прав для обычных пользователей.</span><span class="sxs-lookup"><span data-stu-id="66130-438">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="66130-439">Возможные значения: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="66130-439">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="66130-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="66130-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="66130-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-441">Boolean</span></span>|<span data-ttu-id="66130-442">Включить все запросы на повышение прав, чтобы перейти на рабочий стол интерактивного пользователя, а не на безопасный рабочий стол.</span><span class="sxs-lookup"><span data-stu-id="66130-442">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="66130-443">Используются параметры политики поведения подсказок для администраторов и обычных пользователей.</span><span class="sxs-lookup"><span data-stu-id="66130-443">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="66130-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="66130-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="66130-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-445">Boolean</span></span>|<span data-ttu-id="66130-446">При установке приложений, требующих повышенных привилегий, будут предложены учетные данные администратора. По умолчанию включено</span><span class="sxs-lookup"><span data-stu-id="66130-446">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="66130-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="66130-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="66130-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-448">Boolean</span></span>|<span data-ttu-id="66130-449">Разрешить приложениям UIAccess запрос повышения прав без использования безопасного рабочего стола. По умолчанию включено</span><span class="sxs-lookup"><span data-stu-id="66130-449">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="66130-450">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="66130-450">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="66130-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-451">Boolean</span></span>|<span data-ttu-id="66130-452">Определяет, использует ли встроенная учетная запись администратора режим утверждения администратора или запускает все приложения с полными привилегиями администратора. По умолчанию включено</span><span class="sxs-lookup"><span data-stu-id="66130-452">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="66130-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="66130-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="66130-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-454">Boolean</span></span>|<span data-ttu-id="66130-455">Определите, включен ли режим утверждения администратором и все параметры политики UAC, по умолчанию включено</span><span class="sxs-lookup"><span data-stu-id="66130-455">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="66130-456">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="66130-456">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="66130-457">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="66130-457">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="66130-458">Настройте сведения о пользователе, отображаемые при блокировке сеанса.</span><span class="sxs-lookup"><span data-stu-id="66130-458">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="66130-459">Если этот код не настроен, отображаются отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="66130-459">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="66130-460">Возможные значения: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="66130-460">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="66130-461">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="66130-461">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="66130-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="66130-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="66130-463">Настройте сведения о пользователе, отображаемые при блокировке сеанса.</span><span class="sxs-lookup"><span data-stu-id="66130-463">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="66130-464">Если этот код не настроен, отображаются отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="66130-464">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="66130-465">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="66130-465">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="66130-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="66130-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="66130-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-467">Boolean</span></span>|<span data-ttu-id="66130-468">Этот параметр безопасности определяет, пытается ли клиент SMB согласовать подписывания пакетов SMB.</span><span class="sxs-lookup"><span data-stu-id="66130-468">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="66130-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="66130-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="66130-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-470">Boolean</span></span>|<span data-ttu-id="66130-471">Этот параметр безопасности определяет, требуется ли подписывания пакетов клиентом SMB.</span><span class="sxs-lookup"><span data-stu-id="66130-471">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="66130-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="66130-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="66130-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-473">Boolean</span></span>|<span data-ttu-id="66130-474">Если этот параметр безопасности включен, перенаправлению SMB разрешается отправлять пароли в обычном текстовом тексте на серверы SMB, которые не поддерживают шифрование паролей во время проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="66130-474">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="66130-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="66130-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="66130-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-476">Boolean</span></span>|<span data-ttu-id="66130-477">Этот параметр безопасности определяет, требуется ли подписывания пакетов компонентом сервера SMB.</span><span class="sxs-lookup"><span data-stu-id="66130-477">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="66130-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="66130-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="66130-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-479">Boolean</span></span>|<span data-ttu-id="66130-480">Этот параметр безопасности определяет, будет ли сервер SMB согласовывать подписывания пакетов SMB с клиентами, которые его запрашивают.</span><span class="sxs-lookup"><span data-stu-id="66130-480">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="66130-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="66130-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="66130-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-482">Boolean</span></span>|<span data-ttu-id="66130-483">По умолчанию этот параметр безопасности ограничивает анонимный доступ к ресурсам и передает их в параметры для именовых каналов, к которые можно получить анонимный доступ, и к ним можно получить анонимный доступ.</span><span class="sxs-lookup"><span data-stu-id="66130-483">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="66130-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="66130-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="66130-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-485">Boolean</span></span>|<span data-ttu-id="66130-486">Этот параметр безопасности определяет, какие дополнительные разрешения будут предоставлены для анонимных подключений к компьютеру.</span><span class="sxs-lookup"><span data-stu-id="66130-486">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="66130-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="66130-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="66130-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-488">Boolean</span></span>|<span data-ttu-id="66130-489">Этот параметр безопасности определяет, разрешается ли анонимным пользователям выполнять определенные действия, такие как список имен учетных записей домена и сетевых сетей.</span><span class="sxs-lookup"><span data-stu-id="66130-489">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="66130-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="66130-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="66130-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-491">Boolean</span></span>|<span data-ttu-id="66130-492">Этот параметр безопасности определяет, сохраняется ли при следующей смене пароля значение hash-значения lan Manager (LM) для нового пароля.</span><span class="sxs-lookup"><span data-stu-id="66130-492">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="66130-493">Он не хранится по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="66130-493">It’s not stored by default.</span></span>|
|<span data-ttu-id="66130-494">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="66130-494">localSecurityOptionsSmartCardRemovalBehavior</span></span>|<span data-ttu-id="66130-495">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md);</span><span class="sxs-lookup"><span data-stu-id="66130-495">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)</span></span>|<span data-ttu-id="66130-496">Этот параметр безопасности определяет, что происходит при удалении смарт-карты для пользователя, выходящего из системы чтения смарт-карт.</span><span class="sxs-lookup"><span data-stu-id="66130-496">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="66130-497">Возможные значения: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="66130-497">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="66130-498">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="66130-498">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="66130-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-499">Boolean</span></span>|<span data-ttu-id="66130-500">Используется для отключения отображения области защиты приложения и браузера.</span><span class="sxs-lookup"><span data-stu-id="66130-500">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="66130-501">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="66130-501">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="66130-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-502">Boolean</span></span>|<span data-ttu-id="66130-503">Используется для отключения отображения области параметров семейства.</span><span class="sxs-lookup"><span data-stu-id="66130-503">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="66130-504">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="66130-504">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="66130-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-505">Boolean</span></span>|<span data-ttu-id="66130-506">Используется для отключения отображения области производительности и работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="66130-506">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="66130-507">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="66130-507">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="66130-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-508">Boolean</span></span>|<span data-ttu-id="66130-509">Используется для отключения отображения брандмауэра и области защиты сети.</span><span class="sxs-lookup"><span data-stu-id="66130-509">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="66130-510">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="66130-510">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="66130-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-511">Boolean</span></span>|<span data-ttu-id="66130-512">Используется для отключения отображения области защиты от вирусов и угроз.</span><span class="sxs-lookup"><span data-stu-id="66130-512">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="66130-513">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="66130-513">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="66130-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-514">Boolean</span></span>|<span data-ttu-id="66130-515">Используется для отключения отображения области защиты учетной записи.</span><span class="sxs-lookup"><span data-stu-id="66130-515">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="66130-516">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="66130-516">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="66130-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-517">Boolean</span></span>|<span data-ttu-id="66130-518">Используется для отключения отображения кнопки "Очистить TPM".</span><span class="sxs-lookup"><span data-stu-id="66130-518">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="66130-519">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="66130-519">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="66130-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-520">Boolean</span></span>|<span data-ttu-id="66130-521">Используется для отключения отображения области защиты оборудования.</span><span class="sxs-lookup"><span data-stu-id="66130-521">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="66130-522">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="66130-522">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="66130-523">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-523">Boolean</span></span>|<span data-ttu-id="66130-524">Используется для отключения отображения управления областью уведомлений.</span><span class="sxs-lookup"><span data-stu-id="66130-524">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="66130-525">Чтобы этот параметр вступил в силу, пользователю необходимо выйти и войти в нее или перезагрустить компьютер.</span><span class="sxs-lookup"><span data-stu-id="66130-525">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="66130-526">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="66130-526">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="66130-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-527">Boolean</span></span>|<span data-ttu-id="66130-528">Используется для отключения отображения области защиты от программ-вымогателей.</span><span class="sxs-lookup"><span data-stu-id="66130-528">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="66130-529">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="66130-529">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="66130-530">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-530">Boolean</span></span>|<span data-ttu-id="66130-531">Используется для отключения отображения безопасной области загрузки в режиме безопасности устройства.</span><span class="sxs-lookup"><span data-stu-id="66130-531">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="66130-532">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="66130-532">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="66130-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-533">Boolean</span></span>|<span data-ttu-id="66130-534">Используется для отключения отображения процесса устранения неполадок безопасности в области безопасности устройства.</span><span class="sxs-lookup"><span data-stu-id="66130-534">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="66130-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="66130-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="66130-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-536">Boolean</span></span>|<span data-ttu-id="66130-537">Используется для отключения отображения обновления микропрограммного обеспечения TPM при обнаружении уязвимого микропрограммного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="66130-537">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="66130-538">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="66130-538">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="66130-539">String</span><span class="sxs-lookup"><span data-stu-id="66130-539">String</span></span>|<span data-ttu-id="66130-540">Название компании, которое отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="66130-540">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="66130-541">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="66130-541">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="66130-542">String</span><span class="sxs-lookup"><span data-stu-id="66130-542">String</span></span>|<span data-ttu-id="66130-543">Адрес электронной почты, отображаемой для пользователей.</span><span class="sxs-lookup"><span data-stu-id="66130-543">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="66130-544">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="66130-544">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="66130-545">String</span><span class="sxs-lookup"><span data-stu-id="66130-545">String</span></span>|<span data-ttu-id="66130-546">Номер телефона или ИД Skype, отображаемого для пользователей.</span><span class="sxs-lookup"><span data-stu-id="66130-546">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="66130-547">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="66130-547">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="66130-548">String</span><span class="sxs-lookup"><span data-stu-id="66130-548">String</span></span>|<span data-ttu-id="66130-549">URL-адрес портала справки, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="66130-549">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="66130-550">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="66130-550">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="66130-551">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="66130-551">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="66130-552">Уведомления для отображения из отображаемой области приложения.</span><span class="sxs-lookup"><span data-stu-id="66130-552">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="66130-553">Возможные значения: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="66130-553">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="66130-554">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="66130-554">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="66130-555">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="66130-555">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="66130-556">Настройте, где будут отображаться контактные ИТ-данные для конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="66130-556">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="66130-557">Возможные значения: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="66130-557">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="66130-558">windowsDefenderTamperProtection</span><span class="sxs-lookup"><span data-stu-id="66130-558">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="66130-559">windowsDefenderTamperProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="66130-559">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="66130-560">Настройте параметры Защитника Windows TamperProtection.</span><span class="sxs-lookup"><span data-stu-id="66130-560">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="66130-561">Возможные значения: `notConfigured`, `enable`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="66130-561">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="66130-562">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="66130-562">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="66130-563">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-563">Boolean</span></span>|<span data-ttu-id="66130-564">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="66130-564">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="66130-565">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="66130-565">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="66130-566">Int32</span><span class="sxs-lookup"><span data-stu-id="66130-566">Int32</span></span>|<span data-ttu-id="66130-567">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="66130-567">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="66130-568">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="66130-568">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="66130-569">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="66130-569">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="66130-570">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="66130-570">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="66130-571">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="66130-571">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="66130-572">Выберите предварительную кодику ключа, которая будет использоваться.</span><span class="sxs-lookup"><span data-stu-id="66130-572">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="66130-573">Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="66130-573">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="66130-574">firewallIPSecExemptionsNone</span><span class="sxs-lookup"><span data-stu-id="66130-574">firewallIPSecExemptionsNone</span></span>|<span data-ttu-id="66130-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-575">Boolean</span></span>|<span data-ttu-id="66130-576">Настройка исключений IPSec без исключений</span><span class="sxs-lookup"><span data-stu-id="66130-576">Configures IPSec exemptions to no exemptions</span></span>|
|<span data-ttu-id="66130-577">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="66130-577">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="66130-578">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-578">Boolean</span></span>|<span data-ttu-id="66130-579">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="66130-579">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="66130-580">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="66130-580">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="66130-581">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-581">Boolean</span></span>|<span data-ttu-id="66130-582">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="66130-582">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="66130-583">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="66130-583">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="66130-584">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-584">Boolean</span></span>|<span data-ttu-id="66130-585">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="66130-585">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="66130-586">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="66130-586">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="66130-587">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-587">Boolean</span></span>|<span data-ttu-id="66130-588">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="66130-588">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="66130-589">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="66130-589">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="66130-590">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="66130-590">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="66130-591">Укажите, как будет применяться список отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="66130-591">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="66130-592">Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="66130-592">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="66130-593">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="66130-593">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="66130-594">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-594">Boolean</span></span>|<span data-ttu-id="66130-595">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="66130-595">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="66130-596">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="66130-596">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="66130-597">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="66130-597">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="66130-598">Настраивает реализации очередей пакетов в сценарии шлюза туннеля.</span><span class="sxs-lookup"><span data-stu-id="66130-598">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="66130-599">Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="66130-599">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="66130-600">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="66130-600">firewallProfileDomain</span></span>|[<span data-ttu-id="66130-601">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="66130-601">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="66130-602">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="66130-602">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="66130-603">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="66130-603">firewallProfilePublic</span></span>|[<span data-ttu-id="66130-604">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="66130-604">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="66130-605">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="66130-605">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="66130-606">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="66130-606">firewallProfilePrivate</span></span>|[<span data-ttu-id="66130-607">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="66130-607">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="66130-608">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="66130-608">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="66130-609">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="66130-609">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="66130-610">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-610">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="66130-611">Значение, указывающее поведение Adobe Reader при создании child processes.</span><span class="sxs-lookup"><span data-stu-id="66130-611">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="66130-612">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="66130-612">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="66130-613">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="66130-613">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="66130-614">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="66130-614">String collection</span></span>|<span data-ttu-id="66130-615">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="66130-615">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="66130-616">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="66130-616">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="66130-617">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="66130-617">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="66130-618">Значение, указывающее поведение приложений Office, внедряющихся в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="66130-618">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="66130-619">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="66130-619">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="66130-620">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="66130-620">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="66130-621">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-621">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="66130-622">Значение, указывающее поведение приложений Office, внедряющихся в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="66130-622">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="66130-623">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="66130-623">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="66130-624">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="66130-624">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="66130-625">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-625">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="66130-626">Значение, указывающее поведение приложений office для общения, включая Microsoft Outlook, от создания child processes.</span><span class="sxs-lookup"><span data-stu-id="66130-626">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="66130-627">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="66130-627">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="66130-628">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="66130-628">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="66130-629">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="66130-629">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="66130-630">Значение, указывающее поведение приложений и макроса Office, которые создают или запускают исполняемый контент.</span><span class="sxs-lookup"><span data-stu-id="66130-630">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="66130-631">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="66130-631">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="66130-632">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="66130-632">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="66130-633">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-633">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="66130-634">Значение, указывающее поведение приложений и макроса Office, которые создают или запускают исполняемый контент.</span><span class="sxs-lookup"><span data-stu-id="66130-634">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="66130-635">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="66130-635">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="66130-636">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="66130-636">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="66130-637">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="66130-637">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="66130-638">Значение, указывающее поведение приложения Office, запускающее child processes.</span><span class="sxs-lookup"><span data-stu-id="66130-638">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="66130-639">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="66130-639">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="66130-640">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="66130-640">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="66130-641">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-641">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="66130-642">Значение, указывающее поведение приложения Office, запускающее child processes.</span><span class="sxs-lookup"><span data-stu-id="66130-642">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="66130-643">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="66130-643">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="66130-644">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="66130-644">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="66130-645">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="66130-645">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="66130-646">Значение, указывающее поведение импорта Win32 из кода макроса в Office.</span><span class="sxs-lookup"><span data-stu-id="66130-646">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="66130-647">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="66130-647">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="66130-648">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="66130-648">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="66130-649">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-649">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="66130-650">Значение, указывающее поведение импорта Win32 из кода макроса в Office.</span><span class="sxs-lookup"><span data-stu-id="66130-650">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="66130-651">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="66130-651">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="66130-652">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="66130-652">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="66130-653">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="66130-653">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="66130-654">Значение, указывающее поведение запутываемого кода js/vbs/ps/macro.</span><span class="sxs-lookup"><span data-stu-id="66130-654">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="66130-655">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="66130-655">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="66130-656">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="66130-656">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="66130-657">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-657">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="66130-658">Значение, указывающее поведение запутываемого кода js/vbs/ps/macro.</span><span class="sxs-lookup"><span data-stu-id="66130-658">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="66130-659">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="66130-659">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="66130-660">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="66130-660">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="66130-661">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="66130-661">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="66130-662">Значение, указывающее поведение js/vbs, которые выполняют полезной нагрузки, скачанных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="66130-662">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="66130-663">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="66130-663">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="66130-664">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="66130-664">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="66130-665">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-665">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="66130-666">Значение, указывающее поведение js/vbs, которые выполняют полезной нагрузки, скачанных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="66130-666">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="66130-667">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="66130-667">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="66130-668">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="66130-668">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="66130-669">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-669">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="66130-670">Значение, указывающее, разрешен ли кража учетных данных из подсистемы локального органа безопасности Windows.</span><span class="sxs-lookup"><span data-stu-id="66130-670">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="66130-671">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="66130-671">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="66130-672">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="66130-672">defenderProcessCreationType</span></span>|[<span data-ttu-id="66130-673">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="66130-673">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="66130-674">Значение, указывающее ответ на создание процессов из команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="66130-674">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="66130-675">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="66130-675">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="66130-676">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="66130-676">defenderProcessCreation</span></span>|[<span data-ttu-id="66130-677">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-677">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="66130-678">Значение, указывающее ответ на создание процессов из команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="66130-678">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="66130-679">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="66130-679">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="66130-680">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="66130-680">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="66130-681">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="66130-681">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="66130-682">Значение, указывающее ответ на неподписаные и неподписаные процессы, которые запускают с USB.</span><span class="sxs-lookup"><span data-stu-id="66130-682">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="66130-683">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="66130-683">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="66130-684">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="66130-684">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="66130-685">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-685">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="66130-686">Значение, указывающее ответ на неподписаные и неподписаные процессы, которые запускают с USB.</span><span class="sxs-lookup"><span data-stu-id="66130-686">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="66130-687">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="66130-687">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="66130-688">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="66130-688">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="66130-689">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="66130-689">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="66130-690">Значение, указывающее ответ на исполняемые данные, которые не соответствуют критериям преобладаний, возраста или надежных списков.</span><span class="sxs-lookup"><span data-stu-id="66130-690">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="66130-691">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="66130-691">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="66130-692">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="66130-692">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="66130-693">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-693">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="66130-694">Значение, указывающее ответ на исполняемые данные, которые не соответствуют критериям преобладаний, возраста или надежных списков.</span><span class="sxs-lookup"><span data-stu-id="66130-694">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="66130-695">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="66130-695">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="66130-696">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="66130-696">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="66130-697">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="66130-697">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="66130-698">Значение, указывающее, следует ли отослать выполнение исполняемого содержимого (exe, dll, ps, js, vbs и т. д.) из электронной почты (webmail/mail-client).</span><span class="sxs-lookup"><span data-stu-id="66130-698">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="66130-699">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="66130-699">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="66130-700">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="66130-700">defenderEmailContentExecution</span></span>|[<span data-ttu-id="66130-701">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-701">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="66130-702">Значение, указывающее, следует ли отослать выполнение исполняемого содержимого (exe, dll, ps, js, vbs и т. д.) из электронной почты (webmail/mail-client).</span><span class="sxs-lookup"><span data-stu-id="66130-702">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="66130-703">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="66130-703">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="66130-704">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-704">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="66130-705">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-705">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="66130-706">Значение, указывающее использование advanced protection для защиты от программ-вымогателей.</span><span class="sxs-lookup"><span data-stu-id="66130-706">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="66130-707">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="66130-707">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="66130-708">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="66130-708">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="66130-709">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-709">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="66130-710">Значение, указывающее поведение защищенных папок.</span><span class="sxs-lookup"><span data-stu-id="66130-710">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="66130-711">Возможные значения: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="66130-711">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="66130-712">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="66130-712">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="66130-713">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="66130-713">String collection</span></span>|<span data-ttu-id="66130-714">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="66130-714">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="66130-715">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="66130-715">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="66130-716">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="66130-716">String collection</span></span>|<span data-ttu-id="66130-717">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="66130-717">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="66130-718">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-718">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="66130-719">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-719">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="66130-720">Значение, указывающее поведение NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="66130-720">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="66130-721">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="66130-721">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="66130-722">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="66130-722">defenderExploitProtectionXml</span></span>|<span data-ttu-id="66130-723">Binary</span><span class="sxs-lookup"><span data-stu-id="66130-723">Binary</span></span>|<span data-ttu-id="66130-724">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="66130-724">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="66130-725">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="66130-725">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="66130-726">String</span><span class="sxs-lookup"><span data-stu-id="66130-726">String</span></span>|<span data-ttu-id="66130-727">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="66130-727">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="66130-728">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="66130-728">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="66130-729">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-729">Boolean</span></span>|<span data-ttu-id="66130-730">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="66130-730">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="66130-731">defenderBlockPersistenceThroughWmiType</span><span class="sxs-lookup"><span data-stu-id="66130-731">defenderBlockPersistenceThroughWmiType</span></span>|[<span data-ttu-id="66130-732">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="66130-732">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="66130-733">Значение, указывающее поведение сохраняемости блокировки через подписку на события WMI.</span><span class="sxs-lookup"><span data-stu-id="66130-733">Value indicating the behavior of Block persistence through WMI event subscription.</span></span> <span data-ttu-id="66130-734">Возможные значения: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="66130-734">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="66130-735">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="66130-735">appLockerApplicationControl</span></span>|[<span data-ttu-id="66130-736">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="66130-736">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="66130-737">Позволяет администратору выбирать разрешенные типы приложений для устройств.</span><span class="sxs-lookup"><span data-stu-id="66130-737">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="66130-738">Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="66130-738">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="66130-739">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="66130-739">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="66130-740">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="66130-740">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="66130-741">Включите Credential Guard, если включен уровень безопасности платформы с безопасной загрузкой и безопасностью на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="66130-741">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="66130-742">Возможные значения: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="66130-742">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`, `disable`.</span></span>|
|<span data-ttu-id="66130-743">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="66130-743">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="66130-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-744">Boolean</span></span>|<span data-ttu-id="66130-745">Включает безопасность на основе виртуализации (VBS).</span><span class="sxs-lookup"><span data-stu-id="66130-745">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="66130-746">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="66130-746">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="66130-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-747">Boolean</span></span>|<span data-ttu-id="66130-748">Это свойство будет заменено свойством DeviceGuardSecureBootWithDMA в мае 2019 г.</span><span class="sxs-lookup"><span data-stu-id="66130-748">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="66130-749">Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="66130-749">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="66130-750">deviceGuardSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="66130-750">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="66130-751">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="66130-751">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="66130-752">Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="66130-752">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="66130-753">Возможные значения: `notConfigured`, `withoutDMA`, `withDMA`.</span><span class="sxs-lookup"><span data-stu-id="66130-753">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="66130-754">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="66130-754">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="66130-755">enablement</span><span class="sxs-lookup"><span data-stu-id="66130-755">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="66130-756">Позволяет ИТ-администратору настроить запуск System Guard.</span><span class="sxs-lookup"><span data-stu-id="66130-756">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="66130-757">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="66130-757">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="66130-758">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="66130-758">smartScreenEnableInShell</span></span>|<span data-ttu-id="66130-759">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-759">Boolean</span></span>|<span data-ttu-id="66130-760">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="66130-760">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="66130-761">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="66130-761">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="66130-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-762">Boolean</span></span>|<span data-ttu-id="66130-763">Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="66130-763">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="66130-764">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="66130-764">applicationGuardEnabled</span></span>|<span data-ttu-id="66130-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-765">Boolean</span></span>|<span data-ttu-id="66130-766">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="66130-766">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="66130-767">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="66130-767">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="66130-768">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="66130-768">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="66130-769">В Защитник Windows Application Guard для более новых сборков Windows.</span><span class="sxs-lookup"><span data-stu-id="66130-769">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="66130-770">Возможные значения: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="66130-770">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="66130-771">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="66130-771">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="66130-772">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="66130-772">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="66130-773">Блокировка буфера обмена для передачи файла изображения, текстового файла или ни одного из них.</span><span class="sxs-lookup"><span data-stu-id="66130-773">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="66130-774">Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="66130-774">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="66130-775">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="66130-775">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="66130-776">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-776">Boolean</span></span>|<span data-ttu-id="66130-777">Позволяет заблокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="66130-777">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="66130-778">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="66130-778">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="66130-779">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-779">Boolean</span></span>|<span data-ttu-id="66130-780">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="66130-780">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="66130-781">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="66130-781">applicationGuardForceAuditing</span></span>|<span data-ttu-id="66130-782">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-782">Boolean</span></span>|<span data-ttu-id="66130-783">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="66130-783">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="66130-784">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="66130-784">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="66130-785">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="66130-785">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="66130-786">Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="66130-786">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="66130-787">Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="66130-787">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="66130-788">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="66130-788">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="66130-789">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-789">Boolean</span></span>|<span data-ttu-id="66130-790">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="66130-790">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="66130-791">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="66130-791">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="66130-792">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-792">Boolean</span></span>|<span data-ttu-id="66130-793">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="66130-793">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="66130-794">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="66130-794">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="66130-795">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-795">Boolean</span></span>|<span data-ttu-id="66130-796">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="66130-796">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="66130-797">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="66130-797">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="66130-798">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-798">Boolean</span></span>|<span data-ttu-id="66130-799">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="66130-799">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="66130-800">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="66130-800">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="66130-801">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-801">Boolean</span></span>|<span data-ttu-id="66130-802">Разрешить Application Guard использовать виртуальный GPU</span><span class="sxs-lookup"><span data-stu-id="66130-802">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="66130-803">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="66130-803">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="66130-804">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-804">Boolean</span></span>|<span data-ttu-id="66130-805">Разрешить пользователям скачивать файлы из Edge в контейнере Application Guard и сохранять их в файловой системе ведущего приложения</span><span class="sxs-lookup"><span data-stu-id="66130-805">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="66130-806">applicationGuardAllowCameraMicrophoneRedirection</span><span class="sxs-lookup"><span data-stu-id="66130-806">applicationGuardAllowCameraMicrophoneRedirection</span></span>|<span data-ttu-id="66130-807">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-807">Boolean</span></span>|<span data-ttu-id="66130-808">Получает или задает, могут ли приложения в Application Guard в Microsoft Defender получать доступ к камере и микрофону устройства.</span><span class="sxs-lookup"><span data-stu-id="66130-808">Gets or sets whether applications inside Microsoft Defender Application Guard can access the device’s camera and microphone.</span></span>|
|<span data-ttu-id="66130-809">applicationGuardCertificateThumbprints</span><span class="sxs-lookup"><span data-stu-id="66130-809">applicationGuardCertificateThumbprints</span></span>|<span data-ttu-id="66130-810">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="66130-810">String collection</span></span>|<span data-ttu-id="66130-811">Позволяет использовать определенные корневые сертификаты уровня устройства в контейнере Application Guard в Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="66130-811">Allows certain device level Root Certificates to be shared with the Microsoft Defender Application Guard container.</span></span>|
|<span data-ttu-id="66130-812">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="66130-812">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="66130-813">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-813">Boolean</span></span>|<span data-ttu-id="66130-814">Позволяет администратору разрешить стандартным пользователям включить encrpytion во время присоединить Azure AD.</span><span class="sxs-lookup"><span data-stu-id="66130-814">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="66130-815">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="66130-815">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="66130-816">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-816">Boolean</span></span>|<span data-ttu-id="66130-817">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="66130-817">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="66130-818">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="66130-818">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="66130-819">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-819">Boolean</span></span>|<span data-ttu-id="66130-820">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="66130-820">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="66130-821">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="66130-821">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="66130-822">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="66130-822">bitLockerEncryptDevice</span></span>|<span data-ttu-id="66130-823">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-823">Boolean</span></span>|<span data-ttu-id="66130-824">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="66130-824">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="66130-825">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="66130-825">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="66130-826">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="66130-826">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="66130-827">Политика системного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="66130-827">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="66130-828">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="66130-828">bitLockerFixedDrivePolicy</span></span>|<span data-ttu-id="66130-829">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md);</span><span class="sxs-lookup"><span data-stu-id="66130-829">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)</span></span>|<span data-ttu-id="66130-830">Политика фиксированного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="66130-830">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="66130-831">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="66130-831">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="66130-832">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="66130-832">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="66130-833">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="66130-833">BitLocker Removable Drive Policy.</span></span>|
|<span data-ttu-id="66130-834">bitLockerRecoveryPasswordRotation</span><span class="sxs-lookup"><span data-stu-id="66130-834">bitLockerRecoveryPasswordRotation</span></span>|[<span data-ttu-id="66130-835">bitLockerRecoveryPasswordRotationType</span><span class="sxs-lookup"><span data-stu-id="66130-835">bitLockerRecoveryPasswordRotationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|<span data-ttu-id="66130-836">Этот параметр инициирует ротацию паролей восстановления на основе клиента после восстановления диска ОС (с помощью bootmgr или WinRE).</span><span class="sxs-lookup"><span data-stu-id="66130-836">This setting initiates a client-driven recovery password rotation after an OS drive recovery (either by using bootmgr or WinRE).</span></span> <span data-ttu-id="66130-837">Возможные значения: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span><span class="sxs-lookup"><span data-stu-id="66130-837">Possible values are: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span></span>|
|<span data-ttu-id="66130-838">defenderDisableScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="66130-838">defenderDisableScanArchiveFiles</span></span>|<span data-ttu-id="66130-839">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-839">Boolean</span></span>|<span data-ttu-id="66130-840">Разрешает или не разрешает сканирование архивов.</span><span class="sxs-lookup"><span data-stu-id="66130-840">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="66130-841">defenderAllowScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="66130-841">defenderAllowScanArchiveFiles</span></span>|<span data-ttu-id="66130-842">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-842">Boolean</span></span>|<span data-ttu-id="66130-843">Разрешает или не разрешает сканирование архивов.</span><span class="sxs-lookup"><span data-stu-id="66130-843">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="66130-844">defenderDisableBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="66130-844">defenderDisableBehaviorMonitoring</span></span>|<span data-ttu-id="66130-845">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-845">Boolean</span></span>|<span data-ttu-id="66130-846">Разрешает или не разрешает использовать Защитник Windows мониторинга поведения.</span><span class="sxs-lookup"><span data-stu-id="66130-846">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="66130-847">defenderAllowBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="66130-847">defenderAllowBehaviorMonitoring</span></span>|<span data-ttu-id="66130-848">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-848">Boolean</span></span>|<span data-ttu-id="66130-849">Разрешает или не разрешает использовать Защитник Windows мониторинга поведения.</span><span class="sxs-lookup"><span data-stu-id="66130-849">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="66130-850">defenderDisableCloudProtection</span><span class="sxs-lookup"><span data-stu-id="66130-850">defenderDisableCloudProtection</span></span>|<span data-ttu-id="66130-851">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-851">Boolean</span></span>|<span data-ttu-id="66130-852">Чтобы наилучшим образом защитить компьютер, Защитник Windows отправляет корпорации Майкрософт сведения о любых проблемах, которые она находит.</span><span class="sxs-lookup"><span data-stu-id="66130-852">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="66130-853">Корпорация Майкрософт проанализирует эту информацию, узнайте больше о проблемах, влияющих на вас и других клиентов, и предложит улучшенные решения.</span><span class="sxs-lookup"><span data-stu-id="66130-853">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="66130-854">defenderAllowCloudProtection</span><span class="sxs-lookup"><span data-stu-id="66130-854">defenderAllowCloudProtection</span></span>|<span data-ttu-id="66130-855">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-855">Boolean</span></span>|<span data-ttu-id="66130-856">Чтобы наилучшим образом защитить компьютер, Защитник Windows отправляет корпорации Майкрософт сведения о любых проблемах, которые она находит.</span><span class="sxs-lookup"><span data-stu-id="66130-856">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="66130-857">Корпорация Майкрософт проанализирует эту информацию, узнайте больше о проблемах, влияющих на вас и других клиентов, и предложит улучшенные решения.</span><span class="sxs-lookup"><span data-stu-id="66130-857">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="66130-858">defenderEnableScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="66130-858">defenderEnableScanIncomingMail</span></span>|<span data-ttu-id="66130-859">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-859">Boolean</span></span>|<span data-ttu-id="66130-860">Разрешает или не разрешает сканирование электронной почты.</span><span class="sxs-lookup"><span data-stu-id="66130-860">Allows or disallows scanning of email.</span></span>|
|<span data-ttu-id="66130-861">defenderEnableScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="66130-861">defenderEnableScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="66130-862">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-862">Boolean</span></span>|<span data-ttu-id="66130-863">Разрешает или не разрешает полную проверку сетевых дисков.</span><span class="sxs-lookup"><span data-stu-id="66130-863">Allows or disallows a full scan of mapped network drives.</span></span>|
|<span data-ttu-id="66130-864">defenderDisableScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="66130-864">defenderDisableScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="66130-865">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-865">Boolean</span></span>|<span data-ttu-id="66130-866">Разрешает или не разрешает полную проверку съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="66130-866">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="66130-867">Во время быстрой проверки съемные диски могут по-прежнему проверяться.</span><span class="sxs-lookup"><span data-stu-id="66130-867">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="66130-868">defenderAllowScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="66130-868">defenderAllowScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="66130-869">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-869">Boolean</span></span>|<span data-ttu-id="66130-870">Разрешает или не разрешает полную проверку съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="66130-870">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="66130-871">Во время быстрой проверки съемные диски могут по-прежнему проверяться.</span><span class="sxs-lookup"><span data-stu-id="66130-871">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="66130-872">defenderDisableScanDownloads</span><span class="sxs-lookup"><span data-stu-id="66130-872">defenderDisableScanDownloads</span></span>|<span data-ttu-id="66130-873">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-873">Boolean</span></span>|<span data-ttu-id="66130-874">Разрешает или не разрешает использовать Защитник Windows защиты IOAVP.</span><span class="sxs-lookup"><span data-stu-id="66130-874">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="66130-875">defenderAllowScanDownloads</span><span class="sxs-lookup"><span data-stu-id="66130-875">defenderAllowScanDownloads</span></span>|<span data-ttu-id="66130-876">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-876">Boolean</span></span>|<span data-ttu-id="66130-877">Разрешает или не разрешает использовать Защитник Windows защиты IOAVP.</span><span class="sxs-lookup"><span data-stu-id="66130-877">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="66130-878">defenderDisableIntrusionPreventionSystem</span><span class="sxs-lookup"><span data-stu-id="66130-878">defenderDisableIntrusionPreventionSystem</span></span>|<span data-ttu-id="66130-879">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-879">Boolean</span></span>|<span data-ttu-id="66130-880">Разрешает или не разрешает использовать Защитник Windows предотвращения вторжений.</span><span class="sxs-lookup"><span data-stu-id="66130-880">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="66130-881">defenderAllowIntrusionPreventionSystem</span><span class="sxs-lookup"><span data-stu-id="66130-881">defenderAllowIntrusionPreventionSystem</span></span>|<span data-ttu-id="66130-882">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-882">Boolean</span></span>|<span data-ttu-id="66130-883">Разрешает или не разрешает использовать Защитник Windows предотвращения вторжений.</span><span class="sxs-lookup"><span data-stu-id="66130-883">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="66130-884">defenderDisableOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="66130-884">defenderDisableOnAccessProtection</span></span>|<span data-ttu-id="66130-885">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-885">Boolean</span></span>|<span data-ttu-id="66130-886">Разрешает или Защитник Windows функции Защиты доступа.</span><span class="sxs-lookup"><span data-stu-id="66130-886">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="66130-887">defenderAllowOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="66130-887">defenderAllowOnAccessProtection</span></span>|<span data-ttu-id="66130-888">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-888">Boolean</span></span>|<span data-ttu-id="66130-889">Разрешает или Защитник Windows функции Защиты доступа.</span><span class="sxs-lookup"><span data-stu-id="66130-889">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="66130-890">defenderDisableRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="66130-890">defenderDisableRealTimeMonitoring</span></span>|<span data-ttu-id="66130-891">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-891">Boolean</span></span>|<span data-ttu-id="66130-892">Разрешает или не разрешает использовать Защитник Windows мониторинга в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="66130-892">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="66130-893">defenderAllowRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="66130-893">defenderAllowRealTimeMonitoring</span></span>|<span data-ttu-id="66130-894">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-894">Boolean</span></span>|<span data-ttu-id="66130-895">Разрешает или не разрешает использовать Защитник Windows мониторинга в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="66130-895">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="66130-896">defenderDisableScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="66130-896">defenderDisableScanNetworkFiles</span></span>|<span data-ttu-id="66130-897">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-897">Boolean</span></span>|<span data-ttu-id="66130-898">Разрешает или не разрешает сканирование сетевых файлов.</span><span class="sxs-lookup"><span data-stu-id="66130-898">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="66130-899">defenderAllowScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="66130-899">defenderAllowScanNetworkFiles</span></span>|<span data-ttu-id="66130-900">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-900">Boolean</span></span>|<span data-ttu-id="66130-901">Разрешает или не разрешает сканирование сетевых файлов.</span><span class="sxs-lookup"><span data-stu-id="66130-901">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="66130-902">defenderDisableScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="66130-902">defenderDisableScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="66130-903">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-903">Boolean</span></span>|<span data-ttu-id="66130-904">Разрешает или не разрешает использовать Защитник Windows проверки скриптов.</span><span class="sxs-lookup"><span data-stu-id="66130-904">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="66130-905">defenderAllowScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="66130-905">defenderAllowScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="66130-906">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-906">Boolean</span></span>|<span data-ttu-id="66130-907">Разрешает или не разрешает использовать Защитник Windows проверки скриптов.</span><span class="sxs-lookup"><span data-stu-id="66130-907">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="66130-908">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="66130-908">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="66130-909">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-909">Boolean</span></span>|<span data-ttu-id="66130-910">Разрешает или не разрешает пользователю доступ к Защитник Windows пользовательскому интерфейсу.</span><span class="sxs-lookup"><span data-stu-id="66130-910">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="66130-911">Если это не так, все Защитник Windows уведомления также будут подавляться.</span><span class="sxs-lookup"><span data-stu-id="66130-911">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="66130-912">defenderAllowEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="66130-912">defenderAllowEndUserAccess</span></span>|<span data-ttu-id="66130-913">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-913">Boolean</span></span>|<span data-ttu-id="66130-914">Разрешает или не разрешает пользователю доступ к Защитник Windows пользовательскому интерфейсу.</span><span class="sxs-lookup"><span data-stu-id="66130-914">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="66130-915">Если это не так, все Защитник Windows уведомления также будут подавляться.</span><span class="sxs-lookup"><span data-stu-id="66130-915">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="66130-916">defenderScanMaxCpuPercentage</span><span class="sxs-lookup"><span data-stu-id="66130-916">defenderScanMaxCpuPercentage</span></span>|<span data-ttu-id="66130-917">Int32</span><span class="sxs-lookup"><span data-stu-id="66130-917">Int32</span></span>|<span data-ttu-id="66130-918">Представляет средний коэффициент загрузки ЦП для Защитник Windows проверки (в процентах).</span><span class="sxs-lookup"><span data-stu-id="66130-918">Represents the average CPU load factor for the Windows Defender scan (in percent).</span></span> <span data-ttu-id="66130-919">Значение по умолчанию равно 50.</span><span class="sxs-lookup"><span data-stu-id="66130-919">The default value is 50.</span></span> <span data-ttu-id="66130-920">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="66130-920">Valid values 0 to 100</span></span>|
|<span data-ttu-id="66130-921">defenderCheckForSignaturesBeforeRunningScan</span><span class="sxs-lookup"><span data-stu-id="66130-921">defenderCheckForSignaturesBeforeRunningScan</span></span>|<span data-ttu-id="66130-922">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-922">Boolean</span></span>|<span data-ttu-id="66130-923">Этот параметр политики позволяет управлять проверкой новых определений вирусов и программ-шпионов перед запуском проверки.</span><span class="sxs-lookup"><span data-stu-id="66130-923">This policy setting allows you to manage whether a check for new virus and spyware definitions will occur before running a scan.</span></span>|
|<span data-ttu-id="66130-924">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="66130-924">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="66130-925">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="66130-925">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="66130-926">Добавлено в Windows 10 версии 1709.</span><span class="sxs-lookup"><span data-stu-id="66130-926">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="66130-927">Этот параметр политики определяет, насколько Защитник Windows антивирусная программа будет блокировать и сканировать подозрительные файлы.</span><span class="sxs-lookup"><span data-stu-id="66130-927">This policy setting determines how aggressive Windows Defender Antivirus will be in blocking and scanning suspicious files.</span></span> <span data-ttu-id="66130-928">Тип значения — integer.</span><span class="sxs-lookup"><span data-stu-id="66130-928">Value type is integer.</span></span> <span data-ttu-id="66130-929">Для работы этой функции необходимо включить параметр "Присоединиться к Microsoft MAPS".</span><span class="sxs-lookup"><span data-stu-id="66130-929">This feature requires the "Join Microsoft MAPS" setting enabled in order to function.</span></span> <span data-ttu-id="66130-930">Возможные значения: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span><span class="sxs-lookup"><span data-stu-id="66130-930">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="66130-931">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="66130-931">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="66130-932">Int32</span><span class="sxs-lookup"><span data-stu-id="66130-932">Int32</span></span>|<span data-ttu-id="66130-933">Добавлено в Windows 10 версии 1709.</span><span class="sxs-lookup"><span data-stu-id="66130-933">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="66130-934">Эта функция позволяет Защитник Windows антивирусной программы блокировать подозрительный файл на срок до 60 секунд и сканировать его в облаке, чтобы убедиться в безопасности.</span><span class="sxs-lookup"><span data-stu-id="66130-934">This feature allows Windows Defender Antivirus to block a suspicious file for up to 60 seconds, and scan it in the cloud to make sure it's safe.</span></span> <span data-ttu-id="66130-935">Тип значения — целый, диапазон — от 0 до 50.</span><span class="sxs-lookup"><span data-stu-id="66130-935">Value type is integer, range is 0 - 50.</span></span> <span data-ttu-id="66130-936">Эта функция зависит от трех других параметров MAPS, которые должны быть включены: "Настройка функции "Блокировка при первом взгляда"; " Присоединяйтесь к Microsoft MAPS"; "Отправлять образцы файлов, если требуется дальнейший анализ".</span><span class="sxs-lookup"><span data-stu-id="66130-936">This feature depends on three other MAPS settings the must all be enabled- "Configure the 'Block at First Sight' feature; "Join Microsoft MAPS"; "Send file samples when further analysis is required".</span></span> <span data-ttu-id="66130-937">Допустимые значения: от 0 до 50.</span><span class="sxs-lookup"><span data-stu-id="66130-937">Valid values 0 to 50</span></span>|
|<span data-ttu-id="66130-938">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="66130-938">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="66130-939">Int32</span><span class="sxs-lookup"><span data-stu-id="66130-939">Int32</span></span>|<span data-ttu-id="66130-940">Период времени (в днях), в течение который элементы карантина будут храниться в системе.</span><span class="sxs-lookup"><span data-stu-id="66130-940">Time period (in days) that quarantine items will be stored on the system.</span></span> <span data-ttu-id="66130-941">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="66130-941">Valid values 0 to 90</span></span>|
|<span data-ttu-id="66130-942">defenderDisableCatchupFullScan</span><span class="sxs-lookup"><span data-stu-id="66130-942">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="66130-943">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-943">Boolean</span></span>|<span data-ttu-id="66130-944">Этот параметр политики позволяет настроить более полные запланированные проверки.</span><span class="sxs-lookup"><span data-stu-id="66130-944">This policy setting allows you to configure catch-up scans for scheduled full scans.</span></span> <span data-ttu-id="66130-945">Перевертывка — это сканирование, которое инициалось из-за пропущенной регулярно запланированной проверки.</span><span class="sxs-lookup"><span data-stu-id="66130-945">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="66130-946">Обычно эти запланированные проверки пропускаются, так как компьютер был отключен в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="66130-946">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="66130-947">defenderDisableCatchupQuickScan</span><span class="sxs-lookup"><span data-stu-id="66130-947">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="66130-948">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-948">Boolean</span></span>|<span data-ttu-id="66130-949">Этот параметр политики позволяет настраивать сканирование для запланированных быстрых сканирований.</span><span class="sxs-lookup"><span data-stu-id="66130-949">This policy setting allows you to configure catch-up scans for scheduled quick scans.</span></span> <span data-ttu-id="66130-950">Перевертывка — это сканирование, которое инициалось из-за пропущенной регулярно запланированной проверки.</span><span class="sxs-lookup"><span data-stu-id="66130-950">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="66130-951">Обычно эти запланированные проверки пропускаются, так как компьютер был отключен в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="66130-951">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="66130-952">defenderEnableLowCpuPriority</span><span class="sxs-lookup"><span data-stu-id="66130-952">defenderEnableLowCpuPriority</span></span>|<span data-ttu-id="66130-953">Boolean</span><span class="sxs-lookup"><span data-stu-id="66130-953">Boolean</span></span>|<span data-ttu-id="66130-954">Этот параметр политики позволяет включить или отключить низкий приоритет ЦП для запланированных сканирований.</span><span class="sxs-lookup"><span data-stu-id="66130-954">This policy setting allows you to enable or disable low CPU priority for scheduled scans.</span></span>|
|<span data-ttu-id="66130-955">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="66130-955">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="66130-956">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="66130-956">String collection</span></span>|<span data-ttu-id="66130-957">Расширения файлов, которые необходимо исключить из проверки и защиты в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="66130-957">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="66130-958">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="66130-958">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="66130-959">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="66130-959">String collection</span></span>|<span data-ttu-id="66130-960">Файлы и папки, которые необходимо исключить из проверки и защиты в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="66130-960">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="66130-961">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="66130-961">defenderProcessesToExclude</span></span>|<span data-ttu-id="66130-962">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="66130-962">String collection</span></span>|<span data-ttu-id="66130-963">Процессы, которые необходимо исключить из проверки и защиты в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="66130-963">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="66130-964">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="66130-964">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="66130-965">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="66130-965">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="66130-966">Добавлено в Windows 10 версии 1607.</span><span class="sxs-lookup"><span data-stu-id="66130-966">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="66130-967">Определяет уровень обнаружения потенциально нежелательных приложений (PUA).</span><span class="sxs-lookup"><span data-stu-id="66130-967">Specifies the level of detection for potentially unwanted applications (PUAs).</span></span> <span data-ttu-id="66130-968">Защитник Windows оповещает о загрузке потенциально нежелательного программного обеспечения или попытке установить себя на компьютере.</span><span class="sxs-lookup"><span data-stu-id="66130-968">Windows Defender alerts you when potentially unwanted software is being downloaded or attempts to install itself on your computer.</span></span> <span data-ttu-id="66130-969">Возможные значения: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="66130-969">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="66130-970">defenderScanDirection</span><span class="sxs-lookup"><span data-stu-id="66130-970">defenderScanDirection</span></span>|[<span data-ttu-id="66130-971">defenderRealtimeScanDirection</span><span class="sxs-lookup"><span data-stu-id="66130-971">defenderRealtimeScanDirection</span></span>](../resources/intune-deviceconfig-defenderrealtimescandirection.md)|<span data-ttu-id="66130-972">Определяет, какие наборы файлов следует отслеживать.</span><span class="sxs-lookup"><span data-stu-id="66130-972">Controls which sets of files should be monitored.</span></span> <span data-ttu-id="66130-973">Возможные значения: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span><span class="sxs-lookup"><span data-stu-id="66130-973">Possible values are: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="66130-974">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="66130-974">defenderScanType</span></span>|[<span data-ttu-id="66130-975">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="66130-975">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="66130-976">Выбирает, следует ли выполнять быструю или полную проверку.</span><span class="sxs-lookup"><span data-stu-id="66130-976">Selects whether to perform a quick scan or full scan.</span></span> <span data-ttu-id="66130-977">Возможные значения: `userDefined`, `disabled`, `quick`, `full`.</span><span class="sxs-lookup"><span data-stu-id="66130-977">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="66130-978">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="66130-978">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="66130-979">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="66130-979">TimeOfDay</span></span>|<span data-ttu-id="66130-980">Выбирает время дня, в которое должна Защитник Windows быстрая проверка.</span><span class="sxs-lookup"><span data-stu-id="66130-980">Selects the time of day that the Windows Defender quick scan should run.</span></span> <span data-ttu-id="66130-981">Например, значение 0=12:00AM, значение 60=1:00AM, значение 120=2:00 и так далее до значения 1380=11:00PM.</span><span class="sxs-lookup"><span data-stu-id="66130-981">For example, a value of 0=12:00AM, a value of 60=1:00AM, a value of 120=2:00, and so on, up to a value of 1380=11:00PM.</span></span> <span data-ttu-id="66130-982">Значение по умолчанию — 120.</span><span class="sxs-lookup"><span data-stu-id="66130-982">The default value is 120</span></span>|
|<span data-ttu-id="66130-983">defenderScheduledScanDay</span><span class="sxs-lookup"><span data-stu-id="66130-983">defenderScheduledScanDay</span></span>|[<span data-ttu-id="66130-984">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="66130-984">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="66130-985">Выбирает день запуска Защитник Windows проверки.</span><span class="sxs-lookup"><span data-stu-id="66130-985">Selects the day that the Windows Defender scan should run.</span></span> <span data-ttu-id="66130-986">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="66130-986">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="66130-987">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="66130-987">defenderScheduledScanTime</span></span>|<span data-ttu-id="66130-988">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="66130-988">TimeOfDay</span></span>|<span data-ttu-id="66130-989">Выбирает время дня, в течение Защитник Windows проверки.</span><span class="sxs-lookup"><span data-stu-id="66130-989">Selects the time of day that the Windows Defender scan should run.</span></span>|
|<span data-ttu-id="66130-990">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="66130-990">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="66130-991">Int32</span><span class="sxs-lookup"><span data-stu-id="66130-991">Int32</span></span>|<span data-ttu-id="66130-992">Указывает интервал (в часах), который будет использоваться для проверки подписей, поэтому вместо ScheduleDay и ScheduleTime проверка новых подписей будет устанавливаться в соответствии с интервалом.</span><span class="sxs-lookup"><span data-stu-id="66130-992">Specifies the interval (in hours) that will be used to check for signatures, so instead of using the ScheduleDay and ScheduleTime the check for new signatures will be set according to the interval.</span></span> <span data-ttu-id="66130-993">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="66130-993">Valid values 0 to 24</span></span>|
|<span data-ttu-id="66130-994">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="66130-994">defenderSubmitSamplesConsentType</span></span>|<span data-ttu-id="66130-995">[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md);</span><span class="sxs-lookup"><span data-stu-id="66130-995">[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)</span></span>|<span data-ttu-id="66130-996">Проверяет уровень согласия пользователя в Защитник Windows отправки данных.</span><span class="sxs-lookup"><span data-stu-id="66130-996">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="66130-997">Возможные значения: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span><span class="sxs-lookup"><span data-stu-id="66130-997">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="66130-998">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="66130-998">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="66130-999">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="66130-999">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="66130-1000">Позволяет администратору указать допустимые уровни серьезности угроз и соответствующий ид действия по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="66130-1000">Allows an administrator to specify any valid threat severity levels and the corresponding default action ID to take.</span></span>|



## <a name="response"></a><span data-ttu-id="66130-1001">Отклик</span><span class="sxs-lookup"><span data-stu-id="66130-1001">Response</span></span>
<span data-ttu-id="66130-1002">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="66130-1002">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66130-1003">Пример</span><span class="sxs-lookup"><span data-stu-id="66130-1003">Example</span></span>

### <a name="request"></a><span data-ttu-id="66130-1004">Запрос</span><span class="sxs-lookup"><span data-stu-id="66130-1004">Request</span></span>
<span data-ttu-id="66130-1005">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66130-1005">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="66130-1006">Отклик</span><span class="sxs-lookup"><span data-stu-id="66130-1006">Response</span></span>
<span data-ttu-id="66130-p226">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66130-p226">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




