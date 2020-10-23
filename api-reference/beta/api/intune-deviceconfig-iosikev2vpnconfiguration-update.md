---
title: Обновление iosikEv2VpnConfiguration
description: Обновление свойств объекта iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0b077d66fb8951f08c62da61d98ea3b7022dc629
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733841"
---
# <a name="update-iosikev2vpnconfiguration"></a><span data-ttu-id="67a29-103">Обновление iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="67a29-103">Update iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="67a29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67a29-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67a29-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67a29-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67a29-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="67a29-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67a29-107">Обновление свойств объекта [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="67a29-107">Update the properties of a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67a29-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="67a29-108">Prerequisites</span></span>
<span data-ttu-id="67a29-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67a29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67a29-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67a29-111">Permission type</span></span>|<span data-ttu-id="67a29-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="67a29-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67a29-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67a29-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67a29-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67a29-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="67a29-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67a29-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67a29-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67a29-116">Not supported.</span></span>|
|<span data-ttu-id="67a29-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67a29-117">Application</span></span>|<span data-ttu-id="67a29-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67a29-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67a29-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67a29-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="67a29-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="67a29-120">Request headers</span></span>
|<span data-ttu-id="67a29-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="67a29-121">Header</span></span>|<span data-ttu-id="67a29-122">Значение</span><span class="sxs-lookup"><span data-stu-id="67a29-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67a29-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67a29-123">Authorization</span></span>|<span data-ttu-id="67a29-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67a29-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67a29-125">Accept</span><span class="sxs-lookup"><span data-stu-id="67a29-125">Accept</span></span>|<span data-ttu-id="67a29-126">application/json</span><span class="sxs-lookup"><span data-stu-id="67a29-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67a29-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="67a29-127">Request body</span></span>
<span data-ttu-id="67a29-128">В тексте запроса добавьте представление объекта [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67a29-128">In the request body, supply a JSON representation for the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

<span data-ttu-id="67a29-129">В следующей таблице приведены свойства, необходимые при создании [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67a29-129">The following table shows the properties that are required when you create the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span></span>

|<span data-ttu-id="67a29-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="67a29-130">Property</span></span>|<span data-ttu-id="67a29-131">Тип</span><span class="sxs-lookup"><span data-stu-id="67a29-131">Type</span></span>|<span data-ttu-id="67a29-132">Описание</span><span class="sxs-lookup"><span data-stu-id="67a29-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67a29-133">id</span><span class="sxs-lookup"><span data-stu-id="67a29-133">id</span></span>|<span data-ttu-id="67a29-134">Строка</span><span class="sxs-lookup"><span data-stu-id="67a29-134">String</span></span>|<span data-ttu-id="67a29-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="67a29-135">Key of the entity.</span></span> <span data-ttu-id="67a29-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67a29-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67a29-137">lastModifiedDateTime</span></span>|<span data-ttu-id="67a29-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67a29-138">DateTimeOffset</span></span>|<span data-ttu-id="67a29-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="67a29-139">DateTime the object was last modified.</span></span> <span data-ttu-id="67a29-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67a29-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="67a29-141">roleScopeTagIds</span></span>|<span data-ttu-id="67a29-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="67a29-142">String collection</span></span>|<span data-ttu-id="67a29-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="67a29-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="67a29-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67a29-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="67a29-145">supportsScopeTags</span></span>|<span data-ttu-id="67a29-146">Логический</span><span class="sxs-lookup"><span data-stu-id="67a29-146">Boolean</span></span>|<span data-ttu-id="67a29-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="67a29-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="67a29-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="67a29-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="67a29-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="67a29-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="67a29-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="67a29-150">This property is read-only.</span></span> <span data-ttu-id="67a29-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67a29-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="67a29-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="67a29-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="67a29-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="67a29-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="67a29-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="67a29-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67a29-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="67a29-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="67a29-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="67a29-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="67a29-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="67a29-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="67a29-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67a29-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="67a29-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="67a29-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="67a29-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="67a29-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="67a29-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="67a29-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67a29-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67a29-164">createdDateTime</span></span>|<span data-ttu-id="67a29-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67a29-165">DateTimeOffset</span></span>|<span data-ttu-id="67a29-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="67a29-166">DateTime the object was created.</span></span> <span data-ttu-id="67a29-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67a29-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-168">description</span><span class="sxs-lookup"><span data-stu-id="67a29-168">description</span></span>|<span data-ttu-id="67a29-169">Строка</span><span class="sxs-lookup"><span data-stu-id="67a29-169">String</span></span>|<span data-ttu-id="67a29-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="67a29-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="67a29-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67a29-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-172">displayName</span><span class="sxs-lookup"><span data-stu-id="67a29-172">displayName</span></span>|<span data-ttu-id="67a29-173">Строка</span><span class="sxs-lookup"><span data-stu-id="67a29-173">String</span></span>|<span data-ttu-id="67a29-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="67a29-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="67a29-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67a29-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-176">version</span><span class="sxs-lookup"><span data-stu-id="67a29-176">version</span></span>|<span data-ttu-id="67a29-177">Int32</span><span class="sxs-lookup"><span data-stu-id="67a29-177">Int32</span></span>|<span data-ttu-id="67a29-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="67a29-178">Version of the device configuration.</span></span> <span data-ttu-id="67a29-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67a29-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="67a29-180">connectionName</span></span>|<span data-ttu-id="67a29-181">Строка</span><span class="sxs-lookup"><span data-stu-id="67a29-181">String</span></span>|<span data-ttu-id="67a29-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="67a29-182">Connection name displayed to the user.</span></span> <span data-ttu-id="67a29-183">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="67a29-184">connectionType</span></span>|[<span data-ttu-id="67a29-185">апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="67a29-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="67a29-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="67a29-186">Connection type.</span></span> <span data-ttu-id="67a29-187">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67a29-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="67a29-188">Возможные значения:,,,,,,,,,, `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` ,, `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` , `paloAltoGlobalProtectV2` , `ikEv2` , `alwaysOn` `microsoftTunnel` `netMotionMobility` ,,.</span><span class="sxs-lookup"><span data-stu-id="67a29-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="67a29-189">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="67a29-189">loginGroupOrDomain</span></span>|<span data-ttu-id="67a29-190">Строка</span><span class="sxs-lookup"><span data-stu-id="67a29-190">String</span></span>|<span data-ttu-id="67a29-191">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="67a29-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="67a29-192">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-193">role</span><span class="sxs-lookup"><span data-stu-id="67a29-193">role</span></span>|<span data-ttu-id="67a29-194">Строка</span><span class="sxs-lookup"><span data-stu-id="67a29-194">String</span></span>|<span data-ttu-id="67a29-195">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="67a29-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="67a29-196">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-197">область</span><span class="sxs-lookup"><span data-stu-id="67a29-197">realm</span></span>|<span data-ttu-id="67a29-198">Строка</span><span class="sxs-lookup"><span data-stu-id="67a29-198">String</span></span>|<span data-ttu-id="67a29-199">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="67a29-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="67a29-200">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-201">сервер</span><span class="sxs-lookup"><span data-stu-id="67a29-201">server</span></span>|[<span data-ttu-id="67a29-202">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="67a29-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="67a29-203">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="67a29-203">VPN Server on the network.</span></span> <span data-ttu-id="67a29-204">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="67a29-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="67a29-205">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="67a29-206">identifier</span></span>|<span data-ttu-id="67a29-207">Строка</span><span class="sxs-lookup"><span data-stu-id="67a29-207">String</span></span>|<span data-ttu-id="67a29-208">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="67a29-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="67a29-209">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-210">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="67a29-210">customData</span></span>|<span data-ttu-id="67a29-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="67a29-212">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="67a29-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="67a29-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="67a29-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="67a29-214">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="67a29-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="67a29-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="67a29-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="67a29-216">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="67a29-217">customKeyValueData</span></span>|<span data-ttu-id="67a29-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="67a29-219">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="67a29-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="67a29-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="67a29-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="67a29-221">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="67a29-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="67a29-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="67a29-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="67a29-223">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-224">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="67a29-224">enableSplitTunneling</span></span>|<span data-ttu-id="67a29-225">Логический</span><span class="sxs-lookup"><span data-stu-id="67a29-225">Boolean</span></span>|<span data-ttu-id="67a29-226">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="67a29-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="67a29-227">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-228">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="67a29-228">authenticationMethod</span></span>|[<span data-ttu-id="67a29-229">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="67a29-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="67a29-230">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="67a29-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="67a29-231">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67a29-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="67a29-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="67a29-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="67a29-233">енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="67a29-233">enablePerApp</span></span>|<span data-ttu-id="67a29-234">Логический</span><span class="sxs-lookup"><span data-stu-id="67a29-234">Boolean</span></span>|<span data-ttu-id="67a29-235">Если задать для этого параметра значение true, будут созданы Per-App полезные данные VPN, которые позже могут быть связаны с приложениями, которые могут запускать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="67a29-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="67a29-236">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-237">сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="67a29-237">safariDomains</span></span>|<span data-ttu-id="67a29-238">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="67a29-238">String collection</span></span>|<span data-ttu-id="67a29-239">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="67a29-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="67a29-240">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="67a29-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="67a29-241">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-242">ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="67a29-242">onDemandRules</span></span>|<span data-ttu-id="67a29-243">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="67a29-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="67a29-244">On-Demand Rules.</span></span> <span data-ttu-id="67a29-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="67a29-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="67a29-246">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-247">providerType</span><span class="sxs-lookup"><span data-stu-id="67a29-247">providerType</span></span>|[<span data-ttu-id="67a29-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="67a29-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="67a29-249">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="67a29-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="67a29-250">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67a29-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="67a29-251">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="67a29-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="67a29-252">ексклудеддомаинс</span><span class="sxs-lookup"><span data-stu-id="67a29-252">excludedDomains</span></span>|<span data-ttu-id="67a29-253">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="67a29-253">String collection</span></span>|<span data-ttu-id="67a29-254">Домены, доступ к которым осуществляется через общедоступный Интернет, а не через VPN, даже если VPN для каждого приложения активируется наследуемой от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-254">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-255">дисаблеондемандусероверриде</span><span class="sxs-lookup"><span data-stu-id="67a29-255">disableOnDemandUserOverride</span></span>|<span data-ttu-id="67a29-256">Логический</span><span class="sxs-lookup"><span data-stu-id="67a29-256">Boolean</span></span>|<span data-ttu-id="67a29-257">Переключатель, чтобы запретить пользователям отключать автоматическое VPN в приложении "Параметры", унаследованном от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-257">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-258">проксисервер</span><span class="sxs-lookup"><span data-stu-id="67a29-258">proxyServer</span></span>|[<span data-ttu-id="67a29-259">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="67a29-259">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="67a29-260">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="67a29-260">Proxy Server.</span></span> <span data-ttu-id="67a29-261">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-261">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-262">оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="67a29-262">optInToDeviceIdSharing</span></span>|<span data-ttu-id="67a29-263">Логический</span><span class="sxs-lookup"><span data-stu-id="67a29-263">Boolean</span></span>|<span data-ttu-id="67a29-264">Opt-In для предоставления доступа к идентификатору устройства сторонним VPN-клиентам для использования в процессе проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="67a29-264">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="67a29-265">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-265">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-266">userDomain</span><span class="sxs-lookup"><span data-stu-id="67a29-266">userDomain</span></span>|<span data-ttu-id="67a29-267">Строка</span><span class="sxs-lookup"><span data-stu-id="67a29-267">String</span></span>|<span data-ttu-id="67a29-268">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="67a29-268">Zscaler only.</span></span> <span data-ttu-id="67a29-269">Введите статический домен для предварительного заполнения поля Login в приложении Зскалер.</span><span class="sxs-lookup"><span data-stu-id="67a29-269">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="67a29-270">Если оставить это поле пустым, вместо этого будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="67a29-270">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="67a29-271">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-272">стриктенфорцемент</span><span class="sxs-lookup"><span data-stu-id="67a29-272">strictEnforcement</span></span>|<span data-ttu-id="67a29-273">Логический</span><span class="sxs-lookup"><span data-stu-id="67a29-273">Boolean</span></span>|<span data-ttu-id="67a29-274">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="67a29-274">Zscaler only.</span></span> <span data-ttu-id="67a29-275">Блокирует сетевой трафик до тех пор, пока пользователь не войдет в приложение Зскалер.</span><span class="sxs-lookup"><span data-stu-id="67a29-275">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="67a29-276">"True" означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="67a29-276">"True" means traffic is blocked.</span></span> <span data-ttu-id="67a29-277">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-277">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-278">клауднаме</span><span class="sxs-lookup"><span data-stu-id="67a29-278">cloudName</span></span>|<span data-ttu-id="67a29-279">Строка</span><span class="sxs-lookup"><span data-stu-id="67a29-279">String</span></span>|<span data-ttu-id="67a29-280">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="67a29-280">Zscaler only.</span></span> <span data-ttu-id="67a29-281">Облако зскалер, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="67a29-281">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="67a29-282">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-282">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-283">excludeList</span><span class="sxs-lookup"><span data-stu-id="67a29-283">excludeList</span></span>|<span data-ttu-id="67a29-284">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="67a29-284">String collection</span></span>|<span data-ttu-id="67a29-285">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="67a29-285">Zscaler only.</span></span> <span data-ttu-id="67a29-286">Список сетевых адресов, которые не отправляются через облако Зскалер.</span><span class="sxs-lookup"><span data-stu-id="67a29-286">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="67a29-287">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-287">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-288">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="67a29-288">targetedMobileApps</span></span>|<span data-ttu-id="67a29-289">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-289">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="67a29-290">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="67a29-290">Targeted mobile apps.</span></span> <span data-ttu-id="67a29-291">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="67a29-291">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="67a29-292">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-292">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-293">микрософттуннелситеид</span><span class="sxs-lookup"><span data-stu-id="67a29-293">microsoftTunnelSiteId</span></span>|<span data-ttu-id="67a29-294">Строка</span><span class="sxs-lookup"><span data-stu-id="67a29-294">String</span></span>|<span data-ttu-id="67a29-295">Идентификатор сайта туннеля (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="67a29-295">Microsoft Tunnel site ID.</span></span> <span data-ttu-id="67a29-296">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a29-296">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="67a29-297">чилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="67a29-297">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="67a29-298">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="67a29-298">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="67a29-299">Дочерние параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="67a29-299">Child Security Association Parameters</span></span>|
|<span data-ttu-id="67a29-300">клиентаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="67a29-300">clientAuthenticationType</span></span>|[<span data-ttu-id="67a29-301">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="67a29-301">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="67a29-302">Тип проверки подлинности клиента, который будет использоваться VPN-клиентом.</span><span class="sxs-lookup"><span data-stu-id="67a29-302">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="67a29-303">Возможные значения: `userAuthentication`, `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="67a29-303">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="67a29-304">деадпирдетектионрате</span><span class="sxs-lookup"><span data-stu-id="67a29-304">deadPeerDetectionRate</span></span>|[<span data-ttu-id="67a29-305">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="67a29-305">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="67a29-306">Определите, как часто следует проверять, активен ли одноранговый сеанс.</span><span class="sxs-lookup"><span data-stu-id="67a29-306">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="67a29-307">.</span><span class="sxs-lookup"><span data-stu-id="67a29-307">.</span></span> <span data-ttu-id="67a29-308">Возможные значения: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="67a29-308">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="67a29-309">дисаблемобилитяндмултихоминг</span><span class="sxs-lookup"><span data-stu-id="67a29-309">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="67a29-310">Логический</span><span class="sxs-lookup"><span data-stu-id="67a29-310">Boolean</span></span>|<span data-ttu-id="67a29-311">Отключение МОБИКЕ</span><span class="sxs-lookup"><span data-stu-id="67a29-311">Disable MOBIKE</span></span>|
|<span data-ttu-id="67a29-312">дисаблередирект</span><span class="sxs-lookup"><span data-stu-id="67a29-312">disableRedirect</span></span>|<span data-ttu-id="67a29-313">Логический</span><span class="sxs-lookup"><span data-stu-id="67a29-313">Boolean</span></span>|<span data-ttu-id="67a29-314">Отключение перенаправления</span><span class="sxs-lookup"><span data-stu-id="67a29-314">Disable Redirect</span></span>|
|<span data-ttu-id="67a29-315">енаблецертификатеревокатиончекк</span><span class="sxs-lookup"><span data-stu-id="67a29-315">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="67a29-316">Логический</span><span class="sxs-lookup"><span data-stu-id="67a29-316">Boolean</span></span>|<span data-ttu-id="67a29-317">Включает проверку отзывов и действий. время ожидания отклика сервера не приведет к сбою</span><span class="sxs-lookup"><span data-stu-id="67a29-317">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="67a29-318">енаблиап</span><span class="sxs-lookup"><span data-stu-id="67a29-318">enableEAP</span></span>|<span data-ttu-id="67a29-319">Логический</span><span class="sxs-lookup"><span data-stu-id="67a29-319">Boolean</span></span>|<span data-ttu-id="67a29-320">Включает проверку подлинности только EAP</span><span class="sxs-lookup"><span data-stu-id="67a29-320">Enables EAP only authentication</span></span>|
|<span data-ttu-id="67a29-321">енаблеперфектфорвардсекреци</span><span class="sxs-lookup"><span data-stu-id="67a29-321">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="67a29-322">Логический</span><span class="sxs-lookup"><span data-stu-id="67a29-322">Boolean</span></span>|<span data-ttu-id="67a29-323">Включить безопасную пересылку (PFS).</span><span class="sxs-lookup"><span data-stu-id="67a29-323">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="67a29-324">енаблеусеинтерналсубнетаттрибутес</span><span class="sxs-lookup"><span data-stu-id="67a29-324">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="67a29-325">Логический</span><span class="sxs-lookup"><span data-stu-id="67a29-325">Boolean</span></span>|<span data-ttu-id="67a29-326">Включите использование атрибутов внутренней подсети.</span><span class="sxs-lookup"><span data-stu-id="67a29-326">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="67a29-327">локалидентифиер</span><span class="sxs-lookup"><span data-stu-id="67a29-327">localIdentifier</span></span>|[<span data-ttu-id="67a29-328">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="67a29-328">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="67a29-329">Метод идентификации клиента, который пытается подключиться через VPN.</span><span class="sxs-lookup"><span data-stu-id="67a29-329">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="67a29-330">.</span><span class="sxs-lookup"><span data-stu-id="67a29-330">.</span></span> <span data-ttu-id="67a29-331">Возможные значения: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="67a29-331">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="67a29-332">ремотеидентифиер</span><span class="sxs-lookup"><span data-stu-id="67a29-332">remoteIdentifier</span></span>|<span data-ttu-id="67a29-333">Строка</span><span class="sxs-lookup"><span data-stu-id="67a29-333">String</span></span>|<span data-ttu-id="67a29-334">Адрес сервера IKEv2.</span><span class="sxs-lookup"><span data-stu-id="67a29-334">Address of the IKEv2 server.</span></span> <span data-ttu-id="67a29-335">Должно быть полным доменным именем, Усерфкдн, сетевым адресом или ASN1DN</span><span class="sxs-lookup"><span data-stu-id="67a29-335">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="67a29-336">секуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="67a29-336">securityAssociationParameters</span></span>|[<span data-ttu-id="67a29-337">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="67a29-337">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="67a29-338">Параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="67a29-338">Security Association Parameters</span></span>|
|<span data-ttu-id="67a29-339">серверцертификатекоммоннаме</span><span class="sxs-lookup"><span data-stu-id="67a29-339">serverCertificateCommonName</span></span>|<span data-ttu-id="67a29-340">Строка</span><span class="sxs-lookup"><span data-stu-id="67a29-340">String</span></span>|<span data-ttu-id="67a29-341">Общее имя сертификата сервера IKEv2, используемого при проверке подлинности сервера</span><span class="sxs-lookup"><span data-stu-id="67a29-341">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="67a29-342">серверцертификатеиссуеркоммоннаме</span><span class="sxs-lookup"><span data-stu-id="67a29-342">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="67a29-343">Строка</span><span class="sxs-lookup"><span data-stu-id="67a29-343">String</span></span>|<span data-ttu-id="67a29-344">Общее имя поставщика сертификата сервера IKEv2, используемого при проверке подлинности</span><span class="sxs-lookup"><span data-stu-id="67a29-344">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="67a29-345">серверцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="67a29-345">serverCertificateType</span></span>|[<span data-ttu-id="67a29-346">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="67a29-346">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="67a29-347">Тип сертификата, который VPN-сервер будет предоставлять VPN-клиенту для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="67a29-347">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="67a29-348">Возможные значения: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="67a29-348">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="67a29-349">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="67a29-349">sharedSecret</span></span>|<span data-ttu-id="67a29-350">Строка</span><span class="sxs-lookup"><span data-stu-id="67a29-350">String</span></span>|<span data-ttu-id="67a29-351">Используется, когда выбрана общая секретная проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="67a29-351">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="67a29-352">тлсмаксимумверсион</span><span class="sxs-lookup"><span data-stu-id="67a29-352">tlsMaximumVersion</span></span>|<span data-ttu-id="67a29-353">Строка</span><span class="sxs-lookup"><span data-stu-id="67a29-353">String</span></span>|<span data-ttu-id="67a29-354">Максимальная версия TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="67a29-354">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="67a29-355">тлсминимумверсион</span><span class="sxs-lookup"><span data-stu-id="67a29-355">tlsMinimumVersion</span></span>|<span data-ttu-id="67a29-356">Строка</span><span class="sxs-lookup"><span data-stu-id="67a29-356">String</span></span>|<span data-ttu-id="67a29-357">Минимальная версия протокола TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="67a29-357">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="67a29-358">алловдефаултсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="67a29-358">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="67a29-359">Логический</span><span class="sxs-lookup"><span data-stu-id="67a29-359">Boolean</span></span>|<span data-ttu-id="67a29-360">Разрешает использование параметров сопоставления безопасности путем установки всех параметров для устройства по умолчанию, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="67a29-360">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="67a29-361">алловдефаултчилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="67a29-361">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="67a29-362">Логический</span><span class="sxs-lookup"><span data-stu-id="67a29-362">Boolean</span></span>|<span data-ttu-id="67a29-363">Разрешает использование параметров дочернего сопоставления безопасности, устанавливая все параметры по умолчанию устройства, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="67a29-363">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="67a29-364">алвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="67a29-364">alwaysOnConfiguration</span></span>|[<span data-ttu-id="67a29-365">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="67a29-365">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="67a29-366">Конфигурация AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="67a29-366">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="67a29-367">енаблеалвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="67a29-367">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="67a29-368">Логический</span><span class="sxs-lookup"><span data-stu-id="67a29-368">Boolean</span></span>|<span data-ttu-id="67a29-369">Определяет, включена ли функция "всегда включено" VPN</span><span class="sxs-lookup"><span data-stu-id="67a29-369">Determines if Always on VPN is enabled</span></span>|
|<span data-ttu-id="67a29-370">мтусизеинбитес</span><span class="sxs-lookup"><span data-stu-id="67a29-370">mtuSizeInBytes</span></span>|<span data-ttu-id="67a29-371">Int32</span><span class="sxs-lookup"><span data-stu-id="67a29-371">Int32</span></span>|<span data-ttu-id="67a29-372">Максимальное количество передаваемых данных.</span><span class="sxs-lookup"><span data-stu-id="67a29-372">Maximum transmission unit.</span></span> <span data-ttu-id="67a29-373">Допустимые значения — от 1 до 65536</span><span class="sxs-lookup"><span data-stu-id="67a29-373">Valid values 1 to 65536</span></span>|



## <a name="response"></a><span data-ttu-id="67a29-374">Ответ</span><span class="sxs-lookup"><span data-stu-id="67a29-374">Response</span></span>
<span data-ttu-id="67a29-375">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="67a29-375">If successful, this method returns a `200 OK` response code and an updated [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67a29-376">Пример</span><span class="sxs-lookup"><span data-stu-id="67a29-376">Example</span></span>

### <a name="request"></a><span data-ttu-id="67a29-377">Запрос</span><span class="sxs-lookup"><span data-stu-id="67a29-377">Request</span></span>
<span data-ttu-id="67a29-378">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67a29-378">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 5428

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
  "providerType": "appProxy",
  "excludedDomains": [
    "Excluded Domains value"
  ],
  "disableOnDemandUserOverride": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ],
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value",
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
  "enableAlwaysOnConfiguration": true,
  "mtuSizeInBytes": 14
}
```

### <a name="response"></a><span data-ttu-id="67a29-379">Отклик</span><span class="sxs-lookup"><span data-stu-id="67a29-379">Response</span></span>
<span data-ttu-id="67a29-p142">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67a29-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5600

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
  "providerType": "appProxy",
  "excludedDomains": [
    "Excluded Domains value"
  ],
  "disableOnDemandUserOverride": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ],
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value",
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
  "enableAlwaysOnConfiguration": true,
  "mtuSizeInBytes": 14
}
```





