---
title: Обновление объекта windows10EndpointProtectionConfiguration
description: Обновляет свойства объекта windows10EndpointProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9594362998b5c13e2f38fcd1ca6043cf10fd80cd
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620327"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="4a64d-103">Обновление объекта windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="4a64d-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="4a64d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a64d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a64d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a64d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a64d-106">Обновляет свойства объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a64d-106">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a64d-107">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="4a64d-107">Prerequisites</span></span>
<span data-ttu-id="4a64d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a64d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a64d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a64d-110">Permission type</span></span>|<span data-ttu-id="4a64d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a64d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a64d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a64d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4a64d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a64d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a64d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a64d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a64d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a64d-115">Not supported.</span></span>|
|<span data-ttu-id="4a64d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a64d-116">Application</span></span>|<span data-ttu-id="4a64d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a64d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a64d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a64d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4a64d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a64d-119">Request headers</span></span>
|<span data-ttu-id="4a64d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a64d-120">Header</span></span>|<span data-ttu-id="4a64d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4a64d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a64d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a64d-122">Authorization</span></span>|<span data-ttu-id="4a64d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a64d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a64d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4a64d-124">Accept</span></span>|<span data-ttu-id="4a64d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4a64d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a64d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4a64d-126">Request body</span></span>
<span data-ttu-id="4a64d-127">В теле запроса добавьте представление объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a64d-127">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="4a64d-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a64d-128">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="4a64d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a64d-129">Property</span></span>|<span data-ttu-id="4a64d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4a64d-130">Type</span></span>|<span data-ttu-id="4a64d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4a64d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a64d-132">id</span><span class="sxs-lookup"><span data-stu-id="4a64d-132">id</span></span>|<span data-ttu-id="4a64d-133">String</span><span class="sxs-lookup"><span data-stu-id="4a64d-133">String</span></span>|<span data-ttu-id="4a64d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4a64d-134">Key of the entity.</span></span> <span data-ttu-id="4a64d-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a64d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a64d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a64d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4a64d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a64d-137">DateTimeOffset</span></span>|<span data-ttu-id="4a64d-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4a64d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4a64d-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a64d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a64d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4a64d-140">roleScopeTagIds</span></span>|<span data-ttu-id="4a64d-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4a64d-141">String collection</span></span>|<span data-ttu-id="4a64d-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4a64d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4a64d-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a64d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a64d-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4a64d-144">supportsScopeTags</span></span>|<span data-ttu-id="4a64d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-145">Boolean</span></span>|<span data-ttu-id="4a64d-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4a64d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4a64d-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4a64d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4a64d-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4a64d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4a64d-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a64d-149">This property is read-only.</span></span> <span data-ttu-id="4a64d-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a64d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a64d-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4a64d-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4a64d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4a64d-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4a64d-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4a64d-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4a64d-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a64d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a64d-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4a64d-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4a64d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4a64d-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4a64d-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4a64d-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4a64d-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a64d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a64d-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="4a64d-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4a64d-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="4a64d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4a64d-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4a64d-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4a64d-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a64d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a64d-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a64d-163">createdDateTime</span></span>|<span data-ttu-id="4a64d-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a64d-164">DateTimeOffset</span></span>|<span data-ttu-id="4a64d-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4a64d-165">DateTime the object was created.</span></span> <span data-ttu-id="4a64d-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a64d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a64d-167">description</span><span class="sxs-lookup"><span data-stu-id="4a64d-167">description</span></span>|<span data-ttu-id="4a64d-168">String</span><span class="sxs-lookup"><span data-stu-id="4a64d-168">String</span></span>|<span data-ttu-id="4a64d-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4a64d-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4a64d-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a64d-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a64d-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4a64d-171">displayName</span></span>|<span data-ttu-id="4a64d-172">Строка</span><span class="sxs-lookup"><span data-stu-id="4a64d-172">String</span></span>|<span data-ttu-id="4a64d-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4a64d-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4a64d-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a64d-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a64d-175">version</span><span class="sxs-lookup"><span data-stu-id="4a64d-175">version</span></span>|<span data-ttu-id="4a64d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4a64d-176">Int32</span></span>|<span data-ttu-id="4a64d-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4a64d-177">Version of the device configuration.</span></span> <span data-ttu-id="4a64d-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a64d-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a64d-179">Дмагуарддевицеенумератионполици</span><span class="sxs-lookup"><span data-stu-id="4a64d-179">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="4a64d-180">Дмагуарддевицеенумератионполицитипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-180">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="4a64d-181">Эта политика предназначена для обеспечения дополнительной защиты от внешних устройств с поддержкой прямого доступа к памяти.</span><span class="sxs-lookup"><span data-stu-id="4a64d-181">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="4a64d-182">Он обеспечивает более полный контроль над перечислением устройств с поддержкой внешних устройств с поддержкой прямого доступа к памяти, несовместимых с пересопоставлением и изоляцией памяти устройств и изолированной средой.</span><span class="sxs-lookup"><span data-stu-id="4a64d-182">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="4a64d-183">Эта политика вступает в силу только тогда, когда система защиты DMA поддерживается и включена встроенным встроенным по.</span><span class="sxs-lookup"><span data-stu-id="4a64d-183">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="4a64d-184">Защита от DMA ядра — это компонент платформы, который невозможно контролировать с помощью политики или конечным пользователем.</span><span class="sxs-lookup"><span data-stu-id="4a64d-184">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="4a64d-185">Она должна поддерживаться системой на момент производства.</span><span class="sxs-lookup"><span data-stu-id="4a64d-185">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="4a64d-186">Чтобы проверить, поддерживает ли система защиту DMA, проверьте поле Защита ядра DMA на странице Сводка объекта MSINFO32. exe.</span><span class="sxs-lookup"><span data-stu-id="4a64d-186">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="4a64d-187">Возможные значения: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-187">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="4a64d-188">Фиреваллрулес</span><span class="sxs-lookup"><span data-stu-id="4a64d-188">firewallRules</span></span>|<span data-ttu-id="4a64d-189">Коллекция [виндовсфиреваллруле](../resources/intune-deviceconfig-windowsfirewallrule.md)</span><span class="sxs-lookup"><span data-stu-id="4a64d-189">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="4a64d-190">Настраивает параметры правила брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="4a64d-190">Configures the firewall rule settings.</span></span> <span data-ttu-id="4a64d-191">Эта коллекция может содержать не более 150 элементов.</span><span class="sxs-lookup"><span data-stu-id="4a64d-191">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="4a64d-192">Усерригхтсакцесскредентиалманажераструстедкаллер</span><span class="sxs-lookup"><span data-stu-id="4a64d-192">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="4a64d-193">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-193">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-194">Это право пользователя используется диспетчером учетных данных во время резервного копирования и восстановления.</span><span class="sxs-lookup"><span data-stu-id="4a64d-194">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="4a64d-195">Сохраненные учетные данные пользователей могут быть скомпрометированы, если эта привилегия передана другим субъектам.</span><span class="sxs-lookup"><span data-stu-id="4a64d-195">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="4a64d-196">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-196">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4a64d-197">Усерригхтсалловакцессфромнетворк</span><span class="sxs-lookup"><span data-stu-id="4a64d-197">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="4a64d-198">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-198">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-199">Это право пользователя определяет, какие пользователи и группы могут подключаться к компьютеру через сеть.</span><span class="sxs-lookup"><span data-stu-id="4a64d-199">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="4a64d-200">Допустимое состояние — Supported.</span><span class="sxs-lookup"><span data-stu-id="4a64d-200">State Allowed is supported.</span></span>|
|<span data-ttu-id="4a64d-201">Усерригхтсблоккакцессфромнетворк</span><span class="sxs-lookup"><span data-stu-id="4a64d-201">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="4a64d-202">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-202">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-203">Это право пользователя определяет, каким пользователям и группам запрещается подключаться к компьютеру через сеть.</span><span class="sxs-lookup"><span data-stu-id="4a64d-203">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="4a64d-204">Блок состояния поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a64d-204">State Block is supported.</span></span>|
|<span data-ttu-id="4a64d-205">Усерригхтсактаспартофсеоператингсистем</span><span class="sxs-lookup"><span data-stu-id="4a64d-205">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="4a64d-206">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-206">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-207">Это право пользователя позволяет процессу олицетворять любого пользователя без проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="4a64d-207">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="4a64d-208">Таким образом, процесс может получить доступ к тем же локальным ресурсам, что и пользователь.</span><span class="sxs-lookup"><span data-stu-id="4a64d-208">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="4a64d-209">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4a64d-210">Усерригхтслокаллогон</span><span class="sxs-lookup"><span data-stu-id="4a64d-210">userRightsLocalLogOn</span></span>|[<span data-ttu-id="4a64d-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-212">Это право пользователя определяет, какие пользователи могут входить на компьютер.</span><span class="sxs-lookup"><span data-stu-id="4a64d-212">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="4a64d-213">Состояния NotConfigured, разрешенные и заблокированные поддерживаются</span><span class="sxs-lookup"><span data-stu-id="4a64d-213">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="4a64d-214">Усерригхтсбаккупдата</span><span class="sxs-lookup"><span data-stu-id="4a64d-214">userRightsBackupData</span></span>|[<span data-ttu-id="4a64d-215">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-215">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-216">Это право пользователя определяет, какие пользователи могут обходить разрешения для файлов, каталогов, реестра и других постоянных объектов при резервном копировании файлов и каталогов.</span><span class="sxs-lookup"><span data-stu-id="4a64d-216">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="4a64d-217">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-217">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4a64d-218">Усерригхтсчанжесистемтиме</span><span class="sxs-lookup"><span data-stu-id="4a64d-218">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="4a64d-219">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-219">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-220">Это право пользователя определяет, какие пользователи и группы могут изменять время и дату на внутреннем часовом компьютере.</span><span class="sxs-lookup"><span data-stu-id="4a64d-220">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="4a64d-221">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-221">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4a64d-222">Усерригхтскреатеглобалобжектс</span><span class="sxs-lookup"><span data-stu-id="4a64d-222">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="4a64d-223">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-223">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-224">Этот параметр безопасности определяет, могут ли пользователи создавать глобальные объекты, доступные для всех сеансов.</span><span class="sxs-lookup"><span data-stu-id="4a64d-224">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="4a64d-225">Пользователи, которые могут создавать глобальные объекты, могут повлиять на процессы, выполняемые в сеансах других пользователей, что может привести к сбою приложения или повреждению данных.</span><span class="sxs-lookup"><span data-stu-id="4a64d-225">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="4a64d-226">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4a64d-227">Усерригхтскреатепажефиле</span><span class="sxs-lookup"><span data-stu-id="4a64d-227">userRightsCreatePageFile</span></span>|[<span data-ttu-id="4a64d-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-229">Это право пользователя определяет, какие пользователи и группы могут вызывать внутренний API, чтобы создать и изменить размер файла подкачки.</span><span class="sxs-lookup"><span data-stu-id="4a64d-229">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="4a64d-230">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4a64d-231">Усерригхтскреатеперманентшаредобжектс</span><span class="sxs-lookup"><span data-stu-id="4a64d-231">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="4a64d-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-233">Это право пользователя определяет, какие учетные записи могут использоваться процессами для создания объекта каталога с помощью диспетчера объектов.</span><span class="sxs-lookup"><span data-stu-id="4a64d-233">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="4a64d-234">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4a64d-235">Усерригхтскреатесимболиклинкс</span><span class="sxs-lookup"><span data-stu-id="4a64d-235">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="4a64d-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-237">Это право пользователя определяет, может ли пользователь создать символическую ссылку с компьютера, на который они входили.</span><span class="sxs-lookup"><span data-stu-id="4a64d-237">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="4a64d-238">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-238">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4a64d-239">Усерригхтскреатетокен</span><span class="sxs-lookup"><span data-stu-id="4a64d-239">userRightsCreateToken</span></span>|[<span data-ttu-id="4a64d-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-241">Это право пользователя определяет, какие пользователи и группы могут использоваться процессами для создания маркера, который можно использовать для получения доступа к любому локальному ресурсу, когда процесс использует внутренний API для создания маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="4a64d-241">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="4a64d-242">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-242">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4a64d-243">Усерригхтсдебугпрограмс</span><span class="sxs-lookup"><span data-stu-id="4a64d-243">userRightsDebugPrograms</span></span>|[<span data-ttu-id="4a64d-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-245">Это право пользователя определяет, какие пользователи могут прикреплять отладчик к любому процессу или ядру.</span><span class="sxs-lookup"><span data-stu-id="4a64d-245">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="4a64d-246">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-246">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4a64d-247">Усерригхтсремотедесктопсервицеслогон</span><span class="sxs-lookup"><span data-stu-id="4a64d-247">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="4a64d-248">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-248">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-249">Это право пользователя определяет, каким пользователям и группам запрещается вход в систему в качестве клиента служб удаленных рабочих столов.</span><span class="sxs-lookup"><span data-stu-id="4a64d-249">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="4a64d-250">Поддерживаются только состояния NotConfigured и Block</span><span class="sxs-lookup"><span data-stu-id="4a64d-250">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="4a64d-251">Усерригхтсделегатион</span><span class="sxs-lookup"><span data-stu-id="4a64d-251">userRightsDelegation</span></span>|[<span data-ttu-id="4a64d-252">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-252">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-253">Это право пользователя определяет, какие пользователи могут устанавливать параметр "доверять для делегирования" для объекта пользователя или компьютера.</span><span class="sxs-lookup"><span data-stu-id="4a64d-253">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="4a64d-254">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-254">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4a64d-255">Усерригхтсженератесекуритяудитс</span><span class="sxs-lookup"><span data-stu-id="4a64d-255">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="4a64d-256">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-256">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-257">Это право пользователя определяет, какие учетные записи могут использоваться процессом для добавления записей в журнал безопасности.</span><span class="sxs-lookup"><span data-stu-id="4a64d-257">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="4a64d-258">Журнал безопасности используется для трассировки несанкционированного доступа к системе.</span><span class="sxs-lookup"><span data-stu-id="4a64d-258">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="4a64d-259">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-259">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4a64d-260">Усерригхтсимперсонатеклиент</span><span class="sxs-lookup"><span data-stu-id="4a64d-260">userRightsImpersonateClient</span></span>|[<span data-ttu-id="4a64d-261">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-261">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-262">Назначение этого права пользователю позволяет программам, выполняемым от имени этого пользователя, олицетворять клиента.</span><span class="sxs-lookup"><span data-stu-id="4a64d-262">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="4a64d-263">Требование этого пользователя для такого рода олицетворения запрещает несанкционированному пользователю подключаться к созданной им службе, а затем олицетворять этого клиента, что может повысить уровень разрешений неавторизованного пользователя до Уровни администрирования или системы.</span><span class="sxs-lookup"><span data-stu-id="4a64d-263">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="4a64d-264">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4a64d-265">Усерригхтсинкреасесчедулингприорити</span><span class="sxs-lookup"><span data-stu-id="4a64d-265">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="4a64d-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-267">Это право пользователя определяет, какие учетные записи могут использовать процесс с доступом к свойствам Write для другого процесса, чтобы увеличить приоритет выполнения, назначенный другому процессу.</span><span class="sxs-lookup"><span data-stu-id="4a64d-267">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="4a64d-268">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4a64d-269">Усерригхтслоадунлоаддриверс</span><span class="sxs-lookup"><span data-stu-id="4a64d-269">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="4a64d-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-271">Это право пользователя определяет, какие пользователи могут динамически загружать и выгружать драйверы устройств или другой код в режиме ядра.</span><span class="sxs-lookup"><span data-stu-id="4a64d-271">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="4a64d-272">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4a64d-273">Усерригхтслоккмемори</span><span class="sxs-lookup"><span data-stu-id="4a64d-273">userRightsLockMemory</span></span>|[<span data-ttu-id="4a64d-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-275">Это право пользователя определяет, какие учетные записи могут использовать процесс для хранения данных в физической памяти, что предотвращает их разбиение данных на виртуальную память на диске.</span><span class="sxs-lookup"><span data-stu-id="4a64d-275">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="4a64d-276">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4a64d-277">Усерригхтсманажеаудитингандсекуритилогс</span><span class="sxs-lookup"><span data-stu-id="4a64d-277">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="4a64d-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-279">Это право пользователя определяет, какие пользователи могут задавать параметры аудита доступа к объектам для отдельных ресурсов, таких как файлы, объекты Active Directory и разделы реестра.</span><span class="sxs-lookup"><span data-stu-id="4a64d-279">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="4a64d-280">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4a64d-281">Усерригхтсманажеволумес</span><span class="sxs-lookup"><span data-stu-id="4a64d-281">userRightsManageVolumes</span></span>|[<span data-ttu-id="4a64d-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-283">Это право пользователя определяет, какие пользователи и группы могут выполнять задачи обслуживания для тома, такие как удаленная дефрагментация.</span><span class="sxs-lookup"><span data-stu-id="4a64d-283">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="4a64d-284">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4a64d-285">Усерригхтсмодифифирмваринвиронмент</span><span class="sxs-lookup"><span data-stu-id="4a64d-285">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="4a64d-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-287">Это право пользователя определяет, кто может изменять значения в аппаратной среде.</span><span class="sxs-lookup"><span data-stu-id="4a64d-287">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="4a64d-288">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-288">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4a64d-289">Усерригхтсмодифйобжектлабелс</span><span class="sxs-lookup"><span data-stu-id="4a64d-289">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="4a64d-290">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-290">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-291">Это право пользователя определяет, какие учетные записи пользователей могут изменять метки целостности объектов, таких как файлы, разделы реестра или процессы, принадлежащие другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="4a64d-291">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="4a64d-292">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-292">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4a64d-293">Усерригхтспрофилесинглепроцесс</span><span class="sxs-lookup"><span data-stu-id="4a64d-293">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="4a64d-294">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-294">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-295">Это право пользователя определяет, какие пользователи могут использовать средства мониторинга производительности для наблюдения за производительностью системных процессов.</span><span class="sxs-lookup"><span data-stu-id="4a64d-295">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="4a64d-296">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-296">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4a64d-297">Усерригхтсремотешутдовн</span><span class="sxs-lookup"><span data-stu-id="4a64d-297">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="4a64d-298">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-298">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-299">Это право пользователя определяет, каким пользователям разрешено завершать работу компьютера из удаленного расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="4a64d-299">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="4a64d-300">Неправильное использование этого права пользователя может привести к отказу в обслуживании.</span><span class="sxs-lookup"><span data-stu-id="4a64d-300">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="4a64d-301">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-301">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4a64d-302">Усерригхтсресторедата</span><span class="sxs-lookup"><span data-stu-id="4a64d-302">userRightsRestoreData</span></span>|[<span data-ttu-id="4a64d-303">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-303">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-304">Это право пользователя определяет, какие пользователи могут обходить разрешения для файлов, каталогов, реестра и других постоянных объектов при восстановлении резервных копий файлов и каталогов, и определяет, какие пользователи могут устанавливать любой действительный субъект безопасности в качестве владельца объекта.</span><span class="sxs-lookup"><span data-stu-id="4a64d-304">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="4a64d-305">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-305">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4a64d-306">Усерригхтстакеовнершип</span><span class="sxs-lookup"><span data-stu-id="4a64d-306">userRightsTakeOwnership</span></span>|[<span data-ttu-id="4a64d-307">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-307">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-308">Это право пользователя определяет, какие пользователи могут становиться владельцами любого защищаемого объекта в системе, включая объекты Active Directory, файлы и папки, принтеры, разделы реестра, процессы и потоки.</span><span class="sxs-lookup"><span data-stu-id="4a64d-308">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="4a64d-309">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="4a64d-309">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4a64d-310">Усерригхтсрегистерпроцессассервице</span><span class="sxs-lookup"><span data-stu-id="4a64d-310">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="4a64d-311">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4a64d-311">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4a64d-312">Этот параметр безопасности определяет, каким учетным записям служб запрещается регистрировать процесс в качестве службы.</span><span class="sxs-lookup"><span data-stu-id="4a64d-312">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="4a64d-313">Примечание: этот параметр безопасности не применяется к системным, локальным или сетевым учетным записям служб.</span><span class="sxs-lookup"><span data-stu-id="4a64d-313">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="4a64d-314">Поддерживается только блокирование состояния.</span><span class="sxs-lookup"><span data-stu-id="4a64d-314">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="4a64d-315">Ксбокссервицесенаблексбоксгамесаветаск</span><span class="sxs-lookup"><span data-stu-id="4a64d-315">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="4a64d-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-316">Boolean</span></span>|<span data-ttu-id="4a64d-317">Этот параметр определяет, включена ли функция сохранения игры Xbox (1) или отключена (0).</span><span class="sxs-lookup"><span data-stu-id="4a64d-317">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="4a64d-318">Ксбокссервицесакцессориманажементсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="4a64d-318">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="4a64d-319">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="4a64d-320">Этот параметр определяет, является ли тип запуска службы управления принадлежностью автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="4a64d-320">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="4a64d-321">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="4a64d-321">Default: Manual.</span></span> <span data-ttu-id="4a64d-322">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="4a64d-323">Ксбокссервицесливеаусманажерсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="4a64d-323">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="4a64d-324">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-324">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="4a64d-325">Этот параметр определяет, является ли тип запуска службы диспетчера Live auth автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="4a64d-325">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="4a64d-326">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="4a64d-326">Default: Manual.</span></span> <span data-ttu-id="4a64d-327">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-327">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="4a64d-328">Ксбокссервицесливегамесавесервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="4a64d-328">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="4a64d-329">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-329">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="4a64d-330">Этот параметр определяет, является ли тип запуска службы Live Save Service автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="4a64d-330">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="4a64d-331">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="4a64d-331">Default: Manual.</span></span> <span data-ttu-id="4a64d-332">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-332">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="4a64d-333">Ксбокссервицесливенетворкингсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="4a64d-333">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="4a64d-334">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-334">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="4a64d-335">Этот параметр определяет, является ли тип запуска сетевой службы автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="4a64d-335">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="4a64d-336">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="4a64d-336">Default: Manual.</span></span> <span data-ttu-id="4a64d-337">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-337">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="4a64d-338">Локалсекуритйоптионсблоккмикрософтаккаунтс</span><span class="sxs-lookup"><span data-stu-id="4a64d-338">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="4a64d-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-339">Boolean</span></span>|<span data-ttu-id="4a64d-340">Запретить пользователям добавлять новые учетные записи Майкрософт на этот компьютер.</span><span class="sxs-lookup"><span data-stu-id="4a64d-340">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="4a64d-341">Локалсекуритйоптионсблоккремотелогонвисбланкпассворд</span><span class="sxs-lookup"><span data-stu-id="4a64d-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="4a64d-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-342">Boolean</span></span>|<span data-ttu-id="4a64d-343">Включите локальные учетные записи, не защищенные паролем, для входа в систему из расположений, отличных от физического устройства. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="4a64d-343">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="4a64d-344">Локалсекуритйоптионсдисаблеадминистратораккаунт</span><span class="sxs-lookup"><span data-stu-id="4a64d-344">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="4a64d-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-345">Boolean</span></span>|<span data-ttu-id="4a64d-346">Определяет, включена или отключена учетная запись локального администратора.</span><span class="sxs-lookup"><span data-stu-id="4a64d-346">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="4a64d-347">Локалсекуритйоптионсадминистратораккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="4a64d-347">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="4a64d-348">String</span><span class="sxs-lookup"><span data-stu-id="4a64d-348">String</span></span>|<span data-ttu-id="4a64d-349">Определите имя другой учетной записи, которая будет связана с идентификатором безопасности (SID) учетной записи "Administrator".</span><span class="sxs-lookup"><span data-stu-id="4a64d-349">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="4a64d-350">Локалсекуритйоптионсдисаблегуестаккаунт</span><span class="sxs-lookup"><span data-stu-id="4a64d-350">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="4a64d-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-351">Boolean</span></span>|<span data-ttu-id="4a64d-352">Определяет, включена или отключена Гостевая учетная запись.</span><span class="sxs-lookup"><span data-stu-id="4a64d-352">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="4a64d-353">Локалсекуритйоптионсгуестаккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="4a64d-353">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="4a64d-354">String</span><span class="sxs-lookup"><span data-stu-id="4a64d-354">String</span></span>|<span data-ttu-id="4a64d-355">Определите имя другой учетной записи, которая будет связана с идентификатором безопасности (SID) для учетной записи "гость".</span><span class="sxs-lookup"><span data-stu-id="4a64d-355">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="4a64d-356">Локалсекуритйоптионсалловундокквисаусавингтологон</span><span class="sxs-lookup"><span data-stu-id="4a64d-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="4a64d-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-357">Boolean</span></span>|<span data-ttu-id="4a64d-358">Запретите отстыковку портативного компьютера без необходимости входа в систему.</span><span class="sxs-lookup"><span data-stu-id="4a64d-358">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="4a64d-359">Локалсекуритйоптионсблоккусерсинсталлингпринтердриверс</span><span class="sxs-lookup"><span data-stu-id="4a64d-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="4a64d-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-360">Boolean</span></span>|<span data-ttu-id="4a64d-361">Ограничьте установку драйверов принтеров в рамках подключения к общему принтеру только для администраторов.</span><span class="sxs-lookup"><span data-stu-id="4a64d-361">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="4a64d-362">Локалсекуритйоптионсблоккремотеоптикалдривеакцесс</span><span class="sxs-lookup"><span data-stu-id="4a64d-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="4a64d-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-363">Boolean</span></span>|<span data-ttu-id="4a64d-364">Включение этого параметра позволяет интерактивно вошедший в систему пользователь получать доступ к устройству чтения компакт-дисков.</span><span class="sxs-lookup"><span data-stu-id="4a64d-364">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="4a64d-365">Локалсекуритйоптионсформатандежектофремоваблемедиаалловедусер</span><span class="sxs-lookup"><span data-stu-id="4a64d-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="4a64d-366">Локалсекуритйоптионсформатандежектофремоваблемедиаалловедусертипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="4a64d-367">Определите, кому разрешено форматировать и извлекать съемные носители NTFS.</span><span class="sxs-lookup"><span data-stu-id="4a64d-367">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="4a64d-368">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-368">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="4a64d-369">Локалсекуритйоптионсмачинеинактивитилимит</span><span class="sxs-lookup"><span data-stu-id="4a64d-369">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="4a64d-370">Int32</span><span class="sxs-lookup"><span data-stu-id="4a64d-370">Int32</span></span>|<span data-ttu-id="4a64d-371">Определите максимальное количество минут отсутствия активности на экране входа интерактивного рабочего стола, пока не запустится экранная заставка.</span><span class="sxs-lookup"><span data-stu-id="4a64d-371">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="4a64d-372">Допустимые значения — от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="4a64d-372">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="4a64d-373">Локалсекуритйоптионсмачинеинактивитилимитинминутес</span><span class="sxs-lookup"><span data-stu-id="4a64d-373">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="4a64d-374">Int32</span><span class="sxs-lookup"><span data-stu-id="4a64d-374">Int32</span></span>|<span data-ttu-id="4a64d-375">Определите максимальное количество минут отсутствия активности на экране входа интерактивного рабочего стола, пока не запустится экранная заставка.</span><span class="sxs-lookup"><span data-stu-id="4a64d-375">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="4a64d-376">Допустимые значения — от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="4a64d-376">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="4a64d-377">Локалсекуритйоптионсдонотрекуиректрлалтдел</span><span class="sxs-lookup"><span data-stu-id="4a64d-377">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="4a64d-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-378">Boolean</span></span>|<span data-ttu-id="4a64d-379">Требовать нажатия клавиш CTRL + ALT + DEL, прежде чем пользователь сможет войти в систему.</span><span class="sxs-lookup"><span data-stu-id="4a64d-379">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="4a64d-380">Локалсекуритйоптионшиделастсигнединусер</span><span class="sxs-lookup"><span data-stu-id="4a64d-380">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="4a64d-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-381">Boolean</span></span>|<span data-ttu-id="4a64d-382">Не отображать имя последнего пользователя, выполнившего вход на это устройство.</span><span class="sxs-lookup"><span data-stu-id="4a64d-382">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="4a64d-383">Локалсекуритйоптионшидеусернамеатсигнин</span><span class="sxs-lookup"><span data-stu-id="4a64d-383">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="4a64d-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-384">Boolean</span></span>|<span data-ttu-id="4a64d-385">Не отображать имя пользователя, выполняющего вход на это устройство, после ввода учетных данных и отображения рабочего стола на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4a64d-385">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="4a64d-386">Локалсекуритйоптионслогонмессажетитле</span><span class="sxs-lookup"><span data-stu-id="4a64d-386">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="4a64d-387">String</span><span class="sxs-lookup"><span data-stu-id="4a64d-387">String</span></span>|<span data-ttu-id="4a64d-388">Задайте заголовок сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="4a64d-388">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="4a64d-389">Локалсекуритйоптионслогонмессажетекст</span><span class="sxs-lookup"><span data-stu-id="4a64d-389">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="4a64d-390">String</span><span class="sxs-lookup"><span data-stu-id="4a64d-390">String</span></span>|<span data-ttu-id="4a64d-391">Задайте текст сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="4a64d-391">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="4a64d-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="4a64d-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="4a64d-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-393">Boolean</span></span>|<span data-ttu-id="4a64d-394">Блокировать запросы проверки подлинности PKU2U на этом устройстве для использования сетевых удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4a64d-394">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="4a64d-395">Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажерхелпербул</span><span class="sxs-lookup"><span data-stu-id="4a64d-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="4a64d-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-396">Boolean</span></span>|<span data-ttu-id="4a64d-397">Помощник по пользовательскому интерфейсу Boolean для объекта Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажер</span><span class="sxs-lookup"><span data-stu-id="4a64d-397">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="4a64d-398">Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажер</span><span class="sxs-lookup"><span data-stu-id="4a64d-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="4a64d-399">String</span><span class="sxs-lookup"><span data-stu-id="4a64d-399">String</span></span>|<span data-ttu-id="4a64d-400">Измените строку языка определения дескрипторов безопасности по умолчанию, чтобы разрешить или запретить пользователям и группам совершать удаленные вызовы в SAM.</span><span class="sxs-lookup"><span data-stu-id="4a64d-400">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="4a64d-401">Локалсекуритйоптионсминимумсессионсекуритифорнтлмсспбаседклиентс</span><span class="sxs-lookup"><span data-stu-id="4a64d-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="4a64d-402">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="4a64d-402">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="4a64d-403">Этот параметр безопасности позволяет клиенту требовать согласование 128-разрядного шифрования и/или сеанса защиты сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="4a64d-403">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="4a64d-404">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-404">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="4a64d-405">Локалсекуритйоптионсминимумсессионсекуритифорнтлмсспбаседсерверс</span><span class="sxs-lookup"><span data-stu-id="4a64d-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="4a64d-406">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="4a64d-406">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="4a64d-407">Этот параметр безопасности позволяет серверу требовать согласование 128-разрядного шифрования и/или сеанса защиты сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="4a64d-407">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="4a64d-408">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-408">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="4a64d-409">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="4a64d-409">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="4a64d-410">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="4a64d-410">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="4a64d-411">Этот параметр безопасности определяет, какой протокол проверки подлинности "запрос/ответ" используется для входа в сеть.</span><span class="sxs-lookup"><span data-stu-id="4a64d-411">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="4a64d-412">Возможные значения: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-412">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="4a64d-413">Ланманажерворкстатиондисаблеинсекурегуестлогонс</span><span class="sxs-lookup"><span data-stu-id="4a64d-413">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="4a64d-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-414">Boolean</span></span>|<span data-ttu-id="4a64d-415">Если этот параметр включен, клиент SMB будет разрешать небезопасные гостевые входы.</span><span class="sxs-lookup"><span data-stu-id="4a64d-415">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="4a64d-416">Если этот параметр не настроен, клиент SMB будет отклонять небезопасные гостевые входы.</span><span class="sxs-lookup"><span data-stu-id="4a64d-416">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="4a64d-417">Локалсекуритйоптионсклеарвиртуалмеморипажефиле</span><span class="sxs-lookup"><span data-stu-id="4a64d-417">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="4a64d-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-418">Boolean</span></span>|<span data-ttu-id="4a64d-419">Этот параметр безопасности определяет, будет ли очищаться файл подкачки виртуальной памяти при завершении работы системы.</span><span class="sxs-lookup"><span data-stu-id="4a64d-419">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="4a64d-420">Локалсекуритйоптионсалловсистемтобешутдовнвисаусавингтологон</span><span class="sxs-lookup"><span data-stu-id="4a64d-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="4a64d-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-421">Boolean</span></span>|<span data-ttu-id="4a64d-422">Этот параметр безопасности определяет, можно ли завершить работу компьютера, не выполняя вход в Windows.</span><span class="sxs-lookup"><span data-stu-id="4a64d-422">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="4a64d-423">Локалсекуритйоптионсалловуиакцессаппликатионелеватион</span><span class="sxs-lookup"><span data-stu-id="4a64d-423">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="4a64d-424">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-424">Boolean</span></span>|<span data-ttu-id="4a64d-425">Разрешить UIAccess Apps запрос на повышение прав без использования безопасного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="4a64d-425">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="4a64d-426">Локалсекуритйоптионсвиртуализефилеандрегистривритефаилурестоперусерлокатионс</span><span class="sxs-lookup"><span data-stu-id="4a64d-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="4a64d-427">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-427">Boolean</span></span>|<span data-ttu-id="4a64d-428">Виртуализация сбоев записи в файл и реестр для отдельных расположений пользователей</span><span class="sxs-lookup"><span data-stu-id="4a64d-428">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="4a64d-429">Локалсекуритйоптионсонлелеватесигнедексекутаблес</span><span class="sxs-lookup"><span data-stu-id="4a64d-429">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="4a64d-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-430">Boolean</span></span>|<span data-ttu-id="4a64d-431">Принудительная проверка пути сертификации PKI для указанного исполняемого файла перед тем, как он будет разрешен для запуска.</span><span class="sxs-lookup"><span data-stu-id="4a64d-431">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="4a64d-432">Локалсекуритйоптионсадминистраторелеватионпромптбехавиор</span><span class="sxs-lookup"><span data-stu-id="4a64d-432">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="4a64d-433">Локалсекуритйоптионсадминистраторелеватионпромптбехавиортипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="4a64d-434">Определите поведение запросов на повышение прав для администраторов в режиме одобрения администратором.</span><span class="sxs-lookup"><span data-stu-id="4a64d-434">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="4a64d-435">Возможные значения: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-435">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="4a64d-436">Локалсекуритйоптионсстандардусерелеватионпромптбехавиор</span><span class="sxs-lookup"><span data-stu-id="4a64d-436">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="4a64d-437">Локалсекуритйоптионсстандардусерелеватионпромптбехавиортипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="4a64d-438">Определите поведение запросов на повышение прав для стандартных пользователей.</span><span class="sxs-lookup"><span data-stu-id="4a64d-438">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="4a64d-439">Возможные значения: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-439">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="4a64d-440">Локалсекуритйоптионссвитчтосекуредесктопвхенпромптингфорелеватион</span><span class="sxs-lookup"><span data-stu-id="4a64d-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="4a64d-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-441">Boolean</span></span>|<span data-ttu-id="4a64d-442">Разрешить всем запросам на повышение прав доступ к рабочему столу интерактивного пользователя, а не к безопасному рабочему столу.</span><span class="sxs-lookup"><span data-stu-id="4a64d-442">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="4a64d-443">Используются параметры политики поведения запросов для администраторов и стандартных пользователей.</span><span class="sxs-lookup"><span data-stu-id="4a64d-443">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="4a64d-444">Локалсекуритйоптионсдетектаппликатионинсталлатионсандпромптфорелеватион</span><span class="sxs-lookup"><span data-stu-id="4a64d-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="4a64d-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-445">Boolean</span></span>|<span data-ttu-id="4a64d-446">При установке приложений, требующих повышенных привилегий, запрашиваются учетные данные администратора. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="4a64d-446">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="4a64d-447">Локалсекуритйоптионсалловуиакцессаппликатионсфорсекурелокатионс</span><span class="sxs-lookup"><span data-stu-id="4a64d-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="4a64d-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-448">Boolean</span></span>|<span data-ttu-id="4a64d-449">Разрешить UIAccess Apps запрос на повышение прав без использования безопасного рабочего стола. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="4a64d-449">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="4a64d-450">Локалсекуритйоптионсусеадминаппровалмоде</span><span class="sxs-lookup"><span data-stu-id="4a64d-450">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="4a64d-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-451">Boolean</span></span>|<span data-ttu-id="4a64d-452">Определяет, использует ли встроенная учетная запись администратора режим одобрения администратором или выполняет все приложения с правами полного администратора. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="4a64d-452">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="4a64d-453">Локалсекуритйоптионсусеадминаппровалмодефорадминистраторс</span><span class="sxs-lookup"><span data-stu-id="4a64d-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="4a64d-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-454">Boolean</span></span>|<span data-ttu-id="4a64d-455">Определить, включен ли режим одобрения администратором и все параметры политики контроля учетных записей, по умолчанию включено</span><span class="sxs-lookup"><span data-stu-id="4a64d-455">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="4a64d-456">Локалсекуритйоптионсинформатионшовнонлоккскрин</span><span class="sxs-lookup"><span data-stu-id="4a64d-456">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="4a64d-457">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="4a64d-457">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="4a64d-458">Настройте сведения о пользователе, которые отображаются, когда сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="4a64d-458">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="4a64d-459">Если этот флажок не установлен, отображаются отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="4a64d-459">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="4a64d-460">Возможные значения: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-460">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="4a64d-461">Локалсекуритйоптионсинформатиондисплайедонлоккскрин</span><span class="sxs-lookup"><span data-stu-id="4a64d-461">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="4a64d-462">Локалсекуритйоптионсинформатиондисплайедонлоккскринтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="4a64d-463">Настройте сведения о пользователе, которые отображаются, когда сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="4a64d-463">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="4a64d-464">Если этот флажок не установлен, отображаются отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="4a64d-464">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="4a64d-465">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-465">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="4a64d-466">Локалсекуритйоптионсдисаблеклиентдигиталлисигнкоммуникатионсифсерверагрис</span><span class="sxs-lookup"><span data-stu-id="4a64d-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="4a64d-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-467">Boolean</span></span>|<span data-ttu-id="4a64d-468">Этот параметр безопасности определяет, будет ли клиент SMB пытаться согласовать подписывание SMB пакетов.</span><span class="sxs-lookup"><span data-stu-id="4a64d-468">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="4a64d-469">Локалсекуритйоптионсклиентдигиталлисигнкоммуникатионсалвайс</span><span class="sxs-lookup"><span data-stu-id="4a64d-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="4a64d-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-470">Boolean</span></span>|<span data-ttu-id="4a64d-471">Этот параметр безопасности определяет, требуется ли Подписывание пакетов для клиентского SMB-компонента.</span><span class="sxs-lookup"><span data-stu-id="4a64d-471">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="4a64d-472">Локалсекуритйоптионсклиентсендуненкриптедпассвордтосирдпартисмбсерверс</span><span class="sxs-lookup"><span data-stu-id="4a64d-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="4a64d-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-473">Boolean</span></span>|<span data-ttu-id="4a64d-474">Если этот параметр безопасности включен, перенаправителем SMB (Server Message Block) разрешено отправлять пароли открытым текстом на серверы SMB сторонних производителей, не поддерживающие шифрование паролей во время проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="4a64d-474">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="4a64d-475">Локалсекуритйоптионсдисаблесервердигиталлисигнкоммуникатионсалвайс</span><span class="sxs-lookup"><span data-stu-id="4a64d-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="4a64d-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-476">Boolean</span></span>|<span data-ttu-id="4a64d-477">Этот параметр безопасности определяет, требуется ли подписи пакетов для SMB-компонентов сервера.</span><span class="sxs-lookup"><span data-stu-id="4a64d-477">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="4a64d-478">Локалсекуритйоптионсдисаблесервердигиталлисигнкоммуникатионсифклиентагрис</span><span class="sxs-lookup"><span data-stu-id="4a64d-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="4a64d-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-479">Boolean</span></span>|<span data-ttu-id="4a64d-480">Этот параметр безопасности определяет, будет ли SMB согласовывать подпись SMB Packet с клиентами, которые их запрашивают.</span><span class="sxs-lookup"><span data-stu-id="4a64d-480">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="4a64d-481">Локалсекуритйоптионсрестриктанонимаусакцесстонамедпипесандшарес</span><span class="sxs-lookup"><span data-stu-id="4a64d-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="4a64d-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-482">Boolean</span></span>|<span data-ttu-id="4a64d-483">По умолчанию этот параметр безопасности запрещает анонимный доступ к ресурсам и каналам к параметрам именованных каналов, к которым возможен анонимный доступ, и к общедоступным ресурсам, к которым возможен анонимный доступ</span><span class="sxs-lookup"><span data-stu-id="4a64d-483">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="4a64d-484">Локалсекуритйоптионсдоноталлованонимаусенумератионофсамаккаунтс</span><span class="sxs-lookup"><span data-stu-id="4a64d-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="4a64d-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-485">Boolean</span></span>|<span data-ttu-id="4a64d-486">Этот параметр безопасности определяет, какие дополнительные разрешения будут предоставлены анонимным подключениям к компьютеру.</span><span class="sxs-lookup"><span data-stu-id="4a64d-486">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="4a64d-487">Локалсекуритйоптионсаллованонимаусенумератионофсамаккаунтсандшарес</span><span class="sxs-lookup"><span data-stu-id="4a64d-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="4a64d-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-488">Boolean</span></span>|<span data-ttu-id="4a64d-489">Этот параметр безопасности определяет, разрешено ли анонимным пользователям выполнять определенные действия, например перечислять имена доменных учетных записей и сетевые общие папки.</span><span class="sxs-lookup"><span data-stu-id="4a64d-489">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="4a64d-490">Локалсекуритйоптионсдонотстореланманажерхашвалуеоннекстпассвордчанже</span><span class="sxs-lookup"><span data-stu-id="4a64d-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="4a64d-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-491">Boolean</span></span>|<span data-ttu-id="4a64d-492">Этот параметр безопасности определяет, будет ли сохраняться значение хэша LAN Manager (LM) для нового пароля при следующем изменении пароля.</span><span class="sxs-lookup"><span data-stu-id="4a64d-492">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="4a64d-493">По умолчанию он не хранится.</span><span class="sxs-lookup"><span data-stu-id="4a64d-493">It’s not stored by default.</span></span>|
|<span data-ttu-id="4a64d-494">Локалсекуритйоптионссмарткардремовалбехавиор</span><span class="sxs-lookup"><span data-stu-id="4a64d-494">localSecurityOptionsSmartCardRemovalBehavior</span></span>|<span data-ttu-id="4a64d-495">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md);</span><span class="sxs-lookup"><span data-stu-id="4a64d-495">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)</span></span>|<span data-ttu-id="4a64d-496">Этот параметр безопасности определяет, что происходит при удалении смарт-карты пользователя, выполнившего вход в систему, из устройства чтения смарт-карт.</span><span class="sxs-lookup"><span data-stu-id="4a64d-496">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="4a64d-497">Возможные значения: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-497">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="4a64d-498">Дефендерсекуритицентердисаблеаппбровсеруи</span><span class="sxs-lookup"><span data-stu-id="4a64d-498">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="4a64d-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-499">Boolean</span></span>|<span data-ttu-id="4a64d-500">Используется для отключения отображения области защиты приложений и браузера.</span><span class="sxs-lookup"><span data-stu-id="4a64d-500">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="4a64d-501">Дефендерсекуритицентердисаблефамилюи</span><span class="sxs-lookup"><span data-stu-id="4a64d-501">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="4a64d-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-502">Boolean</span></span>|<span data-ttu-id="4a64d-503">Используется для отключения отображения области семьи.</span><span class="sxs-lookup"><span data-stu-id="4a64d-503">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="4a64d-504">Дефендерсекуритицентердисаблехеалсуи</span><span class="sxs-lookup"><span data-stu-id="4a64d-504">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="4a64d-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-505">Boolean</span></span>|<span data-ttu-id="4a64d-506">Используется для отключения отображения области производительности и работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="4a64d-506">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="4a64d-507">Дефендерсекуритицентердисабленетворкуи</span><span class="sxs-lookup"><span data-stu-id="4a64d-507">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="4a64d-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-508">Boolean</span></span>|<span data-ttu-id="4a64d-509">Используется для отключения отображения зоны "брандмауэр" и "Защита сети".</span><span class="sxs-lookup"><span data-stu-id="4a64d-509">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="4a64d-510">Дефендерсекуритицентердисаблевирусуи</span><span class="sxs-lookup"><span data-stu-id="4a64d-510">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="4a64d-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-511">Boolean</span></span>|<span data-ttu-id="4a64d-512">Используется для отключения отображения области защиты от вирусов и угроз.</span><span class="sxs-lookup"><span data-stu-id="4a64d-512">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="4a64d-513">Дефендерсекуритицентердисаблеаккаунтуи</span><span class="sxs-lookup"><span data-stu-id="4a64d-513">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="4a64d-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-514">Boolean</span></span>|<span data-ttu-id="4a64d-515">Используется для отключения отображения области защиты учетных записей.</span><span class="sxs-lookup"><span data-stu-id="4a64d-515">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="4a64d-516">Дефендерсекуритицентердисаблеклеартпмуи</span><span class="sxs-lookup"><span data-stu-id="4a64d-516">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="4a64d-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-517">Boolean</span></span>|<span data-ttu-id="4a64d-518">Используется для отключения отображения кнопки Очистить доверенный платформенный модуль.</span><span class="sxs-lookup"><span data-stu-id="4a64d-518">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="4a64d-519">Дефендерсекуритицентердисаблехардвареуи</span><span class="sxs-lookup"><span data-stu-id="4a64d-519">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="4a64d-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-520">Boolean</span></span>|<span data-ttu-id="4a64d-521">Используется для отключения отображения области аппаратной защиты.</span><span class="sxs-lookup"><span data-stu-id="4a64d-521">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="4a64d-522">Дефендерсекуритицентердисабленотификатионареауи</span><span class="sxs-lookup"><span data-stu-id="4a64d-522">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="4a64d-523">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-523">Boolean</span></span>|<span data-ttu-id="4a64d-524">Используется для отключения отображения элемента управления "область уведомлений".</span><span class="sxs-lookup"><span data-stu-id="4a64d-524">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="4a64d-525">Для вступления этого параметра в силу пользователю необходимо выйти из системы и войти в нее, а затем перезагрузить компьютер.</span><span class="sxs-lookup"><span data-stu-id="4a64d-525">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="4a64d-526">Дефендерсекуритицентердисаблерансомвареуи</span><span class="sxs-lookup"><span data-stu-id="4a64d-526">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="4a64d-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-527">Boolean</span></span>|<span data-ttu-id="4a64d-528">Используется для отключения отображения области защиты от пошантажистом.</span><span class="sxs-lookup"><span data-stu-id="4a64d-528">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="4a64d-529">Дефендерсекуритицентердисаблесекуребутуи</span><span class="sxs-lookup"><span data-stu-id="4a64d-529">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="4a64d-530">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-530">Boolean</span></span>|<span data-ttu-id="4a64d-531">Используется для отключения отображения области безопасной загрузки в разделе Безопасность устройства.</span><span class="sxs-lookup"><span data-stu-id="4a64d-531">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="4a64d-532">Дефендерсекуритицентердисаблетраублешутингуи</span><span class="sxs-lookup"><span data-stu-id="4a64d-532">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="4a64d-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-533">Boolean</span></span>|<span data-ttu-id="4a64d-534">Используется для отключения отображения устранения неполадок процесса безопасности в разделе Безопасность устройства.</span><span class="sxs-lookup"><span data-stu-id="4a64d-534">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="4a64d-535">Дефендерсекуритицентердисаблевулнераблетпмфирмвареупдатеуи</span><span class="sxs-lookup"><span data-stu-id="4a64d-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="4a64d-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-536">Boolean</span></span>|<span data-ttu-id="4a64d-537">Используется для отключения отображения обновления микропрограммы доверенного платформенного модуля при обнаружении уязвимого программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="4a64d-537">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="4a64d-538">Дефендерсекуритицентерорганизатиондисплайнаме</span><span class="sxs-lookup"><span data-stu-id="4a64d-538">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="4a64d-539">String</span><span class="sxs-lookup"><span data-stu-id="4a64d-539">String</span></span>|<span data-ttu-id="4a64d-540">Имя компании, которое отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="4a64d-540">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="4a64d-541">Дефендерсекуритицентерхелпемаил</span><span class="sxs-lookup"><span data-stu-id="4a64d-541">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="4a64d-542">String</span><span class="sxs-lookup"><span data-stu-id="4a64d-542">String</span></span>|<span data-ttu-id="4a64d-543">Адрес электронной почты, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="4a64d-543">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="4a64d-544">Дефендерсекуритицентерхелпфоне</span><span class="sxs-lookup"><span data-stu-id="4a64d-544">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="4a64d-545">String</span><span class="sxs-lookup"><span data-stu-id="4a64d-545">String</span></span>|<span data-ttu-id="4a64d-546">Номер телефона или идентификатор Skype, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="4a64d-546">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="4a64d-547">Дефендерсекуритицентерхелпурл</span><span class="sxs-lookup"><span data-stu-id="4a64d-547">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="4a64d-548">String</span><span class="sxs-lookup"><span data-stu-id="4a64d-548">String</span></span>|<span data-ttu-id="4a64d-549">URL-адрес портала справки это отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="4a64d-549">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="4a64d-550">Дефендерсекуритицентернотификатионсфромапп</span><span class="sxs-lookup"><span data-stu-id="4a64d-550">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="4a64d-551">Дефендерсекуритицентернотификатионсфромапптипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-551">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="4a64d-552">Уведомления, отображаемые в отображаемых областях приложения.</span><span class="sxs-lookup"><span data-stu-id="4a64d-552">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="4a64d-553">Возможные значения: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-553">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="4a64d-554">Дефендерсекуритицентеритконтактдисплай</span><span class="sxs-lookup"><span data-stu-id="4a64d-554">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="4a64d-555">Дефендерсекуритицентеритконтактдисплайтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-555">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="4a64d-556">Настройка места отображения контактной информации для конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="4a64d-556">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="4a64d-557">Возможные значения: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-557">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="4a64d-558">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="4a64d-558">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="4a64d-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-559">Boolean</span></span>|<span data-ttu-id="4a64d-560">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="4a64d-560">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="4a64d-561">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="4a64d-561">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="4a64d-562">Int32</span><span class="sxs-lookup"><span data-stu-id="4a64d-562">Int32</span></span>|<span data-ttu-id="4a64d-563">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="4a64d-563">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="4a64d-564">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="4a64d-564">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="4a64d-565">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="4a64d-565">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="4a64d-566">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="4a64d-566">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="4a64d-567">Фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-567">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="4a64d-568">Выберите используемую кодировку с общим ключом.</span><span class="sxs-lookup"><span data-stu-id="4a64d-568">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="4a64d-569">Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-569">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="4a64d-570">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="4a64d-570">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="4a64d-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-571">Boolean</span></span>|<span data-ttu-id="4a64d-572">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="4a64d-572">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="4a64d-573">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="4a64d-573">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="4a64d-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-574">Boolean</span></span>|<span data-ttu-id="4a64d-575">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="4a64d-575">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="4a64d-576">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="4a64d-576">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="4a64d-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-577">Boolean</span></span>|<span data-ttu-id="4a64d-578">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="4a64d-578">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="4a64d-579">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="4a64d-579">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="4a64d-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-580">Boolean</span></span>|<span data-ttu-id="4a64d-581">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="4a64d-581">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="4a64d-582">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="4a64d-582">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="4a64d-583">Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-583">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="4a64d-584">Укажите способ применения списка отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4a64d-584">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="4a64d-585">Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-585">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="4a64d-586">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="4a64d-586">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="4a64d-587">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-587">Boolean</span></span>|<span data-ttu-id="4a64d-588">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="4a64d-588">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="4a64d-589">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="4a64d-589">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="4a64d-590">Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-590">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="4a64d-591">Настраивает способ применения очередей пакетов в сценарии туннельного шлюза.</span><span class="sxs-lookup"><span data-stu-id="4a64d-591">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="4a64d-592">Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-592">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="4a64d-593">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="4a64d-593">firewallProfileDomain</span></span>|[<span data-ttu-id="4a64d-594">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="4a64d-594">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="4a64d-595">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="4a64d-595">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="4a64d-596">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="4a64d-596">firewallProfilePublic</span></span>|[<span data-ttu-id="4a64d-597">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="4a64d-597">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="4a64d-598">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="4a64d-598">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="4a64d-599">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="4a64d-599">firewallProfilePrivate</span></span>|[<span data-ttu-id="4a64d-600">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="4a64d-600">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="4a64d-601">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="4a64d-601">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="4a64d-602">Дефендерадобереадерлаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="4a64d-602">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="4a64d-603">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-603">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4a64d-604">Значение, указывающее поведение Adobe Reader при создании дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="4a64d-604">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="4a64d-605">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-605">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-606">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="4a64d-606">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="4a64d-607">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4a64d-607">String collection</span></span>|<span data-ttu-id="4a64d-608">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="4a64d-608">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="4a64d-609">Дефендероффицеаппсосерпроцессинжектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-609">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="4a64d-610">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-610">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4a64d-611">Значение, указывающее поведение приложений Office, добавляемых в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="4a64d-611">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="4a64d-612">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-612">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-613">Дефендероффицеаппсосерпроцессинжектион</span><span class="sxs-lookup"><span data-stu-id="4a64d-613">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="4a64d-614">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-614">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4a64d-615">Значение, указывающее поведение приложений Office, добавляемых в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="4a64d-615">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="4a64d-616">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-616">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-617">Дефендероффицекоммуникатионаппслаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="4a64d-617">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="4a64d-618">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-618">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4a64d-619">Значение, определяющее поведение приложений для связи с Office, включая Microsoft Outlook, от создания дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="4a64d-619">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="4a64d-620">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-620">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-621">Дефендероффицеаппсексекутаблеконтенткреатионорлаунчтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-621">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="4a64d-622">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-622">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4a64d-623">Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого контента.</span><span class="sxs-lookup"><span data-stu-id="4a64d-623">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="4a64d-624">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-624">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-625">Дефендероффицеаппсексекутаблеконтенткреатионорлаунч</span><span class="sxs-lookup"><span data-stu-id="4a64d-625">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="4a64d-626">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-626">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4a64d-627">Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого контента.</span><span class="sxs-lookup"><span data-stu-id="4a64d-627">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="4a64d-628">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-628">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-629">Дефендероффицеаппслаунччилдпроцесстипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-629">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="4a64d-630">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-630">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4a64d-631">Значение, указывающее поведение запуска приложения Office для дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="4a64d-631">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="4a64d-632">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-632">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-633">Дефендероффицеаппслаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="4a64d-633">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="4a64d-634">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-634">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4a64d-635">Значение, указывающее поведение запуска приложения Office для дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="4a64d-635">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="4a64d-636">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-636">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-637">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="4a64d-637">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="4a64d-638">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-638">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4a64d-639">Значение, указывающее поведение импорта Win32 из кода макросов в Office.</span><span class="sxs-lookup"><span data-stu-id="4a64d-639">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="4a64d-640">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-640">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-641">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="4a64d-641">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="4a64d-642">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-642">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4a64d-643">Значение, указывающее поведение импорта Win32 из кода макросов в Office.</span><span class="sxs-lookup"><span data-stu-id="4a64d-643">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="4a64d-644">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-644">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-645">Дефендерскриптобфускатедмакрокодетипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-645">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="4a64d-646">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-646">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4a64d-647">Значение, определяющее поведение кода "замаскированный JS/VBS/PS/макрос".</span><span class="sxs-lookup"><span data-stu-id="4a64d-647">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="4a64d-648">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-648">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-649">Дефендерскриптобфускатедмакрокоде</span><span class="sxs-lookup"><span data-stu-id="4a64d-649">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="4a64d-650">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-650">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4a64d-651">Значение, определяющее поведение кода "замаскированный JS/VBS/PS/макрос".</span><span class="sxs-lookup"><span data-stu-id="4a64d-651">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="4a64d-652">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-652">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-653">Дефендерскриптдовнлоадедпайлоадексекутионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-653">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="4a64d-654">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-654">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4a64d-655">Значение, определяющее поведение JS-и VBS-данных, загруженных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="4a64d-655">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="4a64d-656">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-656">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-657">Дефендерскриптдовнлоадедпайлоадексекутион</span><span class="sxs-lookup"><span data-stu-id="4a64d-657">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="4a64d-658">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-658">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4a64d-659">Значение, определяющее поведение JS-и VBS-данных, загруженных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="4a64d-659">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="4a64d-660">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-660">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-661">Дефендерпревенткредентиалстеалингтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-661">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="4a64d-662">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-662">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4a64d-663">Значение, указывающее, разрешено ли перенос учетных данных из подсистемы локального центра безопасности Windows.</span><span class="sxs-lookup"><span data-stu-id="4a64d-663">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="4a64d-664">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-664">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-665">Дефендерпроцесскреатионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-665">defenderProcessCreationType</span></span>|[<span data-ttu-id="4a64d-666">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-666">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4a64d-667">Значение, указывающее ответ на создание процессов, исходящих от команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="4a64d-667">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="4a64d-668">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-668">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-669">Дефендерпроцесскреатион</span><span class="sxs-lookup"><span data-stu-id="4a64d-669">defenderProcessCreation</span></span>|[<span data-ttu-id="4a64d-670">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-670">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4a64d-671">Значение, указывающее ответ на создание процессов, исходящих от команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="4a64d-671">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="4a64d-672">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-672">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-673">Дефендерунтрустедусбпроцесстипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-673">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="4a64d-674">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-674">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4a64d-675">Значение, указывающее ответ на недоверенные и неподписанные процессы, которые запускаются с USB.</span><span class="sxs-lookup"><span data-stu-id="4a64d-675">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="4a64d-676">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-676">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-677">Дефендерунтрустедусбпроцесс</span><span class="sxs-lookup"><span data-stu-id="4a64d-677">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="4a64d-678">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-678">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4a64d-679">Значение, указывающее ответ на недоверенные и неподписанные процессы, которые запускаются с USB.</span><span class="sxs-lookup"><span data-stu-id="4a64d-679">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="4a64d-680">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-680">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-681">Дефендерунтрустедексекутаблетипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-681">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="4a64d-682">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-682">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4a64d-683">Значение, указывающее ответ на исполняемые файлы, которые не отвечают условиям преобладание, возраст или доверенного списка.</span><span class="sxs-lookup"><span data-stu-id="4a64d-683">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="4a64d-684">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-684">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-685">Дефендерунтрустедексекутабле</span><span class="sxs-lookup"><span data-stu-id="4a64d-685">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="4a64d-686">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-686">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4a64d-687">Значение, указывающее ответ на исполняемые файлы, которые не отвечают условиям преобладание, возраст или доверенного списка.</span><span class="sxs-lookup"><span data-stu-id="4a64d-687">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="4a64d-688">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-688">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-689">Дефендеремаилконтентексекутионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-689">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="4a64d-690">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-690">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4a64d-691">Значение, указывающее, следует ли удалять исполняемые файлы (exe, DLL, PS, JS, VBS и т. д.) из электронной почты (почтовая или почтовая программа).</span><span class="sxs-lookup"><span data-stu-id="4a64d-691">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="4a64d-692">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-692">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-693">Дефендеремаилконтентексекутион</span><span class="sxs-lookup"><span data-stu-id="4a64d-693">defenderEmailContentExecution</span></span>|[<span data-ttu-id="4a64d-694">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-694">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4a64d-695">Значение, указывающее, следует ли удалять исполняемые файлы (exe, DLL, PS, JS, VBS и т. д.) из электронной почты (почтовая или почтовая программа).</span><span class="sxs-lookup"><span data-stu-id="4a64d-695">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="4a64d-696">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-696">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-697">Дефендерадванцедрансомеварепротектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-697">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="4a64d-698">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-698">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4a64d-699">Значение, указывающее на использование расширенной защиты в рансомеваре.</span><span class="sxs-lookup"><span data-stu-id="4a64d-699">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="4a64d-700">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-700">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-701">Дефендергуардмифолдерстипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-701">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="4a64d-702">Фолдерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-702">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="4a64d-703">Значение, указывающее поведение защищенных папок.</span><span class="sxs-lookup"><span data-stu-id="4a64d-703">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="4a64d-704">Возможные значения: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-704">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="4a64d-705">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="4a64d-705">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="4a64d-706">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4a64d-706">String collection</span></span>|<span data-ttu-id="4a64d-707">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="4a64d-707">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="4a64d-708">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="4a64d-708">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="4a64d-709">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4a64d-709">String collection</span></span>|<span data-ttu-id="4a64d-710">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="4a64d-710">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="4a64d-711">Дефендернетворкпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-711">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="4a64d-712">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-712">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4a64d-713">Значение, указывающее поведение Нетворкпротектион.</span><span class="sxs-lookup"><span data-stu-id="4a64d-713">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="4a64d-714">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-714">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4a64d-715">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="4a64d-715">defenderExploitProtectionXml</span></span>|<span data-ttu-id="4a64d-716">Binary</span><span class="sxs-lookup"><span data-stu-id="4a64d-716">Binary</span></span>|<span data-ttu-id="4a64d-717">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="4a64d-717">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="4a64d-718">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="4a64d-718">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="4a64d-719">String</span><span class="sxs-lookup"><span data-stu-id="4a64d-719">String</span></span>|<span data-ttu-id="4a64d-720">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="4a64d-720">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="4a64d-721">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="4a64d-721">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="4a64d-722">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-722">Boolean</span></span>|<span data-ttu-id="4a64d-723">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="4a64d-723">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="4a64d-724">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="4a64d-724">appLockerApplicationControl</span></span>|[<span data-ttu-id="4a64d-725">Апплоккераппликатионконтролтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-725">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="4a64d-726">Позволяет администратору выбирать разрешенные типы приложений для устройств.</span><span class="sxs-lookup"><span data-stu-id="4a64d-726">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="4a64d-727">Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-727">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="4a64d-728">Девицегуардлокалсистемаусоритикредентиалгуардсеттингс</span><span class="sxs-lookup"><span data-stu-id="4a64d-728">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="4a64d-729">Девицегуардлокалсистемаусоритикредентиалгуардтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-729">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="4a64d-730">Включите Guard в учетных данных, когда включен уровень безопасности платформы с безопасной загрузкой и безопасностью на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="4a64d-730">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="4a64d-731">Возможные значения: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-731">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="4a64d-732">Девицегуарденаблевиртуализатионбаседсекурити</span><span class="sxs-lookup"><span data-stu-id="4a64d-732">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="4a64d-733">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-733">Boolean</span></span>|<span data-ttu-id="4a64d-734">Включает безопасность на основе виртуализации (VBS).</span><span class="sxs-lookup"><span data-stu-id="4a64d-734">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="4a64d-735">Девицегуарденаблесекуребутвисдма</span><span class="sxs-lookup"><span data-stu-id="4a64d-735">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="4a64d-736">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-736">Boolean</span></span>|<span data-ttu-id="4a64d-737">Это свойство будет устаревшим в 2019 мая и будет заменено свойством Девицегуардсекуребутвисдма.</span><span class="sxs-lookup"><span data-stu-id="4a64d-737">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="4a64d-738">Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="4a64d-738">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="4a64d-739">Девицегуардсекуребутвисдма</span><span class="sxs-lookup"><span data-stu-id="4a64d-739">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="4a64d-740">Секуребутвисдматипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-740">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="4a64d-741">Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="4a64d-741">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="4a64d-742">Возможные значения: `notConfigured`, `withoutDMA`, `withDMA`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-742">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="4a64d-743">Девицегуардлаунчсистемгуард</span><span class="sxs-lookup"><span data-stu-id="4a64d-743">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="4a64d-744">Включение</span><span class="sxs-lookup"><span data-stu-id="4a64d-744">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4a64d-745">Позволяет ИТ – администратору настраивать запуск системы защиты системы.</span><span class="sxs-lookup"><span data-stu-id="4a64d-745">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="4a64d-746">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-746">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4a64d-747">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="4a64d-747">smartScreenEnableInShell</span></span>|<span data-ttu-id="4a64d-748">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-748">Boolean</span></span>|<span data-ttu-id="4a64d-749">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="4a64d-749">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="4a64d-750">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="4a64d-750">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="4a64d-751">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-751">Boolean</span></span>|<span data-ttu-id="4a64d-752">Позволяет ИТ – администраторам контролировать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="4a64d-752">Allows IT Admins to control whether users can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="4a64d-753">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="4a64d-753">applicationGuardEnabled</span></span>|<span data-ttu-id="4a64d-754">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-754">Boolean</span></span>|<span data-ttu-id="4a64d-755">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="4a64d-755">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="4a64d-756">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="4a64d-756">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="4a64d-757">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="4a64d-757">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="4a64d-758">Включение Application Guard в Защитнике Windows для более новых сборок Windows.</span><span class="sxs-lookup"><span data-stu-id="4a64d-758">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="4a64d-759">Возможные значения: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-759">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="4a64d-760">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="4a64d-760">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="4a64d-761">Аппликатионгуардблоккфилетрансфертипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-761">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="4a64d-762">Блокировать буфер обмена для передачи файла изображения, текстового файла или ни одного из них.</span><span class="sxs-lookup"><span data-stu-id="4a64d-762">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="4a64d-763">Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-763">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="4a64d-764">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="4a64d-764">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="4a64d-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-765">Boolean</span></span>|<span data-ttu-id="4a64d-766">Позволяет заблокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="4a64d-766">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="4a64d-767">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="4a64d-767">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="4a64d-768">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-768">Boolean</span></span>|<span data-ttu-id="4a64d-769">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="4a64d-769">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="4a64d-770">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="4a64d-770">applicationGuardForceAuditing</span></span>|<span data-ttu-id="4a64d-771">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-771">Boolean</span></span>|<span data-ttu-id="4a64d-772">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="4a64d-772">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="4a64d-773">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="4a64d-773">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="4a64d-774">Аппликатионгуардблоккклипбоардшарингтипе</span><span class="sxs-lookup"><span data-stu-id="4a64d-774">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="4a64d-775">Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="4a64d-775">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="4a64d-776">Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="4a64d-776">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="4a64d-777">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="4a64d-777">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="4a64d-778">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-778">Boolean</span></span>|<span data-ttu-id="4a64d-779">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="4a64d-779">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="4a64d-780">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="4a64d-780">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="4a64d-781">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-781">Boolean</span></span>|<span data-ttu-id="4a64d-782">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="4a64d-782">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="4a64d-783">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="4a64d-783">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="4a64d-784">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-784">Boolean</span></span>|<span data-ttu-id="4a64d-785">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="4a64d-785">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="4a64d-786">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="4a64d-786">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="4a64d-787">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-787">Boolean</span></span>|<span data-ttu-id="4a64d-788">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="4a64d-788">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="4a64d-789">Аппликатионгуардалловвиртуалгпу</span><span class="sxs-lookup"><span data-stu-id="4a64d-789">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="4a64d-790">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-790">Boolean</span></span>|<span data-ttu-id="4a64d-791">Разрешить приложению Application Guard использовать виртуальный GPU</span><span class="sxs-lookup"><span data-stu-id="4a64d-791">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="4a64d-792">Аппликатионгуардалловфилесавеонхост</span><span class="sxs-lookup"><span data-stu-id="4a64d-792">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="4a64d-793">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-793">Boolean</span></span>|<span data-ttu-id="4a64d-794">Разрешить пользователям скачивать файлы из EDGE в контейнере Application Guard и сохранять их в файловой системе узла</span><span class="sxs-lookup"><span data-stu-id="4a64d-794">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="4a64d-795">Битлоккералловстандардусеренкриптион</span><span class="sxs-lookup"><span data-stu-id="4a64d-795">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="4a64d-796">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-796">Boolean</span></span>|<span data-ttu-id="4a64d-797">Позволяет администратору разрешить обычным пользователям включать енкрпитион во время присоединения к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4a64d-797">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="4a64d-798">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="4a64d-798">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="4a64d-799">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-799">Boolean</span></span>|<span data-ttu-id="4a64d-800">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="4a64d-800">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="4a64d-801">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="4a64d-801">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="4a64d-802">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-802">Boolean</span></span>|<span data-ttu-id="4a64d-803">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="4a64d-803">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="4a64d-804">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="4a64d-804">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="4a64d-805">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="4a64d-805">bitLockerEncryptDevice</span></span>|<span data-ttu-id="4a64d-806">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a64d-806">Boolean</span></span>|<span data-ttu-id="4a64d-807">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="4a64d-807">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="4a64d-808">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="4a64d-808">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="4a64d-809">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="4a64d-809">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="4a64d-810">Политика системного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="4a64d-810">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="4a64d-811">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="4a64d-811">bitLockerFixedDrivePolicy</span></span>|<span data-ttu-id="4a64d-812">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md);</span><span class="sxs-lookup"><span data-stu-id="4a64d-812">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)</span></span>|<span data-ttu-id="4a64d-813">Политика фиксированного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="4a64d-813">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="4a64d-814">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="4a64d-814">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="4a64d-815">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="4a64d-815">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="4a64d-816">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="4a64d-816">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="4a64d-817">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a64d-817">Response</span></span>
<span data-ttu-id="4a64d-818">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4a64d-818">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a64d-819">Пример</span><span class="sxs-lookup"><span data-stu-id="4a64d-819">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a64d-820">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a64d-820">Request</span></span>
<span data-ttu-id="4a64d-821">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a64d-821">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 28463

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
  "userRightsRegisterProcessAsService": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="4a64d-822">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a64d-822">Response</span></span>
<span data-ttu-id="4a64d-p204">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a64d-p204">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 28635

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
  "userRightsRegisterProcessAsService": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
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
  }
}
```





