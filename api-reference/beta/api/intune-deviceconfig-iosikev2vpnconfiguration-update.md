---
title: Обновление iosikEv2VpnConfiguration
description: Обновление свойств объекта iosikEv2VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bc54a9306df5c8d03bbd4fd9db969a1380cba4da
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41635897"
---
# <a name="update-iosikev2vpnconfiguration"></a><span data-ttu-id="616ad-103">Обновление iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="616ad-103">Update iosikEv2VpnConfiguration</span></span>

> <span data-ttu-id="616ad-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="616ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="616ad-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="616ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="616ad-106">Обновление свойств объекта [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="616ad-106">Update the properties of a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="616ad-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="616ad-107">Prerequisites</span></span>
<span data-ttu-id="616ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="616ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="616ad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="616ad-110">Permission type</span></span>|<span data-ttu-id="616ad-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="616ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="616ad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="616ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="616ad-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="616ad-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="616ad-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="616ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="616ad-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="616ad-115">Not supported.</span></span>|
|<span data-ttu-id="616ad-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="616ad-116">Application</span></span>|<span data-ttu-id="616ad-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="616ad-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="616ad-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="616ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="616ad-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="616ad-119">Request headers</span></span>
|<span data-ttu-id="616ad-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="616ad-120">Header</span></span>|<span data-ttu-id="616ad-121">Значение</span><span class="sxs-lookup"><span data-stu-id="616ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="616ad-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="616ad-122">Authorization</span></span>|<span data-ttu-id="616ad-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="616ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="616ad-124">Accept</span><span class="sxs-lookup"><span data-stu-id="616ad-124">Accept</span></span>|<span data-ttu-id="616ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="616ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="616ad-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="616ad-126">Request body</span></span>
<span data-ttu-id="616ad-127">В тексте запроса добавьте представление объекта [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="616ad-127">In the request body, supply a JSON representation for the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

<span data-ttu-id="616ad-128">В следующей таблице приведены свойства, необходимые при создании [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="616ad-128">The following table shows the properties that are required when you create the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span></span>

|<span data-ttu-id="616ad-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="616ad-129">Property</span></span>|<span data-ttu-id="616ad-130">Тип</span><span class="sxs-lookup"><span data-stu-id="616ad-130">Type</span></span>|<span data-ttu-id="616ad-131">Описание</span><span class="sxs-lookup"><span data-stu-id="616ad-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="616ad-132">id</span><span class="sxs-lookup"><span data-stu-id="616ad-132">id</span></span>|<span data-ttu-id="616ad-133">String</span><span class="sxs-lookup"><span data-stu-id="616ad-133">String</span></span>|<span data-ttu-id="616ad-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="616ad-134">Key of the entity.</span></span> <span data-ttu-id="616ad-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="616ad-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="616ad-136">lastModifiedDateTime</span></span>|<span data-ttu-id="616ad-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="616ad-137">DateTimeOffset</span></span>|<span data-ttu-id="616ad-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="616ad-138">DateTime the object was last modified.</span></span> <span data-ttu-id="616ad-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="616ad-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="616ad-140">roleScopeTagIds</span></span>|<span data-ttu-id="616ad-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="616ad-141">String collection</span></span>|<span data-ttu-id="616ad-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="616ad-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="616ad-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="616ad-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="616ad-144">supportsScopeTags</span></span>|<span data-ttu-id="616ad-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="616ad-145">Boolean</span></span>|<span data-ttu-id="616ad-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="616ad-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="616ad-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="616ad-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="616ad-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="616ad-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="616ad-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="616ad-149">This property is read-only.</span></span> <span data-ttu-id="616ad-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="616ad-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="616ad-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="616ad-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="616ad-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="616ad-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="616ad-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="616ad-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="616ad-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="616ad-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="616ad-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="616ad-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="616ad-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="616ad-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="616ad-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="616ad-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="616ad-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="616ad-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="616ad-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="616ad-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="616ad-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="616ad-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="616ad-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="616ad-163">createdDateTime</span></span>|<span data-ttu-id="616ad-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="616ad-164">DateTimeOffset</span></span>|<span data-ttu-id="616ad-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="616ad-165">DateTime the object was created.</span></span> <span data-ttu-id="616ad-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="616ad-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-167">description</span><span class="sxs-lookup"><span data-stu-id="616ad-167">description</span></span>|<span data-ttu-id="616ad-168">String</span><span class="sxs-lookup"><span data-stu-id="616ad-168">String</span></span>|<span data-ttu-id="616ad-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="616ad-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="616ad-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="616ad-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-171">displayName</span><span class="sxs-lookup"><span data-stu-id="616ad-171">displayName</span></span>|<span data-ttu-id="616ad-172">Строка</span><span class="sxs-lookup"><span data-stu-id="616ad-172">String</span></span>|<span data-ttu-id="616ad-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="616ad-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="616ad-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="616ad-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-175">version</span><span class="sxs-lookup"><span data-stu-id="616ad-175">version</span></span>|<span data-ttu-id="616ad-176">Int32</span><span class="sxs-lookup"><span data-stu-id="616ad-176">Int32</span></span>|<span data-ttu-id="616ad-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="616ad-177">Version of the device configuration.</span></span> <span data-ttu-id="616ad-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="616ad-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-179">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="616ad-179">connectionName</span></span>|<span data-ttu-id="616ad-180">Строка</span><span class="sxs-lookup"><span data-stu-id="616ad-180">String</span></span>|<span data-ttu-id="616ad-181">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="616ad-181">Connection name displayed to the user.</span></span> <span data-ttu-id="616ad-182">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-182">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="616ad-183">connectionType</span></span>|[<span data-ttu-id="616ad-184">апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="616ad-184">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="616ad-185">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="616ad-185">Connection type.</span></span> <span data-ttu-id="616ad-186">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="616ad-186">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="616ad-187">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span><span class="sxs-lookup"><span data-stu-id="616ad-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span></span>|
|<span data-ttu-id="616ad-188">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="616ad-188">loginGroupOrDomain</span></span>|<span data-ttu-id="616ad-189">Строка</span><span class="sxs-lookup"><span data-stu-id="616ad-189">String</span></span>|<span data-ttu-id="616ad-190">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="616ad-190">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="616ad-191">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-191">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-192">role</span><span class="sxs-lookup"><span data-stu-id="616ad-192">role</span></span>|<span data-ttu-id="616ad-193">Строка</span><span class="sxs-lookup"><span data-stu-id="616ad-193">String</span></span>|<span data-ttu-id="616ad-194">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="616ad-194">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="616ad-195">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-195">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-196">область</span><span class="sxs-lookup"><span data-stu-id="616ad-196">realm</span></span>|<span data-ttu-id="616ad-197">Строка</span><span class="sxs-lookup"><span data-stu-id="616ad-197">String</span></span>|<span data-ttu-id="616ad-198">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="616ad-198">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="616ad-199">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-199">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-200">сервер</span><span class="sxs-lookup"><span data-stu-id="616ad-200">server</span></span>|[<span data-ttu-id="616ad-201">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="616ad-201">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="616ad-202">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="616ad-202">VPN Server on the network.</span></span> <span data-ttu-id="616ad-203">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="616ad-203">Make sure end users can access this network location.</span></span> <span data-ttu-id="616ad-204">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-205">идентификатор</span><span class="sxs-lookup"><span data-stu-id="616ad-205">identifier</span></span>|<span data-ttu-id="616ad-206">Строка</span><span class="sxs-lookup"><span data-stu-id="616ad-206">String</span></span>|<span data-ttu-id="616ad-207">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="616ad-207">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="616ad-208">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-208">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-209">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="616ad-209">customData</span></span>|<span data-ttu-id="616ad-210">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="616ad-211">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="616ad-211">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="616ad-212">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="616ad-212">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="616ad-213">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="616ad-213">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="616ad-214">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="616ad-214">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="616ad-215">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-216">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="616ad-216">customKeyValueData</span></span>|<span data-ttu-id="616ad-217">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="616ad-218">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="616ad-218">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="616ad-219">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="616ad-219">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="616ad-220">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="616ad-220">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="616ad-221">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="616ad-221">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="616ad-222">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-222">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-223">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="616ad-223">enableSplitTunneling</span></span>|<span data-ttu-id="616ad-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="616ad-224">Boolean</span></span>|<span data-ttu-id="616ad-225">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="616ad-225">Send all network traffic through VPN.</span></span> <span data-ttu-id="616ad-226">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-226">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-227">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="616ad-227">authenticationMethod</span></span>|[<span data-ttu-id="616ad-228">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="616ad-228">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="616ad-229">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="616ad-229">Authentication method for this VPN connection.</span></span> <span data-ttu-id="616ad-230">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="616ad-230">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="616ad-231">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="616ad-231">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="616ad-232">енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="616ad-232">enablePerApp</span></span>|<span data-ttu-id="616ad-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="616ad-233">Boolean</span></span>|<span data-ttu-id="616ad-234">Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="616ad-234">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="616ad-235">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-235">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-236">сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="616ad-236">safariDomains</span></span>|<span data-ttu-id="616ad-237">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="616ad-237">String collection</span></span>|<span data-ttu-id="616ad-238">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="616ad-238">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="616ad-239">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="616ad-239">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="616ad-240">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-240">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-241">ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="616ad-241">onDemandRules</span></span>|<span data-ttu-id="616ad-242">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="616ad-243">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="616ad-243">On-Demand Rules.</span></span> <span data-ttu-id="616ad-244">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="616ad-244">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="616ad-245">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-245">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-246">проксисервер</span><span class="sxs-lookup"><span data-stu-id="616ad-246">proxyServer</span></span>|[<span data-ttu-id="616ad-247">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="616ad-247">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="616ad-248">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="616ad-248">Proxy Server.</span></span> <span data-ttu-id="616ad-249">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-249">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-250">оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="616ad-250">optInToDeviceIdSharing</span></span>|<span data-ttu-id="616ad-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="616ad-251">Boolean</span></span>|<span data-ttu-id="616ad-252">Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="616ad-252">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="616ad-253">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-253">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-254">providerType</span><span class="sxs-lookup"><span data-stu-id="616ad-254">providerType</span></span>|[<span data-ttu-id="616ad-255">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="616ad-255">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="616ad-256">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="616ad-256">Provider type for per-app VPN.</span></span> <span data-ttu-id="616ad-257">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="616ad-257">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="616ad-258">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="616ad-258">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="616ad-259">userDomain</span><span class="sxs-lookup"><span data-stu-id="616ad-259">userDomain</span></span>|<span data-ttu-id="616ad-260">Строка</span><span class="sxs-lookup"><span data-stu-id="616ad-260">String</span></span>|<span data-ttu-id="616ad-261">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="616ad-261">Zscaler only.</span></span> <span data-ttu-id="616ad-262">Введите статический домен для предварительного заполнения поля Login в приложении Зскалер.</span><span class="sxs-lookup"><span data-stu-id="616ad-262">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="616ad-263">Если оставить это поле пустым, вместо этого будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="616ad-263">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="616ad-264">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-264">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-265">стриктенфорцемент</span><span class="sxs-lookup"><span data-stu-id="616ad-265">strictEnforcement</span></span>|<span data-ttu-id="616ad-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="616ad-266">Boolean</span></span>|<span data-ttu-id="616ad-267">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="616ad-267">Zscaler only.</span></span> <span data-ttu-id="616ad-268">Блокирует сетевой трафик до тех пор, пока пользователь не войдет в приложение Зскалер.</span><span class="sxs-lookup"><span data-stu-id="616ad-268">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="616ad-269">"True" означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="616ad-269">"True" means traffic is blocked.</span></span> <span data-ttu-id="616ad-270">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-270">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-271">клауднаме</span><span class="sxs-lookup"><span data-stu-id="616ad-271">cloudName</span></span>|<span data-ttu-id="616ad-272">Строка</span><span class="sxs-lookup"><span data-stu-id="616ad-272">String</span></span>|<span data-ttu-id="616ad-273">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="616ad-273">Zscaler only.</span></span> <span data-ttu-id="616ad-274">Облако зскалер, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="616ad-274">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="616ad-275">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-275">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-276">excludeList</span><span class="sxs-lookup"><span data-stu-id="616ad-276">excludeList</span></span>|<span data-ttu-id="616ad-277">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="616ad-277">String collection</span></span>|<span data-ttu-id="616ad-278">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="616ad-278">Zscaler only.</span></span> <span data-ttu-id="616ad-279">Список сетевых адресов, которые не отправляются через облако Зскалер.</span><span class="sxs-lookup"><span data-stu-id="616ad-279">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="616ad-280">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="616ad-280">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="616ad-281">чилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="616ad-281">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="616ad-282">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="616ad-282">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="616ad-283">Дочерние параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="616ad-283">Child Security Association Parameters</span></span>|
|<span data-ttu-id="616ad-284">клиентаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="616ad-284">clientAuthenticationType</span></span>|[<span data-ttu-id="616ad-285">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="616ad-285">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="616ad-286">Тип проверки подлинности клиента, который будет использоваться VPN-клиентом.</span><span class="sxs-lookup"><span data-stu-id="616ad-286">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="616ad-287">Возможные значения: `userAuthentication`, `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="616ad-287">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="616ad-288">деадпирдетектионрате</span><span class="sxs-lookup"><span data-stu-id="616ad-288">deadPeerDetectionRate</span></span>|[<span data-ttu-id="616ad-289">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="616ad-289">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="616ad-290">Определите, как часто следует проверять, активен ли одноранговый сеанс.</span><span class="sxs-lookup"><span data-stu-id="616ad-290">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="616ad-291">.</span><span class="sxs-lookup"><span data-stu-id="616ad-291">.</span></span> <span data-ttu-id="616ad-292">Возможные значения: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="616ad-292">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="616ad-293">дисаблемобилитяндмултихоминг</span><span class="sxs-lookup"><span data-stu-id="616ad-293">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="616ad-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="616ad-294">Boolean</span></span>|<span data-ttu-id="616ad-295">Отключение МОБИКЕ</span><span class="sxs-lookup"><span data-stu-id="616ad-295">Disable MOBIKE</span></span>|
|<span data-ttu-id="616ad-296">дисаблередирект</span><span class="sxs-lookup"><span data-stu-id="616ad-296">disableRedirect</span></span>|<span data-ttu-id="616ad-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="616ad-297">Boolean</span></span>|<span data-ttu-id="616ad-298">Отключение перенаправления</span><span class="sxs-lookup"><span data-stu-id="616ad-298">Disable Redirect</span></span>|
|<span data-ttu-id="616ad-299">енаблецертификатеревокатиончекк</span><span class="sxs-lookup"><span data-stu-id="616ad-299">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="616ad-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="616ad-300">Boolean</span></span>|<span data-ttu-id="616ad-301">Включает проверку отзывов и действий. время ожидания отклика сервера не приведет к сбою</span><span class="sxs-lookup"><span data-stu-id="616ad-301">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="616ad-302">енаблиап</span><span class="sxs-lookup"><span data-stu-id="616ad-302">enableEAP</span></span>|<span data-ttu-id="616ad-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="616ad-303">Boolean</span></span>|<span data-ttu-id="616ad-304">Включает проверку подлинности только EAP</span><span class="sxs-lookup"><span data-stu-id="616ad-304">Enables EAP only authentication</span></span>|
|<span data-ttu-id="616ad-305">енаблеперфектфорвардсекреци</span><span class="sxs-lookup"><span data-stu-id="616ad-305">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="616ad-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="616ad-306">Boolean</span></span>|<span data-ttu-id="616ad-307">Включить безопасную пересылку (PFS).</span><span class="sxs-lookup"><span data-stu-id="616ad-307">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="616ad-308">енаблеусеинтерналсубнетаттрибутес</span><span class="sxs-lookup"><span data-stu-id="616ad-308">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="616ad-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="616ad-309">Boolean</span></span>|<span data-ttu-id="616ad-310">Включите использование атрибутов внутренней подсети.</span><span class="sxs-lookup"><span data-stu-id="616ad-310">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="616ad-311">локалидентифиер</span><span class="sxs-lookup"><span data-stu-id="616ad-311">localIdentifier</span></span>|[<span data-ttu-id="616ad-312">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="616ad-312">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="616ad-313">Метод идентификации клиента, который пытается подключиться через VPN.</span><span class="sxs-lookup"><span data-stu-id="616ad-313">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="616ad-314">.</span><span class="sxs-lookup"><span data-stu-id="616ad-314">.</span></span> <span data-ttu-id="616ad-315">Возможные значения: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="616ad-315">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="616ad-316">ремотеидентифиер</span><span class="sxs-lookup"><span data-stu-id="616ad-316">remoteIdentifier</span></span>|<span data-ttu-id="616ad-317">Строка</span><span class="sxs-lookup"><span data-stu-id="616ad-317">String</span></span>|<span data-ttu-id="616ad-318">Адрес сервера IKEv2.</span><span class="sxs-lookup"><span data-stu-id="616ad-318">Address of the IKEv2 server.</span></span> <span data-ttu-id="616ad-319">Должно быть полным доменным именем, Усерфкдн, сетевым адресом или ASN1DN</span><span class="sxs-lookup"><span data-stu-id="616ad-319">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="616ad-320">секуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="616ad-320">securityAssociationParameters</span></span>|[<span data-ttu-id="616ad-321">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="616ad-321">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="616ad-322">Параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="616ad-322">Security Association Parameters</span></span>|
|<span data-ttu-id="616ad-323">серверцертификатекоммоннаме</span><span class="sxs-lookup"><span data-stu-id="616ad-323">serverCertificateCommonName</span></span>|<span data-ttu-id="616ad-324">Строка</span><span class="sxs-lookup"><span data-stu-id="616ad-324">String</span></span>|<span data-ttu-id="616ad-325">Общее имя сертификата сервера IKEv2, используемого при проверке подлинности сервера</span><span class="sxs-lookup"><span data-stu-id="616ad-325">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="616ad-326">серверцертификатеиссуеркоммоннаме</span><span class="sxs-lookup"><span data-stu-id="616ad-326">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="616ad-327">Строка</span><span class="sxs-lookup"><span data-stu-id="616ad-327">String</span></span>|<span data-ttu-id="616ad-328">Общее имя поставщика сертификата сервера IKEv2, используемого при проверке подлинности</span><span class="sxs-lookup"><span data-stu-id="616ad-328">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="616ad-329">серверцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="616ad-329">serverCertificateType</span></span>|[<span data-ttu-id="616ad-330">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="616ad-330">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="616ad-331">Тип сертификата, который VPN-сервер будет предоставлять VPN-клиенту для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="616ad-331">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="616ad-332">Возможные значения: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="616ad-332">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="616ad-333">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="616ad-333">sharedSecret</span></span>|<span data-ttu-id="616ad-334">Строка</span><span class="sxs-lookup"><span data-stu-id="616ad-334">String</span></span>|<span data-ttu-id="616ad-335">Используется, когда выбрана общая секретная проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="616ad-335">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="616ad-336">тлсмаксимумверсион</span><span class="sxs-lookup"><span data-stu-id="616ad-336">tlsMaximumVersion</span></span>|<span data-ttu-id="616ad-337">Строка</span><span class="sxs-lookup"><span data-stu-id="616ad-337">String</span></span>|<span data-ttu-id="616ad-338">Максимальная версия TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="616ad-338">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="616ad-339">тлсминимумверсион</span><span class="sxs-lookup"><span data-stu-id="616ad-339">tlsMinimumVersion</span></span>|<span data-ttu-id="616ad-340">Строка</span><span class="sxs-lookup"><span data-stu-id="616ad-340">String</span></span>|<span data-ttu-id="616ad-341">Минимальная версия протокола TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="616ad-341">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="616ad-342">алловдефаултсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="616ad-342">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="616ad-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="616ad-343">Boolean</span></span>|<span data-ttu-id="616ad-344">Разрешает использование параметров сопоставления безопасности путем установки всех параметров для устройства по умолчанию, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="616ad-344">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="616ad-345">алловдефаултчилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="616ad-345">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="616ad-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="616ad-346">Boolean</span></span>|<span data-ttu-id="616ad-347">Разрешает использование параметров дочернего сопоставления безопасности, устанавливая все параметры по умолчанию устройства, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="616ad-347">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="616ad-348">алвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="616ad-348">alwaysOnConfiguration</span></span>|[<span data-ttu-id="616ad-349">апплевпналвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="616ad-349">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="616ad-350">Конфигурация AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="616ad-350">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="616ad-351">енаблеалвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="616ad-351">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="616ad-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="616ad-352">Boolean</span></span>|<span data-ttu-id="616ad-353">Определяет, включена ли функция "всегда включено" VPN</span><span class="sxs-lookup"><span data-stu-id="616ad-353">Determines if Always on VPN is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="616ad-354">Отклик</span><span class="sxs-lookup"><span data-stu-id="616ad-354">Response</span></span>
<span data-ttu-id="616ad-355">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="616ad-355">If successful, this method returns a `200 OK` response code and an updated [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="616ad-356">Пример</span><span class="sxs-lookup"><span data-stu-id="616ad-356">Example</span></span>

### <a name="request"></a><span data-ttu-id="616ad-357">Запрос</span><span class="sxs-lookup"><span data-stu-id="616ad-357">Request</span></span>
<span data-ttu-id="616ad-358">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="616ad-358">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4984

{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
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
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ],
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "clientAuthenticationType": "deviceAuthentication",
  "deadPeerDetectionRate": "none",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "empty",
  "remoteIdentifier": "Remote Identifier value",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "serverCertificateCommonName": "Server Certificate Common Name value",
  "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
  "serverCertificateType": "ecdsa256",
  "sharedSecret": "Shared Secret value",
  "tlsMaximumVersion": "Tls Maximum Version value",
  "tlsMinimumVersion": "Tls Minimum Version value",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true,
  "alwaysOnConfiguration": {
    "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration",
    "tunnelConfiguration": "cellular",
    "userToggleEnabled": true,
    "voicemailExceptionAction": "allowTrafficOutside",
    "airPrintExceptionAction": "allowTrafficOutside",
    "cellularExceptionAction": "allowTrafficOutside",
    "allowAllCaptiveNetworkPlugins": true,
    "allowedCaptiveNetworkPlugins": {
      "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
      "allowedBundleIdentifiers": [
        "Allowed Bundle Identifiers value"
      ]
    },
    "allowCaptiveWebSheet": true,
    "natKeepAliveIntervalInSeconds": 13,
    "natKeepAliveOffloadEnable": true
  },
  "enableAlwaysOnConfiguration": true
}
```

### <a name="response"></a><span data-ttu-id="616ad-359">Отклик</span><span class="sxs-lookup"><span data-stu-id="616ad-359">Response</span></span>
<span data-ttu-id="616ad-p139">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="616ad-p139">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5156

{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
  "id": "b87b0327-0327-b87b-2703-7bb827037bb8",
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
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ],
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "clientAuthenticationType": "deviceAuthentication",
  "deadPeerDetectionRate": "none",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "empty",
  "remoteIdentifier": "Remote Identifier value",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "serverCertificateCommonName": "Server Certificate Common Name value",
  "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
  "serverCertificateType": "ecdsa256",
  "sharedSecret": "Shared Secret value",
  "tlsMaximumVersion": "Tls Maximum Version value",
  "tlsMinimumVersion": "Tls Minimum Version value",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true,
  "alwaysOnConfiguration": {
    "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration",
    "tunnelConfiguration": "cellular",
    "userToggleEnabled": true,
    "voicemailExceptionAction": "allowTrafficOutside",
    "airPrintExceptionAction": "allowTrafficOutside",
    "cellularExceptionAction": "allowTrafficOutside",
    "allowAllCaptiveNetworkPlugins": true,
    "allowedCaptiveNetworkPlugins": {
      "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
      "allowedBundleIdentifiers": [
        "Allowed Bundle Identifiers value"
      ]
    },
    "allowCaptiveWebSheet": true,
    "natKeepAliveIntervalInSeconds": 13,
    "natKeepAliveOffloadEnable": true
  },
  "enableAlwaysOnConfiguration": true
}
```





