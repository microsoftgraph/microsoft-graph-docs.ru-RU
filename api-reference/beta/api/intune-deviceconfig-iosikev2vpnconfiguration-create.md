---
title: Создание iosikEv2VpnConfiguration
description: Создание нового объекта iosikEv2VpnConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 297f47534430511524e8b5c6c6bb0f1e0e77b2b2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42750483"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="07509-103">Создание iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="07509-103">Create iosikEv2VpnConfiguration</span></span>

> <span data-ttu-id="07509-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07509-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07509-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07509-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07509-106">Создание нового объекта [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="07509-106">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07509-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="07509-107">Prerequisites</span></span>
<span data-ttu-id="07509-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07509-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07509-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07509-110">Permission type</span></span>|<span data-ttu-id="07509-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="07509-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07509-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07509-112">Delegated (work or school account)</span></span>|<span data-ttu-id="07509-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07509-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="07509-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07509-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07509-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07509-115">Not supported.</span></span>|
|<span data-ttu-id="07509-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="07509-116">Application</span></span>|<span data-ttu-id="07509-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07509-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07509-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07509-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="07509-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="07509-119">Request headers</span></span>
|<span data-ttu-id="07509-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07509-120">Header</span></span>|<span data-ttu-id="07509-121">Значение</span><span class="sxs-lookup"><span data-stu-id="07509-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07509-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="07509-122">Authorization</span></span>|<span data-ttu-id="07509-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07509-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07509-124">Accept</span><span class="sxs-lookup"><span data-stu-id="07509-124">Accept</span></span>|<span data-ttu-id="07509-125">application/json</span><span class="sxs-lookup"><span data-stu-id="07509-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07509-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07509-126">Request body</span></span>
<span data-ttu-id="07509-127">В тексте запроса добавьте представление объекта iosikEv2VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07509-127">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="07509-128">В следующей таблице приведены свойства, необходимые при создании iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="07509-128">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="07509-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="07509-129">Property</span></span>|<span data-ttu-id="07509-130">Тип</span><span class="sxs-lookup"><span data-stu-id="07509-130">Type</span></span>|<span data-ttu-id="07509-131">Описание</span><span class="sxs-lookup"><span data-stu-id="07509-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07509-132">id</span><span class="sxs-lookup"><span data-stu-id="07509-132">id</span></span>|<span data-ttu-id="07509-133">String</span><span class="sxs-lookup"><span data-stu-id="07509-133">String</span></span>|<span data-ttu-id="07509-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="07509-134">Key of the entity.</span></span> <span data-ttu-id="07509-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07509-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07509-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07509-136">lastModifiedDateTime</span></span>|<span data-ttu-id="07509-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07509-137">DateTimeOffset</span></span>|<span data-ttu-id="07509-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="07509-138">DateTime the object was last modified.</span></span> <span data-ttu-id="07509-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07509-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07509-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="07509-140">roleScopeTagIds</span></span>|<span data-ttu-id="07509-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="07509-141">String collection</span></span>|<span data-ttu-id="07509-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="07509-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="07509-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07509-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07509-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="07509-144">supportsScopeTags</span></span>|<span data-ttu-id="07509-145">Логический</span><span class="sxs-lookup"><span data-stu-id="07509-145">Boolean</span></span>|<span data-ttu-id="07509-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="07509-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="07509-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="07509-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="07509-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="07509-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="07509-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="07509-149">This property is read-only.</span></span> <span data-ttu-id="07509-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07509-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07509-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="07509-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="07509-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="07509-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="07509-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="07509-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="07509-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07509-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07509-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="07509-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="07509-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="07509-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="07509-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="07509-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="07509-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07509-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07509-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="07509-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="07509-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="07509-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="07509-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="07509-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="07509-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07509-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07509-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07509-163">createdDateTime</span></span>|<span data-ttu-id="07509-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07509-164">DateTimeOffset</span></span>|<span data-ttu-id="07509-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="07509-165">DateTime the object was created.</span></span> <span data-ttu-id="07509-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07509-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07509-167">description</span><span class="sxs-lookup"><span data-stu-id="07509-167">description</span></span>|<span data-ttu-id="07509-168">String</span><span class="sxs-lookup"><span data-stu-id="07509-168">String</span></span>|<span data-ttu-id="07509-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="07509-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="07509-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07509-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07509-171">displayName</span><span class="sxs-lookup"><span data-stu-id="07509-171">displayName</span></span>|<span data-ttu-id="07509-172">Строка</span><span class="sxs-lookup"><span data-stu-id="07509-172">String</span></span>|<span data-ttu-id="07509-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="07509-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="07509-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07509-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07509-175">version</span><span class="sxs-lookup"><span data-stu-id="07509-175">version</span></span>|<span data-ttu-id="07509-176">Int32</span><span class="sxs-lookup"><span data-stu-id="07509-176">Int32</span></span>|<span data-ttu-id="07509-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="07509-177">Version of the device configuration.</span></span> <span data-ttu-id="07509-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07509-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07509-179">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="07509-179">connectionName</span></span>|<span data-ttu-id="07509-180">String</span><span class="sxs-lookup"><span data-stu-id="07509-180">String</span></span>|<span data-ttu-id="07509-181">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="07509-181">Connection name displayed to the user.</span></span> <span data-ttu-id="07509-182">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07509-182">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="07509-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="07509-183">connectionType</span></span>|[<span data-ttu-id="07509-184">апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="07509-184">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="07509-185">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="07509-185">Connection type.</span></span> <span data-ttu-id="07509-186">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07509-186">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="07509-187">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span><span class="sxs-lookup"><span data-stu-id="07509-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span></span>|
|<span data-ttu-id="07509-188">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="07509-188">loginGroupOrDomain</span></span>|<span data-ttu-id="07509-189">String</span><span class="sxs-lookup"><span data-stu-id="07509-189">String</span></span>|<span data-ttu-id="07509-190">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="07509-190">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="07509-191">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07509-191">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="07509-192">role</span><span class="sxs-lookup"><span data-stu-id="07509-192">role</span></span>|<span data-ttu-id="07509-193">String</span><span class="sxs-lookup"><span data-stu-id="07509-193">String</span></span>|<span data-ttu-id="07509-194">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="07509-194">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="07509-195">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07509-195">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="07509-196">область</span><span class="sxs-lookup"><span data-stu-id="07509-196">realm</span></span>|<span data-ttu-id="07509-197">String</span><span class="sxs-lookup"><span data-stu-id="07509-197">String</span></span>|<span data-ttu-id="07509-198">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="07509-198">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="07509-199">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07509-199">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="07509-200">сервер</span><span class="sxs-lookup"><span data-stu-id="07509-200">server</span></span>|[<span data-ttu-id="07509-201">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="07509-201">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="07509-202">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="07509-202">VPN Server on the network.</span></span> <span data-ttu-id="07509-203">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="07509-203">Make sure end users can access this network location.</span></span> <span data-ttu-id="07509-204">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07509-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="07509-205">идентификатор</span><span class="sxs-lookup"><span data-stu-id="07509-205">identifier</span></span>|<span data-ttu-id="07509-206">String</span><span class="sxs-lookup"><span data-stu-id="07509-206">String</span></span>|<span data-ttu-id="07509-207">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="07509-207">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="07509-208">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07509-208">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="07509-209">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="07509-209">customData</span></span>|<span data-ttu-id="07509-210">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="07509-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="07509-211">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="07509-211">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="07509-212">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="07509-212">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="07509-213">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="07509-213">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="07509-214">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="07509-214">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="07509-215">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07509-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="07509-216">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="07509-216">customKeyValueData</span></span>|<span data-ttu-id="07509-217">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="07509-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="07509-218">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="07509-218">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="07509-219">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="07509-219">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="07509-220">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="07509-220">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="07509-221">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="07509-221">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="07509-222">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07509-222">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="07509-223">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="07509-223">enableSplitTunneling</span></span>|<span data-ttu-id="07509-224">Логический</span><span class="sxs-lookup"><span data-stu-id="07509-224">Boolean</span></span>|<span data-ttu-id="07509-225">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="07509-225">Send all network traffic through VPN.</span></span> <span data-ttu-id="07509-226">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07509-226">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="07509-227">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="07509-227">authenticationMethod</span></span>|[<span data-ttu-id="07509-228">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="07509-228">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="07509-229">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="07509-229">Authentication method for this VPN connection.</span></span> <span data-ttu-id="07509-230">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07509-230">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="07509-231">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="07509-231">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="07509-232">енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="07509-232">enablePerApp</span></span>|<span data-ttu-id="07509-233">Логический</span><span class="sxs-lookup"><span data-stu-id="07509-233">Boolean</span></span>|<span data-ttu-id="07509-234">Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="07509-234">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="07509-235">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07509-235">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="07509-236">сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="07509-236">safariDomains</span></span>|<span data-ttu-id="07509-237">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="07509-237">String collection</span></span>|<span data-ttu-id="07509-238">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="07509-238">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="07509-239">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="07509-239">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="07509-240">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07509-240">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="07509-241">ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="07509-241">onDemandRules</span></span>|<span data-ttu-id="07509-242">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="07509-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="07509-243">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="07509-243">On-Demand Rules.</span></span> <span data-ttu-id="07509-244">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="07509-244">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="07509-245">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07509-245">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="07509-246">проксисервер</span><span class="sxs-lookup"><span data-stu-id="07509-246">proxyServer</span></span>|[<span data-ttu-id="07509-247">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="07509-247">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="07509-248">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="07509-248">Proxy Server.</span></span> <span data-ttu-id="07509-249">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07509-249">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="07509-250">оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="07509-250">optInToDeviceIdSharing</span></span>|<span data-ttu-id="07509-251">Логический</span><span class="sxs-lookup"><span data-stu-id="07509-251">Boolean</span></span>|<span data-ttu-id="07509-252">Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="07509-252">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="07509-253">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07509-253">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="07509-254">providerType</span><span class="sxs-lookup"><span data-stu-id="07509-254">providerType</span></span>|[<span data-ttu-id="07509-255">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="07509-255">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="07509-256">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="07509-256">Provider type for per-app VPN.</span></span> <span data-ttu-id="07509-257">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07509-257">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="07509-258">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="07509-258">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="07509-259">userDomain</span><span class="sxs-lookup"><span data-stu-id="07509-259">userDomain</span></span>|<span data-ttu-id="07509-260">String</span><span class="sxs-lookup"><span data-stu-id="07509-260">String</span></span>|<span data-ttu-id="07509-261">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="07509-261">Zscaler only.</span></span> <span data-ttu-id="07509-262">Введите статический домен для предварительного заполнения поля Login в приложении Зскалер.</span><span class="sxs-lookup"><span data-stu-id="07509-262">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="07509-263">Если оставить это поле пустым, вместо этого будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="07509-263">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="07509-264">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07509-264">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="07509-265">стриктенфорцемент</span><span class="sxs-lookup"><span data-stu-id="07509-265">strictEnforcement</span></span>|<span data-ttu-id="07509-266">Логический</span><span class="sxs-lookup"><span data-stu-id="07509-266">Boolean</span></span>|<span data-ttu-id="07509-267">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="07509-267">Zscaler only.</span></span> <span data-ttu-id="07509-268">Блокирует сетевой трафик до тех пор, пока пользователь не войдет в приложение Зскалер.</span><span class="sxs-lookup"><span data-stu-id="07509-268">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="07509-269">"True" означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="07509-269">"True" means traffic is blocked.</span></span> <span data-ttu-id="07509-270">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07509-270">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="07509-271">клауднаме</span><span class="sxs-lookup"><span data-stu-id="07509-271">cloudName</span></span>|<span data-ttu-id="07509-272">String</span><span class="sxs-lookup"><span data-stu-id="07509-272">String</span></span>|<span data-ttu-id="07509-273">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="07509-273">Zscaler only.</span></span> <span data-ttu-id="07509-274">Облако зскалер, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="07509-274">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="07509-275">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07509-275">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="07509-276">excludeList</span><span class="sxs-lookup"><span data-stu-id="07509-276">excludeList</span></span>|<span data-ttu-id="07509-277">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="07509-277">String collection</span></span>|<span data-ttu-id="07509-278">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="07509-278">Zscaler only.</span></span> <span data-ttu-id="07509-279">Список сетевых адресов, которые не отправляются через облако Зскалер.</span><span class="sxs-lookup"><span data-stu-id="07509-279">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="07509-280">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07509-280">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="07509-281">чилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="07509-281">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="07509-282">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="07509-282">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="07509-283">Дочерние параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="07509-283">Child Security Association Parameters</span></span>|
|<span data-ttu-id="07509-284">клиентаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="07509-284">clientAuthenticationType</span></span>|[<span data-ttu-id="07509-285">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="07509-285">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="07509-286">Тип проверки подлинности клиента, который будет использоваться VPN-клиентом.</span><span class="sxs-lookup"><span data-stu-id="07509-286">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="07509-287">Возможные значения: `userAuthentication`, `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="07509-287">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="07509-288">деадпирдетектионрате</span><span class="sxs-lookup"><span data-stu-id="07509-288">deadPeerDetectionRate</span></span>|[<span data-ttu-id="07509-289">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="07509-289">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="07509-290">Определите, как часто следует проверять, активен ли одноранговый сеанс.</span><span class="sxs-lookup"><span data-stu-id="07509-290">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="07509-291">.</span><span class="sxs-lookup"><span data-stu-id="07509-291">.</span></span> <span data-ttu-id="07509-292">Возможные значения: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="07509-292">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="07509-293">дисаблемобилитяндмултихоминг</span><span class="sxs-lookup"><span data-stu-id="07509-293">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="07509-294">Логический</span><span class="sxs-lookup"><span data-stu-id="07509-294">Boolean</span></span>|<span data-ttu-id="07509-295">Отключение МОБИКЕ</span><span class="sxs-lookup"><span data-stu-id="07509-295">Disable MOBIKE</span></span>|
|<span data-ttu-id="07509-296">дисаблередирект</span><span class="sxs-lookup"><span data-stu-id="07509-296">disableRedirect</span></span>|<span data-ttu-id="07509-297">Логический</span><span class="sxs-lookup"><span data-stu-id="07509-297">Boolean</span></span>|<span data-ttu-id="07509-298">Отключение перенаправления</span><span class="sxs-lookup"><span data-stu-id="07509-298">Disable Redirect</span></span>|
|<span data-ttu-id="07509-299">енаблецертификатеревокатиончекк</span><span class="sxs-lookup"><span data-stu-id="07509-299">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="07509-300">Логический</span><span class="sxs-lookup"><span data-stu-id="07509-300">Boolean</span></span>|<span data-ttu-id="07509-301">Включает проверку отзывов и действий. время ожидания отклика сервера не приведет к сбою</span><span class="sxs-lookup"><span data-stu-id="07509-301">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="07509-302">енаблиап</span><span class="sxs-lookup"><span data-stu-id="07509-302">enableEAP</span></span>|<span data-ttu-id="07509-303">Логический</span><span class="sxs-lookup"><span data-stu-id="07509-303">Boolean</span></span>|<span data-ttu-id="07509-304">Включает проверку подлинности только EAP</span><span class="sxs-lookup"><span data-stu-id="07509-304">Enables EAP only authentication</span></span>|
|<span data-ttu-id="07509-305">енаблеперфектфорвардсекреци</span><span class="sxs-lookup"><span data-stu-id="07509-305">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="07509-306">Логический</span><span class="sxs-lookup"><span data-stu-id="07509-306">Boolean</span></span>|<span data-ttu-id="07509-307">Включить безопасную пересылку (PFS).</span><span class="sxs-lookup"><span data-stu-id="07509-307">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="07509-308">енаблеусеинтерналсубнетаттрибутес</span><span class="sxs-lookup"><span data-stu-id="07509-308">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="07509-309">Логический</span><span class="sxs-lookup"><span data-stu-id="07509-309">Boolean</span></span>|<span data-ttu-id="07509-310">Включите использование атрибутов внутренней подсети.</span><span class="sxs-lookup"><span data-stu-id="07509-310">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="07509-311">локалидентифиер</span><span class="sxs-lookup"><span data-stu-id="07509-311">localIdentifier</span></span>|[<span data-ttu-id="07509-312">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="07509-312">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="07509-313">Метод идентификации клиента, который пытается подключиться через VPN.</span><span class="sxs-lookup"><span data-stu-id="07509-313">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="07509-314">.</span><span class="sxs-lookup"><span data-stu-id="07509-314">.</span></span> <span data-ttu-id="07509-315">Возможные значения: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="07509-315">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="07509-316">ремотеидентифиер</span><span class="sxs-lookup"><span data-stu-id="07509-316">remoteIdentifier</span></span>|<span data-ttu-id="07509-317">String</span><span class="sxs-lookup"><span data-stu-id="07509-317">String</span></span>|<span data-ttu-id="07509-318">Адрес сервера IKEv2.</span><span class="sxs-lookup"><span data-stu-id="07509-318">Address of the IKEv2 server.</span></span> <span data-ttu-id="07509-319">Должно быть полным доменным именем, Усерфкдн, сетевым адресом или ASN1DN</span><span class="sxs-lookup"><span data-stu-id="07509-319">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="07509-320">секуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="07509-320">securityAssociationParameters</span></span>|[<span data-ttu-id="07509-321">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="07509-321">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="07509-322">Параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="07509-322">Security Association Parameters</span></span>|
|<span data-ttu-id="07509-323">серверцертификатекоммоннаме</span><span class="sxs-lookup"><span data-stu-id="07509-323">serverCertificateCommonName</span></span>|<span data-ttu-id="07509-324">String</span><span class="sxs-lookup"><span data-stu-id="07509-324">String</span></span>|<span data-ttu-id="07509-325">Общее имя сертификата сервера IKEv2, используемого при проверке подлинности сервера</span><span class="sxs-lookup"><span data-stu-id="07509-325">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="07509-326">серверцертификатеиссуеркоммоннаме</span><span class="sxs-lookup"><span data-stu-id="07509-326">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="07509-327">String</span><span class="sxs-lookup"><span data-stu-id="07509-327">String</span></span>|<span data-ttu-id="07509-328">Общее имя поставщика сертификата сервера IKEv2, используемого при проверке подлинности</span><span class="sxs-lookup"><span data-stu-id="07509-328">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="07509-329">серверцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="07509-329">serverCertificateType</span></span>|[<span data-ttu-id="07509-330">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="07509-330">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="07509-331">Тип сертификата, который VPN-сервер будет предоставлять VPN-клиенту для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="07509-331">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="07509-332">Возможные значения: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="07509-332">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="07509-333">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="07509-333">sharedSecret</span></span>|<span data-ttu-id="07509-334">String</span><span class="sxs-lookup"><span data-stu-id="07509-334">String</span></span>|<span data-ttu-id="07509-335">Используется, когда выбрана общая секретная проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="07509-335">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="07509-336">тлсмаксимумверсион</span><span class="sxs-lookup"><span data-stu-id="07509-336">tlsMaximumVersion</span></span>|<span data-ttu-id="07509-337">String</span><span class="sxs-lookup"><span data-stu-id="07509-337">String</span></span>|<span data-ttu-id="07509-338">Максимальная версия TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="07509-338">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="07509-339">тлсминимумверсион</span><span class="sxs-lookup"><span data-stu-id="07509-339">tlsMinimumVersion</span></span>|<span data-ttu-id="07509-340">String</span><span class="sxs-lookup"><span data-stu-id="07509-340">String</span></span>|<span data-ttu-id="07509-341">Минимальная версия протокола TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="07509-341">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="07509-342">алловдефаултсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="07509-342">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="07509-343">Логический</span><span class="sxs-lookup"><span data-stu-id="07509-343">Boolean</span></span>|<span data-ttu-id="07509-344">Разрешает использование параметров сопоставления безопасности путем установки всех параметров для устройства по умолчанию, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="07509-344">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="07509-345">алловдефаултчилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="07509-345">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="07509-346">Логический</span><span class="sxs-lookup"><span data-stu-id="07509-346">Boolean</span></span>|<span data-ttu-id="07509-347">Разрешает использование параметров дочернего сопоставления безопасности, устанавливая все параметры по умолчанию устройства, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="07509-347">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="07509-348">алвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="07509-348">alwaysOnConfiguration</span></span>|[<span data-ttu-id="07509-349">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="07509-349">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="07509-350">Конфигурация AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="07509-350">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="07509-351">енаблеалвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="07509-351">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="07509-352">Логический</span><span class="sxs-lookup"><span data-stu-id="07509-352">Boolean</span></span>|<span data-ttu-id="07509-353">Определяет, включена ли функция "всегда включено" VPN</span><span class="sxs-lookup"><span data-stu-id="07509-353">Determines if Always on VPN is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="07509-354">Отклик</span><span class="sxs-lookup"><span data-stu-id="07509-354">Response</span></span>
<span data-ttu-id="07509-355">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="07509-355">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07509-356">Пример</span><span class="sxs-lookup"><span data-stu-id="07509-356">Example</span></span>

### <a name="request"></a><span data-ttu-id="07509-357">Запрос</span><span class="sxs-lookup"><span data-stu-id="07509-357">Request</span></span>
<span data-ttu-id="07509-358">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07509-358">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="07509-359">Отклик</span><span class="sxs-lookup"><span data-stu-id="07509-359">Response</span></span>
<span data-ttu-id="07509-p139">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07509-p139">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




