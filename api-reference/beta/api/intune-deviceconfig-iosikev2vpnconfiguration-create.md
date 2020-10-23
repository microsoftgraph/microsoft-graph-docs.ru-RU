---
title: Создание iosikEv2VpnConfiguration
description: Создание нового объекта iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2763f91c085a1c11d33ef1c0a8854eebc34f1581
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48689799"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="0346e-103">Создание iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0346e-103">Create iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="0346e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0346e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0346e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0346e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0346e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0346e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0346e-107">Создание нового объекта [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0346e-107">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0346e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0346e-108">Prerequisites</span></span>
<span data-ttu-id="0346e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0346e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0346e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0346e-111">Permission type</span></span>|<span data-ttu-id="0346e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0346e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0346e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0346e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0346e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0346e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0346e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0346e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0346e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0346e-116">Not supported.</span></span>|
|<span data-ttu-id="0346e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0346e-117">Application</span></span>|<span data-ttu-id="0346e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0346e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0346e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0346e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0346e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0346e-120">Request headers</span></span>
|<span data-ttu-id="0346e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0346e-121">Header</span></span>|<span data-ttu-id="0346e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0346e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0346e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0346e-123">Authorization</span></span>|<span data-ttu-id="0346e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0346e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0346e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0346e-125">Accept</span></span>|<span data-ttu-id="0346e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0346e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0346e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0346e-127">Request body</span></span>
<span data-ttu-id="0346e-128">В тексте запроса добавьте представление объекта iosikEv2VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0346e-128">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="0346e-129">В следующей таблице приведены свойства, необходимые при создании iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0346e-129">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="0346e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0346e-130">Property</span></span>|<span data-ttu-id="0346e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0346e-131">Type</span></span>|<span data-ttu-id="0346e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0346e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0346e-133">id</span><span class="sxs-lookup"><span data-stu-id="0346e-133">id</span></span>|<span data-ttu-id="0346e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0346e-134">String</span></span>|<span data-ttu-id="0346e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0346e-135">Key of the entity.</span></span> <span data-ttu-id="0346e-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0346e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0346e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0346e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0346e-138">DateTimeOffset</span></span>|<span data-ttu-id="0346e-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0346e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0346e-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0346e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0346e-141">roleScopeTagIds</span></span>|<span data-ttu-id="0346e-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0346e-142">String collection</span></span>|<span data-ttu-id="0346e-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="0346e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0346e-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0346e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="0346e-145">supportsScopeTags</span></span>|<span data-ttu-id="0346e-146">Логический</span><span class="sxs-lookup"><span data-stu-id="0346e-146">Boolean</span></span>|<span data-ttu-id="0346e-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="0346e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0346e-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="0346e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0346e-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="0346e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0346e-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0346e-150">This property is read-only.</span></span> <span data-ttu-id="0346e-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0346e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0346e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0346e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0346e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0346e-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0346e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0346e-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0346e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0346e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0346e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0346e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0346e-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0346e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0346e-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0346e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0346e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0346e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0346e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0346e-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0346e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0346e-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0346e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0346e-164">createdDateTime</span></span>|<span data-ttu-id="0346e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0346e-165">DateTimeOffset</span></span>|<span data-ttu-id="0346e-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0346e-166">DateTime the object was created.</span></span> <span data-ttu-id="0346e-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0346e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-168">description</span><span class="sxs-lookup"><span data-stu-id="0346e-168">description</span></span>|<span data-ttu-id="0346e-169">Строка</span><span class="sxs-lookup"><span data-stu-id="0346e-169">String</span></span>|<span data-ttu-id="0346e-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0346e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0346e-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0346e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0346e-172">displayName</span></span>|<span data-ttu-id="0346e-173">Строка</span><span class="sxs-lookup"><span data-stu-id="0346e-173">String</span></span>|<span data-ttu-id="0346e-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0346e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0346e-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0346e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-176">version</span><span class="sxs-lookup"><span data-stu-id="0346e-176">version</span></span>|<span data-ttu-id="0346e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0346e-177">Int32</span></span>|<span data-ttu-id="0346e-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0346e-178">Version of the device configuration.</span></span> <span data-ttu-id="0346e-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0346e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="0346e-180">connectionName</span></span>|<span data-ttu-id="0346e-181">Строка</span><span class="sxs-lookup"><span data-stu-id="0346e-181">String</span></span>|<span data-ttu-id="0346e-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="0346e-182">Connection name displayed to the user.</span></span> <span data-ttu-id="0346e-183">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="0346e-184">connectionType</span></span>|[<span data-ttu-id="0346e-185">апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="0346e-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="0346e-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="0346e-186">Connection type.</span></span> <span data-ttu-id="0346e-187">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0346e-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0346e-188">Возможные значения:,,,,,,,,,, `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` ,, `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` , `paloAltoGlobalProtectV2` , `ikEv2` , `alwaysOn` `microsoftTunnel` `netMotionMobility` ,,.</span><span class="sxs-lookup"><span data-stu-id="0346e-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="0346e-189">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="0346e-189">loginGroupOrDomain</span></span>|<span data-ttu-id="0346e-190">Строка</span><span class="sxs-lookup"><span data-stu-id="0346e-190">String</span></span>|<span data-ttu-id="0346e-191">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="0346e-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="0346e-192">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-193">role</span><span class="sxs-lookup"><span data-stu-id="0346e-193">role</span></span>|<span data-ttu-id="0346e-194">Строка</span><span class="sxs-lookup"><span data-stu-id="0346e-194">String</span></span>|<span data-ttu-id="0346e-195">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="0346e-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="0346e-196">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-197">область</span><span class="sxs-lookup"><span data-stu-id="0346e-197">realm</span></span>|<span data-ttu-id="0346e-198">Строка</span><span class="sxs-lookup"><span data-stu-id="0346e-198">String</span></span>|<span data-ttu-id="0346e-199">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="0346e-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="0346e-200">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-201">сервер</span><span class="sxs-lookup"><span data-stu-id="0346e-201">server</span></span>|[<span data-ttu-id="0346e-202">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="0346e-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="0346e-203">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="0346e-203">VPN Server on the network.</span></span> <span data-ttu-id="0346e-204">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="0346e-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="0346e-205">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="0346e-206">identifier</span></span>|<span data-ttu-id="0346e-207">Строка</span><span class="sxs-lookup"><span data-stu-id="0346e-207">String</span></span>|<span data-ttu-id="0346e-208">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="0346e-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0346e-209">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-210">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="0346e-210">customData</span></span>|<span data-ttu-id="0346e-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="0346e-212">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="0346e-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0346e-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="0346e-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="0346e-214">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="0346e-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="0346e-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="0346e-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="0346e-216">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="0346e-217">customKeyValueData</span></span>|<span data-ttu-id="0346e-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0346e-219">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="0346e-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="0346e-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="0346e-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="0346e-221">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="0346e-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="0346e-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="0346e-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="0346e-223">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-224">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="0346e-224">enableSplitTunneling</span></span>|<span data-ttu-id="0346e-225">Логический</span><span class="sxs-lookup"><span data-stu-id="0346e-225">Boolean</span></span>|<span data-ttu-id="0346e-226">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="0346e-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="0346e-227">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-228">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="0346e-228">authenticationMethod</span></span>|[<span data-ttu-id="0346e-229">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="0346e-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="0346e-230">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="0346e-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="0346e-231">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0346e-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0346e-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="0346e-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="0346e-233">енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="0346e-233">enablePerApp</span></span>|<span data-ttu-id="0346e-234">Логический</span><span class="sxs-lookup"><span data-stu-id="0346e-234">Boolean</span></span>|<span data-ttu-id="0346e-235">Если задать для этого параметра значение true, будут созданы Per-App полезные данные VPN, которые позже могут быть связаны с приложениями, которые могут запускать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="0346e-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="0346e-236">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-237">сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="0346e-237">safariDomains</span></span>|<span data-ttu-id="0346e-238">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0346e-238">String collection</span></span>|<span data-ttu-id="0346e-239">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="0346e-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="0346e-240">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="0346e-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="0346e-241">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-242">ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="0346e-242">onDemandRules</span></span>|<span data-ttu-id="0346e-243">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="0346e-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="0346e-244">On-Demand Rules.</span></span> <span data-ttu-id="0346e-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="0346e-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0346e-246">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-247">providerType</span><span class="sxs-lookup"><span data-stu-id="0346e-247">providerType</span></span>|[<span data-ttu-id="0346e-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="0346e-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="0346e-249">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="0346e-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="0346e-250">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0346e-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="0346e-251">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="0346e-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="0346e-252">ексклудеддомаинс</span><span class="sxs-lookup"><span data-stu-id="0346e-252">excludedDomains</span></span>|<span data-ttu-id="0346e-253">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0346e-253">String collection</span></span>|<span data-ttu-id="0346e-254">Домены, доступ к которым осуществляется через общедоступный Интернет, а не через VPN, даже если VPN для каждого приложения активируется наследуемой от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-254">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-255">дисаблеондемандусероверриде</span><span class="sxs-lookup"><span data-stu-id="0346e-255">disableOnDemandUserOverride</span></span>|<span data-ttu-id="0346e-256">Логический</span><span class="sxs-lookup"><span data-stu-id="0346e-256">Boolean</span></span>|<span data-ttu-id="0346e-257">Переключатель, чтобы запретить пользователям отключать автоматическое VPN в приложении "Параметры", унаследованном от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-257">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-258">проксисервер</span><span class="sxs-lookup"><span data-stu-id="0346e-258">proxyServer</span></span>|[<span data-ttu-id="0346e-259">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="0346e-259">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="0346e-260">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="0346e-260">Proxy Server.</span></span> <span data-ttu-id="0346e-261">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-261">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-262">оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="0346e-262">optInToDeviceIdSharing</span></span>|<span data-ttu-id="0346e-263">Логический</span><span class="sxs-lookup"><span data-stu-id="0346e-263">Boolean</span></span>|<span data-ttu-id="0346e-264">Opt-In для предоставления доступа к идентификатору устройства сторонним VPN-клиентам для использования в процессе проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="0346e-264">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="0346e-265">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-265">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-266">userDomain</span><span class="sxs-lookup"><span data-stu-id="0346e-266">userDomain</span></span>|<span data-ttu-id="0346e-267">Строка</span><span class="sxs-lookup"><span data-stu-id="0346e-267">String</span></span>|<span data-ttu-id="0346e-268">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="0346e-268">Zscaler only.</span></span> <span data-ttu-id="0346e-269">Введите статический домен для предварительного заполнения поля Login в приложении Зскалер.</span><span class="sxs-lookup"><span data-stu-id="0346e-269">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="0346e-270">Если оставить это поле пустым, вместо этого будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="0346e-270">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="0346e-271">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-272">стриктенфорцемент</span><span class="sxs-lookup"><span data-stu-id="0346e-272">strictEnforcement</span></span>|<span data-ttu-id="0346e-273">Логический</span><span class="sxs-lookup"><span data-stu-id="0346e-273">Boolean</span></span>|<span data-ttu-id="0346e-274">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="0346e-274">Zscaler only.</span></span> <span data-ttu-id="0346e-275">Блокирует сетевой трафик до тех пор, пока пользователь не войдет в приложение Зскалер.</span><span class="sxs-lookup"><span data-stu-id="0346e-275">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="0346e-276">"True" означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="0346e-276">"True" means traffic is blocked.</span></span> <span data-ttu-id="0346e-277">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-277">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-278">клауднаме</span><span class="sxs-lookup"><span data-stu-id="0346e-278">cloudName</span></span>|<span data-ttu-id="0346e-279">Строка</span><span class="sxs-lookup"><span data-stu-id="0346e-279">String</span></span>|<span data-ttu-id="0346e-280">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="0346e-280">Zscaler only.</span></span> <span data-ttu-id="0346e-281">Облако зскалер, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="0346e-281">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="0346e-282">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-282">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-283">excludeList</span><span class="sxs-lookup"><span data-stu-id="0346e-283">excludeList</span></span>|<span data-ttu-id="0346e-284">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0346e-284">String collection</span></span>|<span data-ttu-id="0346e-285">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="0346e-285">Zscaler only.</span></span> <span data-ttu-id="0346e-286">Список сетевых адресов, которые не отправляются через облако Зскалер.</span><span class="sxs-lookup"><span data-stu-id="0346e-286">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="0346e-287">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-287">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-288">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="0346e-288">targetedMobileApps</span></span>|<span data-ttu-id="0346e-289">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-289">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="0346e-290">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="0346e-290">Targeted mobile apps.</span></span> <span data-ttu-id="0346e-291">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="0346e-291">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0346e-292">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-292">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-293">микрософттуннелситеид</span><span class="sxs-lookup"><span data-stu-id="0346e-293">microsoftTunnelSiteId</span></span>|<span data-ttu-id="0346e-294">Строка</span><span class="sxs-lookup"><span data-stu-id="0346e-294">String</span></span>|<span data-ttu-id="0346e-295">Идентификатор сайта туннеля (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="0346e-295">Microsoft Tunnel site ID.</span></span> <span data-ttu-id="0346e-296">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0346e-296">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0346e-297">чилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="0346e-297">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="0346e-298">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0346e-298">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="0346e-299">Дочерние параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="0346e-299">Child Security Association Parameters</span></span>|
|<span data-ttu-id="0346e-300">клиентаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="0346e-300">clientAuthenticationType</span></span>|[<span data-ttu-id="0346e-301">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="0346e-301">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="0346e-302">Тип проверки подлинности клиента, который будет использоваться VPN-клиентом.</span><span class="sxs-lookup"><span data-stu-id="0346e-302">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="0346e-303">Возможные значения: `userAuthentication`, `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="0346e-303">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="0346e-304">деадпирдетектионрате</span><span class="sxs-lookup"><span data-stu-id="0346e-304">deadPeerDetectionRate</span></span>|[<span data-ttu-id="0346e-305">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="0346e-305">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="0346e-306">Определите, как часто следует проверять, активен ли одноранговый сеанс.</span><span class="sxs-lookup"><span data-stu-id="0346e-306">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="0346e-307">.</span><span class="sxs-lookup"><span data-stu-id="0346e-307">.</span></span> <span data-ttu-id="0346e-308">Возможные значения: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="0346e-308">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="0346e-309">дисаблемобилитяндмултихоминг</span><span class="sxs-lookup"><span data-stu-id="0346e-309">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="0346e-310">Логический</span><span class="sxs-lookup"><span data-stu-id="0346e-310">Boolean</span></span>|<span data-ttu-id="0346e-311">Отключение МОБИКЕ</span><span class="sxs-lookup"><span data-stu-id="0346e-311">Disable MOBIKE</span></span>|
|<span data-ttu-id="0346e-312">дисаблередирект</span><span class="sxs-lookup"><span data-stu-id="0346e-312">disableRedirect</span></span>|<span data-ttu-id="0346e-313">Логический</span><span class="sxs-lookup"><span data-stu-id="0346e-313">Boolean</span></span>|<span data-ttu-id="0346e-314">Отключение перенаправления</span><span class="sxs-lookup"><span data-stu-id="0346e-314">Disable Redirect</span></span>|
|<span data-ttu-id="0346e-315">енаблецертификатеревокатиончекк</span><span class="sxs-lookup"><span data-stu-id="0346e-315">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="0346e-316">Логический</span><span class="sxs-lookup"><span data-stu-id="0346e-316">Boolean</span></span>|<span data-ttu-id="0346e-317">Включает проверку отзывов и действий. время ожидания отклика сервера не приведет к сбою</span><span class="sxs-lookup"><span data-stu-id="0346e-317">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="0346e-318">енаблиап</span><span class="sxs-lookup"><span data-stu-id="0346e-318">enableEAP</span></span>|<span data-ttu-id="0346e-319">Логический</span><span class="sxs-lookup"><span data-stu-id="0346e-319">Boolean</span></span>|<span data-ttu-id="0346e-320">Включает проверку подлинности только EAP</span><span class="sxs-lookup"><span data-stu-id="0346e-320">Enables EAP only authentication</span></span>|
|<span data-ttu-id="0346e-321">енаблеперфектфорвардсекреци</span><span class="sxs-lookup"><span data-stu-id="0346e-321">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="0346e-322">Логический</span><span class="sxs-lookup"><span data-stu-id="0346e-322">Boolean</span></span>|<span data-ttu-id="0346e-323">Включить безопасную пересылку (PFS).</span><span class="sxs-lookup"><span data-stu-id="0346e-323">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="0346e-324">енаблеусеинтерналсубнетаттрибутес</span><span class="sxs-lookup"><span data-stu-id="0346e-324">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="0346e-325">Логический</span><span class="sxs-lookup"><span data-stu-id="0346e-325">Boolean</span></span>|<span data-ttu-id="0346e-326">Включите использование атрибутов внутренней подсети.</span><span class="sxs-lookup"><span data-stu-id="0346e-326">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="0346e-327">локалидентифиер</span><span class="sxs-lookup"><span data-stu-id="0346e-327">localIdentifier</span></span>|[<span data-ttu-id="0346e-328">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="0346e-328">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="0346e-329">Метод идентификации клиента, который пытается подключиться через VPN.</span><span class="sxs-lookup"><span data-stu-id="0346e-329">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="0346e-330">.</span><span class="sxs-lookup"><span data-stu-id="0346e-330">.</span></span> <span data-ttu-id="0346e-331">Возможные значения: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="0346e-331">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="0346e-332">ремотеидентифиер</span><span class="sxs-lookup"><span data-stu-id="0346e-332">remoteIdentifier</span></span>|<span data-ttu-id="0346e-333">Строка</span><span class="sxs-lookup"><span data-stu-id="0346e-333">String</span></span>|<span data-ttu-id="0346e-334">Адрес сервера IKEv2.</span><span class="sxs-lookup"><span data-stu-id="0346e-334">Address of the IKEv2 server.</span></span> <span data-ttu-id="0346e-335">Должно быть полным доменным именем, Усерфкдн, сетевым адресом или ASN1DN</span><span class="sxs-lookup"><span data-stu-id="0346e-335">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="0346e-336">секуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="0346e-336">securityAssociationParameters</span></span>|[<span data-ttu-id="0346e-337">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="0346e-337">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="0346e-338">Параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="0346e-338">Security Association Parameters</span></span>|
|<span data-ttu-id="0346e-339">серверцертификатекоммоннаме</span><span class="sxs-lookup"><span data-stu-id="0346e-339">serverCertificateCommonName</span></span>|<span data-ttu-id="0346e-340">Строка</span><span class="sxs-lookup"><span data-stu-id="0346e-340">String</span></span>|<span data-ttu-id="0346e-341">Общее имя сертификата сервера IKEv2, используемого при проверке подлинности сервера</span><span class="sxs-lookup"><span data-stu-id="0346e-341">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="0346e-342">серверцертификатеиссуеркоммоннаме</span><span class="sxs-lookup"><span data-stu-id="0346e-342">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="0346e-343">Строка</span><span class="sxs-lookup"><span data-stu-id="0346e-343">String</span></span>|<span data-ttu-id="0346e-344">Общее имя поставщика сертификата сервера IKEv2, используемого при проверке подлинности</span><span class="sxs-lookup"><span data-stu-id="0346e-344">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="0346e-345">серверцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="0346e-345">serverCertificateType</span></span>|[<span data-ttu-id="0346e-346">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="0346e-346">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="0346e-347">Тип сертификата, который VPN-сервер будет предоставлять VPN-клиенту для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="0346e-347">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="0346e-348">Возможные значения: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="0346e-348">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="0346e-349">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="0346e-349">sharedSecret</span></span>|<span data-ttu-id="0346e-350">Строка</span><span class="sxs-lookup"><span data-stu-id="0346e-350">String</span></span>|<span data-ttu-id="0346e-351">Используется, когда выбрана общая секретная проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="0346e-351">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="0346e-352">тлсмаксимумверсион</span><span class="sxs-lookup"><span data-stu-id="0346e-352">tlsMaximumVersion</span></span>|<span data-ttu-id="0346e-353">Строка</span><span class="sxs-lookup"><span data-stu-id="0346e-353">String</span></span>|<span data-ttu-id="0346e-354">Максимальная версия TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="0346e-354">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="0346e-355">тлсминимумверсион</span><span class="sxs-lookup"><span data-stu-id="0346e-355">tlsMinimumVersion</span></span>|<span data-ttu-id="0346e-356">Строка</span><span class="sxs-lookup"><span data-stu-id="0346e-356">String</span></span>|<span data-ttu-id="0346e-357">Минимальная версия протокола TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="0346e-357">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="0346e-358">алловдефаултсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="0346e-358">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="0346e-359">Логический</span><span class="sxs-lookup"><span data-stu-id="0346e-359">Boolean</span></span>|<span data-ttu-id="0346e-360">Разрешает использование параметров сопоставления безопасности путем установки всех параметров для устройства по умолчанию, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="0346e-360">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="0346e-361">алловдефаултчилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="0346e-361">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="0346e-362">Логический</span><span class="sxs-lookup"><span data-stu-id="0346e-362">Boolean</span></span>|<span data-ttu-id="0346e-363">Разрешает использование параметров дочернего сопоставления безопасности, устанавливая все параметры по умолчанию устройства, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="0346e-363">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="0346e-364">алвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="0346e-364">alwaysOnConfiguration</span></span>|[<span data-ttu-id="0346e-365">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0346e-365">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="0346e-366">Конфигурация AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="0346e-366">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="0346e-367">енаблеалвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="0346e-367">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="0346e-368">Логический</span><span class="sxs-lookup"><span data-stu-id="0346e-368">Boolean</span></span>|<span data-ttu-id="0346e-369">Определяет, включена ли функция "всегда включено" VPN</span><span class="sxs-lookup"><span data-stu-id="0346e-369">Determines if Always on VPN is enabled</span></span>|
|<span data-ttu-id="0346e-370">мтусизеинбитес</span><span class="sxs-lookup"><span data-stu-id="0346e-370">mtuSizeInBytes</span></span>|<span data-ttu-id="0346e-371">Int32</span><span class="sxs-lookup"><span data-stu-id="0346e-371">Int32</span></span>|<span data-ttu-id="0346e-372">Максимальное количество передаваемых данных.</span><span class="sxs-lookup"><span data-stu-id="0346e-372">Maximum transmission unit.</span></span> <span data-ttu-id="0346e-373">Допустимые значения — от 1 до 65536</span><span class="sxs-lookup"><span data-stu-id="0346e-373">Valid values 1 to 65536</span></span>|



## <a name="response"></a><span data-ttu-id="0346e-374">Ответ</span><span class="sxs-lookup"><span data-stu-id="0346e-374">Response</span></span>
<span data-ttu-id="0346e-375">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0346e-375">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0346e-376">Пример</span><span class="sxs-lookup"><span data-stu-id="0346e-376">Example</span></span>

### <a name="request"></a><span data-ttu-id="0346e-377">Запрос</span><span class="sxs-lookup"><span data-stu-id="0346e-377">Request</span></span>
<span data-ttu-id="0346e-378">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0346e-378">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="0346e-379">Отклик</span><span class="sxs-lookup"><span data-stu-id="0346e-379">Response</span></span>
<span data-ttu-id="0346e-p142">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0346e-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





