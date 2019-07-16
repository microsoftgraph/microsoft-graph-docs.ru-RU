---
title: Создание windows10EndpointProtectionConfiguration
description: Создание объекта windows10EndpointProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa73f3d61ec7af2045b0d6b7cc53fac135b8fe76
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715300"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="d0fc3-103">Создание windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0fc3-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="d0fc3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0fc3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0fc3-106">Создание объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-106">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0fc3-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d0fc3-107">Prerequisites</span></span>
<span data-ttu-id="d0fc3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0fc3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0fc3-110">Permission type</span></span>|<span data-ttu-id="d0fc3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0fc3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0fc3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0fc3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0fc3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0fc3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d0fc3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0fc3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0fc3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-115">Not supported.</span></span>|
|<span data-ttu-id="d0fc3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0fc3-116">Application</span></span>|<span data-ttu-id="d0fc3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0fc3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0fc3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d0fc3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0fc3-119">Request headers</span></span>
|<span data-ttu-id="d0fc3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0fc3-120">Header</span></span>|<span data-ttu-id="d0fc3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d0fc3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0fc3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0fc3-122">Authorization</span></span>|<span data-ttu-id="d0fc3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0fc3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d0fc3-124">Accept</span></span>|<span data-ttu-id="d0fc3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0fc3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0fc3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d0fc3-126">Request body</span></span>
<span data-ttu-id="d0fc3-127">В теле запроса добавьте представление объекта windows10EndpointProtectionConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-127">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="d0fc3-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-128">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="d0fc3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0fc3-129">Property</span></span>|<span data-ttu-id="d0fc3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d0fc3-130">Type</span></span>|<span data-ttu-id="d0fc3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d0fc3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0fc3-132">id</span><span class="sxs-lookup"><span data-stu-id="d0fc3-132">id</span></span>|<span data-ttu-id="d0fc3-133">String</span><span class="sxs-lookup"><span data-stu-id="d0fc3-133">String</span></span>|<span data-ttu-id="d0fc3-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-134">Key of the entity.</span></span> <span data-ttu-id="d0fc3-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fc3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0fc3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d0fc3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0fc3-137">DateTimeOffset</span></span>|<span data-ttu-id="d0fc3-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d0fc3-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fc3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d0fc3-140">roleScopeTagIds</span></span>|<span data-ttu-id="d0fc3-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d0fc3-141">String collection</span></span>|<span data-ttu-id="d0fc3-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d0fc3-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fc3-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-144">supportsScopeTags</span></span>|<span data-ttu-id="d0fc3-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-145">Boolean</span></span>|<span data-ttu-id="d0fc3-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d0fc3-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d0fc3-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d0fc3-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-149">This property is read-only.</span></span> <span data-ttu-id="d0fc3-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fc3-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d0fc3-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d0fc3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d0fc3-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d0fc3-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d0fc3-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fc3-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d0fc3-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d0fc3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d0fc3-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d0fc3-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d0fc3-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fc3-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d0fc3-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d0fc3-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d0fc3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d0fc3-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d0fc3-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fc3-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0fc3-163">createdDateTime</span></span>|<span data-ttu-id="d0fc3-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0fc3-164">DateTimeOffset</span></span>|<span data-ttu-id="d0fc3-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-165">DateTime the object was created.</span></span> <span data-ttu-id="d0fc3-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fc3-167">description</span><span class="sxs-lookup"><span data-stu-id="d0fc3-167">description</span></span>|<span data-ttu-id="d0fc3-168">String</span><span class="sxs-lookup"><span data-stu-id="d0fc3-168">String</span></span>|<span data-ttu-id="d0fc3-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d0fc3-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fc3-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d0fc3-171">displayName</span></span>|<span data-ttu-id="d0fc3-172">Строка</span><span class="sxs-lookup"><span data-stu-id="d0fc3-172">String</span></span>|<span data-ttu-id="d0fc3-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d0fc3-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fc3-175">version</span><span class="sxs-lookup"><span data-stu-id="d0fc3-175">version</span></span>|<span data-ttu-id="d0fc3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d0fc3-176">Int32</span></span>|<span data-ttu-id="d0fc3-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-177">Version of the device configuration.</span></span> <span data-ttu-id="d0fc3-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0fc3-179">Дмагуарддевицеенумератионполици</span><span class="sxs-lookup"><span data-stu-id="d0fc3-179">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="d0fc3-180">Дмагуарддевицеенумератионполицитипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-180">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="d0fc3-181">Эта политика предназначена для обеспечения дополнительной защиты от внешних устройств с поддержкой прямого доступа к памяти.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-181">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="d0fc3-182">Он обеспечивает более полный контроль над перечислением устройств с поддержкой внешних устройств с поддержкой прямого доступа к памяти, несовместимых с пересопоставлением и изоляцией памяти устройств и изолированной средой.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-182">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="d0fc3-183">Эта политика вступает в силу только тогда, когда система защиты DMA поддерживается и включена встроенным встроенным по.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-183">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="d0fc3-184">Защита от DMA ядра — это компонент платформы, который невозможно контролировать с помощью политики или конечным пользователем.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-184">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="d0fc3-185">Она должна поддерживаться системой на момент производства.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-185">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="d0fc3-186">Чтобы проверить, поддерживает ли система защиту DMA, проверьте поле Защита ядра DMA на странице Сводка объекта MSINFO32. exe.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-186">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="d0fc3-187">Возможные значения: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-187">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="d0fc3-188">Фиреваллрулес</span><span class="sxs-lookup"><span data-stu-id="d0fc3-188">firewallRules</span></span>|<span data-ttu-id="d0fc3-189">Коллекция [виндовсфиреваллруле](../resources/intune-deviceconfig-windowsfirewallrule.md)</span><span class="sxs-lookup"><span data-stu-id="d0fc3-189">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="d0fc3-190">Настраивает параметры правила брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-190">Configures the firewall rule settings.</span></span> <span data-ttu-id="d0fc3-191">Эта коллекция может содержать не более 150 элементов.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-191">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="d0fc3-192">Усерригхтсакцесскредентиалманажераструстедкаллер</span><span class="sxs-lookup"><span data-stu-id="d0fc3-192">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="d0fc3-193">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-193">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-194">Это право пользователя используется диспетчером учетных данных во время резервного копирования и восстановления.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-194">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="d0fc3-195">Сохраненные учетные данные пользователей могут быть скомпрометированы, если эта привилегия передана другим субъектам.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-195">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="d0fc3-196">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-196">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0fc3-197">Усерригхтсалловакцессфромнетворк</span><span class="sxs-lookup"><span data-stu-id="d0fc3-197">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="d0fc3-198">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-198">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-199">Это право пользователя определяет, какие пользователи и группы могут подключаться к компьютеру через сеть.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-199">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="d0fc3-200">Допустимое состояние — Supported.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-200">State Allowed is supported.</span></span>|
|<span data-ttu-id="d0fc3-201">Усерригхтсблоккакцессфромнетворк</span><span class="sxs-lookup"><span data-stu-id="d0fc3-201">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="d0fc3-202">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-202">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-203">Это право пользователя определяет, каким пользователям и группам запрещается подключаться к компьютеру через сеть.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-203">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="d0fc3-204">Блок состояния поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-204">State Block is supported.</span></span>|
|<span data-ttu-id="d0fc3-205">Усерригхтсактаспартофсеоператингсистем</span><span class="sxs-lookup"><span data-stu-id="d0fc3-205">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="d0fc3-206">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-206">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-207">Это право пользователя позволяет процессу олицетворять любого пользователя без проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-207">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="d0fc3-208">Таким образом, процесс может получить доступ к тем же локальным ресурсам, что и пользователь.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-208">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="d0fc3-209">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0fc3-210">Усерригхтслокаллогон</span><span class="sxs-lookup"><span data-stu-id="d0fc3-210">userRightsLocalLogOn</span></span>|[<span data-ttu-id="d0fc3-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-212">Это право пользователя определяет, какие пользователи могут входить на компьютер.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-212">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="d0fc3-213">Допустимые состояния NotConfigured, Поддерживаемые</span><span class="sxs-lookup"><span data-stu-id="d0fc3-213">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="d0fc3-214">Усерригхтсденилокаллогон</span><span class="sxs-lookup"><span data-stu-id="d0fc3-214">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="d0fc3-215">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-215">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-216">Это право пользователя определяет, какие пользователи не могут войти на компьютер.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-216">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="d0fc3-217">Состояния NotConfigured, блокировки поддерживаются</span><span class="sxs-lookup"><span data-stu-id="d0fc3-217">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="d0fc3-218">Усерригхтсбаккупдата</span><span class="sxs-lookup"><span data-stu-id="d0fc3-218">userRightsBackupData</span></span>|[<span data-ttu-id="d0fc3-219">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-219">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-220">Это право пользователя определяет, какие пользователи могут обходить разрешения для файлов, каталогов, реестра и других постоянных объектов при резервном копировании файлов и каталогов.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-220">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="d0fc3-221">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-221">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0fc3-222">Усерригхтсчанжесистемтиме</span><span class="sxs-lookup"><span data-stu-id="d0fc3-222">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="d0fc3-223">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-223">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-224">Это право пользователя определяет, какие пользователи и группы могут изменять время и дату на внутреннем часовом компьютере.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-224">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="d0fc3-225">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-225">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0fc3-226">Усерригхтскреатеглобалобжектс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-226">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="d0fc3-227">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-227">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-228">Этот параметр безопасности определяет, могут ли пользователи создавать глобальные объекты, доступные для всех сеансов.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-228">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="d0fc3-229">Пользователи, которые могут создавать глобальные объекты, могут повлиять на процессы, выполняемые в сеансах других пользователей, что может привести к сбою приложения или повреждению данных.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-229">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="d0fc3-230">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0fc3-231">Усерригхтскреатепажефиле</span><span class="sxs-lookup"><span data-stu-id="d0fc3-231">userRightsCreatePageFile</span></span>|[<span data-ttu-id="d0fc3-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-233">Это право пользователя определяет, какие пользователи и группы могут вызывать внутренний API, чтобы создать и изменить размер файла подкачки.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-233">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="d0fc3-234">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0fc3-235">Усерригхтскреатеперманентшаредобжектс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-235">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="d0fc3-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-237">Это право пользователя определяет, какие учетные записи могут использоваться процессами для создания объекта каталога с помощью диспетчера объектов.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-237">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="d0fc3-238">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-238">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0fc3-239">Усерригхтскреатесимболиклинкс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-239">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="d0fc3-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-241">Это право пользователя определяет, может ли пользователь создать символическую ссылку с компьютера, на который они входили.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-241">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="d0fc3-242">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-242">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0fc3-243">Усерригхтскреатетокен</span><span class="sxs-lookup"><span data-stu-id="d0fc3-243">userRightsCreateToken</span></span>|[<span data-ttu-id="d0fc3-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-245">Это право пользователя определяет, какие пользователи и группы могут использоваться процессами для создания маркера, который можно использовать для получения доступа к любому локальному ресурсу, когда процесс использует внутренний API для создания маркера доступа.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-245">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="d0fc3-246">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-246">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0fc3-247">Усерригхтсдебугпрограмс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-247">userRightsDebugPrograms</span></span>|[<span data-ttu-id="d0fc3-248">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-248">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-249">Это право пользователя определяет, какие пользователи могут прикреплять отладчик к любому процессу или ядру.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-249">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="d0fc3-250">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-250">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0fc3-251">Усерригхтсремотедесктопсервицеслогон</span><span class="sxs-lookup"><span data-stu-id="d0fc3-251">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="d0fc3-252">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-252">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-253">Это право пользователя определяет, каким пользователям и группам запрещается вход в систему в качестве клиента служб удаленных рабочих столов.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-253">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="d0fc3-254">Поддерживаются только состояния NotConfigured и Block</span><span class="sxs-lookup"><span data-stu-id="d0fc3-254">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="d0fc3-255">Усерригхтсделегатион</span><span class="sxs-lookup"><span data-stu-id="d0fc3-255">userRightsDelegation</span></span>|[<span data-ttu-id="d0fc3-256">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-256">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-257">Это право пользователя определяет, какие пользователи могут устанавливать параметр "доверять для делегирования" для объекта пользователя или компьютера.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-257">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="d0fc3-258">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-258">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0fc3-259">Усерригхтсженератесекуритяудитс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-259">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="d0fc3-260">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-260">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-261">Это право пользователя определяет, какие учетные записи могут использоваться процессом для добавления записей в журнал безопасности.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-261">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="d0fc3-262">Журнал безопасности используется для трассировки несанкционированного доступа к системе.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-262">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="d0fc3-263">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-263">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0fc3-264">Усерригхтсимперсонатеклиент</span><span class="sxs-lookup"><span data-stu-id="d0fc3-264">userRightsImpersonateClient</span></span>|[<span data-ttu-id="d0fc3-265">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-265">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-266">Назначение этого права пользователю позволяет программам, выполняемым от имени этого пользователя, олицетворять клиента.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-266">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="d0fc3-267">Требование этого пользователя для такого рода олицетворения запрещает несанкционированному пользователю подключаться к созданной им службе, а затем олицетворять этого клиента, что может повысить уровень разрешений неавторизованного пользователя до Уровни администрирования или системы.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-267">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="d0fc3-268">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0fc3-269">Усерригхтсинкреасесчедулингприорити</span><span class="sxs-lookup"><span data-stu-id="d0fc3-269">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="d0fc3-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-271">Это право пользователя определяет, какие учетные записи могут использовать процесс с доступом к свойствам Write для другого процесса, чтобы увеличить приоритет выполнения, назначенный другому процессу.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-271">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="d0fc3-272">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0fc3-273">Усерригхтслоадунлоаддриверс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-273">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="d0fc3-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-275">Это право пользователя определяет, какие пользователи могут динамически загружать и выгружать драйверы устройств или другой код в режиме ядра.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-275">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="d0fc3-276">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0fc3-277">Усерригхтслоккмемори</span><span class="sxs-lookup"><span data-stu-id="d0fc3-277">userRightsLockMemory</span></span>|[<span data-ttu-id="d0fc3-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-279">Это право пользователя определяет, какие учетные записи могут использовать процесс для хранения данных в физической памяти, что предотвращает их разбиение данных на виртуальную память на диске.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-279">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="d0fc3-280">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0fc3-281">Усерригхтсманажеаудитингандсекуритилогс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-281">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="d0fc3-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-283">Это право пользователя определяет, какие пользователи могут задавать параметры аудита доступа к объектам для отдельных ресурсов, таких как файлы, объекты Active Directory и разделы реестра.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-283">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="d0fc3-284">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0fc3-285">Усерригхтсманажеволумес</span><span class="sxs-lookup"><span data-stu-id="d0fc3-285">userRightsManageVolumes</span></span>|[<span data-ttu-id="d0fc3-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-287">Это право пользователя определяет, какие пользователи и группы могут выполнять задачи обслуживания для тома, такие как удаленная дефрагментация.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-287">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="d0fc3-288">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-288">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0fc3-289">Усерригхтсмодифифирмваринвиронмент</span><span class="sxs-lookup"><span data-stu-id="d0fc3-289">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="d0fc3-290">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-290">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-291">Это право пользователя определяет, кто может изменять значения в аппаратной среде.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-291">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="d0fc3-292">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-292">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0fc3-293">Усерригхтсмодифйобжектлабелс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-293">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="d0fc3-294">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-294">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-295">Это право пользователя определяет, какие учетные записи пользователей могут изменять метки целостности объектов, таких как файлы, разделы реестра или процессы, принадлежащие другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-295">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="d0fc3-296">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-296">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0fc3-297">Усерригхтспрофилесинглепроцесс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-297">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="d0fc3-298">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-298">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-299">Это право пользователя определяет, какие пользователи могут использовать средства мониторинга производительности для наблюдения за производительностью системных процессов.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-299">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="d0fc3-300">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-300">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0fc3-301">Усерригхтсремотешутдовн</span><span class="sxs-lookup"><span data-stu-id="d0fc3-301">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="d0fc3-302">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-302">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-303">Это право пользователя определяет, каким пользователям разрешено завершать работу компьютера из удаленного расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-303">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="d0fc3-304">Неправильное использование этого права пользователя может привести к отказу в обслуживании.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-304">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="d0fc3-305">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-305">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0fc3-306">Усерригхтсресторедата</span><span class="sxs-lookup"><span data-stu-id="d0fc3-306">userRightsRestoreData</span></span>|[<span data-ttu-id="d0fc3-307">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-307">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-308">Это право пользователя определяет, какие пользователи могут обходить разрешения для файлов, каталогов, реестра и других постоянных объектов при восстановлении резервных копий файлов и каталогов, и определяет, какие пользователи могут устанавливать любой действительный субъект безопасности в качестве владельца объекта.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-308">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="d0fc3-309">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-309">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0fc3-310">Усерригхтстакеовнершип</span><span class="sxs-lookup"><span data-stu-id="d0fc3-310">userRightsTakeOwnership</span></span>|[<span data-ttu-id="d0fc3-311">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-311">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-312">Это право пользователя определяет, какие пользователи могут становиться владельцами любого защищаемого объекта в системе, включая объекты Active Directory, файлы и папки, принтеры, разделы реестра, процессы и потоки.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-312">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="d0fc3-313">Поддерживаются только состояния NotConfigured и Allowed.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-313">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0fc3-314">Усерригхтсрегистерпроцессассервице</span><span class="sxs-lookup"><span data-stu-id="d0fc3-314">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="d0fc3-315">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0fc3-315">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0fc3-316">Этот параметр безопасности определяет, каким учетным записям служб запрещается регистрировать процесс в качестве службы.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-316">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="d0fc3-317">Примечание: этот параметр безопасности не применяется к системным, локальным или сетевым учетным записям служб.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-317">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="d0fc3-318">Поддерживается только блокирование состояния.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-318">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="d0fc3-319">Ксбокссервицесенаблексбоксгамесаветаск</span><span class="sxs-lookup"><span data-stu-id="d0fc3-319">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="d0fc3-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-320">Boolean</span></span>|<span data-ttu-id="d0fc3-321">Этот параметр определяет, включена ли функция сохранения игры Xbox (1) или отключена (0).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-321">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="d0fc3-322">Ксбокссервицесакцессориманажементсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="d0fc3-322">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="d0fc3-323">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-323">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="d0fc3-324">Этот параметр определяет, является ли тип запуска службы управления принадлежностью автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-324">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="d0fc3-325">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-325">Default: Manual.</span></span> <span data-ttu-id="d0fc3-326">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-326">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="d0fc3-327">Ксбокссервицесливеаусманажерсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="d0fc3-327">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="d0fc3-328">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-328">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="d0fc3-329">Этот параметр определяет, является ли тип запуска службы диспетчера Live auth автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-329">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="d0fc3-330">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-330">Default: Manual.</span></span> <span data-ttu-id="d0fc3-331">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-331">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="d0fc3-332">Ксбокссервицесливегамесавесервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="d0fc3-332">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="d0fc3-333">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-333">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="d0fc3-334">Этот параметр определяет, является ли тип запуска службы Live Save Service автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-334">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="d0fc3-335">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-335">Default: Manual.</span></span> <span data-ttu-id="d0fc3-336">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-336">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="d0fc3-337">Ксбокссервицесливенетворкингсервицестартупмоде</span><span class="sxs-lookup"><span data-stu-id="d0fc3-337">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="d0fc3-338">Сервицестарттипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-338">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="d0fc3-339">Этот параметр определяет, является ли тип запуска сетевой службы автоматическим (2), вручную (3), отключенным (4).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-339">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="d0fc3-340">По умолчанию: вручную.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-340">Default: Manual.</span></span> <span data-ttu-id="d0fc3-341">Возможные значения: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-341">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="d0fc3-342">Локалсекуритйоптионсблоккмикрософтаккаунтс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-342">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="d0fc3-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-343">Boolean</span></span>|<span data-ttu-id="d0fc3-344">Запретить пользователям добавлять новые учетные записи Майкрософт на этот компьютер.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-344">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="d0fc3-345">Локалсекуритйоптионсблоккремотелогонвисбланкпассворд</span><span class="sxs-lookup"><span data-stu-id="d0fc3-345">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="d0fc3-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-346">Boolean</span></span>|<span data-ttu-id="d0fc3-347">Включите локальные учетные записи, не защищенные паролем, для входа в систему из расположений, отличных от физического устройства. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="d0fc3-347">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="d0fc3-348">Локалсекуритйоптионсдисаблеадминистратораккаунт</span><span class="sxs-lookup"><span data-stu-id="d0fc3-348">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="d0fc3-349">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-349">Boolean</span></span>|<span data-ttu-id="d0fc3-350">Определяет, включена или отключена учетная запись локального администратора.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-350">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="d0fc3-351">Локалсекуритйоптионсадминистратораккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="d0fc3-351">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="d0fc3-352">String</span><span class="sxs-lookup"><span data-stu-id="d0fc3-352">String</span></span>|<span data-ttu-id="d0fc3-353">Определите имя другой учетной записи, которая будет связана с идентификатором безопасности (SID) учетной записи "Administrator".</span><span class="sxs-lookup"><span data-stu-id="d0fc3-353">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="d0fc3-354">Локалсекуритйоптионсдисаблегуестаккаунт</span><span class="sxs-lookup"><span data-stu-id="d0fc3-354">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="d0fc3-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-355">Boolean</span></span>|<span data-ttu-id="d0fc3-356">Определяет, включена или отключена Гостевая учетная запись.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-356">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="d0fc3-357">Локалсекуритйоптионсгуестаккаунтнаме</span><span class="sxs-lookup"><span data-stu-id="d0fc3-357">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="d0fc3-358">String</span><span class="sxs-lookup"><span data-stu-id="d0fc3-358">String</span></span>|<span data-ttu-id="d0fc3-359">Определите имя другой учетной записи, которая будет связана с идентификатором безопасности (SID) для учетной записи "гость".</span><span class="sxs-lookup"><span data-stu-id="d0fc3-359">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="d0fc3-360">Локалсекуритйоптионсалловундокквисаусавингтологон</span><span class="sxs-lookup"><span data-stu-id="d0fc3-360">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="d0fc3-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-361">Boolean</span></span>|<span data-ttu-id="d0fc3-362">Запретите отстыковку портативного компьютера без необходимости входа в систему.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-362">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="d0fc3-363">Локалсекуритйоптионсблоккусерсинсталлингпринтердриверс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-363">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="d0fc3-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-364">Boolean</span></span>|<span data-ttu-id="d0fc3-365">Ограничьте установку драйверов принтеров в рамках подключения к общему принтеру только для администраторов.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-365">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="d0fc3-366">Локалсекуритйоптионсблоккремотеоптикалдривеакцесс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-366">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="d0fc3-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-367">Boolean</span></span>|<span data-ttu-id="d0fc3-368">Включение этого параметра позволяет интерактивно вошедший в систему пользователь получать доступ к устройству чтения компакт-дисков.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-368">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="d0fc3-369">Локалсекуритйоптионсформатандежектофремоваблемедиаалловедусер</span><span class="sxs-lookup"><span data-stu-id="d0fc3-369">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="d0fc3-370">Локалсекуритйоптионсформатандежектофремоваблемедиаалловедусертипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-370">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="d0fc3-371">Определите, кому разрешено форматировать и извлекать съемные носители NTFS.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-371">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="d0fc3-372">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-372">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="d0fc3-373">Локалсекуритйоптионсмачинеинактивитилимит</span><span class="sxs-lookup"><span data-stu-id="d0fc3-373">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="d0fc3-374">Int32</span><span class="sxs-lookup"><span data-stu-id="d0fc3-374">Int32</span></span>|<span data-ttu-id="d0fc3-375">Определите максимальное количество минут отсутствия активности на экране входа интерактивного рабочего стола, пока не запустится экранная заставка.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-375">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="d0fc3-376">Допустимые значения — от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="d0fc3-376">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="d0fc3-377">Локалсекуритйоптионсмачинеинактивитилимитинминутес</span><span class="sxs-lookup"><span data-stu-id="d0fc3-377">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="d0fc3-378">Int32</span><span class="sxs-lookup"><span data-stu-id="d0fc3-378">Int32</span></span>|<span data-ttu-id="d0fc3-379">Определите максимальное количество минут отсутствия активности на экране входа интерактивного рабочего стола, пока не запустится экранная заставка.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-379">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="d0fc3-380">Допустимые значения — от 0 до 9999</span><span class="sxs-lookup"><span data-stu-id="d0fc3-380">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="d0fc3-381">Локалсекуритйоптионсдонотрекуиректрлалтдел</span><span class="sxs-lookup"><span data-stu-id="d0fc3-381">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="d0fc3-382">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-382">Boolean</span></span>|<span data-ttu-id="d0fc3-383">Требовать нажатия клавиш CTRL + ALT + DEL, прежде чем пользователь сможет войти в систему.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-383">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="d0fc3-384">Локалсекуритйоптионшиделастсигнединусер</span><span class="sxs-lookup"><span data-stu-id="d0fc3-384">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="d0fc3-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-385">Boolean</span></span>|<span data-ttu-id="d0fc3-386">Не отображать имя последнего пользователя, выполнившего вход на это устройство.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-386">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="d0fc3-387">Локалсекуритйоптионшидеусернамеатсигнин</span><span class="sxs-lookup"><span data-stu-id="d0fc3-387">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="d0fc3-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-388">Boolean</span></span>|<span data-ttu-id="d0fc3-389">Не отображать имя пользователя, выполняющего вход на это устройство, после ввода учетных данных и отображения рабочего стола на устройстве.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-389">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="d0fc3-390">Локалсекуритйоптионслогонмессажетитле</span><span class="sxs-lookup"><span data-stu-id="d0fc3-390">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="d0fc3-391">String</span><span class="sxs-lookup"><span data-stu-id="d0fc3-391">String</span></span>|<span data-ttu-id="d0fc3-392">Задайте заголовок сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-392">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="d0fc3-393">Локалсекуритйоптионслогонмессажетекст</span><span class="sxs-lookup"><span data-stu-id="d0fc3-393">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="d0fc3-394">String</span><span class="sxs-lookup"><span data-stu-id="d0fc3-394">String</span></span>|<span data-ttu-id="d0fc3-395">Задайте текст сообщения для пользователей, пытающихся войти в систему.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-395">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="d0fc3-396">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="d0fc3-396">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="d0fc3-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-397">Boolean</span></span>|<span data-ttu-id="d0fc3-398">Блокировать запросы проверки подлинности PKU2U на этом устройстве для использования сетевых удостоверений.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-398">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="d0fc3-399">Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажерхелпербул</span><span class="sxs-lookup"><span data-stu-id="d0fc3-399">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="d0fc3-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-400">Boolean</span></span>|<span data-ttu-id="d0fc3-401">Помощник по пользовательскому интерфейсу Boolean для объекта Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажер</span><span class="sxs-lookup"><span data-stu-id="d0fc3-401">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="d0fc3-402">Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажер</span><span class="sxs-lookup"><span data-stu-id="d0fc3-402">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="d0fc3-403">String</span><span class="sxs-lookup"><span data-stu-id="d0fc3-403">String</span></span>|<span data-ttu-id="d0fc3-404">Измените строку языка определения дескрипторов безопасности по умолчанию, чтобы разрешить или запретить пользователям и группам совершать удаленные вызовы в SAM.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-404">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="d0fc3-405">Локалсекуритйоптионсминимумсессионсекуритифорнтлмсспбаседклиентс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="d0fc3-406">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="d0fc3-406">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="d0fc3-407">Этот параметр безопасности позволяет клиенту требовать согласование 128-разрядного шифрования и/или сеанса защиты сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-407">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="d0fc3-408">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-408">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="d0fc3-409">Локалсекуритйоптионсминимумсессионсекуритифорнтлмсспбаседсерверс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-409">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="d0fc3-410">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="d0fc3-410">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="d0fc3-411">Этот параметр безопасности позволяет серверу требовать согласование 128-разрядного шифрования и/или сеанса защиты сеанса NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-411">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="d0fc3-412">Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-412">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="d0fc3-413">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="d0fc3-413">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="d0fc3-414">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="d0fc3-414">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="d0fc3-415">Этот параметр безопасности определяет, какой протокол проверки подлинности "запрос/ответ" используется для входа в сеть.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-415">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="d0fc3-416">Возможные значения: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-416">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="d0fc3-417">Ланманажерворкстатиондисаблеинсекурегуестлогонс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-417">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="d0fc3-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-418">Boolean</span></span>|<span data-ttu-id="d0fc3-419">Если этот параметр включен, клиент SMB будет разрешать небезопасные гостевые входы.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-419">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="d0fc3-420">Если этот параметр не настроен, клиент SMB будет отклонять небезопасные гостевые входы.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-420">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="d0fc3-421">Локалсекуритйоптионсклеарвиртуалмеморипажефиле</span><span class="sxs-lookup"><span data-stu-id="d0fc3-421">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="d0fc3-422">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-422">Boolean</span></span>|<span data-ttu-id="d0fc3-423">Этот параметр безопасности определяет, будет ли очищаться файл подкачки виртуальной памяти при завершении работы системы.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-423">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="d0fc3-424">Локалсекуритйоптионсалловсистемтобешутдовнвисаусавингтологон</span><span class="sxs-lookup"><span data-stu-id="d0fc3-424">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="d0fc3-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-425">Boolean</span></span>|<span data-ttu-id="d0fc3-426">Этот параметр безопасности определяет, можно ли завершить работу компьютера, не выполняя вход в Windows.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-426">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="d0fc3-427">Локалсекуритйоптионсалловуиакцессаппликатионелеватион</span><span class="sxs-lookup"><span data-stu-id="d0fc3-427">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="d0fc3-428">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-428">Boolean</span></span>|<span data-ttu-id="d0fc3-429">Разрешить UIAccess Apps запрос на повышение прав без использования безопасного рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-429">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="d0fc3-430">Локалсекуритйоптионсвиртуализефилеандрегистривритефаилурестоперусерлокатионс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-430">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="d0fc3-431">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-431">Boolean</span></span>|<span data-ttu-id="d0fc3-432">Виртуализация сбоев записи в файл и реестр для отдельных расположений пользователей</span><span class="sxs-lookup"><span data-stu-id="d0fc3-432">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="d0fc3-433">Локалсекуритйоптионсонлелеватесигнедексекутаблес</span><span class="sxs-lookup"><span data-stu-id="d0fc3-433">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="d0fc3-434">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-434">Boolean</span></span>|<span data-ttu-id="d0fc3-435">Принудительная проверка пути сертификации PKI для указанного исполняемого файла перед тем, как он будет разрешен для запуска.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-435">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="d0fc3-436">Локалсекуритйоптионсадминистраторелеватионпромптбехавиор</span><span class="sxs-lookup"><span data-stu-id="d0fc3-436">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="d0fc3-437">Локалсекуритйоптионсадминистраторелеватионпромптбехавиортипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-437">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="d0fc3-438">Определите поведение запросов на повышение прав для администраторов в режиме одобрения администратором.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-438">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="d0fc3-439">Возможные значения: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-439">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="d0fc3-440">Локалсекуритйоптионсстандардусерелеватионпромптбехавиор</span><span class="sxs-lookup"><span data-stu-id="d0fc3-440">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="d0fc3-441">Локалсекуритйоптионсстандардусерелеватионпромптбехавиортипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-441">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="d0fc3-442">Определите поведение запросов на повышение прав для стандартных пользователей.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-442">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="d0fc3-443">Возможные значения: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-443">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="d0fc3-444">Локалсекуритйоптионссвитчтосекуредесктопвхенпромптингфорелеватион</span><span class="sxs-lookup"><span data-stu-id="d0fc3-444">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="d0fc3-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-445">Boolean</span></span>|<span data-ttu-id="d0fc3-446">Разрешить всем запросам на повышение прав доступ к рабочему столу интерактивного пользователя, а не к безопасному рабочему столу.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-446">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="d0fc3-447">Используются параметры политики поведения запросов для администраторов и стандартных пользователей.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-447">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="d0fc3-448">Локалсекуритйоптионсдетектаппликатионинсталлатионсандпромптфорелеватион</span><span class="sxs-lookup"><span data-stu-id="d0fc3-448">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="d0fc3-449">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-449">Boolean</span></span>|<span data-ttu-id="d0fc3-450">При установке приложений, требующих повышенных привилегий, запрашиваются учетные данные администратора. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="d0fc3-450">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="d0fc3-451">Локалсекуритйоптионсалловуиакцессаппликатионсфорсекурелокатионс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-451">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="d0fc3-452">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-452">Boolean</span></span>|<span data-ttu-id="d0fc3-453">Разрешить UIAccess Apps запрос на повышение прав без использования безопасного рабочего стола. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="d0fc3-453">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="d0fc3-454">Локалсекуритйоптионсусеадминаппровалмоде</span><span class="sxs-lookup"><span data-stu-id="d0fc3-454">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="d0fc3-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-455">Boolean</span></span>|<span data-ttu-id="d0fc3-456">Определяет, использует ли встроенная учетная запись администратора режим одобрения администратором или выполняет все приложения с правами полного администратора. Включено по умолчанию</span><span class="sxs-lookup"><span data-stu-id="d0fc3-456">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="d0fc3-457">Локалсекуритйоптионсусеадминаппровалмодефорадминистраторс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-457">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="d0fc3-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-458">Boolean</span></span>|<span data-ttu-id="d0fc3-459">Определить, включен ли режим одобрения администратором и все параметры политики контроля учетных записей, по умолчанию включено</span><span class="sxs-lookup"><span data-stu-id="d0fc3-459">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="d0fc3-460">Локалсекуритйоптионсинформатионшовнонлоккскрин</span><span class="sxs-lookup"><span data-stu-id="d0fc3-460">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="d0fc3-461">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="d0fc3-461">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="d0fc3-462">Настройте сведения о пользователе, которые отображаются, когда сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-462">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="d0fc3-463">Если этот флажок не установлен, отображаются отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-463">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="d0fc3-464">Возможные значения: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-464">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="d0fc3-465">Локалсекуритйоптионсинформатиондисплайедонлоккскрин</span><span class="sxs-lookup"><span data-stu-id="d0fc3-465">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="d0fc3-466">Локалсекуритйоптионсинформатиондисплайедонлоккскринтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-466">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="d0fc3-467">Настройте сведения о пользователе, которые отображаются, когда сеанс заблокирован.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-467">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="d0fc3-468">Если этот флажок не установлен, отображаются отображаемое имя пользователя, домен и имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-468">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="d0fc3-469">Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-469">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="d0fc3-470">Локалсекуритйоптионсдисаблеклиентдигиталлисигнкоммуникатионсифсерверагрис</span><span class="sxs-lookup"><span data-stu-id="d0fc3-470">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="d0fc3-471">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-471">Boolean</span></span>|<span data-ttu-id="d0fc3-472">Этот параметр безопасности определяет, будет ли клиент SMB пытаться согласовать подписывание SMB пакетов.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-472">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="d0fc3-473">Локалсекуритйоптионсклиентдигиталлисигнкоммуникатионсалвайс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-473">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="d0fc3-474">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-474">Boolean</span></span>|<span data-ttu-id="d0fc3-475">Этот параметр безопасности определяет, требуется ли Подписывание пакетов для клиентского SMB-компонента.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-475">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="d0fc3-476">Локалсекуритйоптионсклиентсендуненкриптедпассвордтосирдпартисмбсерверс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-476">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="d0fc3-477">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-477">Boolean</span></span>|<span data-ttu-id="d0fc3-478">Если этот параметр безопасности включен, перенаправителем SMB (Server Message Block) разрешено отправлять пароли открытым текстом на серверы SMB сторонних производителей, не поддерживающие шифрование паролей во время проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-478">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="d0fc3-479">Локалсекуритйоптионсдисаблесервердигиталлисигнкоммуникатионсалвайс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-479">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="d0fc3-480">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-480">Boolean</span></span>|<span data-ttu-id="d0fc3-481">Этот параметр безопасности определяет, требуется ли подписи пакетов для SMB-компонентов сервера.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-481">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="d0fc3-482">Локалсекуритйоптионсдисаблесервердигиталлисигнкоммуникатионсифклиентагрис</span><span class="sxs-lookup"><span data-stu-id="d0fc3-482">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="d0fc3-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-483">Boolean</span></span>|<span data-ttu-id="d0fc3-484">Этот параметр безопасности определяет, будет ли SMB согласовывать подпись SMB Packet с клиентами, которые их запрашивают.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-484">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="d0fc3-485">Локалсекуритйоптионсрестриктанонимаусакцесстонамедпипесандшарес</span><span class="sxs-lookup"><span data-stu-id="d0fc3-485">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="d0fc3-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-486">Boolean</span></span>|<span data-ttu-id="d0fc3-487">По умолчанию этот параметр безопасности запрещает анонимный доступ к ресурсам и каналам к параметрам именованных каналов, к которым возможен анонимный доступ, и к общедоступным ресурсам, к которым возможен анонимный доступ</span><span class="sxs-lookup"><span data-stu-id="d0fc3-487">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="d0fc3-488">Локалсекуритйоптионсдоноталлованонимаусенумератионофсамаккаунтс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-488">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="d0fc3-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-489">Boolean</span></span>|<span data-ttu-id="d0fc3-490">Этот параметр безопасности определяет, какие дополнительные разрешения будут предоставлены анонимным подключениям к компьютеру.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-490">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="d0fc3-491">Локалсекуритйоптионсаллованонимаусенумератионофсамаккаунтсандшарес</span><span class="sxs-lookup"><span data-stu-id="d0fc3-491">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="d0fc3-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-492">Boolean</span></span>|<span data-ttu-id="d0fc3-493">Этот параметр безопасности определяет, разрешено ли анонимным пользователям выполнять определенные действия, например перечислять имена доменных учетных записей и сетевые общие папки.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-493">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="d0fc3-494">Локалсекуритйоптионсдонотстореланманажерхашвалуеоннекстпассвордчанже</span><span class="sxs-lookup"><span data-stu-id="d0fc3-494">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="d0fc3-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-495">Boolean</span></span>|<span data-ttu-id="d0fc3-496">Этот параметр безопасности определяет, будет ли сохраняться значение хэша LAN Manager (LM) для нового пароля при следующем изменении пароля.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-496">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="d0fc3-497">По умолчанию он не хранится.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-497">It’s not stored by default.</span></span>|
|<span data-ttu-id="d0fc3-498">Локалсекуритйоптионссмарткардремовалбехавиор</span><span class="sxs-lookup"><span data-stu-id="d0fc3-498">localSecurityOptionsSmartCardRemovalBehavior</span></span>|<span data-ttu-id="d0fc3-499">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md);</span><span class="sxs-lookup"><span data-stu-id="d0fc3-499">[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)</span></span>|<span data-ttu-id="d0fc3-500">Этот параметр безопасности определяет, что происходит при удалении смарт-карты пользователя, выполнившего вход в систему, из устройства чтения смарт-карт.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-500">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="d0fc3-501">Возможные значения: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-501">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="d0fc3-502">Дефендерсекуритицентердисаблеаппбровсеруи</span><span class="sxs-lookup"><span data-stu-id="d0fc3-502">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="d0fc3-503">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-503">Boolean</span></span>|<span data-ttu-id="d0fc3-504">Используется для отключения отображения области защиты приложений и браузера.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-504">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="d0fc3-505">Дефендерсекуритицентердисаблефамилюи</span><span class="sxs-lookup"><span data-stu-id="d0fc3-505">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="d0fc3-506">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-506">Boolean</span></span>|<span data-ttu-id="d0fc3-507">Используется для отключения отображения области семьи.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-507">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="d0fc3-508">Дефендерсекуритицентердисаблехеалсуи</span><span class="sxs-lookup"><span data-stu-id="d0fc3-508">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="d0fc3-509">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-509">Boolean</span></span>|<span data-ttu-id="d0fc3-510">Используется для отключения отображения области производительности и работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-510">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="d0fc3-511">Дефендерсекуритицентердисабленетворкуи</span><span class="sxs-lookup"><span data-stu-id="d0fc3-511">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="d0fc3-512">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-512">Boolean</span></span>|<span data-ttu-id="d0fc3-513">Используется для отключения отображения зоны "брандмауэр" и "Защита сети".</span><span class="sxs-lookup"><span data-stu-id="d0fc3-513">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="d0fc3-514">Дефендерсекуритицентердисаблевирусуи</span><span class="sxs-lookup"><span data-stu-id="d0fc3-514">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="d0fc3-515">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-515">Boolean</span></span>|<span data-ttu-id="d0fc3-516">Используется для отключения отображения области защиты от вирусов и угроз.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-516">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="d0fc3-517">Дефендерсекуритицентердисаблеаккаунтуи</span><span class="sxs-lookup"><span data-stu-id="d0fc3-517">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="d0fc3-518">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-518">Boolean</span></span>|<span data-ttu-id="d0fc3-519">Используется для отключения отображения области защиты учетных записей.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-519">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="d0fc3-520">Дефендерсекуритицентердисаблеклеартпмуи</span><span class="sxs-lookup"><span data-stu-id="d0fc3-520">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="d0fc3-521">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-521">Boolean</span></span>|<span data-ttu-id="d0fc3-522">Используется для отключения отображения кнопки Очистить доверенный платформенный модуль.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-522">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="d0fc3-523">Дефендерсекуритицентердисаблехардвареуи</span><span class="sxs-lookup"><span data-stu-id="d0fc3-523">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="d0fc3-524">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-524">Boolean</span></span>|<span data-ttu-id="d0fc3-525">Используется для отключения отображения области аппаратной защиты.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-525">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="d0fc3-526">Дефендерсекуритицентердисабленотификатионареауи</span><span class="sxs-lookup"><span data-stu-id="d0fc3-526">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="d0fc3-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-527">Boolean</span></span>|<span data-ttu-id="d0fc3-528">Используется для отключения отображения элемента управления "область уведомлений".</span><span class="sxs-lookup"><span data-stu-id="d0fc3-528">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="d0fc3-529">Для вступления этого параметра в силу пользователю необходимо выйти из системы и войти в нее, а затем перезагрузить компьютер.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-529">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="d0fc3-530">Дефендерсекуритицентердисаблерансомвареуи</span><span class="sxs-lookup"><span data-stu-id="d0fc3-530">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="d0fc3-531">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-531">Boolean</span></span>|<span data-ttu-id="d0fc3-532">Используется для отключения отображения области защиты от пошантажистом.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-532">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="d0fc3-533">Дефендерсекуритицентердисаблесекуребутуи</span><span class="sxs-lookup"><span data-stu-id="d0fc3-533">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="d0fc3-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-534">Boolean</span></span>|<span data-ttu-id="d0fc3-535">Используется для отключения отображения области безопасной загрузки в разделе Безопасность устройства.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-535">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="d0fc3-536">Дефендерсекуритицентердисаблетраублешутингуи</span><span class="sxs-lookup"><span data-stu-id="d0fc3-536">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="d0fc3-537">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-537">Boolean</span></span>|<span data-ttu-id="d0fc3-538">Используется для отключения отображения устранения неполадок процесса безопасности в разделе Безопасность устройства.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-538">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="d0fc3-539">Дефендерсекуритицентердисаблевулнераблетпмфирмвареупдатеуи</span><span class="sxs-lookup"><span data-stu-id="d0fc3-539">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="d0fc3-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-540">Boolean</span></span>|<span data-ttu-id="d0fc3-541">Используется для отключения отображения обновления микропрограммы доверенного платформенного модуля при обнаружении уязвимого программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-541">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="d0fc3-542">Дефендерсекуритицентерорганизатиондисплайнаме</span><span class="sxs-lookup"><span data-stu-id="d0fc3-542">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="d0fc3-543">String</span><span class="sxs-lookup"><span data-stu-id="d0fc3-543">String</span></span>|<span data-ttu-id="d0fc3-544">Имя компании, которое отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-544">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="d0fc3-545">Дефендерсекуритицентерхелпемаил</span><span class="sxs-lookup"><span data-stu-id="d0fc3-545">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="d0fc3-546">String</span><span class="sxs-lookup"><span data-stu-id="d0fc3-546">String</span></span>|<span data-ttu-id="d0fc3-547">Адрес электронной почты, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-547">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="d0fc3-548">Дефендерсекуритицентерхелпфоне</span><span class="sxs-lookup"><span data-stu-id="d0fc3-548">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="d0fc3-549">String</span><span class="sxs-lookup"><span data-stu-id="d0fc3-549">String</span></span>|<span data-ttu-id="d0fc3-550">Номер телефона или идентификатор Skype, который отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-550">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="d0fc3-551">Дефендерсекуритицентерхелпурл</span><span class="sxs-lookup"><span data-stu-id="d0fc3-551">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="d0fc3-552">String</span><span class="sxs-lookup"><span data-stu-id="d0fc3-552">String</span></span>|<span data-ttu-id="d0fc3-553">URL-адрес портала справки это отображается для пользователей.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-553">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="d0fc3-554">Дефендерсекуритицентернотификатионсфромапп</span><span class="sxs-lookup"><span data-stu-id="d0fc3-554">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="d0fc3-555">Дефендерсекуритицентернотификатионсфромапптипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-555">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="d0fc3-556">Уведомления, отображаемые в отображаемых областях приложения.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-556">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="d0fc3-557">Возможные значения: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-557">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="d0fc3-558">Дефендерсекуритицентеритконтактдисплай</span><span class="sxs-lookup"><span data-stu-id="d0fc3-558">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="d0fc3-559">Дефендерсекуритицентеритконтактдисплайтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-559">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="d0fc3-560">Настройка места отображения контактной информации для конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-560">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="d0fc3-561">Возможные значения: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-561">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="d0fc3-562">Виндовсдефендертамперпротектион</span><span class="sxs-lookup"><span data-stu-id="d0fc3-562">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="d0fc3-563">Виндовсдефендертамперпротектионоптионс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-563">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="d0fc3-564">Настройка параметров Тамперпротектион для защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-564">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="d0fc3-565">Возможные значения: `notConfigured`, `enable`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-565">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="d0fc3-566">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="d0fc3-566">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="d0fc3-567">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-567">Boolean</span></span>|<span data-ttu-id="d0fc3-568">Блокирует FTP-подключения к устройству с отслеживанием состояния.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-568">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="d0fc3-569">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="d0fc3-569">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="d0fc3-570">Int32</span><span class="sxs-lookup"><span data-stu-id="d0fc3-570">Int32</span></span>|<span data-ttu-id="d0fc3-571">Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-571">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="d0fc3-572">По истечении этого срока сопоставления безопасности перестают действовать и удаляются.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-572">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="d0fc3-573">Допустимые значения: от 300 до 3600</span><span class="sxs-lookup"><span data-stu-id="d0fc3-573">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="d0fc3-574">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="d0fc3-574">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="d0fc3-575">Фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-575">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="d0fc3-576">Выберите используемую кодировку с общим ключом.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-576">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="d0fc3-577">Возможные значения: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-577">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="d0fc3-578">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="d0fc3-578">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="d0fc3-579">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-579">Boolean</span></span>|<span data-ttu-id="d0fc3-580">Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-580">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="d0fc3-581">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="d0fc3-581">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="d0fc3-582">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-582">Boolean</span></span>|<span data-ttu-id="d0fc3-583">Настраивает исключения IPSec для разрешения ICMP</span><span class="sxs-lookup"><span data-stu-id="d0fc3-583">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="d0fc3-584">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="d0fc3-584">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="d0fc3-585">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-585">Boolean</span></span>|<span data-ttu-id="d0fc3-586">Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-586">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="d0fc3-587">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="d0fc3-587">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="d0fc3-588">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-588">Boolean</span></span>|<span data-ttu-id="d0fc3-589">Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6</span><span class="sxs-lookup"><span data-stu-id="d0fc3-589">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="d0fc3-590">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="d0fc3-590">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="d0fc3-591">Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-591">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="d0fc3-592">Укажите способ применения списка отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-592">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="d0fc3-593">Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-593">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="d0fc3-594">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="d0fc3-594">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="d0fc3-595">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-595">Boolean</span></span>|<span data-ttu-id="d0fc3-596">Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор</span><span class="sxs-lookup"><span data-stu-id="d0fc3-596">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="d0fc3-597">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="d0fc3-597">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="d0fc3-598">Фиреваллпаккеткуеуеингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-598">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="d0fc3-599">Настраивает способ применения очередей пакетов в сценарии туннельного шлюза.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-599">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="d0fc3-600">Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-600">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="d0fc3-601">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="d0fc3-601">firewallProfileDomain</span></span>|[<span data-ttu-id="d0fc3-602">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d0fc3-602">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="d0fc3-603">Настраивает параметры профиля брандмауэра для доменных сетей</span><span class="sxs-lookup"><span data-stu-id="d0fc3-603">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="d0fc3-604">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="d0fc3-604">firewallProfilePublic</span></span>|[<span data-ttu-id="d0fc3-605">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d0fc3-605">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="d0fc3-606">Настраивает параметры профиля брандмауэра для общедоступных сетей</span><span class="sxs-lookup"><span data-stu-id="d0fc3-606">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="d0fc3-607">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="d0fc3-607">firewallProfilePrivate</span></span>|[<span data-ttu-id="d0fc3-608">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d0fc3-608">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="d0fc3-609">Настраивает параметры профиля брандмауэра для частных сетей</span><span class="sxs-lookup"><span data-stu-id="d0fc3-609">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="d0fc3-610">Дефендерадобереадерлаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-610">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="d0fc3-611">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-611">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0fc3-612">Значение, указывающее поведение Adobe Reader при создании дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-612">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="d0fc3-613">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-613">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-614">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="d0fc3-614">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="d0fc3-615">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d0fc3-615">String collection</span></span>|<span data-ttu-id="d0fc3-616">Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак</span><span class="sxs-lookup"><span data-stu-id="d0fc3-616">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="d0fc3-617">Дефендероффицеаппсосерпроцессинжектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-617">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="d0fc3-618">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-618">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0fc3-619">Значение, указывающее поведение приложений Office, добавляемых в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-619">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="d0fc3-620">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-620">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-621">Дефендероффицеаппсосерпроцессинжектион</span><span class="sxs-lookup"><span data-stu-id="d0fc3-621">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="d0fc3-622">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-622">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0fc3-623">Значение, указывающее поведение приложений Office, добавляемых в другие процессы.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-623">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="d0fc3-624">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-624">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-625">Дефендероффицекоммуникатионаппслаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-625">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="d0fc3-626">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-626">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0fc3-627">Значение, определяющее поведение приложений для связи с Office, включая Microsoft Outlook, от создания дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-627">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="d0fc3-628">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-628">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-629">Дефендероффицеаппсексекутаблеконтенткреатионорлаунчтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-629">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="d0fc3-630">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-630">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0fc3-631">Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого контента.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-631">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="d0fc3-632">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-632">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-633">Дефендероффицеаппсексекутаблеконтенткреатионорлаунч</span><span class="sxs-lookup"><span data-stu-id="d0fc3-633">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="d0fc3-634">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-634">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0fc3-635">Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого контента.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-635">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="d0fc3-636">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-636">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-637">Дефендероффицеаппслаунччилдпроцесстипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-637">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="d0fc3-638">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-638">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0fc3-639">Значение, указывающее поведение запуска приложения Office для дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-639">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="d0fc3-640">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-640">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-641">Дефендероффицеаппслаунччилдпроцесс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-641">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="d0fc3-642">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-642">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0fc3-643">Значение, указывающее поведение запуска приложения Office для дочерних процессов.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-643">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="d0fc3-644">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-644">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-645">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="d0fc3-645">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="d0fc3-646">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-646">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0fc3-647">Значение, указывающее поведение импорта Win32 из кода макросов в Office.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-647">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="d0fc3-648">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-648">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-649">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="d0fc3-649">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="d0fc3-650">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-650">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0fc3-651">Значение, указывающее поведение импорта Win32 из кода макросов в Office.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-651">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="d0fc3-652">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-652">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-653">Дефендерскриптобфускатедмакрокодетипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-653">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="d0fc3-654">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-654">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0fc3-655">Значение, определяющее поведение кода "замаскированный JS/VBS/PS/макрос".</span><span class="sxs-lookup"><span data-stu-id="d0fc3-655">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="d0fc3-656">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-656">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-657">Дефендерскриптобфускатедмакрокоде</span><span class="sxs-lookup"><span data-stu-id="d0fc3-657">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="d0fc3-658">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-658">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0fc3-659">Значение, определяющее поведение кода "замаскированный JS/VBS/PS/макрос".</span><span class="sxs-lookup"><span data-stu-id="d0fc3-659">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="d0fc3-660">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-660">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-661">Дефендерскриптдовнлоадедпайлоадексекутионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-661">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="d0fc3-662">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-662">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0fc3-663">Значение, определяющее поведение JS-и VBS-данных, загруженных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-663">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="d0fc3-664">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-664">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-665">Дефендерскриптдовнлоадедпайлоадексекутион</span><span class="sxs-lookup"><span data-stu-id="d0fc3-665">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="d0fc3-666">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-666">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0fc3-667">Значение, определяющее поведение JS-и VBS-данных, загруженных из Интернета.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-667">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="d0fc3-668">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-668">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-669">Дефендерпревенткредентиалстеалингтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-669">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="d0fc3-670">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-670">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0fc3-671">Значение, указывающее, разрешено ли перенос учетных данных из подсистемы локального центра безопасности Windows.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-671">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="d0fc3-672">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-672">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-673">Дефендерпроцесскреатионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-673">defenderProcessCreationType</span></span>|[<span data-ttu-id="d0fc3-674">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-674">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0fc3-675">Значение, указывающее ответ на создание процессов, исходящих от команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-675">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="d0fc3-676">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-676">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-677">Дефендерпроцесскреатион</span><span class="sxs-lookup"><span data-stu-id="d0fc3-677">defenderProcessCreation</span></span>|[<span data-ttu-id="d0fc3-678">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-678">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0fc3-679">Значение, указывающее ответ на создание процессов, исходящих от команд PSExec и WMI.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-679">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="d0fc3-680">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-680">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-681">Дефендерунтрустедусбпроцесстипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-681">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="d0fc3-682">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-682">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0fc3-683">Значение, указывающее ответ на недоверенные и неподписанные процессы, которые запускаются с USB.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-683">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="d0fc3-684">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-684">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-685">Дефендерунтрустедусбпроцесс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-685">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="d0fc3-686">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-686">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0fc3-687">Значение, указывающее ответ на недоверенные и неподписанные процессы, которые запускаются с USB.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-687">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="d0fc3-688">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-688">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-689">Дефендерунтрустедексекутаблетипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-689">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="d0fc3-690">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-690">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0fc3-691">Значение, указывающее ответ на исполняемые файлы, которые не отвечают условиям преобладание, возраст или доверенного списка.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-691">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="d0fc3-692">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-692">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-693">Дефендерунтрустедексекутабле</span><span class="sxs-lookup"><span data-stu-id="d0fc3-693">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="d0fc3-694">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-694">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0fc3-695">Значение, указывающее ответ на исполняемые файлы, которые не отвечают условиям преобладание, возраст или доверенного списка.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-695">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="d0fc3-696">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-696">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-697">Дефендеремаилконтентексекутионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-697">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="d0fc3-698">Дефендераттакксурфацетипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-698">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0fc3-699">Значение, указывающее, следует ли удалять исполняемые файлы (exe, DLL, PS, JS, VBS и т. д.) из электронной почты (почтовая или почтовая программа).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-699">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="d0fc3-700">Возможные значения: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-700">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-701">Дефендеремаилконтентексекутион</span><span class="sxs-lookup"><span data-stu-id="d0fc3-701">defenderEmailContentExecution</span></span>|[<span data-ttu-id="d0fc3-702">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-702">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0fc3-703">Значение, указывающее, следует ли удалять исполняемые файлы (exe, DLL, PS, JS, VBS и т. д.) из электронной почты (почтовая или почтовая программа).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-703">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="d0fc3-704">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-704">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-705">Дефендерадванцедрансомеварепротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-705">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="d0fc3-706">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-706">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0fc3-707">Значение, указывающее на использование расширенной защиты в рансомеваре.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-707">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="d0fc3-708">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-708">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-709">Дефендергуардмифолдерстипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-709">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="d0fc3-710">Фолдерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-710">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="d0fc3-711">Значение, указывающее поведение защищенных папок.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-711">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="d0fc3-712">Возможные значения: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-712">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="d0fc3-713">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="d0fc3-713">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="d0fc3-714">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d0fc3-714">String collection</span></span>|<span data-ttu-id="d0fc3-715">Список путей к файлам EXE, которым разрешен доступ к защищенным папкам</span><span class="sxs-lookup"><span data-stu-id="d0fc3-715">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="d0fc3-716">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="d0fc3-716">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="d0fc3-717">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d0fc3-717">String collection</span></span>|<span data-ttu-id="d0fc3-718">Список путей к папкам, которые следует добавить в список защищенных папок</span><span class="sxs-lookup"><span data-stu-id="d0fc3-718">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="d0fc3-719">Дефендернетворкпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-719">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="d0fc3-720">Дефендерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-720">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0fc3-721">Значение, указывающее поведение Нетворкпротектион.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-721">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="d0fc3-722">Возможные значения: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-722">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0fc3-723">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="d0fc3-723">defenderExploitProtectionXml</span></span>|<span data-ttu-id="d0fc3-724">Binary</span><span class="sxs-lookup"><span data-stu-id="d0fc3-724">Binary</span></span>|<span data-ttu-id="d0fc3-725">XML-файл с информацией о защите от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-725">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="d0fc3-726">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="d0fc3-726">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="d0fc3-727">String</span><span class="sxs-lookup"><span data-stu-id="d0fc3-727">String</span></span>|<span data-ttu-id="d0fc3-728">Имя файла, из которого получено свойство DefenderExploitProtectionXml.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-728">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="d0fc3-729">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="d0fc3-729">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="d0fc3-730">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-730">Boolean</span></span>|<span data-ttu-id="d0fc3-731">Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-731">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="d0fc3-732">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="d0fc3-732">appLockerApplicationControl</span></span>|[<span data-ttu-id="d0fc3-733">Апплоккераппликатионконтролтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-733">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="d0fc3-734">Позволяет администратору выбирать разрешенные типы приложений для устройств.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-734">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="d0fc3-735">Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-735">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="d0fc3-736">Девицегуардлокалсистемаусоритикредентиалгуардсеттингс</span><span class="sxs-lookup"><span data-stu-id="d0fc3-736">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="d0fc3-737">Девицегуардлокалсистемаусоритикредентиалгуардтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-737">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="d0fc3-738">Включите Guard в учетных данных, когда включен уровень безопасности платформы с безопасной загрузкой и безопасностью на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-738">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="d0fc3-739">Возможные значения: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-739">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="d0fc3-740">Девицегуарденаблевиртуализатионбаседсекурити</span><span class="sxs-lookup"><span data-stu-id="d0fc3-740">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="d0fc3-741">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-741">Boolean</span></span>|<span data-ttu-id="d0fc3-742">Включает безопасность на основе виртуализации (VBS).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-742">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="d0fc3-743">Девицегуарденаблесекуребутвисдма</span><span class="sxs-lookup"><span data-stu-id="d0fc3-743">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="d0fc3-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-744">Boolean</span></span>|<span data-ttu-id="d0fc3-745">Это свойство будет устаревшим в 2019 мая и будет заменено свойством Девицегуардсекуребутвисдма.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-745">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="d0fc3-746">Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-746">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="d0fc3-747">Девицегуардсекуребутвисдма</span><span class="sxs-lookup"><span data-stu-id="d0fc3-747">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="d0fc3-748">Секуребутвисдматипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-748">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="d0fc3-749">Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-749">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="d0fc3-750">Возможные значения: `notConfigured`, `withoutDMA`, `withDMA`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-750">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="d0fc3-751">Девицегуардлаунчсистемгуард</span><span class="sxs-lookup"><span data-stu-id="d0fc3-751">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="d0fc3-752">Включение</span><span class="sxs-lookup"><span data-stu-id="d0fc3-752">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="d0fc3-753">Позволяет ИТ – администратору настраивать запуск системы защиты системы.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-753">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="d0fc3-754">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-754">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="d0fc3-755">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="d0fc3-755">smartScreenEnableInShell</span></span>|<span data-ttu-id="d0fc3-756">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-756">Boolean</span></span>|<span data-ttu-id="d0fc3-757">Позволяет ИТ-администраторам настраивать SmartScreen для Windows.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-757">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="d0fc3-758">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="d0fc3-758">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="d0fc3-759">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-759">Boolean</span></span>|<span data-ttu-id="d0fc3-760">Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-760">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="d0fc3-761">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="d0fc3-761">applicationGuardEnabled</span></span>|<span data-ttu-id="d0fc3-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-762">Boolean</span></span>|<span data-ttu-id="d0fc3-763">Включение Application Guard в Защитнике Windows</span><span class="sxs-lookup"><span data-stu-id="d0fc3-763">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="d0fc3-764">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="d0fc3-764">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="d0fc3-765">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="d0fc3-765">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="d0fc3-766">Включение Application Guard в Защитнике Windows для более новых сборок Windows.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-766">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="d0fc3-767">Возможные значения: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-767">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="d0fc3-768">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="d0fc3-768">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="d0fc3-769">Аппликатионгуардблоккфилетрансфертипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-769">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="d0fc3-770">Блокировать буфер обмена для передачи файла изображения, текстового файла или ни одного из них.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-770">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="d0fc3-771">Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-771">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="d0fc3-772">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="d0fc3-772">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="d0fc3-773">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-773">Boolean</span></span>|<span data-ttu-id="d0fc3-774">Позволяет заблокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-774">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="d0fc3-775">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="d0fc3-775">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="d0fc3-776">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-776">Boolean</span></span>|<span data-ttu-id="d0fc3-777">Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).</span><span class="sxs-lookup"><span data-stu-id="d0fc3-777">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="d0fc3-778">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="d0fc3-778">applicationGuardForceAuditing</span></span>|<span data-ttu-id="d0fc3-779">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-779">Boolean</span></span>|<span data-ttu-id="d0fc3-780">Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-780">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="d0fc3-781">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="d0fc3-781">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="d0fc3-782">Аппликатионгуардблоккклипбоардшарингтипе</span><span class="sxs-lookup"><span data-stu-id="d0fc3-782">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="d0fc3-783">Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-783">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="d0fc3-784">Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-784">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="d0fc3-785">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="d0fc3-785">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="d0fc3-786">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-786">Boolean</span></span>|<span data-ttu-id="d0fc3-787">Позволяет разрешить печать в PDF из контейнера.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-787">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="d0fc3-788">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="d0fc3-788">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="d0fc3-789">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-789">Boolean</span></span>|<span data-ttu-id="d0fc3-790">Позволяет разрешить печать в XPS из контейнера.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-790">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="d0fc3-791">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="d0fc3-791">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="d0fc3-792">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-792">Boolean</span></span>|<span data-ttu-id="d0fc3-793">Позволяет разрешить печать на локальных принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-793">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="d0fc3-794">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="d0fc3-794">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="d0fc3-795">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-795">Boolean</span></span>|<span data-ttu-id="d0fc3-796">Позволяет разрешить печать на сетевых принтерах из контейнера.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-796">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="d0fc3-797">Аппликатионгуардалловвиртуалгпу</span><span class="sxs-lookup"><span data-stu-id="d0fc3-797">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="d0fc3-798">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-798">Boolean</span></span>|<span data-ttu-id="d0fc3-799">Разрешить приложению Application Guard использовать виртуальный GPU</span><span class="sxs-lookup"><span data-stu-id="d0fc3-799">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="d0fc3-800">Аппликатионгуардалловфилесавеонхост</span><span class="sxs-lookup"><span data-stu-id="d0fc3-800">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="d0fc3-801">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-801">Boolean</span></span>|<span data-ttu-id="d0fc3-802">Разрешить пользователям скачивать файлы из EDGE в контейнере Application Guard и сохранять их в файловой системе узла</span><span class="sxs-lookup"><span data-stu-id="d0fc3-802">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="d0fc3-803">Битлоккералловстандардусеренкриптион</span><span class="sxs-lookup"><span data-stu-id="d0fc3-803">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="d0fc3-804">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-804">Boolean</span></span>|<span data-ttu-id="d0fc3-805">Позволяет администратору разрешить обычным пользователям включать енкрпитион во время присоединения к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-805">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="d0fc3-806">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="d0fc3-806">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="d0fc3-807">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-807">Boolean</span></span>|<span data-ttu-id="d0fc3-808">Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-808">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="d0fc3-809">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="d0fc3-809">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="d0fc3-810">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-810">Boolean</span></span>|<span data-ttu-id="d0fc3-811">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-811">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="d0fc3-812">Эта политика действительна только для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-812">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="d0fc3-813">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="d0fc3-813">bitLockerEncryptDevice</span></span>|<span data-ttu-id="d0fc3-814">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0fc3-814">Boolean</span></span>|<span data-ttu-id="d0fc3-815">Позволяет администратору требовать включения шифрования с помощью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-815">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="d0fc3-816">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d0fc3-816">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="d0fc3-817">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d0fc3-817">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="d0fc3-818">Политика системного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-818">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="d0fc3-819">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d0fc3-819">bitLockerFixedDrivePolicy</span></span>|<span data-ttu-id="d0fc3-820">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md);</span><span class="sxs-lookup"><span data-stu-id="d0fc3-820">[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)</span></span>|<span data-ttu-id="d0fc3-821">Политика фиксированного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-821">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="d0fc3-822">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d0fc3-822">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="d0fc3-823">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d0fc3-823">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="d0fc3-824">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-824">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="d0fc3-825">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0fc3-825">Response</span></span>
<span data-ttu-id="d0fc3-826">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-826">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0fc3-827">Пример</span><span class="sxs-lookup"><span data-stu-id="d0fc3-827">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0fc3-828">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0fc3-828">Request</span></span>
<span data-ttu-id="d0fc3-829">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-829">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d0fc3-830">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0fc3-830">Response</span></span>
<span data-ttu-id="d0fc3-p206">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0fc3-p206">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





