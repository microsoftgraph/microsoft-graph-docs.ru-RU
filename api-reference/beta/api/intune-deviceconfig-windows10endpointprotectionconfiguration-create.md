---
title: Создание windows10EndpointProtectionConfiguration
description: Создание объекта windows10EndpointProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6080578ae14d0446ca725247be6baa9d7633058e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976938"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="47394-103">Создание windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="47394-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="47394-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47394-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47394-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47394-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47394-106">Создание объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47394-106">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47394-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="47394-107">Prerequisites</span></span>
<span data-ttu-id="47394-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47394-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47394-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47394-110">Permission type</span></span>|<span data-ttu-id="47394-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47394-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47394-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47394-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47394-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47394-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47394-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47394-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47394-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47394-115">Not supported.</span></span>|
|<span data-ttu-id="47394-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47394-116">Application</span></span>|<span data-ttu-id="47394-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47394-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47394-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47394-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="47394-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47394-119">Request headers</span></span>
|<span data-ttu-id="47394-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47394-120">Header</span></span>|<span data-ttu-id="47394-121">Значение</span><span class="sxs-lookup"><span data-stu-id="47394-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47394-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47394-122">Authorization</span></span>|<span data-ttu-id="47394-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47394-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47394-124">Accept</span><span class="sxs-lookup"><span data-stu-id="47394-124">Accept</span></span>|<span data-ttu-id="47394-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47394-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47394-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="47394-126">Request body</span></span>
<span data-ttu-id="47394-127">В теле запроса добавьте представление объекта windows10EndpointProtectionConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47394-127">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="47394-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="47394-128">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="47394-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="47394-129">Property</span></span>|<span data-ttu-id="47394-130">Тип</span><span class="sxs-lookup"><span data-stu-id="47394-130">Type</span></span>|<span data-ttu-id="47394-131">Описание</span><span class="sxs-lookup"><span data-stu-id="47394-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47394-132">id</span><span class="sxs-lookup"><span data-stu-id="47394-132">id</span></span>|<span data-ttu-id="47394-133">String</span><span class="sxs-lookup"><span data-stu-id="47394-133">String</span></span>|<span data-ttu-id="47394-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="47394-134">Key of the entity.</span></span> <span data-ttu-id="47394-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47394-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47394-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47394-136">lastModifiedDateTime</span></span>|<span data-ttu-id="47394-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47394-137">DateTimeOffset</span></span>|<span data-ttu-id="47394-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="47394-138">DateTime the object was last modified.</span></span> <span data-ttu-id="47394-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47394-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47394-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="47394-140">roleScopeTagIds</span></span>|<span data-ttu-id="47394-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="47394-141">String collection</span></span>|<span data-ttu-id="47394-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="47394-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="47394-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47394-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47394-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="47394-144">supportsScopeTags</span></span>|<span data-ttu-id="47394-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-145">Boolean</span></span>|<span data-ttu-id="47394-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="47394-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="47394-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="47394-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="47394-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="47394-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="47394-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47394-149">This property is read-only.</span></span> <span data-ttu-id="47394-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47394-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47394-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="47394-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="47394-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="47394-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="47394-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="47394-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="47394-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47394-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47394-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="47394-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="47394-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="47394-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="47394-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="47394-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="47394-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47394-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47394-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="47394-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="47394-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="47394-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="47394-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="47394-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="47394-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47394-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47394-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47394-163">createdDateTime</span></span>|<span data-ttu-id="47394-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47394-164">DateTimeOffset</span></span>|<span data-ttu-id="47394-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="47394-165">DateTime the object was created.</span></span> <span data-ttu-id="47394-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47394-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47394-167">description</span><span class="sxs-lookup"><span data-stu-id="47394-167">description</span></span>|<span data-ttu-id="47394-168">String</span><span class="sxs-lookup"><span data-stu-id="47394-168">String</span></span>|<span data-ttu-id="47394-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="47394-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="47394-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47394-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47394-171">displayName</span><span class="sxs-lookup"><span data-stu-id="47394-171">displayName</span></span>|<span data-ttu-id="47394-172">Строка</span><span class="sxs-lookup"><span data-stu-id="47394-172">String</span></span>|<span data-ttu-id="47394-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="47394-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="47394-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47394-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47394-175">version</span><span class="sxs-lookup"><span data-stu-id="47394-175">version</span></span>|<span data-ttu-id="47394-176">Int32</span><span class="sxs-lookup"><span data-stu-id="47394-176">Int32</span></span>|<span data-ttu-id="47394-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="47394-177">Version of the device configuration.</span></span> <span data-ttu-id="47394-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47394-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47394-179">Дмагуарддевицеенумератионполици</span><span class="sxs-lookup"><span data-stu-id="47394-179">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="47394-180">Дмагуарддевицеенумератионполицитипе</span><span class="sxs-lookup"><span data-stu-id="47394-180">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="47394-181">Эта политика предназначена для обеспечения дополнительной защиты от внешних устройств с поддержкой прямого доступа к памяти.</span><span class="sxs-lookup"><span data-stu-id="47394-181">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="47394-182">Он обеспечивает более полный контроль над перечислением устройств с поддержкой внешних устройств с поддержкой прямого доступа к памяти, несовместимых с пересопоставлением и изоляцией памяти устройств и изолированной средой.</span><span class="sxs-lookup"><span data-stu-id="47394-182">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="47394-183">Эта политика вступает в силу только тогда, когда система защиты DMA поддерживается и включена встроенным встроенным по.</span><span class="sxs-lookup"><span data-stu-id="47394-183">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="47394-184">Защита от DMA ядра — это компонент платформы, который невозможно контролировать с помощью политики или конечным пользователем.</span><span class="sxs-lookup"><span data-stu-id="47394-184">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="47394-185">Она должна поддерживаться системой на момент производства.</span><span class="sxs-lookup"><span data-stu-id="47394-185">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="47394-186">Чтобы проверить, поддерживает ли система защиту DMA, проверьте поле Защита ядра DMA на странице Сводка объекта MSINFO32. exe.</span><span class="sxs-lookup"><span data-stu-id="47394-186">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="47394-187">Возможные значения: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="47394-187">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="47394-188">Фиреваллрулес</span><span class="sxs-lookup"><span data-stu-id="47394-188">firewallRules</span></span>|<span data-ttu-id="47394-189">Коллекция [виндовсфиреваллруле](../resources/intune-deviceconfig-windowsfirewallrule.md)</span><span class="sxs-lookup"><span data-stu-id="47394-189">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="47394-190">Настраивает параметры правила брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="47394-190">Configures the firewall rule settings.</span></span> <span data-ttu-id="47394-191">Эта коллекция может содержать не более 150 элементов.</span><span class="sxs-lookup"><span data-stu-id="47394-191">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="47394-192">Усерригхтсакцесскредентиалманажераструстедкаллер</span><span class="sxs-lookup"><span data-stu-id="47394-192">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="47394-193">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-193">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-194">Это право пользователя используется диспетчером учетных данных во время резервного копирования и восстановления.</span><span class="sxs-lookup"><span data-stu-id="47394-194">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="47394-195">Сохраненные учетные данные пользователей могут быть скомпрометированы, если эта привилегия передана другим субъектам.</span><span class="sxs-lookup"><span data-stu-id="47394-195">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="47394-196">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-196">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="47394-197">Усерригхтсалловакцессфромнетворк</span><span class="sxs-lookup"><span data-stu-id="47394-197">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="47394-198">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-198">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-199">Это право пользователя определяет, какие пользователи и группы могут подключаться к компьютеру через сеть.</span><span class="sxs-lookup"><span data-stu-id="47394-199">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="47394-200">Допустимое состояние — Supported.</span><span class="sxs-lookup"><span data-stu-id="47394-200">State Allowed is supported.</span></span>|
|<span data-ttu-id="47394-201">Усерригхтсблоккакцессфромнетворк</span><span class="sxs-lookup"><span data-stu-id="47394-201">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="47394-202">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-202">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-203">Это право пользователя определяет, каким пользователям и группам запрещается подключаться к компьютеру через сеть.</span><span class="sxs-lookup"><span data-stu-id="47394-203">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="47394-204">Блок состояния поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47394-204">State Block is supported.</span></span>|
|<span data-ttu-id="47394-205">Усерригхтсактаспартофсеоператингсистем</span><span class="sxs-lookup"><span data-stu-id="47394-205">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="47394-206">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-206">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-207">Это право пользователя позволяет процессу олицетворять любого пользователя без проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="47394-207">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="47394-208">Таким образом, процесс может получить доступ к тем же локальным ресурсам, что и пользователь.</span><span class="sxs-lookup"><span data-stu-id="47394-208">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="47394-209">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="47394-210">Усерригхтслокаллогон</span><span class="sxs-lookup"><span data-stu-id="47394-210">userRightsLocalLogOn</span></span>|[<span data-ttu-id="47394-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-212">Это право пользователя определяет, какие пользователи могут входить на компьютер.</span><span class="sxs-lookup"><span data-stu-id="47394-212">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="47394-213">Допустимые состояния NotConfigured, Поддерживаемые</span><span class="sxs-lookup"><span data-stu-id="47394-213">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="47394-214">Усерригхтсденилокаллогон</span><span class="sxs-lookup"><span data-stu-id="47394-214">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="47394-215">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-215">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-216">Это право пользователя определяет, какие пользователи не могут войти на компьютер.</span><span class="sxs-lookup"><span data-stu-id="47394-216">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="47394-217">Состояния NotConfigured, блокировки поддерживаются</span><span class="sxs-lookup"><span data-stu-id="47394-217">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="47394-218">Усерригхтсбаккупдата</span><span class="sxs-lookup"><span data-stu-id="47394-218">userRightsBackupData</span></span>|[<span data-ttu-id="47394-219">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-219">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-220">Это право пользователя определяет, какие пользователи могут обходить разрешения для файлов, каталогов, реестра и других постоянных объектов при резервном копировании файлов и каталогов.</span><span class="sxs-lookup"><span data-stu-id="47394-220">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="47394-221">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-221">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="47394-222">Усерригхтсчанжесистемтиме</span><span class="sxs-lookup"><span data-stu-id="47394-222">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="47394-223">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-223">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-224">Это право пользователя определяет, какие пользователи и группы могут изменять время и дату на внутреннем часовом компьютере.</span><span class="sxs-lookup"><span data-stu-id="47394-224">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="47394-225">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-225">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="47394-226">Усерригхтскреатеглобалобжектс</span><span class="sxs-lookup"><span data-stu-id="47394-226">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="47394-227">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-227">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-228">Этот параметр безопасности определяет, могут ли пользователи создавать глобальные объекты, доступные для всех сеансов.</span><span class="sxs-lookup"><span data-stu-id="47394-228">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="47394-229">Пользователи, которые могут создавать глобальные объекты, могут повлиять на процессы, выполняемые в сеансах других пользователей, что может привести к сбою приложения или повреждению данных.</span><span class="sxs-lookup"><span data-stu-id="47394-229">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="47394-230">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="47394-231">Усерригхтскреатепажефиле</span><span class="sxs-lookup"><span data-stu-id="47394-231">userRightsCreatePageFile</span></span>|[<span data-ttu-id="47394-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-233">Это право пользователя определяет, какие пользователи и группы могут вызывать внутренний API, чтобы создать и изменить размер файла подкачки.</span><span class="sxs-lookup"><span data-stu-id="47394-233">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="47394-234">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="47394-235">Усерригхтскреатеперманентшаредобжектс</span><span class="sxs-lookup"><span data-stu-id="47394-235">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="47394-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-237">Это право пользователя определяет, какие учетные записи могут использоваться процессами для создания объекта каталога с помощью диспетчера объектов.</span><span class="sxs-lookup"><span data-stu-id="47394-237">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="47394-238">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-238">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="47394-239">Усерригхтскреатесимболиклинкс</span><span class="sxs-lookup"><span data-stu-id="47394-239">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="47394-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-241">Это право пользователя определяет, может ли пользователь создать символическую ссылку с компьютера, на который они входили.</span><span class="sxs-lookup"><span data-stu-id="47394-241">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="47394-242">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-242">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="47394-243">Усерригхтскреатетокен</span><span class="sxs-lookup"><span data-stu-id="47394-243">userRightsCreateToken</span></span>|[<span data-ttu-id="47394-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-245">Это право пользователя определяет, какие пользователи и группы могут использоваться процессами для создания маркера, который можно использовать для получения доступа к любому локальному ресурсу, когда процесс использует внутренний API для создания маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="47394-245">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="47394-246">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-246">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="47394-247">Усерригхтсдебугпрограмс</span><span class="sxs-lookup"><span data-stu-id="47394-247">userRightsDebugPrograms</span></span>|[<span data-ttu-id="47394-248">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-248">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-249">Это право пользователя определяет, какие пользователи могут прикреплять отладчик к любому процессу или ядру.</span><span class="sxs-lookup"><span data-stu-id="47394-249">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="47394-250">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-250">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="47394-251">Усерригхтсремотедесктопсервицеслогон</span><span class="sxs-lookup"><span data-stu-id="47394-251">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="47394-252">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-252">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-253">Это право пользователя определяет, каким пользователям и группам запрещается вход в систему в качестве клиента служб удаленных рабочих столов.</span><span class="sxs-lookup"><span data-stu-id="47394-253">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="47394-254">Поддерживаются только состояния NotConfigured и Block</span><span class="sxs-lookup"><span data-stu-id="47394-254">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="47394-255">Усерригхтсделегатион</span><span class="sxs-lookup"><span data-stu-id="47394-255">userRightsDelegation</span></span>|[<span data-ttu-id="47394-256">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-256">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-257">Это право пользователя определяет, какие пользователи могут устанавливать параметр "доверять для делегирования" для объекта пользователя или компьютера.</span><span class="sxs-lookup"><span data-stu-id="47394-257">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="47394-258">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-258">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="47394-259">Усерригхтсженератесекуритяудитс</span><span class="sxs-lookup"><span data-stu-id="47394-259">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="47394-260">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-260">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-261">Это право пользователя определяет, какие учетные записи могут использоваться процессом для добавления записей в журнал безопасности.</span><span class="sxs-lookup"><span data-stu-id="47394-261">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="47394-262">Журнал безопасности используется для трассировки несанкционированного доступа к системе.</span><span class="sxs-lookup"><span data-stu-id="47394-262">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="47394-263">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-263">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="47394-264">Усерригхтсимперсонатеклиент</span><span class="sxs-lookup"><span data-stu-id="47394-264">userRightsImpersonateClient</span></span>|[<span data-ttu-id="47394-265">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-265">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-266">Назначение этого права пользователю позволяет программам, выполняемым от имени этого пользователя, олицетворять клиента.</span><span class="sxs-lookup"><span data-stu-id="47394-266">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="47394-267">Требование этого пользователя для такого рода олицетворения запрещает несанкционированному пользователю подключаться к созданной им службе, а затем олицетворять этого клиента, что может повысить уровень разрешений неавторизованного пользователя до Уровни администрирования или системы.</span><span class="sxs-lookup"><span data-stu-id="47394-267">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="47394-268">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="47394-269">Усерригхтсинкреасесчедулингприорити</span><span class="sxs-lookup"><span data-stu-id="47394-269">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="47394-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-271">Это право пользователя определяет, какие учетные записи могут использовать процесс с доступом к свойствам Write для другого процесса, чтобы увеличить приоритет выполнения, назначенный другому процессу.</span><span class="sxs-lookup"><span data-stu-id="47394-271">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="47394-272">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="47394-273">Усерригхтслоадунлоаддриверс</span><span class="sxs-lookup"><span data-stu-id="47394-273">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="47394-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-275">Это право пользователя определяет, какие пользователи могут динамически загружать и выгружать драйверы устройств или другой код в режиме ядра.</span><span class="sxs-lookup"><span data-stu-id="47394-275">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="47394-276">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="47394-277">Усерригхтслоккмемори</span><span class="sxs-lookup"><span data-stu-id="47394-277">userRightsLockMemory</span></span>|[<span data-ttu-id="47394-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-279">Это право пользователя определяет, какие учетные записи могут использовать процесс для хранения данных в физической памяти, что предотвращает их разбиение данных на виртуальную память на диске.</span><span class="sxs-lookup"><span data-stu-id="47394-279">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="47394-280">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="47394-281">Усерригхтсманажеаудитингандсекуритилогс</span><span class="sxs-lookup"><span data-stu-id="47394-281">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="47394-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-283">Это право пользователя определяет, какие пользователи могут задавать параметры аудита доступа к объектам для отдельных ресурсов, таких как файлы, объекты Active Directory и разделы реестра.</span><span class="sxs-lookup"><span data-stu-id="47394-283">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="47394-284">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="47394-285">Усерригхтсманажеволумес</span><span class="sxs-lookup"><span data-stu-id="47394-285">userRightsManageVolumes</span></span>|[<span data-ttu-id="47394-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-287">Это право пользователя определяет, какие пользователи и группы могут выполнять задачи обслуживания для тома, такие как удаленная дефрагментация.</span><span class="sxs-lookup"><span data-stu-id="47394-287">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="47394-288">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-288">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="47394-289">Усерригхтсмодифифирмваринвиронмент</span><span class="sxs-lookup"><span data-stu-id="47394-289">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="47394-290">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-290">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-291">Это право пользователя определяет, кто может изменять значения в аппаратной среде.</span><span class="sxs-lookup"><span data-stu-id="47394-291">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="47394-292">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-292">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="47394-293">Усерригхтсмодифйобжектлабелс</span><span class="sxs-lookup"><span data-stu-id="47394-293">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="47394-294">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-294">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-295">Это право пользователя определяет, какие учетные записи пользователей могут изменять метки целостности объектов, таких как файлы, разделы реестра или процессы, принадлежащие другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="47394-295">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="47394-296">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-296">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="47394-297">Усерригхтспрофилесинглепроцесс</span><span class="sxs-lookup"><span data-stu-id="47394-297">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="47394-298">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-298">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-299">Это право пользователя определяет, какие пользователи могут использовать средства мониторинга производительности для наблюдения за производительностью системных процессов.</span><span class="sxs-lookup"><span data-stu-id="47394-299">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="47394-300">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-300">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="47394-301">Усерригхтсремотешутдовн</span><span class="sxs-lookup"><span data-stu-id="47394-301">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="47394-302">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-302">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-303">Это право пользователя определяет, каким пользователям разрешено завершать работу компьютера из удаленного расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="47394-303">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="47394-304">Неправильное использование этого права пользователя может привести к отказу в обслуживании.</span><span class="sxs-lookup"><span data-stu-id="47394-304">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="47394-305">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-305">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="47394-306">Усерригхтсресторедата</span><span class="sxs-lookup"><span data-stu-id="47394-306">userRightsRestoreData</span></span>|[<span data-ttu-id="47394-307">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-307">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-308">Это право пользователя определяет, какие пользователи могут обходить разрешения для файлов, каталогов, реестра и других постоянных объектов при восстановлении резервных копий файлов и каталогов, и определяет, какие пользователи могут устанавливать любой действительный субъект безопасности в качестве владельца объекта.</span><span class="sxs-lookup"><span data-stu-id="47394-308">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="47394-309">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-309">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="47394-310">Усерригхтстакеовнершип</span><span class="sxs-lookup"><span data-stu-id="47394-310">userRightsTakeOwnership</span></span>|[<span data-ttu-id="47394-311">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-311">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-312">Это право пользователя определяет, какие пользователи могут становиться владельцами любого защищаемого объекта в системе, включая объекты Active Directory, файлы и папки, принтеры, разделы реестра, процессы и потоки.</span><span class="sxs-lookup"><span data-stu-id="47394-312">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="47394-313">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="47394-313">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="47394-314">Усерригхтсрегистерпроцессассервице</span><span class="sxs-lookup"><span data-stu-id="47394-314">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="47394-315">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="47394-315">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="47394-316">Этот параметр безопасности определяет, каким учетным записям служб запрещается регистрировать процесс в качестве службы.</span><span class="sxs-lookup"><span data-stu-id="47394-316">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="47394-317">Примечание: этот параметр безопасности не применяется к системным, локальным или сетевым учетным записям служб.</span><span class="sxs-lookup"><span data-stu-id="47394-317">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="47394-318">Поддерживается только блокирование состояния.</span><span class="sxs-lookup"><span data-stu-id="47394-318">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="47394-319">Ксбокссервицесенаблексбоксгамесаветаск</span><span class="sxs-lookup"><span data-stu-id="47394-319">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="47394-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-320">Boolean</span></span>|<span data-ttu-id="47394-321">Этот параметр определяет, включена ли функция сохранения игры Xbox (1) или отключена (0).</span><span class="sxs-lookup"><span data-stu-id="47394-321">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="47394-322">Ксбокссервицесакцессориманажементсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="47394-322">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="47394-323">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="47394-323">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="47394-324">Этот параметр определяет, является ли тип запуска службы управления принадлежностью автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="47394-324">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="47394-325">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="47394-325">Default: Manual.</span></span> <span data-ttu-id="47394-326">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="47394-326">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="47394-327">Ксбокссервицесливеаусманажерсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="47394-327">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="47394-328">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="47394-328">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="47394-329">Этот параметр определяет, является ли тип запуска службы диспетчера Live auth автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="47394-329">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="47394-330">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="47394-330">Default: Manual.</span></span> <span data-ttu-id="47394-331">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="47394-331">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="47394-332">Ксбокссервицесливегамесавесервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="47394-332">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="47394-333">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="47394-333">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="47394-334">Этот параметр определяет, является ли тип запуска службы Live Save Service автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="47394-334">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="47394-335">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="47394-335">Default: Manual.</span></span> <span data-ttu-id="47394-336">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="47394-336">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="47394-337">Ксбокссервицесливенетворкингсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="47394-337">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="47394-338">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="47394-338">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="47394-339">Этот параметр определяет, является ли тип запуска сетевой службы автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="47394-339">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="47394-340">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="47394-340">Default: Manual.</span></span> <span data-ttu-id="47394-341">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="47394-341">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="47394-342">Локалсекуритйоптионсблоккмикрософтаккаунтс</span><span class="sxs-lookup"><span data-stu-id="47394-342">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="47394-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-343">Boolean</span></span>|<span data-ttu-id="47394-344">Запретить пользователям добавлять новые учетные записи Майкрософт на этот компьютер.</span><span class="sxs-lookup"><span data-stu-id="47394-344">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="47394-345">Локалсекуритйоптионсблоккремотелогонвисбланкпассворд</span><span class="sxs-lookup"><span data-stu-id="47394-345">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="47394-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-346">Boolean</span></span>|<span data-ttu-id="47394-347">Включите локальные учетные записи, не защищенные паролем, для входа в систему из расположений, отличных от физического устройства. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="47394-347">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="47394-348">Локалсекуритйоптионсдисаблеадминистратораккаунт</span><span class="sxs-lookup"><span data-stu-id="47394-348">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="47394-349">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-349">Boolean</span></span>|<span data-ttu-id="47394-350">Определяет, включена или отключена учетная запись локального администратора.</span><span class="sxs-lookup"><span data-stu-id="47394-350">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="47394-351">Локалсекуритйоптионсадминистратораккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="47394-351">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="47394-352">String</span><span class="sxs-lookup"><span data-stu-id="47394-352">String</span></span>|<span data-ttu-id="47394-353">Определите имя другой учетной записи, которая будет связана с идентификатором безопасности (SID) учетной записи "Administrator".</span><span class="sxs-lookup"><span data-stu-id="47394-353">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="47394-354">Локалсекуритйоптионсдисаблегуестаккаунт</span><span class="sxs-lookup"><span data-stu-id="47394-354">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="47394-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-355">Boolean</span></span>|<span data-ttu-id="47394-356">Определяет, включена или отключена Гостевая учетная запись.</span><span class="sxs-lookup"><span data-stu-id="47394-356">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="47394-357">Локалсекуритйоптионсгуестаккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="47394-357">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="47394-358">String</span><span class="sxs-lookup"><span data-stu-id="47394-358">String</span></span>|<span data-ttu-id="47394-359">Определите имя другой учетной записи, которая будет связана с идентификатором безопасности (SID) для учетной записи "гость".</span><span class="sxs-lookup"><span data-stu-id="47394-359">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="47394-360">Локалсекуритйоптионсалловундокквисаусавингтологон</span><span class="sxs-lookup"><span data-stu-id="47394-360">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="47394-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-361">Boolean</span></span>|<span data-ttu-id="47394-362">Запретите отстыковку портативного компьютера без необходимости входа в систему.</span><span class="sxs-lookup"><span data-stu-id="47394-362">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="47394-363">Локалсекуритйоптионсблоккусерсинсталлингпринтердриверс</span><span class="sxs-lookup"><span data-stu-id="47394-363">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="47394-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-364">Boolean</span></span>|<span data-ttu-id="47394-365">Ограничьте установку драйверов принтеров в рамках подключения к общему принтеру только для администраторов.</span><span class="sxs-lookup"><span data-stu-id="47394-365">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="47394-366">Локалсекуритйоптионсблоккремотеоптикалдривеакцесс</span><span class="sxs-lookup"><span data-stu-id="47394-366">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="47394-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-367">Boolean</span></span>|<span data-ttu-id="47394-368">Включение этого параметра позволяет интерактивно вошедший в систему пользователь получать доступ к устройству чтения компакт-дисков.</span><span class="sxs-lookup"><span data-stu-id="47394-368">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="47394-369">Локалсекуритйоптионсформатандежектофремоваблемедиаалловедусер</span><span class="sxs-lookup"><span data-stu-id="47394-369">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="47394-370">Локалсекуритйоптионсформатандежектофремоваблемедиаалловедусертипе</span><span class="sxs-lookup"><span data-stu-id="47394-370">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="47394-371">Определите, кому разрешено форматировать и извлекать съемные носители NTFS.</span><span class="sxs-lookup"><span data-stu-id="47394-371">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="47394-372">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="47394-372">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="47394-373">Локалсекуритйоптионсмачинеинактивитилимит</span><span class="sxs-lookup"><span data-stu-id="47394-373">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="47394-374">Int32</span><span class="sxs-lookup"><span data-stu-id="47394-374">Int32</span></span>|<span data-ttu-id="47394-375">Определите максимальное количество минут отсутствия активности на экране входа интерактивного рабочего стола, пока не запустится экранная заставка.</span><span class="sxs-lookup"><span data-stu-id="47394-375">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="47394-376">Допустимые значения — от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="47394-376">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="47394-377">Локалсекуритйоптионсмачинеинактивитилимитинминутес</span><span class="sxs-lookup"><span data-stu-id="47394-377">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="47394-378">Int32</span><span class="sxs-lookup"><span data-stu-id="47394-378">Int32</span></span>|<span data-ttu-id="47394-379">Определите максимальное количество минут отсутствия активности на экране входа интерактивного рабочего стола, пока не запустится экранная заставка.</span><span class="sxs-lookup"><span data-stu-id="47394-379">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="47394-380">Допустимые значения — от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="47394-380">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="47394-381">Локалсекуритйоптионсдонотрекуиректрлалтдел</span><span class="sxs-lookup"><span data-stu-id="47394-381">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="47394-382">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-382">Boolean</span></span>|<span data-ttu-id="47394-383">Требовать нажатия клавиш CTRL + ALT + DEL, прежде чем пользователь сможет войти в систему.</span><span class="sxs-lookup"><span data-stu-id="47394-383">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="47394-384">Локалсекуритйоптионшиделастсигнединусер</span><span class="sxs-lookup"><span data-stu-id="47394-384">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="47394-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-385">Boolean</span></span>|<span data-ttu-id="47394-386">Не отображать имя последнего пользователя, выполнившего вход на это устройство.</span><span class="sxs-lookup"><span data-stu-id="47394-386">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="47394-387">Локалсекуритйоптионшидеусернамеатсигнин</span><span class="sxs-lookup"><span data-stu-id="47394-387">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="47394-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-388">Boolean</span></span>|<span data-ttu-id="47394-389">Не отображать имя пользователя, выполняющего вход на это устройство, после ввода учетных данных и отображения рабочего стола на устройстве.</span><span class="sxs-lookup"><span data-stu-id="47394-389">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="47394-390">Локалсекуритйоптионслогонмессажетитле</span><span class="sxs-lookup"><span data-stu-id="47394-390">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="47394-391">String</span><span class="sxs-lookup"><span data-stu-id="47394-391">String</span></span>|<span data-ttu-id="47394-392">Задайте заголовок сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="47394-392">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="47394-393">Локалсекуритйоптионслогонмессажетекст</span><span class="sxs-lookup"><span data-stu-id="47394-393">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="47394-394">String</span><span class="sxs-lookup"><span data-stu-id="47394-394">String</span></span>|<span data-ttu-id="47394-395">Задайте текст сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="47394-395">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="47394-396">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="47394-396">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="47394-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-397">Boolean</span></span>|<span data-ttu-id="47394-398">Блокировать запросы проверки подлинности PKU2U на этом устройстве для использования сетевых удостоверений.</span><span class="sxs-lookup"><span data-stu-id="47394-398">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="47394-399">Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажерхелпербул</span><span class="sxs-lookup"><span data-stu-id="47394-399">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="47394-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-400">Boolean</span></span>|<span data-ttu-id="47394-401">Помощник по пользовательскому интерфейсу Boolean для объекта Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажер</span><span class="sxs-lookup"><span data-stu-id="47394-401">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="47394-402">Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажер</span><span class="sxs-lookup"><span data-stu-id="47394-402">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="47394-403">String</span><span class="sxs-lookup"><span data-stu-id="47394-403">String</span></span>|<span data-ttu-id="47394-404">Измените строку языка определения дескрипторов безопасности по умолчанию, чтобы разрешить или запретить пользователям и группам совершать удаленные вызовы в SAM.</span><span class="sxs-lookup"><span data-stu-id="47394-404">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="47394-405">Локалсекуритйоптионсминимумсессионсекуритифорнтлмсспбаседклиентс</span><span class="sxs-lookup"><span data-stu-id="47394-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="47394-406">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="47394-406">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="47394-407">Этот параметр безопасности позволяет клиенту требовать согласование 128-разрядного шифрования и/или сеанса защиты сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="47394-407">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="47394-408">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="47394-408">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="47394-409">Локалсекуритйоптионсминимумсессионсекуритифорнтлмсспбаседсерверс</span><span class="sxs-lookup"><span data-stu-id="47394-409">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="47394-410">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="47394-410">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="47394-411">Этот параметр безопасности позволяет серверу требовать согласование 128-разрядного шифрования и/или сеанса защиты сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="47394-411">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="47394-412">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="47394-412">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="47394-413">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="47394-413">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="47394-414">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="47394-414">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="47394-415">Этот параметр безопасности определяет, какой протокол проверки подлинности "запрос/ответ" используется для входа в сеть.</span><span class="sxs-lookup"><span data-stu-id="47394-415">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="47394-416">Возможные значения: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="47394-416">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="47394-417">Ланманажерворкстатиондисаблеинсекурегуестлогонс</span><span class="sxs-lookup"><span data-stu-id="47394-417">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="47394-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-418">Boolean</span></span>|<span data-ttu-id="47394-419">Если этот параметр включен, клиент SMB будет разрешать небезопасные гостевые входы.</span><span class="sxs-lookup"><span data-stu-id="47394-419">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="47394-420">Если этот параметр не настроен, клиент SMB будет отклонять небезопасные гостевые входы.</span><span class="sxs-lookup"><span data-stu-id="47394-420">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="47394-421">Локалсекуритйоптионсклеарвиртуалмеморипажефиле</span><span class="sxs-lookup"><span data-stu-id="47394-421">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="47394-422">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-422">Boolean</span></span>|<span data-ttu-id="47394-423">Этот параметр безопасности определяет, будет ли очищаться файл подкачки виртуальной памяти при завершении работы системы.</span><span class="sxs-lookup"><span data-stu-id="47394-423">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="47394-424">Локалсекуритйоптионсалловсистемтобешутдовнвисаусавингтологон</span><span class="sxs-lookup"><span data-stu-id="47394-424">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="47394-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-425">Boolean</span></span>|<span data-ttu-id="47394-426">Этот параметр безопасности определяет, можно ли завершить работу компьютера, не выполняя вход в Windows.</span><span class="sxs-lookup"><span data-stu-id="47394-426">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="47394-427">Локалсекуритйоптионсалловуиакцессаппликатионелеватион</span><span class="sxs-lookup"><span data-stu-id="47394-427">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="47394-428">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-428">Boolean</span></span>|<span data-ttu-id="47394-429">Разрешить UIAccess Apps запрос на повышение прав без использования безопасного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="47394-429">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="47394-430">Локалсекуритйоптионсвиртуализефилеандрегистривритефаилурестоперусерлокатионс</span><span class="sxs-lookup"><span data-stu-id="47394-430">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="47394-431">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-431">Boolean</span></span>|<span data-ttu-id="47394-432">Виртуализация сбоев записи в файл и реестр для отдельных расположений пользователей</span><span class="sxs-lookup"><span data-stu-id="47394-432">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="47394-433">Локалсекуритйоптионсонлелеватесигнедексекутаблес</span><span class="sxs-lookup"><span data-stu-id="47394-433">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="47394-434">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-434">Boolean</span></span>|<span data-ttu-id="47394-435">Принудительная проверка пути сертификации PKI для указанного исполняемого файла перед тем, как он будет разрешен для запуска.</span><span class="sxs-lookup"><span data-stu-id="47394-435">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="47394-436">Локалсекуритйоптионсадминистраторелеватионпромптбехавиор</span><span class="sxs-lookup"><span data-stu-id="47394-436">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="47394-437">Локалсекуритйоптионсадминистраторелеватионпромптбехавиортипе</span><span class="sxs-lookup"><span data-stu-id="47394-437">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="47394-438">Определите поведение запросов на повышение прав для администраторов в режиме одобрения администратором.</span><span class="sxs-lookup"><span data-stu-id="47394-438">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="47394-439">Возможные значения: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="47394-439">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="47394-440">Локалсекуритйоптионсстандардусерелеватионпромптбехавиор</span><span class="sxs-lookup"><span data-stu-id="47394-440">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="47394-441">Локалсекуритйоптионсстандардусерелеватионпромптбехавиортипе</span><span class="sxs-lookup"><span data-stu-id="47394-441">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="47394-442">Определите поведение запросов на повышение прав для стандартных пользователей.</span><span class="sxs-lookup"><span data-stu-id="47394-442">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="47394-443">Возможные значения: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="47394-443">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="47394-444">Локалсекуритйоптионссвитчтосекуредесктопвхенпромптингфорелеватион</span><span class="sxs-lookup"><span data-stu-id="47394-444">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="47394-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-445">Boolean</span></span>|<span data-ttu-id="47394-446">Разрешить всем запросам на повышение прав доступ к рабочему столу интерактивного пользователя, а не к безопасному рабочему столу.</span><span class="sxs-lookup"><span data-stu-id="47394-446">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="47394-447">Используются параметры политики поведения запросов для администраторов и стандартных пользователей.</span><span class="sxs-lookup"><span data-stu-id="47394-447">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="47394-448">Локалсекуритйоптионсдетектаппликатионинсталлатионсандпромптфорелеватион</span><span class="sxs-lookup"><span data-stu-id="47394-448">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="47394-449">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-449">Boolean</span></span>|<span data-ttu-id="47394-450">При установке приложений, требующих повышенных привилегий, запрашиваются учетные данные администратора. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="47394-450">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="47394-451">Локалсекуритйоптионсалловуиакцессаппликатионсфорсекурелокатионс</span><span class="sxs-lookup"><span data-stu-id="47394-451">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="47394-452">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-452">Boolean</span></span>|<span data-ttu-id="47394-453">Разрешить UIAccess Apps запрос на повышение прав без использования безопасного рабочего стола. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="47394-453">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="47394-454">Локалсекуритйоптионсусеадминаппровалмоде</span><span class="sxs-lookup"><span data-stu-id="47394-454">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="47394-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-455">Boolean</span></span>|<span data-ttu-id="47394-456">Определяет, использует ли встроенная учетная запись администратора режим одобрения администратором или выполняет все приложения с правами полного администратора. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="47394-456">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="47394-457">Локалсекуритйоптионсусеадминаппровалмодефорадминистраторс</span><span class="sxs-lookup"><span data-stu-id="47394-457">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="47394-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-458">Boolean</span></span>|<span data-ttu-id="47394-459">Определить, включен ли режим одобрения администратором и все параметры политики контроля учетных записей, по умолчанию включено</span><span class="sxs-lookup"><span data-stu-id="47394-459">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="47394-460">Локалсекуритйоптионсинформатионшовнонлоккскрин</span><span class="sxs-lookup"><span data-stu-id="47394-460">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="47394-461">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="47394-461">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="47394-462">Настройте сведения о пользователе, которые отображаются, когда сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="47394-462">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="47394-463">Если этот флажок не установлен, отображаются отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="47394-463">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="47394-464">Возможные значения: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="47394-464">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="47394-465">Локалсекуритйоптионсинформатиондисплайедонлоккскрин</span><span class="sxs-lookup"><span data-stu-id="47394-465">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="47394-466">Локалсекуритйоптионсинформатиондисплайедонлоккскринтипе</span><span class="sxs-lookup"><span data-stu-id="47394-466">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="47394-467">Настройте сведения о пользователе, которые отображаются, когда сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="47394-467">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="47394-468">Если этот флажок не установлен, отображаются отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="47394-468">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="47394-469">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="47394-469">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="47394-470">Локалсекуритйоптионсдисаблеклиентдигиталлисигнкоммуникатионсифсерверагрис</span><span class="sxs-lookup"><span data-stu-id="47394-470">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="47394-471">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-471">Boolean</span></span>|<span data-ttu-id="47394-472">Этот параметр безопасности определяет, будет ли клиент SMB пытаться согласовать подписывание SMB пакетов.</span><span class="sxs-lookup"><span data-stu-id="47394-472">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="47394-473">Локалсекуритйоптионсклиентдигиталлисигнкоммуникатионсалвайс</span><span class="sxs-lookup"><span data-stu-id="47394-473">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="47394-474">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-474">Boolean</span></span>|<span data-ttu-id="47394-475">Этот параметр безопасности определяет, требуется ли Подписывание пакетов для клиентского SMB-компонента.</span><span class="sxs-lookup"><span data-stu-id="47394-475">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="47394-476">Локалсекуритйоптионсклиентсендуненкриптедпассвордтосирдпартисмбсерверс</span><span class="sxs-lookup"><span data-stu-id="47394-476">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="47394-477">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-477">Boolean</span></span>|<span data-ttu-id="47394-478">Если этот параметр безопасности включен, перенаправителем SMB (Server Message Block) разрешено отправлять пароли открытым текстом на серверы SMB сторонних производителей, не поддерживающие шифрование паролей во время проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="47394-478">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="47394-479">Локалсекуритйоптионсдисаблесервердигиталлисигнкоммуникатионсалвайс</span><span class="sxs-lookup"><span data-stu-id="47394-479">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="47394-480">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-480">Boolean</span></span>|<span data-ttu-id="47394-481">Этот параметр безопасности определяет, требуется ли подписи пакетов для SMB-компонентов сервера.</span><span class="sxs-lookup"><span data-stu-id="47394-481">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="47394-482">Локалсекуритйоптионсдисаблесервердигиталлисигнкоммуникатионсифклиентагрис</span><span class="sxs-lookup"><span data-stu-id="47394-482">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="47394-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-483">Boolean</span></span>|<span data-ttu-id="47394-484">Этот параметр безопасности определяет, будет ли SMB согласовывать подпись SMB Packet с клиентами, которые их запрашивают.</span><span class="sxs-lookup"><span data-stu-id="47394-484">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="47394-485">Локалсекуритйоптионсрестриктанонимаусакцесстонамедпипесандшарес</span><span class="sxs-lookup"><span data-stu-id="47394-485">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="47394-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-486">Boolean</span></span>|<span data-ttu-id="47394-487">По умолчанию этот параметр безопасности запрещает анонимный доступ к ресурсам и каналам к параметрам именованных каналов, к которым возможен анонимный доступ, и к общедоступным ресурсам, к которым возможен анонимный доступ</span><span class="sxs-lookup"><span data-stu-id="47394-487">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="47394-488">Локалсекуритйоптионсдоноталлованонимаусенумератионофсамаккаунтс</span><span class="sxs-lookup"><span data-stu-id="47394-488">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="47394-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-489">Boolean</span></span>|<span data-ttu-id="47394-490">Этот параметр безопасности определяет, какие дополнительные разрешения будут предоставлены анонимным подключениям к компьютеру.</span><span class="sxs-lookup"><span data-stu-id="47394-490">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="47394-491">Локалсекуритйоптионсаллованонимаусенумератионофсамаккаунтсандшарес</span><span class="sxs-lookup"><span data-stu-id="47394-491">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="47394-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-492">Boolean</span></span>|<span data-ttu-id="47394-493">Этот параметр безопасности определяет, разрешено ли анонимным пользователям выполнять определенные действия, например перечислять имена доменных учетных записей и сетевые общие папки.</span><span class="sxs-lookup"><span data-stu-id="47394-493">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="47394-494">Локалсекуритйоптионсдонотстореланманажерхашвалуеоннекстпассвордчанже</span><span class="sxs-lookup"><span data-stu-id="47394-494">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="47394-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-495">Boolean</span></span>|<span data-ttu-id="47394-496">Этот параметр безопасности определяет, будет ли сохраняться значение хэша LAN Manager (LM) для нового пароля при следующем изменении пароля.</span><span class="sxs-lookup"><span data-stu-id="47394-496">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="47394-497">По умолчанию он не хранится.</span><span class="sxs-lookup"><span data-stu-id="47394-497">It’s not stored by default.</span></span>|
|<span data-ttu-id="47394-498">Локалсекуритйоптионссмарткардремовалбехавиор</span><span class="sxs-lookup"><span data-stu-id="47394-498">localSecurityOptionsSmartCardRemovalBehavior</span></span>|<span data-ttu-id="47394-499">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md);</span><span class="sxs-lookup"><span data-stu-id="47394-499">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)</span></span>|<span data-ttu-id="47394-500">Этот параметр безопасности определяет, что происходит при удалении смарт-карты пользователя, выполнившего вход в систему, из устройства чтения смарт-карт.</span><span class="sxs-lookup"><span data-stu-id="47394-500">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="47394-501">Возможные значения: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="47394-501">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="47394-502">Дефендерсекуритицентердисаблеаппбровсеруи</span><span class="sxs-lookup"><span data-stu-id="47394-502">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="47394-503">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-503">Boolean</span></span>|<span data-ttu-id="47394-504">Используется для отключения отображения области защиты приложений и браузера.</span><span class="sxs-lookup"><span data-stu-id="47394-504">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="47394-505">Дефендерсекуритицентердисаблефамилюи</span><span class="sxs-lookup"><span data-stu-id="47394-505">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="47394-506">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-506">Boolean</span></span>|<span data-ttu-id="47394-507">Используется для отключения отображения области семьи.</span><span class="sxs-lookup"><span data-stu-id="47394-507">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="47394-508">Дефендерсекуритицентердисаблехеалсуи</span><span class="sxs-lookup"><span data-stu-id="47394-508">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="47394-509">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-509">Boolean</span></span>|<span data-ttu-id="47394-510">Используется для отключения отображения области производительности и работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="47394-510">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="47394-511">Дефендерсекуритицентердисабленетворкуи</span><span class="sxs-lookup"><span data-stu-id="47394-511">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="47394-512">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-512">Boolean</span></span>|<span data-ttu-id="47394-513">Используется для отключения отображения зоны "брандмауэр" и "Защита сети".</span><span class="sxs-lookup"><span data-stu-id="47394-513">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="47394-514">Дефендерсекуритицентердисаблевирусуи</span><span class="sxs-lookup"><span data-stu-id="47394-514">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="47394-515">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-515">Boolean</span></span>|<span data-ttu-id="47394-516">Используется для отключения отображения области защиты от вирусов и угроз.</span><span class="sxs-lookup"><span data-stu-id="47394-516">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="47394-517">Дефендерсекуритицентердисаблеаккаунтуи</span><span class="sxs-lookup"><span data-stu-id="47394-517">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="47394-518">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-518">Boolean</span></span>|<span data-ttu-id="47394-519">Используется для отключения отображения области защиты учетных записей.</span><span class="sxs-lookup"><span data-stu-id="47394-519">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="47394-520">Дефендерсекуритицентердисаблеклеартпмуи</span><span class="sxs-lookup"><span data-stu-id="47394-520">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="47394-521">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-521">Boolean</span></span>|<span data-ttu-id="47394-522">Используется для отключения отображения кнопки Очистить доверенный платформенный модуль.</span><span class="sxs-lookup"><span data-stu-id="47394-522">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="47394-523">Дефендерсекуритицентердисаблехардвареуи</span><span class="sxs-lookup"><span data-stu-id="47394-523">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="47394-524">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-524">Boolean</span></span>|<span data-ttu-id="47394-525">Используется для отключения отображения области аппаратной защиты.</span><span class="sxs-lookup"><span data-stu-id="47394-525">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="47394-526">Дефендерсекуритицентердисабленотификатионареауи</span><span class="sxs-lookup"><span data-stu-id="47394-526">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="47394-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-527">Boolean</span></span>|<span data-ttu-id="47394-528">Используется для отключения отображения элемента управления "область уведомлений".</span><span class="sxs-lookup"><span data-stu-id="47394-528">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="47394-529">Для вступления этого параметра в силу пользователю необходимо выйти из системы и войти в нее, а затем перезагрузить компьютер.</span><span class="sxs-lookup"><span data-stu-id="47394-529">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="47394-530">Дефендерсекуритицентердисаблерансомвареуи</span><span class="sxs-lookup"><span data-stu-id="47394-530">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="47394-531">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-531">Boolean</span></span>|<span data-ttu-id="47394-532">Используется для отключения отображения области защиты от пошантажистом.</span><span class="sxs-lookup"><span data-stu-id="47394-532">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="47394-533">Дефендерсекуритицентердисаблесекуребутуи</span><span class="sxs-lookup"><span data-stu-id="47394-533">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="47394-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-534">Boolean</span></span>|<span data-ttu-id="47394-535">Используется для отключения отображения области безопасной загрузки в разделе Безопасность устройства.</span><span class="sxs-lookup"><span data-stu-id="47394-535">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="47394-536">Дефендерсекуритицентердисаблетраублешутингуи</span><span class="sxs-lookup"><span data-stu-id="47394-536">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="47394-537">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-537">Boolean</span></span>|<span data-ttu-id="47394-538">Используется для отключения отображения устранения неполадок процесса безопасности в разделе Безопасность устройства.</span><span class="sxs-lookup"><span data-stu-id="47394-538">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="47394-539">Дефендерсекуритицентердисаблевулнераблетпмфирмвареупдатеуи</span><span class="sxs-lookup"><span data-stu-id="47394-539">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="47394-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-540">Boolean</span></span>|<span data-ttu-id="47394-541">Используется для отключения отображения обновления микропрограммы доверенного платформенного модуля при обнаружении уязвимого программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="47394-541">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="47394-542">Дефендерсекуритицентерорганизатиондисплайнаме</span><span class="sxs-lookup"><span data-stu-id="47394-542">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="47394-543">String</span><span class="sxs-lookup"><span data-stu-id="47394-543">String</span></span>|<span data-ttu-id="47394-544">Имя компании, которое отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="47394-544">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="47394-545">Дефендерсекуритицентерхелпемаил</span><span class="sxs-lookup"><span data-stu-id="47394-545">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="47394-546">String</span><span class="sxs-lookup"><span data-stu-id="47394-546">String</span></span>|<span data-ttu-id="47394-547">Адрес электронной почты, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="47394-547">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="47394-548">Дефендерсекуритицентерхелпфоне</span><span class="sxs-lookup"><span data-stu-id="47394-548">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="47394-549">String</span><span class="sxs-lookup"><span data-stu-id="47394-549">String</span></span>|<span data-ttu-id="47394-550">Номер телефона или идентификатор Skype, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="47394-550">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="47394-551">Дефендерсекуритицентерхелпурл</span><span class="sxs-lookup"><span data-stu-id="47394-551">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="47394-552">String</span><span class="sxs-lookup"><span data-stu-id="47394-552">String</span></span>|<span data-ttu-id="47394-553">URL-адрес портала справки это отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="47394-553">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="47394-554">Дефендерсекуритицентернотификатионсфромапп</span><span class="sxs-lookup"><span data-stu-id="47394-554">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="47394-555">Дефендерсекуритицентернотификатионсфромапптипе</span><span class="sxs-lookup"><span data-stu-id="47394-555">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="47394-556">Уведомления, отображаемые в отображаемых областях приложения.</span><span class="sxs-lookup"><span data-stu-id="47394-556">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="47394-557">Возможные значения: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="47394-557">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="47394-558">Дефендерсекуритицентеритконтактдисплай</span><span class="sxs-lookup"><span data-stu-id="47394-558">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="47394-559">Дефендерсекуритицентеритконтактдисплайтипе</span><span class="sxs-lookup"><span data-stu-id="47394-559">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="47394-560">Настройка места отображения контактной информации для конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="47394-560">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="47394-561">Возможные значения: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="47394-561">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="47394-562">Виндовсдефендертамперпротектион</span><span class="sxs-lookup"><span data-stu-id="47394-562">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="47394-563">Виндовсдефендертамперпротектионоптионс</span><span class="sxs-lookup"><span data-stu-id="47394-563">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="47394-564">Настройка параметров Тамперпротектион для защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="47394-564">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="47394-565">Возможные значения: `notConfigured`, `enable`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="47394-565">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="47394-566">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="47394-566">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="47394-567">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-567">Boolean</span></span>|<span data-ttu-id="47394-568">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="47394-568">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="47394-569">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="47394-569">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="47394-570">Int32</span><span class="sxs-lookup"><span data-stu-id="47394-570">Int32</span></span>|<span data-ttu-id="47394-571">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="47394-571">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="47394-572">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="47394-572">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="47394-573">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="47394-573">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="47394-574">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="47394-574">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="47394-575">Фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="47394-575">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="47394-576">Выберите используемую кодировку с общим ключом.</span><span class="sxs-lookup"><span data-stu-id="47394-576">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="47394-577">Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="47394-577">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="47394-578">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="47394-578">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="47394-579">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-579">Boolean</span></span>|<span data-ttu-id="47394-580">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="47394-580">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="47394-581">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="47394-581">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="47394-582">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-582">Boolean</span></span>|<span data-ttu-id="47394-583">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="47394-583">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="47394-584">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="47394-584">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="47394-585">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-585">Boolean</span></span>|<span data-ttu-id="47394-586">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="47394-586">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="47394-587">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="47394-587">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="47394-588">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-588">Boolean</span></span>|<span data-ttu-id="47394-589">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="47394-589">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="47394-590">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="47394-590">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="47394-591">Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="47394-591">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="47394-592">Укажите способ применения списка отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="47394-592">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="47394-593">Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="47394-593">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="47394-594">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="47394-594">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="47394-595">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-595">Boolean</span></span>|<span data-ttu-id="47394-596">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="47394-596">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="47394-597">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="47394-597">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="47394-598">Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="47394-598">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="47394-599">Настраивает способ применения очередей пакетов в сценарии туннельного шлюза.</span><span class="sxs-lookup"><span data-stu-id="47394-599">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="47394-600">Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="47394-600">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="47394-601">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="47394-601">firewallProfileDomain</span></span>|[<span data-ttu-id="47394-602">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="47394-602">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="47394-603">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="47394-603">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="47394-604">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="47394-604">firewallProfilePublic</span></span>|[<span data-ttu-id="47394-605">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="47394-605">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="47394-606">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="47394-606">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="47394-607">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="47394-607">firewallProfilePrivate</span></span>|[<span data-ttu-id="47394-608">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="47394-608">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="47394-609">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="47394-609">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="47394-610">Дефендерадобереадерлаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="47394-610">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="47394-611">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-611">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="47394-612">Значение, указывающее поведение Adobe Reader при создании дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="47394-612">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="47394-613">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-613">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-614">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="47394-614">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="47394-615">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="47394-615">String collection</span></span>|<span data-ttu-id="47394-616">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="47394-616">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="47394-617">Дефендероффицеаппсосерпроцессинжектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-617">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="47394-618">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="47394-618">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="47394-619">Значение, указывающее поведение приложений Office, добавляемых в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="47394-619">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="47394-620">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-620">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-621">Дефендероффицеаппсосерпроцессинжектион</span><span class="sxs-lookup"><span data-stu-id="47394-621">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="47394-622">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-622">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="47394-623">Значение, указывающее поведение приложений Office, добавляемых в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="47394-623">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="47394-624">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-624">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-625">Дефендероффицекоммуникатионаппслаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="47394-625">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="47394-626">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-626">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="47394-627">Значение, определяющее поведение приложений для связи с Office, включая Microsoft Outlook, от создания дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="47394-627">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="47394-628">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-628">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-629">Дефендероффицеаппсексекутаблеконтенткреатионорлаунчтипе</span><span class="sxs-lookup"><span data-stu-id="47394-629">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="47394-630">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="47394-630">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="47394-631">Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого контента.</span><span class="sxs-lookup"><span data-stu-id="47394-631">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="47394-632">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-632">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-633">Дефендероффицеаппсексекутаблеконтенткреатионорлаунч</span><span class="sxs-lookup"><span data-stu-id="47394-633">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="47394-634">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-634">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="47394-635">Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого контента.</span><span class="sxs-lookup"><span data-stu-id="47394-635">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="47394-636">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-636">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-637">Дефендероффицеаппслаунччилдпроцесстипе</span><span class="sxs-lookup"><span data-stu-id="47394-637">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="47394-638">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="47394-638">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="47394-639">Значение, указывающее поведение запуска приложения Office для дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="47394-639">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="47394-640">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-640">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-641">Дефендероффицеаппслаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="47394-641">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="47394-642">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-642">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="47394-643">Значение, указывающее поведение запуска приложения Office для дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="47394-643">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="47394-644">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-644">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-645">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="47394-645">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="47394-646">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="47394-646">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="47394-647">Значение, указывающее поведение импорта Win32 из кода макросов в Office.</span><span class="sxs-lookup"><span data-stu-id="47394-647">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="47394-648">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-648">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-649">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="47394-649">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="47394-650">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-650">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="47394-651">Значение, указывающее поведение импорта Win32 из кода макросов в Office.</span><span class="sxs-lookup"><span data-stu-id="47394-651">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="47394-652">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-652">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-653">Дефендерскриптобфускатедмакрокодетипе</span><span class="sxs-lookup"><span data-stu-id="47394-653">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="47394-654">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="47394-654">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="47394-655">Значение, определяющее поведение кода "замаскированный JS/VBS/PS/макрос".</span><span class="sxs-lookup"><span data-stu-id="47394-655">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="47394-656">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-656">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-657">Дефендерскриптобфускатедмакрокоде</span><span class="sxs-lookup"><span data-stu-id="47394-657">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="47394-658">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-658">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="47394-659">Значение, определяющее поведение кода "замаскированный JS/VBS/PS/макрос".</span><span class="sxs-lookup"><span data-stu-id="47394-659">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="47394-660">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-660">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-661">Дефендерскриптдовнлоадедпайлоадексекутионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-661">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="47394-662">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="47394-662">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="47394-663">Значение, определяющее поведение JS-и VBS-данных, загруженных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="47394-663">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="47394-664">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-664">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-665">Дефендерскриптдовнлоадедпайлоадексекутион</span><span class="sxs-lookup"><span data-stu-id="47394-665">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="47394-666">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-666">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="47394-667">Значение, определяющее поведение JS-и VBS-данных, загруженных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="47394-667">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="47394-668">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-668">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-669">Дефендерпревенткредентиалстеалингтипе</span><span class="sxs-lookup"><span data-stu-id="47394-669">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="47394-670">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-670">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="47394-671">Значение, указывающее, разрешено ли перенос учетных данных из подсистемы локального центра безопасности Windows.</span><span class="sxs-lookup"><span data-stu-id="47394-671">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="47394-672">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-672">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-673">Дефендерпроцесскреатионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-673">defenderProcessCreationType</span></span>|[<span data-ttu-id="47394-674">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="47394-674">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="47394-675">Значение, указывающее ответ на создание процессов, исходящих от команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="47394-675">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="47394-676">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-676">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-677">Дефендерпроцесскреатион</span><span class="sxs-lookup"><span data-stu-id="47394-677">defenderProcessCreation</span></span>|[<span data-ttu-id="47394-678">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-678">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="47394-679">Значение, указывающее ответ на создание процессов, исходящих от команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="47394-679">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="47394-680">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-680">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-681">Дефендерунтрустедусбпроцесстипе</span><span class="sxs-lookup"><span data-stu-id="47394-681">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="47394-682">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="47394-682">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="47394-683">Значение, указывающее ответ на недоверенные и неподписанные процессы, которые запускаются с USB.</span><span class="sxs-lookup"><span data-stu-id="47394-683">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="47394-684">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-684">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-685">Дефендерунтрустедусбпроцесс</span><span class="sxs-lookup"><span data-stu-id="47394-685">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="47394-686">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-686">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="47394-687">Значение, указывающее ответ на недоверенные и неподписанные процессы, которые запускаются с USB.</span><span class="sxs-lookup"><span data-stu-id="47394-687">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="47394-688">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-688">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-689">Дефендерунтрустедексекутаблетипе</span><span class="sxs-lookup"><span data-stu-id="47394-689">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="47394-690">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="47394-690">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="47394-691">Значение, указывающее ответ на исполняемые файлы, которые не отвечают условиям преобладание, возраст или доверенного списка.</span><span class="sxs-lookup"><span data-stu-id="47394-691">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="47394-692">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-692">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-693">Дефендерунтрустедексекутабле</span><span class="sxs-lookup"><span data-stu-id="47394-693">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="47394-694">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-694">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="47394-695">Значение, указывающее ответ на исполняемые файлы, которые не отвечают условиям преобладание, возраст или доверенного списка.</span><span class="sxs-lookup"><span data-stu-id="47394-695">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="47394-696">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-696">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-697">Дефендеремаилконтентексекутионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-697">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="47394-698">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="47394-698">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="47394-699">Значение, указывающее, следует ли удалять исполняемые файлы (exe, DLL, PS, JS, VBS и т. д.) из электронной почты (почтовая или почтовая программа).</span><span class="sxs-lookup"><span data-stu-id="47394-699">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="47394-700">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-700">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-701">Дефендеремаилконтентексекутион</span><span class="sxs-lookup"><span data-stu-id="47394-701">defenderEmailContentExecution</span></span>|[<span data-ttu-id="47394-702">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-702">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="47394-703">Значение, указывающее, следует ли удалять исполняемые файлы (exe, DLL, PS, JS, VBS и т. д.) из электронной почты (почтовая или почтовая программа).</span><span class="sxs-lookup"><span data-stu-id="47394-703">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="47394-704">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-704">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-705">Дефендерадванцедрансомеварепротектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-705">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="47394-706">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-706">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="47394-707">Значение, указывающее на использование расширенной защиты в рансомеваре.</span><span class="sxs-lookup"><span data-stu-id="47394-707">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="47394-708">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-708">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-709">Дефендергуардмифолдерстипе</span><span class="sxs-lookup"><span data-stu-id="47394-709">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="47394-710">Фолдерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-710">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="47394-711">Значение, указывающее поведение защищенных папок.</span><span class="sxs-lookup"><span data-stu-id="47394-711">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="47394-712">Возможные значения: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="47394-712">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="47394-713">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="47394-713">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="47394-714">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="47394-714">String collection</span></span>|<span data-ttu-id="47394-715">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="47394-715">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="47394-716">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="47394-716">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="47394-717">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="47394-717">String collection</span></span>|<span data-ttu-id="47394-718">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="47394-718">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="47394-719">Дефендернетворкпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-719">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="47394-720">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="47394-720">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="47394-721">Значение, указывающее поведение Нетворкпротектион.</span><span class="sxs-lookup"><span data-stu-id="47394-721">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="47394-722">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="47394-722">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="47394-723">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="47394-723">defenderExploitProtectionXml</span></span>|<span data-ttu-id="47394-724">Binary</span><span class="sxs-lookup"><span data-stu-id="47394-724">Binary</span></span>|<span data-ttu-id="47394-725">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="47394-725">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="47394-726">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="47394-726">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="47394-727">String</span><span class="sxs-lookup"><span data-stu-id="47394-727">String</span></span>|<span data-ttu-id="47394-728">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="47394-728">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="47394-729">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="47394-729">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="47394-730">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-730">Boolean</span></span>|<span data-ttu-id="47394-731">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="47394-731">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="47394-732">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="47394-732">appLockerApplicationControl</span></span>|[<span data-ttu-id="47394-733">Апплоккераппликатионконтролтипе</span><span class="sxs-lookup"><span data-stu-id="47394-733">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="47394-734">Позволяет администратору выбирать разрешенные типы приложений для устройств.</span><span class="sxs-lookup"><span data-stu-id="47394-734">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="47394-735">Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="47394-735">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="47394-736">Девицегуардлокалсистемаусоритикредентиалгуардсеттингс</span><span class="sxs-lookup"><span data-stu-id="47394-736">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="47394-737">Девицегуардлокалсистемаусоритикредентиалгуардтипе</span><span class="sxs-lookup"><span data-stu-id="47394-737">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="47394-738">Включите Guard в учетных данных, когда включен уровень безопасности платформы с безопасной загрузкой и безопасностью на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="47394-738">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="47394-739">Возможные значения: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="47394-739">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="47394-740">Девицегуарденаблевиртуализатионбаседсекурити</span><span class="sxs-lookup"><span data-stu-id="47394-740">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="47394-741">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-741">Boolean</span></span>|<span data-ttu-id="47394-742">Включает безопасность на основе виртуализации (VBS).</span><span class="sxs-lookup"><span data-stu-id="47394-742">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="47394-743">Девицегуарденаблесекуребутвисдма</span><span class="sxs-lookup"><span data-stu-id="47394-743">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="47394-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-744">Boolean</span></span>|<span data-ttu-id="47394-745">Это свойство будет устаревшим в 2019 мая и будет заменено свойством Девицегуардсекуребутвисдма.</span><span class="sxs-lookup"><span data-stu-id="47394-745">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="47394-746">Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="47394-746">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="47394-747">Девицегуардсекуребутвисдма</span><span class="sxs-lookup"><span data-stu-id="47394-747">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="47394-748">Секуребутвисдматипе</span><span class="sxs-lookup"><span data-stu-id="47394-748">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="47394-749">Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="47394-749">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="47394-750">Возможные значения: `notConfigured`, `withoutDMA`, `withDMA`.</span><span class="sxs-lookup"><span data-stu-id="47394-750">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="47394-751">Девицегуардлаунчсистемгуард</span><span class="sxs-lookup"><span data-stu-id="47394-751">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="47394-752">Включение</span><span class="sxs-lookup"><span data-stu-id="47394-752">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="47394-753">Позволяет ИТ – администратору настраивать запуск системы защиты системы.</span><span class="sxs-lookup"><span data-stu-id="47394-753">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="47394-754">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="47394-754">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="47394-755">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="47394-755">smartScreenEnableInShell</span></span>|<span data-ttu-id="47394-756">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-756">Boolean</span></span>|<span data-ttu-id="47394-757">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="47394-757">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="47394-758">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="47394-758">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="47394-759">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-759">Boolean</span></span>|<span data-ttu-id="47394-760">Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="47394-760">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="47394-761">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="47394-761">applicationGuardEnabled</span></span>|<span data-ttu-id="47394-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-762">Boolean</span></span>|<span data-ttu-id="47394-763">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="47394-763">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="47394-764">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="47394-764">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="47394-765">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="47394-765">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="47394-766">Включение Application Guard в Защитнике Windows для более новых сборок Windows.</span><span class="sxs-lookup"><span data-stu-id="47394-766">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="47394-767">Возможные значения: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="47394-767">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="47394-768">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="47394-768">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="47394-769">Аппликатионгуардблоккфилетрансфертипе</span><span class="sxs-lookup"><span data-stu-id="47394-769">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="47394-770">Блокировать буфер обмена для передачи файла изображения, текстового файла или ни одного из них.</span><span class="sxs-lookup"><span data-stu-id="47394-770">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="47394-771">Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="47394-771">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="47394-772">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="47394-772">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="47394-773">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-773">Boolean</span></span>|<span data-ttu-id="47394-774">Позволяет заблокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="47394-774">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="47394-775">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="47394-775">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="47394-776">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-776">Boolean</span></span>|<span data-ttu-id="47394-777">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="47394-777">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="47394-778">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="47394-778">applicationGuardForceAuditing</span></span>|<span data-ttu-id="47394-779">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-779">Boolean</span></span>|<span data-ttu-id="47394-780">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="47394-780">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="47394-781">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="47394-781">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="47394-782">Аппликатионгуардблоккклипбоардшарингтипе</span><span class="sxs-lookup"><span data-stu-id="47394-782">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="47394-783">Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="47394-783">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="47394-784">Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="47394-784">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="47394-785">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="47394-785">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="47394-786">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-786">Boolean</span></span>|<span data-ttu-id="47394-787">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="47394-787">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="47394-788">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="47394-788">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="47394-789">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-789">Boolean</span></span>|<span data-ttu-id="47394-790">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="47394-790">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="47394-791">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="47394-791">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="47394-792">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-792">Boolean</span></span>|<span data-ttu-id="47394-793">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="47394-793">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="47394-794">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="47394-794">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="47394-795">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-795">Boolean</span></span>|<span data-ttu-id="47394-796">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="47394-796">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="47394-797">Аппликатионгуардалловвиртуалгпу</span><span class="sxs-lookup"><span data-stu-id="47394-797">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="47394-798">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-798">Boolean</span></span>|<span data-ttu-id="47394-799">Разрешить приложению Application Guard использовать виртуальный GPU</span><span class="sxs-lookup"><span data-stu-id="47394-799">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="47394-800">Аппликатионгуардалловфилесавеонхост</span><span class="sxs-lookup"><span data-stu-id="47394-800">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="47394-801">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-801">Boolean</span></span>|<span data-ttu-id="47394-802">Разрешить пользователям скачивать файлы из EDGE в контейнере Application Guard и сохранять их в файловой системе узла</span><span class="sxs-lookup"><span data-stu-id="47394-802">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="47394-803">Битлоккералловстандардусеренкриптион</span><span class="sxs-lookup"><span data-stu-id="47394-803">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="47394-804">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-804">Boolean</span></span>|<span data-ttu-id="47394-805">Позволяет администратору разрешить обычным пользователям включать енкрпитион во время присоединения к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="47394-805">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="47394-806">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="47394-806">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="47394-807">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-807">Boolean</span></span>|<span data-ttu-id="47394-808">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="47394-808">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="47394-809">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="47394-809">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="47394-810">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-810">Boolean</span></span>|<span data-ttu-id="47394-811">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="47394-811">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="47394-812">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="47394-812">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="47394-813">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="47394-813">bitLockerEncryptDevice</span></span>|<span data-ttu-id="47394-814">Boolean</span><span class="sxs-lookup"><span data-stu-id="47394-814">Boolean</span></span>|<span data-ttu-id="47394-815">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="47394-815">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="47394-816">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="47394-816">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="47394-817">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="47394-817">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="47394-818">Политика системного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="47394-818">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="47394-819">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="47394-819">bitLockerFixedDrivePolicy</span></span>|<span data-ttu-id="47394-820">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md);</span><span class="sxs-lookup"><span data-stu-id="47394-820">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)</span></span>|<span data-ttu-id="47394-821">Политика фиксированного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="47394-821">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="47394-822">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="47394-822">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="47394-823">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="47394-823">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="47394-824">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="47394-824">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="47394-825">Отклик</span><span class="sxs-lookup"><span data-stu-id="47394-825">Response</span></span>
<span data-ttu-id="47394-826">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="47394-826">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47394-827">Пример</span><span class="sxs-lookup"><span data-stu-id="47394-827">Example</span></span>

### <a name="request"></a><span data-ttu-id="47394-828">Запрос</span><span class="sxs-lookup"><span data-stu-id="47394-828">Request</span></span>
<span data-ttu-id="47394-829">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47394-829">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 28958

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
  }
}
```

### <a name="response"></a><span data-ttu-id="47394-830">Отклик</span><span class="sxs-lookup"><span data-stu-id="47394-830">Response</span></span>
<span data-ttu-id="47394-p206">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47394-p206">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 29130

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
  }
}
```





