---
title: Создание iosikEv2VpnConfiguration
description: Создание нового объекта iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b80b625c96ef25ca060f4a5225b91dc553158d1c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49220737"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="243b6-103">Создание iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="243b6-103">Create iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="243b6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="243b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="243b6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="243b6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="243b6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="243b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="243b6-107">Создание нового объекта [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="243b6-107">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="243b6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="243b6-108">Prerequisites</span></span>
<span data-ttu-id="243b6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="243b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="243b6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="243b6-111">Permission type</span></span>|<span data-ttu-id="243b6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="243b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="243b6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="243b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="243b6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="243b6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="243b6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="243b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="243b6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="243b6-116">Not supported.</span></span>|
|<span data-ttu-id="243b6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="243b6-117">Application</span></span>|<span data-ttu-id="243b6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="243b6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="243b6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="243b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="243b6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="243b6-120">Request headers</span></span>
|<span data-ttu-id="243b6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="243b6-121">Header</span></span>|<span data-ttu-id="243b6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="243b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="243b6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="243b6-123">Authorization</span></span>|<span data-ttu-id="243b6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="243b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="243b6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="243b6-125">Accept</span></span>|<span data-ttu-id="243b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="243b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="243b6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="243b6-127">Request body</span></span>
<span data-ttu-id="243b6-128">В тексте запроса добавьте представление объекта iosikEv2VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="243b6-128">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="243b6-129">В следующей таблице приведены свойства, необходимые при создании iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="243b6-129">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="243b6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="243b6-130">Property</span></span>|<span data-ttu-id="243b6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="243b6-131">Type</span></span>|<span data-ttu-id="243b6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="243b6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="243b6-133">id</span><span class="sxs-lookup"><span data-stu-id="243b6-133">id</span></span>|<span data-ttu-id="243b6-134">String</span><span class="sxs-lookup"><span data-stu-id="243b6-134">String</span></span>|<span data-ttu-id="243b6-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="243b6-135">Key of the entity.</span></span> <span data-ttu-id="243b6-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="243b6-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="243b6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="243b6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="243b6-138">DateTimeOffset</span></span>|<span data-ttu-id="243b6-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="243b6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="243b6-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="243b6-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="243b6-141">roleScopeTagIds</span></span>|<span data-ttu-id="243b6-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="243b6-142">String collection</span></span>|<span data-ttu-id="243b6-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="243b6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="243b6-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="243b6-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="243b6-145">supportsScopeTags</span></span>|<span data-ttu-id="243b6-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="243b6-146">Boolean</span></span>|<span data-ttu-id="243b6-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="243b6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="243b6-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="243b6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="243b6-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="243b6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="243b6-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="243b6-150">This property is read-only.</span></span> <span data-ttu-id="243b6-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="243b6-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="243b6-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="243b6-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="243b6-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="243b6-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="243b6-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="243b6-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="243b6-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="243b6-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="243b6-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="243b6-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="243b6-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="243b6-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="243b6-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="243b6-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="243b6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="243b6-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="243b6-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="243b6-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="243b6-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="243b6-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="243b6-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="243b6-164">createdDateTime</span></span>|<span data-ttu-id="243b6-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="243b6-165">DateTimeOffset</span></span>|<span data-ttu-id="243b6-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="243b6-166">DateTime the object was created.</span></span> <span data-ttu-id="243b6-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="243b6-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-168">description</span><span class="sxs-lookup"><span data-stu-id="243b6-168">description</span></span>|<span data-ttu-id="243b6-169">String</span><span class="sxs-lookup"><span data-stu-id="243b6-169">String</span></span>|<span data-ttu-id="243b6-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="243b6-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="243b6-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="243b6-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-172">displayName</span><span class="sxs-lookup"><span data-stu-id="243b6-172">displayName</span></span>|<span data-ttu-id="243b6-173">String</span><span class="sxs-lookup"><span data-stu-id="243b6-173">String</span></span>|<span data-ttu-id="243b6-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="243b6-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="243b6-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="243b6-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-176">version</span><span class="sxs-lookup"><span data-stu-id="243b6-176">version</span></span>|<span data-ttu-id="243b6-177">Int32</span><span class="sxs-lookup"><span data-stu-id="243b6-177">Int32</span></span>|<span data-ttu-id="243b6-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="243b6-178">Version of the device configuration.</span></span> <span data-ttu-id="243b6-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="243b6-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="243b6-180">connectionName</span></span>|<span data-ttu-id="243b6-181">String</span><span class="sxs-lookup"><span data-stu-id="243b6-181">String</span></span>|<span data-ttu-id="243b6-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="243b6-182">Connection name displayed to the user.</span></span> <span data-ttu-id="243b6-183">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="243b6-184">connectionType</span></span>|[<span data-ttu-id="243b6-185">апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="243b6-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="243b6-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="243b6-186">Connection type.</span></span> <span data-ttu-id="243b6-187">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="243b6-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="243b6-188">Возможные значения:,,,,,,,,,, `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` ,, `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` , `paloAltoGlobalProtectV2` , `ikEv2` , `alwaysOn` `microsoftTunnel` `netMotionMobility` ,,.</span><span class="sxs-lookup"><span data-stu-id="243b6-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="243b6-189">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="243b6-189">loginGroupOrDomain</span></span>|<span data-ttu-id="243b6-190">String</span><span class="sxs-lookup"><span data-stu-id="243b6-190">String</span></span>|<span data-ttu-id="243b6-191">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="243b6-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="243b6-192">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-193">role</span><span class="sxs-lookup"><span data-stu-id="243b6-193">role</span></span>|<span data-ttu-id="243b6-194">String</span><span class="sxs-lookup"><span data-stu-id="243b6-194">String</span></span>|<span data-ttu-id="243b6-195">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="243b6-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="243b6-196">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-197">область</span><span class="sxs-lookup"><span data-stu-id="243b6-197">realm</span></span>|<span data-ttu-id="243b6-198">String</span><span class="sxs-lookup"><span data-stu-id="243b6-198">String</span></span>|<span data-ttu-id="243b6-199">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="243b6-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="243b6-200">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-201">сервер</span><span class="sxs-lookup"><span data-stu-id="243b6-201">server</span></span>|[<span data-ttu-id="243b6-202">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="243b6-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="243b6-203">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="243b6-203">VPN Server on the network.</span></span> <span data-ttu-id="243b6-204">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="243b6-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="243b6-205">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="243b6-206">identifier</span></span>|<span data-ttu-id="243b6-207">String</span><span class="sxs-lookup"><span data-stu-id="243b6-207">String</span></span>|<span data-ttu-id="243b6-208">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="243b6-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="243b6-209">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-210">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="243b6-210">customData</span></span>|<span data-ttu-id="243b6-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="243b6-212">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="243b6-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="243b6-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="243b6-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="243b6-214">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="243b6-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="243b6-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="243b6-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="243b6-216">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="243b6-217">customKeyValueData</span></span>|<span data-ttu-id="243b6-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="243b6-219">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="243b6-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="243b6-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="243b6-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="243b6-221">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="243b6-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="243b6-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="243b6-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="243b6-223">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-224">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="243b6-224">enableSplitTunneling</span></span>|<span data-ttu-id="243b6-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="243b6-225">Boolean</span></span>|<span data-ttu-id="243b6-226">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="243b6-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="243b6-227">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-228">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="243b6-228">authenticationMethod</span></span>|[<span data-ttu-id="243b6-229">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="243b6-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="243b6-230">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="243b6-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="243b6-231">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="243b6-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="243b6-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="243b6-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="243b6-233">енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="243b6-233">enablePerApp</span></span>|<span data-ttu-id="243b6-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="243b6-234">Boolean</span></span>|<span data-ttu-id="243b6-235">Если задать для этого параметра значение true, будут созданы Per-App полезные данные VPN, которые позже могут быть связаны с приложениями, которые могут запускать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="243b6-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="243b6-236">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-237">сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="243b6-237">safariDomains</span></span>|<span data-ttu-id="243b6-238">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="243b6-238">String collection</span></span>|<span data-ttu-id="243b6-239">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="243b6-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="243b6-240">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="243b6-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="243b6-241">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-242">ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="243b6-242">onDemandRules</span></span>|<span data-ttu-id="243b6-243">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="243b6-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="243b6-244">On-Demand Rules.</span></span> <span data-ttu-id="243b6-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="243b6-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="243b6-246">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-247">providerType</span><span class="sxs-lookup"><span data-stu-id="243b6-247">providerType</span></span>|[<span data-ttu-id="243b6-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="243b6-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="243b6-249">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="243b6-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="243b6-250">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="243b6-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="243b6-251">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="243b6-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="243b6-252">ексклудеддомаинс</span><span class="sxs-lookup"><span data-stu-id="243b6-252">excludedDomains</span></span>|<span data-ttu-id="243b6-253">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="243b6-253">String collection</span></span>|<span data-ttu-id="243b6-254">Домены, доступ к которым осуществляется через общедоступный Интернет, а не через VPN, даже если VPN для каждого приложения активируется наследуемой от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-254">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-255">дисаблеондемандусероверриде</span><span class="sxs-lookup"><span data-stu-id="243b6-255">disableOnDemandUserOverride</span></span>|<span data-ttu-id="243b6-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="243b6-256">Boolean</span></span>|<span data-ttu-id="243b6-257">Переключатель, чтобы запретить пользователям отключать автоматическое VPN в приложении "Параметры", унаследованном от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-257">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-258">проксисервер</span><span class="sxs-lookup"><span data-stu-id="243b6-258">proxyServer</span></span>|[<span data-ttu-id="243b6-259">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="243b6-259">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="243b6-260">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="243b6-260">Proxy Server.</span></span> <span data-ttu-id="243b6-261">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-261">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-262">оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="243b6-262">optInToDeviceIdSharing</span></span>|<span data-ttu-id="243b6-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="243b6-263">Boolean</span></span>|<span data-ttu-id="243b6-264">Opt-In для предоставления доступа к идентификатору устройства сторонним VPN-клиентам для использования в процессе проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="243b6-264">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="243b6-265">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-265">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-266">userDomain</span><span class="sxs-lookup"><span data-stu-id="243b6-266">userDomain</span></span>|<span data-ttu-id="243b6-267">String</span><span class="sxs-lookup"><span data-stu-id="243b6-267">String</span></span>|<span data-ttu-id="243b6-268">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="243b6-268">Zscaler only.</span></span> <span data-ttu-id="243b6-269">Введите статический домен для предварительного заполнения поля Login в приложении Зскалер.</span><span class="sxs-lookup"><span data-stu-id="243b6-269">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="243b6-270">Если оставить это поле пустым, вместо этого будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="243b6-270">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="243b6-271">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-272">стриктенфорцемент</span><span class="sxs-lookup"><span data-stu-id="243b6-272">strictEnforcement</span></span>|<span data-ttu-id="243b6-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="243b6-273">Boolean</span></span>|<span data-ttu-id="243b6-274">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="243b6-274">Zscaler only.</span></span> <span data-ttu-id="243b6-275">Блокирует сетевой трафик до тех пор, пока пользователь не войдет в приложение Зскалер.</span><span class="sxs-lookup"><span data-stu-id="243b6-275">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="243b6-276">"True" означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="243b6-276">"True" means traffic is blocked.</span></span> <span data-ttu-id="243b6-277">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-277">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-278">клауднаме</span><span class="sxs-lookup"><span data-stu-id="243b6-278">cloudName</span></span>|<span data-ttu-id="243b6-279">String</span><span class="sxs-lookup"><span data-stu-id="243b6-279">String</span></span>|<span data-ttu-id="243b6-280">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="243b6-280">Zscaler only.</span></span> <span data-ttu-id="243b6-281">Облако зскалер, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="243b6-281">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="243b6-282">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-282">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-283">excludeList</span><span class="sxs-lookup"><span data-stu-id="243b6-283">excludeList</span></span>|<span data-ttu-id="243b6-284">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="243b6-284">String collection</span></span>|<span data-ttu-id="243b6-285">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="243b6-285">Zscaler only.</span></span> <span data-ttu-id="243b6-286">Список сетевых адресов, которые не отправляются через облако Зскалер.</span><span class="sxs-lookup"><span data-stu-id="243b6-286">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="243b6-287">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-287">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-288">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="243b6-288">targetedMobileApps</span></span>|<span data-ttu-id="243b6-289">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-289">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="243b6-290">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="243b6-290">Targeted mobile apps.</span></span> <span data-ttu-id="243b6-291">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="243b6-291">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="243b6-292">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-292">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-293">микрософттуннелситеид</span><span class="sxs-lookup"><span data-stu-id="243b6-293">microsoftTunnelSiteId</span></span>|<span data-ttu-id="243b6-294">String</span><span class="sxs-lookup"><span data-stu-id="243b6-294">String</span></span>|<span data-ttu-id="243b6-295">Идентификатор сайта туннеля (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="243b6-295">Microsoft Tunnel site ID.</span></span> <span data-ttu-id="243b6-296">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="243b6-296">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="243b6-297">чилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="243b6-297">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="243b6-298">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="243b6-298">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="243b6-299">Дочерние параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="243b6-299">Child Security Association Parameters</span></span>|
|<span data-ttu-id="243b6-300">клиентаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="243b6-300">clientAuthenticationType</span></span>|[<span data-ttu-id="243b6-301">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="243b6-301">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="243b6-302">Тип проверки подлинности клиента, который будет использоваться VPN-клиентом.</span><span class="sxs-lookup"><span data-stu-id="243b6-302">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="243b6-303">Возможные значения: `userAuthentication`, `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="243b6-303">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="243b6-304">деадпирдетектионрате</span><span class="sxs-lookup"><span data-stu-id="243b6-304">deadPeerDetectionRate</span></span>|[<span data-ttu-id="243b6-305">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="243b6-305">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="243b6-306">Определите, как часто следует проверять, активен ли одноранговый сеанс.</span><span class="sxs-lookup"><span data-stu-id="243b6-306">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="243b6-307">.</span><span class="sxs-lookup"><span data-stu-id="243b6-307">.</span></span> <span data-ttu-id="243b6-308">Возможные значения: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="243b6-308">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="243b6-309">дисаблемобилитяндмултихоминг</span><span class="sxs-lookup"><span data-stu-id="243b6-309">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="243b6-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="243b6-310">Boolean</span></span>|<span data-ttu-id="243b6-311">Отключение МОБИКЕ</span><span class="sxs-lookup"><span data-stu-id="243b6-311">Disable MOBIKE</span></span>|
|<span data-ttu-id="243b6-312">дисаблередирект</span><span class="sxs-lookup"><span data-stu-id="243b6-312">disableRedirect</span></span>|<span data-ttu-id="243b6-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="243b6-313">Boolean</span></span>|<span data-ttu-id="243b6-314">Отключение перенаправления</span><span class="sxs-lookup"><span data-stu-id="243b6-314">Disable Redirect</span></span>|
|<span data-ttu-id="243b6-315">енаблецертификатеревокатиончекк</span><span class="sxs-lookup"><span data-stu-id="243b6-315">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="243b6-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="243b6-316">Boolean</span></span>|<span data-ttu-id="243b6-317">Включает проверку отзывов и действий. время ожидания отклика сервера не приведет к сбою</span><span class="sxs-lookup"><span data-stu-id="243b6-317">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="243b6-318">енаблиап</span><span class="sxs-lookup"><span data-stu-id="243b6-318">enableEAP</span></span>|<span data-ttu-id="243b6-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="243b6-319">Boolean</span></span>|<span data-ttu-id="243b6-320">Включает проверку подлинности только EAP</span><span class="sxs-lookup"><span data-stu-id="243b6-320">Enables EAP only authentication</span></span>|
|<span data-ttu-id="243b6-321">енаблеперфектфорвардсекреци</span><span class="sxs-lookup"><span data-stu-id="243b6-321">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="243b6-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="243b6-322">Boolean</span></span>|<span data-ttu-id="243b6-323">Включить безопасную пересылку (PFS).</span><span class="sxs-lookup"><span data-stu-id="243b6-323">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="243b6-324">енаблеусеинтерналсубнетаттрибутес</span><span class="sxs-lookup"><span data-stu-id="243b6-324">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="243b6-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="243b6-325">Boolean</span></span>|<span data-ttu-id="243b6-326">Включите использование атрибутов внутренней подсети.</span><span class="sxs-lookup"><span data-stu-id="243b6-326">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="243b6-327">локалидентифиер</span><span class="sxs-lookup"><span data-stu-id="243b6-327">localIdentifier</span></span>|[<span data-ttu-id="243b6-328">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="243b6-328">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="243b6-329">Метод идентификации клиента, который пытается подключиться через VPN.</span><span class="sxs-lookup"><span data-stu-id="243b6-329">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="243b6-330">.</span><span class="sxs-lookup"><span data-stu-id="243b6-330">.</span></span> <span data-ttu-id="243b6-331">Возможные значения: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="243b6-331">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="243b6-332">ремотеидентифиер</span><span class="sxs-lookup"><span data-stu-id="243b6-332">remoteIdentifier</span></span>|<span data-ttu-id="243b6-333">String</span><span class="sxs-lookup"><span data-stu-id="243b6-333">String</span></span>|<span data-ttu-id="243b6-334">Адрес сервера IKEv2.</span><span class="sxs-lookup"><span data-stu-id="243b6-334">Address of the IKEv2 server.</span></span> <span data-ttu-id="243b6-335">Должно быть полным доменным именем, Усерфкдн, сетевым адресом или ASN1DN</span><span class="sxs-lookup"><span data-stu-id="243b6-335">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="243b6-336">секуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="243b6-336">securityAssociationParameters</span></span>|[<span data-ttu-id="243b6-337">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="243b6-337">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="243b6-338">Параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="243b6-338">Security Association Parameters</span></span>|
|<span data-ttu-id="243b6-339">серверцертификатекоммоннаме</span><span class="sxs-lookup"><span data-stu-id="243b6-339">serverCertificateCommonName</span></span>|<span data-ttu-id="243b6-340">String</span><span class="sxs-lookup"><span data-stu-id="243b6-340">String</span></span>|<span data-ttu-id="243b6-341">Общее имя сертификата сервера IKEv2, используемого при проверке подлинности сервера</span><span class="sxs-lookup"><span data-stu-id="243b6-341">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="243b6-342">серверцертификатеиссуеркоммоннаме</span><span class="sxs-lookup"><span data-stu-id="243b6-342">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="243b6-343">String</span><span class="sxs-lookup"><span data-stu-id="243b6-343">String</span></span>|<span data-ttu-id="243b6-344">Общее имя поставщика сертификата сервера IKEv2, используемого при проверке подлинности</span><span class="sxs-lookup"><span data-stu-id="243b6-344">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="243b6-345">серверцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="243b6-345">serverCertificateType</span></span>|[<span data-ttu-id="243b6-346">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="243b6-346">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="243b6-347">Тип сертификата, который VPN-сервер будет предоставлять VPN-клиенту для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="243b6-347">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="243b6-348">Возможные значения: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="243b6-348">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="243b6-349">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="243b6-349">sharedSecret</span></span>|<span data-ttu-id="243b6-350">String</span><span class="sxs-lookup"><span data-stu-id="243b6-350">String</span></span>|<span data-ttu-id="243b6-351">Используется, когда выбрана общая секретная проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="243b6-351">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="243b6-352">тлсмаксимумверсион</span><span class="sxs-lookup"><span data-stu-id="243b6-352">tlsMaximumVersion</span></span>|<span data-ttu-id="243b6-353">String</span><span class="sxs-lookup"><span data-stu-id="243b6-353">String</span></span>|<span data-ttu-id="243b6-354">Максимальная версия TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="243b6-354">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="243b6-355">тлсминимумверсион</span><span class="sxs-lookup"><span data-stu-id="243b6-355">tlsMinimumVersion</span></span>|<span data-ttu-id="243b6-356">String</span><span class="sxs-lookup"><span data-stu-id="243b6-356">String</span></span>|<span data-ttu-id="243b6-357">Минимальная версия протокола TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="243b6-357">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="243b6-358">алловдефаултсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="243b6-358">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="243b6-359">Boolean</span><span class="sxs-lookup"><span data-stu-id="243b6-359">Boolean</span></span>|<span data-ttu-id="243b6-360">Разрешает использование параметров сопоставления безопасности путем установки всех параметров для устройства по умолчанию, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="243b6-360">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="243b6-361">алловдефаултчилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="243b6-361">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="243b6-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="243b6-362">Boolean</span></span>|<span data-ttu-id="243b6-363">Разрешает использование параметров дочернего сопоставления безопасности, устанавливая все параметры по умолчанию устройства, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="243b6-363">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="243b6-364">алвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="243b6-364">alwaysOnConfiguration</span></span>|[<span data-ttu-id="243b6-365">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="243b6-365">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="243b6-366">Конфигурация AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="243b6-366">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="243b6-367">енаблеалвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="243b6-367">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="243b6-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="243b6-368">Boolean</span></span>|<span data-ttu-id="243b6-369">Определяет, включена ли функция "всегда включено" VPN</span><span class="sxs-lookup"><span data-stu-id="243b6-369">Determines if Always on VPN is enabled</span></span>|
|<span data-ttu-id="243b6-370">мтусизеинбитес</span><span class="sxs-lookup"><span data-stu-id="243b6-370">mtuSizeInBytes</span></span>|<span data-ttu-id="243b6-371">Int32</span><span class="sxs-lookup"><span data-stu-id="243b6-371">Int32</span></span>|<span data-ttu-id="243b6-372">Максимальное количество передаваемых данных.</span><span class="sxs-lookup"><span data-stu-id="243b6-372">Maximum transmission unit.</span></span> <span data-ttu-id="243b6-373">Допустимые значения — от 1 до 65536</span><span class="sxs-lookup"><span data-stu-id="243b6-373">Valid values 1 to 65536</span></span>|



## <a name="response"></a><span data-ttu-id="243b6-374">Отклик</span><span class="sxs-lookup"><span data-stu-id="243b6-374">Response</span></span>
<span data-ttu-id="243b6-375">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="243b6-375">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="243b6-376">Пример</span><span class="sxs-lookup"><span data-stu-id="243b6-376">Example</span></span>

### <a name="request"></a><span data-ttu-id="243b6-377">Запрос</span><span class="sxs-lookup"><span data-stu-id="243b6-377">Request</span></span>
<span data-ttu-id="243b6-378">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="243b6-378">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="243b6-379">Отклик</span><span class="sxs-lookup"><span data-stu-id="243b6-379">Response</span></span>
<span data-ttu-id="243b6-p142">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="243b6-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




