---
title: Обновление Макосвпнконфигуратион
description: Обновление свойств объекта Макосвпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5afa2adab20a5bfb5c8633c1e78980d4878659f9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287412"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="d4898-103">Обновление Макосвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="d4898-103">Update macOSVpnConfiguration</span></span>

<span data-ttu-id="d4898-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4898-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4898-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4898-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4898-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4898-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4898-107">Обновление свойств объекта [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d4898-107">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4898-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d4898-108">Prerequisites</span></span>
<span data-ttu-id="d4898-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4898-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4898-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4898-111">Permission type</span></span>|<span data-ttu-id="d4898-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4898-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4898-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4898-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4898-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4898-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4898-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4898-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4898-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4898-116">Not supported.</span></span>|
|<span data-ttu-id="d4898-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4898-117">Application</span></span>|<span data-ttu-id="d4898-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4898-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4898-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4898-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d4898-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d4898-120">Request headers</span></span>
|<span data-ttu-id="d4898-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4898-121">Header</span></span>|<span data-ttu-id="d4898-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d4898-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4898-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4898-123">Authorization</span></span>|<span data-ttu-id="d4898-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4898-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4898-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4898-125">Accept</span></span>|<span data-ttu-id="d4898-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4898-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4898-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4898-127">Request body</span></span>
<span data-ttu-id="d4898-128">В тексте запроса добавьте представление объекта [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4898-128">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="d4898-129">В следующей таблице приведены свойства, необходимые при создании [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4898-129">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="d4898-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4898-130">Property</span></span>|<span data-ttu-id="d4898-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d4898-131">Type</span></span>|<span data-ttu-id="d4898-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d4898-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4898-133">id</span><span class="sxs-lookup"><span data-stu-id="d4898-133">id</span></span>|<span data-ttu-id="d4898-134">String</span><span class="sxs-lookup"><span data-stu-id="d4898-134">String</span></span>|<span data-ttu-id="d4898-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d4898-135">Key of the entity.</span></span> <span data-ttu-id="d4898-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4898-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4898-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d4898-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4898-138">DateTimeOffset</span></span>|<span data-ttu-id="d4898-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d4898-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d4898-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4898-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d4898-141">roleScopeTagIds</span></span>|<span data-ttu-id="d4898-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d4898-142">String collection</span></span>|<span data-ttu-id="d4898-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d4898-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d4898-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4898-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d4898-145">supportsScopeTags</span></span>|<span data-ttu-id="d4898-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4898-146">Boolean</span></span>|<span data-ttu-id="d4898-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d4898-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d4898-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d4898-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d4898-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d4898-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d4898-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d4898-150">This property is read-only.</span></span> <span data-ttu-id="d4898-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4898-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d4898-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d4898-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d4898-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d4898-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d4898-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d4898-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4898-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d4898-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d4898-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d4898-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d4898-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d4898-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d4898-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4898-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d4898-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d4898-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d4898-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d4898-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d4898-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d4898-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4898-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4898-164">createdDateTime</span></span>|<span data-ttu-id="d4898-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4898-165">DateTimeOffset</span></span>|<span data-ttu-id="d4898-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d4898-166">DateTime the object was created.</span></span> <span data-ttu-id="d4898-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4898-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-168">description</span><span class="sxs-lookup"><span data-stu-id="d4898-168">description</span></span>|<span data-ttu-id="d4898-169">String</span><span class="sxs-lookup"><span data-stu-id="d4898-169">String</span></span>|<span data-ttu-id="d4898-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d4898-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d4898-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4898-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d4898-172">displayName</span></span>|<span data-ttu-id="d4898-173">String</span><span class="sxs-lookup"><span data-stu-id="d4898-173">String</span></span>|<span data-ttu-id="d4898-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d4898-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d4898-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4898-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-176">version</span><span class="sxs-lookup"><span data-stu-id="d4898-176">version</span></span>|<span data-ttu-id="d4898-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d4898-177">Int32</span></span>|<span data-ttu-id="d4898-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d4898-178">Version of the device configuration.</span></span> <span data-ttu-id="d4898-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4898-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="d4898-180">connectionName</span></span>|<span data-ttu-id="d4898-181">String</span><span class="sxs-lookup"><span data-stu-id="d4898-181">String</span></span>|<span data-ttu-id="d4898-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="d4898-182">Connection name displayed to the user.</span></span> <span data-ttu-id="d4898-183">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="d4898-184">connectionType</span></span>|[<span data-ttu-id="d4898-185">апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="d4898-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="d4898-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="d4898-186">Connection type.</span></span> <span data-ttu-id="d4898-187">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4898-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="d4898-188">Возможные значения:,,,,,,,,,, `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` ,, `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` , `paloAltoGlobalProtectV2` , `ikEv2` , `alwaysOn` `microsoftTunnel` `netMotionMobility` ,,.</span><span class="sxs-lookup"><span data-stu-id="d4898-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="d4898-189">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="d4898-189">loginGroupOrDomain</span></span>|<span data-ttu-id="d4898-190">String</span><span class="sxs-lookup"><span data-stu-id="d4898-190">String</span></span>|<span data-ttu-id="d4898-191">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="d4898-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="d4898-192">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-193">role</span><span class="sxs-lookup"><span data-stu-id="d4898-193">role</span></span>|<span data-ttu-id="d4898-194">String</span><span class="sxs-lookup"><span data-stu-id="d4898-194">String</span></span>|<span data-ttu-id="d4898-195">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="d4898-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="d4898-196">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-197">область</span><span class="sxs-lookup"><span data-stu-id="d4898-197">realm</span></span>|<span data-ttu-id="d4898-198">String</span><span class="sxs-lookup"><span data-stu-id="d4898-198">String</span></span>|<span data-ttu-id="d4898-199">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="d4898-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="d4898-200">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-201">сервер</span><span class="sxs-lookup"><span data-stu-id="d4898-201">server</span></span>|[<span data-ttu-id="d4898-202">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="d4898-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="d4898-203">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="d4898-203">VPN Server on the network.</span></span> <span data-ttu-id="d4898-204">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="d4898-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="d4898-205">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="d4898-206">identifier</span></span>|<span data-ttu-id="d4898-207">String</span><span class="sxs-lookup"><span data-stu-id="d4898-207">String</span></span>|<span data-ttu-id="d4898-208">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="d4898-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="d4898-209">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-210">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="d4898-210">customData</span></span>|<span data-ttu-id="d4898-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="d4898-212">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="d4898-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="d4898-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="d4898-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="d4898-214">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="d4898-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="d4898-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="d4898-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="d4898-216">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="d4898-217">customKeyValueData</span></span>|<span data-ttu-id="d4898-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d4898-219">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="d4898-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="d4898-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="d4898-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="d4898-221">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="d4898-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="d4898-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="d4898-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="d4898-223">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-224">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="d4898-224">enableSplitTunneling</span></span>|<span data-ttu-id="d4898-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4898-225">Boolean</span></span>|<span data-ttu-id="d4898-226">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="d4898-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="d4898-227">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-228">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="d4898-228">authenticationMethod</span></span>|[<span data-ttu-id="d4898-229">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="d4898-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="d4898-230">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="d4898-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="d4898-231">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4898-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="d4898-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="d4898-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="d4898-233">енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="d4898-233">enablePerApp</span></span>|<span data-ttu-id="d4898-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4898-234">Boolean</span></span>|<span data-ttu-id="d4898-235">Если задать для этого параметра значение true, будут созданы Per-App полезные данные VPN, которые позже могут быть связаны с приложениями, которые могут запускать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d4898-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="d4898-236">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-237">сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="d4898-237">safariDomains</span></span>|<span data-ttu-id="d4898-238">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d4898-238">String collection</span></span>|<span data-ttu-id="d4898-239">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="d4898-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="d4898-240">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="d4898-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="d4898-241">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-242">ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="d4898-242">onDemandRules</span></span>|<span data-ttu-id="d4898-243">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="d4898-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="d4898-244">On-Demand Rules.</span></span> <span data-ttu-id="d4898-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="d4898-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d4898-246">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-247">providerType</span><span class="sxs-lookup"><span data-stu-id="d4898-247">providerType</span></span>|[<span data-ttu-id="d4898-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="d4898-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="d4898-249">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="d4898-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="d4898-250">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4898-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="d4898-251">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="d4898-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="d4898-252">ексклудеддомаинс</span><span class="sxs-lookup"><span data-stu-id="d4898-252">excludedDomains</span></span>|<span data-ttu-id="d4898-253">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d4898-253">String collection</span></span>|<span data-ttu-id="d4898-254">Домены, доступ к которым осуществляется через общедоступный Интернет, а не через VPN, даже если VPN для каждого приложения активируется наследуемой от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-254">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-255">дисаблеондемандусероверриде</span><span class="sxs-lookup"><span data-stu-id="d4898-255">disableOnDemandUserOverride</span></span>|<span data-ttu-id="d4898-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4898-256">Boolean</span></span>|<span data-ttu-id="d4898-257">Переключатель, чтобы запретить пользователям отключать автоматическое VPN в приложении "Параметры", унаследованном от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-257">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-258">проксисервер</span><span class="sxs-lookup"><span data-stu-id="d4898-258">proxyServer</span></span>|[<span data-ttu-id="d4898-259">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="d4898-259">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="d4898-260">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="d4898-260">Proxy Server.</span></span> <span data-ttu-id="d4898-261">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-261">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d4898-262">оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="d4898-262">optInToDeviceIdSharing</span></span>|<span data-ttu-id="d4898-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4898-263">Boolean</span></span>|<span data-ttu-id="d4898-264">Opt-In для предоставления доступа к идентификатору устройства сторонним VPN-клиентам для использования в процессе проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="d4898-264">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="d4898-265">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4898-265">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d4898-266">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4898-266">Response</span></span>
<span data-ttu-id="d4898-267">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4898-267">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4898-268">Пример</span><span class="sxs-lookup"><span data-stu-id="d4898-268">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4898-269">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4898-269">Request</span></span>
<span data-ttu-id="d4898-270">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4898-270">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2761

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
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
  "optInToDeviceIdSharing": true
}
```

### <a name="response"></a><span data-ttu-id="d4898-271">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4898-271">Response</span></span>
<span data-ttu-id="d4898-p130">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4898-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2933

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
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
  "optInToDeviceIdSharing": true
}
```




