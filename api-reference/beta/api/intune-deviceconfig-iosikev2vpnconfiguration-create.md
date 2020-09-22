---
title: Создание iosikEv2VpnConfiguration
description: Создание нового объекта iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9fbfe09b286cd02dfcda8089c5b65780f024ef85
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47995298"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="a8327-103">Создание iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8327-103">Create iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="a8327-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8327-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8327-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8327-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8327-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8327-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8327-107">Создание нового объекта [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a8327-107">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8327-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a8327-108">Prerequisites</span></span>
<span data-ttu-id="a8327-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8327-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8327-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8327-111">Permission type</span></span>|<span data-ttu-id="a8327-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8327-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8327-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8327-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8327-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8327-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a8327-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8327-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8327-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8327-116">Not supported.</span></span>|
|<span data-ttu-id="a8327-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8327-117">Application</span></span>|<span data-ttu-id="a8327-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8327-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8327-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8327-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a8327-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a8327-120">Request headers</span></span>
|<span data-ttu-id="a8327-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8327-121">Header</span></span>|<span data-ttu-id="a8327-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a8327-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8327-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8327-123">Authorization</span></span>|<span data-ttu-id="a8327-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8327-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8327-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a8327-125">Accept</span></span>|<span data-ttu-id="a8327-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8327-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8327-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a8327-127">Request body</span></span>
<span data-ttu-id="a8327-128">В тексте запроса добавьте представление объекта iosikEv2VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8327-128">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="a8327-129">В следующей таблице приведены свойства, необходимые при создании iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a8327-129">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="a8327-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8327-130">Property</span></span>|<span data-ttu-id="a8327-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a8327-131">Type</span></span>|<span data-ttu-id="a8327-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a8327-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8327-133">id</span><span class="sxs-lookup"><span data-stu-id="a8327-133">id</span></span>|<span data-ttu-id="a8327-134">String</span><span class="sxs-lookup"><span data-stu-id="a8327-134">String</span></span>|<span data-ttu-id="a8327-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a8327-135">Key of the entity.</span></span> <span data-ttu-id="a8327-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8327-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8327-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a8327-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8327-138">DateTimeOffset</span></span>|<span data-ttu-id="a8327-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a8327-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a8327-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8327-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a8327-141">roleScopeTagIds</span></span>|<span data-ttu-id="a8327-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a8327-142">String collection</span></span>|<span data-ttu-id="a8327-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a8327-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a8327-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8327-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a8327-145">supportsScopeTags</span></span>|<span data-ttu-id="a8327-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8327-146">Boolean</span></span>|<span data-ttu-id="a8327-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a8327-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a8327-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a8327-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a8327-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a8327-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a8327-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8327-150">This property is read-only.</span></span> <span data-ttu-id="a8327-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8327-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a8327-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a8327-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a8327-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a8327-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a8327-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a8327-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8327-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a8327-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a8327-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a8327-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a8327-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a8327-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a8327-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8327-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a8327-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a8327-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a8327-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a8327-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a8327-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a8327-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8327-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8327-164">createdDateTime</span></span>|<span data-ttu-id="a8327-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8327-165">DateTimeOffset</span></span>|<span data-ttu-id="a8327-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a8327-166">DateTime the object was created.</span></span> <span data-ttu-id="a8327-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8327-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-168">description</span><span class="sxs-lookup"><span data-stu-id="a8327-168">description</span></span>|<span data-ttu-id="a8327-169">String</span><span class="sxs-lookup"><span data-stu-id="a8327-169">String</span></span>|<span data-ttu-id="a8327-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a8327-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a8327-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8327-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a8327-172">displayName</span></span>|<span data-ttu-id="a8327-173">String</span><span class="sxs-lookup"><span data-stu-id="a8327-173">String</span></span>|<span data-ttu-id="a8327-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a8327-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a8327-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8327-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-176">version</span><span class="sxs-lookup"><span data-stu-id="a8327-176">version</span></span>|<span data-ttu-id="a8327-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a8327-177">Int32</span></span>|<span data-ttu-id="a8327-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a8327-178">Version of the device configuration.</span></span> <span data-ttu-id="a8327-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8327-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="a8327-180">connectionName</span></span>|<span data-ttu-id="a8327-181">String</span><span class="sxs-lookup"><span data-stu-id="a8327-181">String</span></span>|<span data-ttu-id="a8327-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a8327-182">Connection name displayed to the user.</span></span> <span data-ttu-id="a8327-183">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="a8327-184">connectionType</span></span>|[<span data-ttu-id="a8327-185">апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="a8327-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="a8327-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="a8327-186">Connection type.</span></span> <span data-ttu-id="a8327-187">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8327-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="a8327-188">Возможные значения:,,,,,,,,,, `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` ,, `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` , `paloAltoGlobalProtectV2` , `ikEv2` , `alwaysOn` `microsoftTunnel` `netMotionMobility` ,,.</span><span class="sxs-lookup"><span data-stu-id="a8327-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="a8327-189">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="a8327-189">loginGroupOrDomain</span></span>|<span data-ttu-id="a8327-190">String</span><span class="sxs-lookup"><span data-stu-id="a8327-190">String</span></span>|<span data-ttu-id="a8327-191">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="a8327-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="a8327-192">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-193">role</span><span class="sxs-lookup"><span data-stu-id="a8327-193">role</span></span>|<span data-ttu-id="a8327-194">String</span><span class="sxs-lookup"><span data-stu-id="a8327-194">String</span></span>|<span data-ttu-id="a8327-195">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="a8327-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="a8327-196">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-197">область</span><span class="sxs-lookup"><span data-stu-id="a8327-197">realm</span></span>|<span data-ttu-id="a8327-198">String</span><span class="sxs-lookup"><span data-stu-id="a8327-198">String</span></span>|<span data-ttu-id="a8327-199">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="a8327-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="a8327-200">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-201">сервер</span><span class="sxs-lookup"><span data-stu-id="a8327-201">server</span></span>|[<span data-ttu-id="a8327-202">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="a8327-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="a8327-203">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="a8327-203">VPN Server on the network.</span></span> <span data-ttu-id="a8327-204">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="a8327-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="a8327-205">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="a8327-206">identifier</span></span>|<span data-ttu-id="a8327-207">String</span><span class="sxs-lookup"><span data-stu-id="a8327-207">String</span></span>|<span data-ttu-id="a8327-208">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="a8327-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="a8327-209">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-210">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="a8327-210">customData</span></span>|<span data-ttu-id="a8327-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="a8327-212">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="a8327-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="a8327-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="a8327-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="a8327-214">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="a8327-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="a8327-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="a8327-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="a8327-216">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="a8327-217">customKeyValueData</span></span>|<span data-ttu-id="a8327-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a8327-219">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="a8327-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="a8327-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="a8327-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="a8327-221">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="a8327-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="a8327-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="a8327-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="a8327-223">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-224">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="a8327-224">enableSplitTunneling</span></span>|<span data-ttu-id="a8327-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8327-225">Boolean</span></span>|<span data-ttu-id="a8327-226">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="a8327-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="a8327-227">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-228">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="a8327-228">authenticationMethod</span></span>|[<span data-ttu-id="a8327-229">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="a8327-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="a8327-230">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="a8327-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="a8327-231">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8327-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="a8327-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="a8327-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="a8327-233">енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="a8327-233">enablePerApp</span></span>|<span data-ttu-id="a8327-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8327-234">Boolean</span></span>|<span data-ttu-id="a8327-235">Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="a8327-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="a8327-236">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-237">сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="a8327-237">safariDomains</span></span>|<span data-ttu-id="a8327-238">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a8327-238">String collection</span></span>|<span data-ttu-id="a8327-239">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="a8327-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="a8327-240">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="a8327-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="a8327-241">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-242">ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="a8327-242">onDemandRules</span></span>|<span data-ttu-id="a8327-243">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="a8327-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="a8327-244">On-Demand Rules.</span></span> <span data-ttu-id="a8327-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a8327-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a8327-246">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-247">providerType</span><span class="sxs-lookup"><span data-stu-id="a8327-247">providerType</span></span>|[<span data-ttu-id="a8327-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="a8327-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="a8327-249">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="a8327-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="a8327-250">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a8327-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="a8327-251">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="a8327-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="a8327-252">ексклудеддомаинс</span><span class="sxs-lookup"><span data-stu-id="a8327-252">excludedDomains</span></span>|<span data-ttu-id="a8327-253">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a8327-253">String collection</span></span>|<span data-ttu-id="a8327-254">Домены, доступ к которым осуществляется через общедоступный Интернет, а не через VPN, даже если VPN для каждого приложения активируется наследуемой от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-254">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-255">дисаблеондемандусероверриде</span><span class="sxs-lookup"><span data-stu-id="a8327-255">disableOnDemandUserOverride</span></span>|<span data-ttu-id="a8327-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8327-256">Boolean</span></span>|<span data-ttu-id="a8327-257">Переключатель, чтобы запретить пользователям отключать автоматическое VPN в приложении "Параметры", унаследованном от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-257">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-258">проксисервер</span><span class="sxs-lookup"><span data-stu-id="a8327-258">proxyServer</span></span>|[<span data-ttu-id="a8327-259">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="a8327-259">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="a8327-260">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="a8327-260">Proxy Server.</span></span> <span data-ttu-id="a8327-261">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-261">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-262">оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="a8327-262">optInToDeviceIdSharing</span></span>|<span data-ttu-id="a8327-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8327-263">Boolean</span></span>|<span data-ttu-id="a8327-264">Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="a8327-264">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="a8327-265">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-265">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-266">userDomain</span><span class="sxs-lookup"><span data-stu-id="a8327-266">userDomain</span></span>|<span data-ttu-id="a8327-267">String</span><span class="sxs-lookup"><span data-stu-id="a8327-267">String</span></span>|<span data-ttu-id="a8327-268">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="a8327-268">Zscaler only.</span></span> <span data-ttu-id="a8327-269">Введите статический домен для предварительного заполнения поля Login в приложении Зскалер.</span><span class="sxs-lookup"><span data-stu-id="a8327-269">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="a8327-270">Если оставить это поле пустым, вместо этого будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="a8327-270">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="a8327-271">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-272">стриктенфорцемент</span><span class="sxs-lookup"><span data-stu-id="a8327-272">strictEnforcement</span></span>|<span data-ttu-id="a8327-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8327-273">Boolean</span></span>|<span data-ttu-id="a8327-274">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="a8327-274">Zscaler only.</span></span> <span data-ttu-id="a8327-275">Блокирует сетевой трафик до тех пор, пока пользователь не войдет в приложение Зскалер.</span><span class="sxs-lookup"><span data-stu-id="a8327-275">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="a8327-276">"True" означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="a8327-276">"True" means traffic is blocked.</span></span> <span data-ttu-id="a8327-277">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-277">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-278">клауднаме</span><span class="sxs-lookup"><span data-stu-id="a8327-278">cloudName</span></span>|<span data-ttu-id="a8327-279">String</span><span class="sxs-lookup"><span data-stu-id="a8327-279">String</span></span>|<span data-ttu-id="a8327-280">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="a8327-280">Zscaler only.</span></span> <span data-ttu-id="a8327-281">Облако зскалер, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="a8327-281">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="a8327-282">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-282">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-283">excludeList</span><span class="sxs-lookup"><span data-stu-id="a8327-283">excludeList</span></span>|<span data-ttu-id="a8327-284">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a8327-284">String collection</span></span>|<span data-ttu-id="a8327-285">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="a8327-285">Zscaler only.</span></span> <span data-ttu-id="a8327-286">Список сетевых адресов, которые не отправляются через облако Зскалер.</span><span class="sxs-lookup"><span data-stu-id="a8327-286">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="a8327-287">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-287">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-288">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="a8327-288">targetedMobileApps</span></span>|<span data-ttu-id="a8327-289">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-289">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="a8327-290">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="a8327-290">Targeted mobile apps.</span></span> <span data-ttu-id="a8327-291">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a8327-291">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a8327-292">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-292">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-293">микрософттуннелситеид</span><span class="sxs-lookup"><span data-stu-id="a8327-293">microsoftTunnelSiteId</span></span>|<span data-ttu-id="a8327-294">String</span><span class="sxs-lookup"><span data-stu-id="a8327-294">String</span></span>|<span data-ttu-id="a8327-295">Идентификатор сайта туннеля (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="a8327-295">Microsoft Tunnel site ID.</span></span> <span data-ttu-id="a8327-296">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8327-296">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a8327-297">чилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="a8327-297">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="a8327-298">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="a8327-298">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="a8327-299">Дочерние параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="a8327-299">Child Security Association Parameters</span></span>|
|<span data-ttu-id="a8327-300">клиентаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="a8327-300">clientAuthenticationType</span></span>|[<span data-ttu-id="a8327-301">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="a8327-301">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="a8327-302">Тип проверки подлинности клиента, который будет использоваться VPN-клиентом.</span><span class="sxs-lookup"><span data-stu-id="a8327-302">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="a8327-303">Возможные значения: `userAuthentication`, `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="a8327-303">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="a8327-304">деадпирдетектионрате</span><span class="sxs-lookup"><span data-stu-id="a8327-304">deadPeerDetectionRate</span></span>|[<span data-ttu-id="a8327-305">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="a8327-305">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="a8327-306">Определите, как часто следует проверять, активен ли одноранговый сеанс.</span><span class="sxs-lookup"><span data-stu-id="a8327-306">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="a8327-307">.</span><span class="sxs-lookup"><span data-stu-id="a8327-307">.</span></span> <span data-ttu-id="a8327-308">Возможные значения: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="a8327-308">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="a8327-309">дисаблемобилитяндмултихоминг</span><span class="sxs-lookup"><span data-stu-id="a8327-309">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="a8327-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8327-310">Boolean</span></span>|<span data-ttu-id="a8327-311">Отключение МОБИКЕ</span><span class="sxs-lookup"><span data-stu-id="a8327-311">Disable MOBIKE</span></span>|
|<span data-ttu-id="a8327-312">дисаблередирект</span><span class="sxs-lookup"><span data-stu-id="a8327-312">disableRedirect</span></span>|<span data-ttu-id="a8327-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8327-313">Boolean</span></span>|<span data-ttu-id="a8327-314">Отключение перенаправления</span><span class="sxs-lookup"><span data-stu-id="a8327-314">Disable Redirect</span></span>|
|<span data-ttu-id="a8327-315">енаблецертификатеревокатиончекк</span><span class="sxs-lookup"><span data-stu-id="a8327-315">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="a8327-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8327-316">Boolean</span></span>|<span data-ttu-id="a8327-317">Включает проверку отзывов и действий. время ожидания отклика сервера не приведет к сбою</span><span class="sxs-lookup"><span data-stu-id="a8327-317">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="a8327-318">енаблиап</span><span class="sxs-lookup"><span data-stu-id="a8327-318">enableEAP</span></span>|<span data-ttu-id="a8327-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8327-319">Boolean</span></span>|<span data-ttu-id="a8327-320">Включает проверку подлинности только EAP</span><span class="sxs-lookup"><span data-stu-id="a8327-320">Enables EAP only authentication</span></span>|
|<span data-ttu-id="a8327-321">енаблеперфектфорвардсекреци</span><span class="sxs-lookup"><span data-stu-id="a8327-321">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="a8327-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8327-322">Boolean</span></span>|<span data-ttu-id="a8327-323">Включить безопасную пересылку (PFS).</span><span class="sxs-lookup"><span data-stu-id="a8327-323">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="a8327-324">енаблеусеинтерналсубнетаттрибутес</span><span class="sxs-lookup"><span data-stu-id="a8327-324">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="a8327-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8327-325">Boolean</span></span>|<span data-ttu-id="a8327-326">Включите использование атрибутов внутренней подсети.</span><span class="sxs-lookup"><span data-stu-id="a8327-326">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="a8327-327">локалидентифиер</span><span class="sxs-lookup"><span data-stu-id="a8327-327">localIdentifier</span></span>|[<span data-ttu-id="a8327-328">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="a8327-328">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="a8327-329">Метод идентификации клиента, который пытается подключиться через VPN.</span><span class="sxs-lookup"><span data-stu-id="a8327-329">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="a8327-330">.</span><span class="sxs-lookup"><span data-stu-id="a8327-330">.</span></span> <span data-ttu-id="a8327-331">Возможные значения: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="a8327-331">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="a8327-332">ремотеидентифиер</span><span class="sxs-lookup"><span data-stu-id="a8327-332">remoteIdentifier</span></span>|<span data-ttu-id="a8327-333">String</span><span class="sxs-lookup"><span data-stu-id="a8327-333">String</span></span>|<span data-ttu-id="a8327-334">Адрес сервера IKEv2.</span><span class="sxs-lookup"><span data-stu-id="a8327-334">Address of the IKEv2 server.</span></span> <span data-ttu-id="a8327-335">Должно быть полным доменным именем, Усерфкдн, сетевым адресом или ASN1DN</span><span class="sxs-lookup"><span data-stu-id="a8327-335">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="a8327-336">секуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="a8327-336">securityAssociationParameters</span></span>|[<span data-ttu-id="a8327-337">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="a8327-337">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="a8327-338">Параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="a8327-338">Security Association Parameters</span></span>|
|<span data-ttu-id="a8327-339">серверцертификатекоммоннаме</span><span class="sxs-lookup"><span data-stu-id="a8327-339">serverCertificateCommonName</span></span>|<span data-ttu-id="a8327-340">String</span><span class="sxs-lookup"><span data-stu-id="a8327-340">String</span></span>|<span data-ttu-id="a8327-341">Общее имя сертификата сервера IKEv2, используемого при проверке подлинности сервера</span><span class="sxs-lookup"><span data-stu-id="a8327-341">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="a8327-342">серверцертификатеиссуеркоммоннаме</span><span class="sxs-lookup"><span data-stu-id="a8327-342">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="a8327-343">String</span><span class="sxs-lookup"><span data-stu-id="a8327-343">String</span></span>|<span data-ttu-id="a8327-344">Общее имя поставщика сертификата сервера IKEv2, используемого при проверке подлинности</span><span class="sxs-lookup"><span data-stu-id="a8327-344">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="a8327-345">серверцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="a8327-345">serverCertificateType</span></span>|[<span data-ttu-id="a8327-346">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="a8327-346">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="a8327-347">Тип сертификата, который VPN-сервер будет предоставлять VPN-клиенту для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="a8327-347">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="a8327-348">Возможные значения: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="a8327-348">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="a8327-349">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="a8327-349">sharedSecret</span></span>|<span data-ttu-id="a8327-350">String</span><span class="sxs-lookup"><span data-stu-id="a8327-350">String</span></span>|<span data-ttu-id="a8327-351">Используется, когда выбрана общая секретная проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="a8327-351">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="a8327-352">тлсмаксимумверсион</span><span class="sxs-lookup"><span data-stu-id="a8327-352">tlsMaximumVersion</span></span>|<span data-ttu-id="a8327-353">String</span><span class="sxs-lookup"><span data-stu-id="a8327-353">String</span></span>|<span data-ttu-id="a8327-354">Максимальная версия TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="a8327-354">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="a8327-355">тлсминимумверсион</span><span class="sxs-lookup"><span data-stu-id="a8327-355">tlsMinimumVersion</span></span>|<span data-ttu-id="a8327-356">String</span><span class="sxs-lookup"><span data-stu-id="a8327-356">String</span></span>|<span data-ttu-id="a8327-357">Минимальная версия протокола TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="a8327-357">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="a8327-358">алловдефаултсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="a8327-358">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="a8327-359">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8327-359">Boolean</span></span>|<span data-ttu-id="a8327-360">Разрешает использование параметров сопоставления безопасности путем установки всех параметров для устройства по умолчанию, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="a8327-360">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="a8327-361">алловдефаултчилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="a8327-361">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="a8327-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8327-362">Boolean</span></span>|<span data-ttu-id="a8327-363">Разрешает использование параметров дочернего сопоставления безопасности, устанавливая все параметры по умолчанию устройства, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="a8327-363">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="a8327-364">алвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="a8327-364">alwaysOnConfiguration</span></span>|[<span data-ttu-id="a8327-365">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8327-365">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="a8327-366">Конфигурация AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="a8327-366">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="a8327-367">енаблеалвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="a8327-367">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="a8327-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8327-368">Boolean</span></span>|<span data-ttu-id="a8327-369">Определяет, включена ли функция "всегда включено" VPN</span><span class="sxs-lookup"><span data-stu-id="a8327-369">Determines if Always on VPN is enabled</span></span>|
|<span data-ttu-id="a8327-370">мтусизеинбитес</span><span class="sxs-lookup"><span data-stu-id="a8327-370">mtuSizeInBytes</span></span>|<span data-ttu-id="a8327-371">Int32</span><span class="sxs-lookup"><span data-stu-id="a8327-371">Int32</span></span>|<span data-ttu-id="a8327-372">Максимальное количество передаваемых данных.</span><span class="sxs-lookup"><span data-stu-id="a8327-372">Maximum transmission unit.</span></span> <span data-ttu-id="a8327-373">Допустимые значения — от 1 до 65536</span><span class="sxs-lookup"><span data-stu-id="a8327-373">Valid values 1 to 65536</span></span>|



## <a name="response"></a><span data-ttu-id="a8327-374">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8327-374">Response</span></span>
<span data-ttu-id="a8327-375">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a8327-375">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8327-376">Пример</span><span class="sxs-lookup"><span data-stu-id="a8327-376">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8327-377">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8327-377">Request</span></span>
<span data-ttu-id="a8327-378">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8327-378">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a8327-379">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8327-379">Response</span></span>
<span data-ttu-id="a8327-p142">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8327-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






