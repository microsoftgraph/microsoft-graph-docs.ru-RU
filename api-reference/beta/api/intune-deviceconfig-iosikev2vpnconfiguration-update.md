---
title: Обновление iosikEv2VpnConfiguration
description: Обновление свойств объекта iosikEv2VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 647b5ae72fe33458a68f9098bc32ab8df82841fc
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "35001708"
---
# <a name="update-iosikev2vpnconfiguration"></a><span data-ttu-id="d7259-103">Обновление iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d7259-103">Update iosikEv2VpnConfiguration</span></span>

> <span data-ttu-id="d7259-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7259-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7259-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7259-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7259-106">Обновление свойств объекта [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d7259-106">Update the properties of a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7259-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d7259-107">Prerequisites</span></span>
<span data-ttu-id="d7259-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7259-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7259-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7259-110">Permission type</span></span>|<span data-ttu-id="d7259-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7259-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7259-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7259-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7259-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7259-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7259-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7259-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7259-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7259-115">Not supported.</span></span>|
|<span data-ttu-id="d7259-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7259-116">Application</span></span>|<span data-ttu-id="d7259-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7259-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7259-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7259-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d7259-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7259-119">Request headers</span></span>
|<span data-ttu-id="d7259-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7259-120">Header</span></span>|<span data-ttu-id="d7259-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d7259-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7259-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7259-122">Authorization</span></span>|<span data-ttu-id="d7259-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7259-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7259-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d7259-124">Accept</span></span>|<span data-ttu-id="d7259-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7259-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7259-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d7259-126">Request body</span></span>
<span data-ttu-id="d7259-127">В тексте запроса добавьте представление объекта [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7259-127">In the request body, supply a JSON representation for the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

<span data-ttu-id="d7259-128">В следующей таблице приведены свойства, необходимые при создании [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7259-128">The following table shows the properties that are required when you create the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span></span>

|<span data-ttu-id="d7259-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7259-129">Property</span></span>|<span data-ttu-id="d7259-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d7259-130">Type</span></span>|<span data-ttu-id="d7259-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d7259-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7259-132">id</span><span class="sxs-lookup"><span data-stu-id="d7259-132">id</span></span>|<span data-ttu-id="d7259-133">String</span><span class="sxs-lookup"><span data-stu-id="d7259-133">String</span></span>|<span data-ttu-id="d7259-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d7259-134">Key of the entity.</span></span> <span data-ttu-id="d7259-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7259-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7259-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d7259-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7259-137">DateTimeOffset</span></span>|<span data-ttu-id="d7259-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d7259-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d7259-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7259-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d7259-140">roleScopeTagIds</span></span>|<span data-ttu-id="d7259-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d7259-141">String collection</span></span>|<span data-ttu-id="d7259-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d7259-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d7259-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7259-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d7259-144">supportsScopeTags</span></span>|<span data-ttu-id="d7259-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7259-145">Boolean</span></span>|<span data-ttu-id="d7259-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d7259-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d7259-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d7259-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d7259-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d7259-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d7259-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7259-149">This property is read-only.</span></span> <span data-ttu-id="d7259-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7259-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d7259-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d7259-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d7259-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d7259-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d7259-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d7259-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7259-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d7259-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d7259-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d7259-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d7259-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d7259-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d7259-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7259-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d7259-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d7259-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d7259-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d7259-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d7259-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d7259-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7259-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7259-163">createdDateTime</span></span>|<span data-ttu-id="d7259-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7259-164">DateTimeOffset</span></span>|<span data-ttu-id="d7259-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d7259-165">DateTime the object was created.</span></span> <span data-ttu-id="d7259-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7259-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-167">description</span><span class="sxs-lookup"><span data-stu-id="d7259-167">description</span></span>|<span data-ttu-id="d7259-168">String</span><span class="sxs-lookup"><span data-stu-id="d7259-168">String</span></span>|<span data-ttu-id="d7259-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d7259-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d7259-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7259-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d7259-171">displayName</span></span>|<span data-ttu-id="d7259-172">Строка</span><span class="sxs-lookup"><span data-stu-id="d7259-172">String</span></span>|<span data-ttu-id="d7259-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d7259-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d7259-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7259-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-175">version</span><span class="sxs-lookup"><span data-stu-id="d7259-175">version</span></span>|<span data-ttu-id="d7259-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d7259-176">Int32</span></span>|<span data-ttu-id="d7259-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d7259-177">Version of the device configuration.</span></span> <span data-ttu-id="d7259-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7259-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-179">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="d7259-179">connectionName</span></span>|<span data-ttu-id="d7259-180">String</span><span class="sxs-lookup"><span data-stu-id="d7259-180">String</span></span>|<span data-ttu-id="d7259-181">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="d7259-181">Connection name displayed to the user.</span></span> <span data-ttu-id="d7259-182">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-182">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="d7259-183">connectionType</span></span>|[<span data-ttu-id="d7259-184">Апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="d7259-184">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="d7259-185">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="d7259-185">Connection type.</span></span> <span data-ttu-id="d7259-186">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7259-186">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="d7259-187">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`,. `ikEv2`</span><span class="sxs-lookup"><span data-stu-id="d7259-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`.</span></span>|
|<span data-ttu-id="d7259-188">Логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="d7259-188">loginGroupOrDomain</span></span>|<span data-ttu-id="d7259-189">String</span><span class="sxs-lookup"><span data-stu-id="d7259-189">String</span></span>|<span data-ttu-id="d7259-190">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="d7259-190">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="d7259-191">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-191">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-192">role</span><span class="sxs-lookup"><span data-stu-id="d7259-192">role</span></span>|<span data-ttu-id="d7259-193">String</span><span class="sxs-lookup"><span data-stu-id="d7259-193">String</span></span>|<span data-ttu-id="d7259-194">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="d7259-194">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="d7259-195">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-195">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-196">область</span><span class="sxs-lookup"><span data-stu-id="d7259-196">realm</span></span>|<span data-ttu-id="d7259-197">String</span><span class="sxs-lookup"><span data-stu-id="d7259-197">String</span></span>|<span data-ttu-id="d7259-198">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="d7259-198">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="d7259-199">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-199">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-200">сервер</span><span class="sxs-lookup"><span data-stu-id="d7259-200">server</span></span>|[<span data-ttu-id="d7259-201">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="d7259-201">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="d7259-202">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="d7259-202">VPN Server on the network.</span></span> <span data-ttu-id="d7259-203">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="d7259-203">Make sure end users can access this network location.</span></span> <span data-ttu-id="d7259-204">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-205">идентификатор</span><span class="sxs-lookup"><span data-stu-id="d7259-205">identifier</span></span>|<span data-ttu-id="d7259-206">String</span><span class="sxs-lookup"><span data-stu-id="d7259-206">String</span></span>|<span data-ttu-id="d7259-207">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="d7259-207">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="d7259-208">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-208">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-209">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="d7259-209">customData</span></span>|<span data-ttu-id="d7259-210">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="d7259-211">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="d7259-211">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="d7259-212">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="d7259-212">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="d7259-213">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="d7259-213">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="d7259-214">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="d7259-214">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="d7259-215">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-216">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="d7259-216">customKeyValueData</span></span>|<span data-ttu-id="d7259-217">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d7259-218">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="d7259-218">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="d7259-219">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="d7259-219">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="d7259-220">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="d7259-220">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="d7259-221">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="d7259-221">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="d7259-222">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-222">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-223">Енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="d7259-223">enableSplitTunneling</span></span>|<span data-ttu-id="d7259-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7259-224">Boolean</span></span>|<span data-ttu-id="d7259-225">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="d7259-225">Send all network traffic through VPN.</span></span> <span data-ttu-id="d7259-226">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-226">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-227">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="d7259-227">authenticationMethod</span></span>|[<span data-ttu-id="d7259-228">Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="d7259-228">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="d7259-229">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="d7259-229">Authentication method for this VPN connection.</span></span> <span data-ttu-id="d7259-230">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7259-230">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="d7259-231">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="d7259-231">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="d7259-232">Енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="d7259-232">enablePerApp</span></span>|<span data-ttu-id="d7259-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7259-233">Boolean</span></span>|<span data-ttu-id="d7259-234">Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d7259-234">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="d7259-235">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-235">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-236">Сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="d7259-236">safariDomains</span></span>|<span data-ttu-id="d7259-237">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d7259-237">String collection</span></span>|<span data-ttu-id="d7259-238">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="d7259-238">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="d7259-239">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="d7259-239">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="d7259-240">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-240">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-241">Ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="d7259-241">onDemandRules</span></span>|<span data-ttu-id="d7259-242">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="d7259-243">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="d7259-243">On-Demand Rules.</span></span> <span data-ttu-id="d7259-244">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="d7259-244">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d7259-245">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-245">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-246">проксисервер</span><span class="sxs-lookup"><span data-stu-id="d7259-246">proxyServer</span></span>|[<span data-ttu-id="d7259-247">Впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="d7259-247">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="d7259-248">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="d7259-248">Proxy Server.</span></span> <span data-ttu-id="d7259-249">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-249">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-250">Оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="d7259-250">optInToDeviceIdSharing</span></span>|<span data-ttu-id="d7259-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7259-251">Boolean</span></span>|<span data-ttu-id="d7259-252">Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="d7259-252">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="d7259-253">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-253">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-254">providerType</span><span class="sxs-lookup"><span data-stu-id="d7259-254">providerType</span></span>|[<span data-ttu-id="d7259-255">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="d7259-255">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="d7259-256">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="d7259-256">Provider type for per-app VPN.</span></span> <span data-ttu-id="d7259-257">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7259-257">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="d7259-258">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="d7259-258">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="d7259-259">userDomain</span><span class="sxs-lookup"><span data-stu-id="d7259-259">userDomain</span></span>|<span data-ttu-id="d7259-260">String</span><span class="sxs-lookup"><span data-stu-id="d7259-260">String</span></span>|<span data-ttu-id="d7259-261">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="d7259-261">Zscaler only.</span></span> <span data-ttu-id="d7259-262">Введите статический домен для предварительного заполнения поля Login в приложении Зскалер.</span><span class="sxs-lookup"><span data-stu-id="d7259-262">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="d7259-263">Если оставить это поле пустым, вместо этого будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="d7259-263">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="d7259-264">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-264">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-265">Стриктенфорцемент</span><span class="sxs-lookup"><span data-stu-id="d7259-265">strictEnforcement</span></span>|<span data-ttu-id="d7259-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7259-266">Boolean</span></span>|<span data-ttu-id="d7259-267">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="d7259-267">Zscaler only.</span></span> <span data-ttu-id="d7259-268">Блокирует сетевой трафик до тех пор, пока пользователь не войдет в приложение Зскалер.</span><span class="sxs-lookup"><span data-stu-id="d7259-268">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="d7259-269">"True" означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="d7259-269">"True" means traffic is blocked.</span></span> <span data-ttu-id="d7259-270">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-270">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-271">Клауднаме</span><span class="sxs-lookup"><span data-stu-id="d7259-271">cloudName</span></span>|<span data-ttu-id="d7259-272">String</span><span class="sxs-lookup"><span data-stu-id="d7259-272">String</span></span>|<span data-ttu-id="d7259-273">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="d7259-273">Zscaler only.</span></span> <span data-ttu-id="d7259-274">Облако зскалер, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="d7259-274">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="d7259-275">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-275">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-276">excludeList</span><span class="sxs-lookup"><span data-stu-id="d7259-276">excludeList</span></span>|<span data-ttu-id="d7259-277">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d7259-277">String collection</span></span>|<span data-ttu-id="d7259-278">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="d7259-278">Zscaler only.</span></span> <span data-ttu-id="d7259-279">Список сетевых адресов, которые не отправляются через облако Зскалер.</span><span class="sxs-lookup"><span data-stu-id="d7259-279">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="d7259-280">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7259-280">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d7259-281">ЧилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="d7259-281">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="d7259-282">ИосвпнсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="d7259-282">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="d7259-283">Дочерние параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="d7259-283">Child Security Association Parameters</span></span>|
|<span data-ttu-id="d7259-284">Клиентаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="d7259-284">clientAuthenticationType</span></span>|[<span data-ttu-id="d7259-285">Впнклиентаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="d7259-285">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="d7259-286">Тип проверки подлинности клиента, который будет использоваться VPN-клиентом.</span><span class="sxs-lookup"><span data-stu-id="d7259-286">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="d7259-287">Возможные значения: `userAuthentication`, `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="d7259-287">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="d7259-288">Деадпирдетектионрате</span><span class="sxs-lookup"><span data-stu-id="d7259-288">deadPeerDetectionRate</span></span>|[<span data-ttu-id="d7259-289">Впндеадпирдетектионрате</span><span class="sxs-lookup"><span data-stu-id="d7259-289">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="d7259-290">Определите, как часто следует проверять, активен ли одноранговый сеанс.</span><span class="sxs-lookup"><span data-stu-id="d7259-290">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="d7259-291">.</span><span class="sxs-lookup"><span data-stu-id="d7259-291"></span></span> <span data-ttu-id="d7259-292">Возможные значения: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="d7259-292">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="d7259-293">Дисаблемобилитяндмултихоминг</span><span class="sxs-lookup"><span data-stu-id="d7259-293">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="d7259-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7259-294">Boolean</span></span>|<span data-ttu-id="d7259-295">Отключение МОБИКЕ</span><span class="sxs-lookup"><span data-stu-id="d7259-295">Disable MOBIKE</span></span>|
|<span data-ttu-id="d7259-296">Дисаблередирект</span><span class="sxs-lookup"><span data-stu-id="d7259-296">disableRedirect</span></span>|<span data-ttu-id="d7259-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7259-297">Boolean</span></span>|<span data-ttu-id="d7259-298">Отключение перенаправления</span><span class="sxs-lookup"><span data-stu-id="d7259-298">Disable Redirect</span></span>|
|<span data-ttu-id="d7259-299">Енаблецертификатеревокатиончекк</span><span class="sxs-lookup"><span data-stu-id="d7259-299">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="d7259-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7259-300">Boolean</span></span>|<span data-ttu-id="d7259-301">Включает проверку отзывов и действий. время ожидания отклика сервера не приведет к сбою</span><span class="sxs-lookup"><span data-stu-id="d7259-301">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="d7259-302">Енаблиап</span><span class="sxs-lookup"><span data-stu-id="d7259-302">enableEAP</span></span>|<span data-ttu-id="d7259-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7259-303">Boolean</span></span>|<span data-ttu-id="d7259-304">Включает проверку подлинности только EAP</span><span class="sxs-lookup"><span data-stu-id="d7259-304">Enables EAP only authentication</span></span>|
|<span data-ttu-id="d7259-305">Енаблеперфектфорвардсекреци</span><span class="sxs-lookup"><span data-stu-id="d7259-305">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="d7259-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7259-306">Boolean</span></span>|<span data-ttu-id="d7259-307">Включить безопасную пересылку (PFS).</span><span class="sxs-lookup"><span data-stu-id="d7259-307">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="d7259-308">Енаблеусеинтерналсубнетаттрибутес</span><span class="sxs-lookup"><span data-stu-id="d7259-308">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="d7259-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7259-309">Boolean</span></span>|<span data-ttu-id="d7259-310">Включите использование атрибутов внутренней подсети.</span><span class="sxs-lookup"><span data-stu-id="d7259-310">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="d7259-311">Локалидентифиер</span><span class="sxs-lookup"><span data-stu-id="d7259-311">localIdentifier</span></span>|[<span data-ttu-id="d7259-312">Впнлокалидентифиер</span><span class="sxs-lookup"><span data-stu-id="d7259-312">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="d7259-313">Метод идентификации клиента, который пытается подключиться через VPN.</span><span class="sxs-lookup"><span data-stu-id="d7259-313">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="d7259-314">.</span><span class="sxs-lookup"><span data-stu-id="d7259-314"></span></span> <span data-ttu-id="d7259-315">Возможные значения: `deviceFQDN`.</span><span class="sxs-lookup"><span data-stu-id="d7259-315">Possible values are: `deviceFQDN`.</span></span>|
|<span data-ttu-id="d7259-316">Ремотеидентифиер</span><span class="sxs-lookup"><span data-stu-id="d7259-316">remoteIdentifier</span></span>|<span data-ttu-id="d7259-317">String</span><span class="sxs-lookup"><span data-stu-id="d7259-317">String</span></span>|<span data-ttu-id="d7259-318">Адрес сервера IKEv2.</span><span class="sxs-lookup"><span data-stu-id="d7259-318">Address of the IKEv2 server.</span></span> <span data-ttu-id="d7259-319">Должно быть полным доменным именем, Усерфкдн, сетевым адресом или ASN1DN</span><span class="sxs-lookup"><span data-stu-id="d7259-319">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="d7259-320">СекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="d7259-320">securityAssociationParameters</span></span>|[<span data-ttu-id="d7259-321">ИосвпнсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="d7259-321">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="d7259-322">Параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="d7259-322">Security Association Parameters</span></span>|
|<span data-ttu-id="d7259-323">Серверцертификатекоммоннаме</span><span class="sxs-lookup"><span data-stu-id="d7259-323">serverCertificateCommonName</span></span>|<span data-ttu-id="d7259-324">String</span><span class="sxs-lookup"><span data-stu-id="d7259-324">String</span></span>|<span data-ttu-id="d7259-325">Общее имя сертификата сервера IKEv2, используемого при проверке подлинности сервера</span><span class="sxs-lookup"><span data-stu-id="d7259-325">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="d7259-326">Серверцертификатеиссуеркоммоннаме</span><span class="sxs-lookup"><span data-stu-id="d7259-326">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="d7259-327">String</span><span class="sxs-lookup"><span data-stu-id="d7259-327">String</span></span>|<span data-ttu-id="d7259-328">Общее имя поставщика сертификата сервера IKEv2, используемого при проверке подлинности</span><span class="sxs-lookup"><span data-stu-id="d7259-328">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="d7259-329">Серверцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="d7259-329">serverCertificateType</span></span>|[<span data-ttu-id="d7259-330">Впнсерверцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="d7259-330">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="d7259-331">Тип сертификата, который VPN-сервер будет предоставлять VPN-клиенту для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d7259-331">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="d7259-332">Возможные значения: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="d7259-332">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="d7259-333">Шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="d7259-333">sharedSecret</span></span>|<span data-ttu-id="d7259-334">String</span><span class="sxs-lookup"><span data-stu-id="d7259-334">String</span></span>|<span data-ttu-id="d7259-335">Используется, когда выбрана общая секретная проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="d7259-335">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="d7259-336">Тлсмаксимумверсион</span><span class="sxs-lookup"><span data-stu-id="d7259-336">tlsMaximumVersion</span></span>|<span data-ttu-id="d7259-337">String</span><span class="sxs-lookup"><span data-stu-id="d7259-337">String</span></span>|<span data-ttu-id="d7259-338">Максимальная версия TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="d7259-338">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="d7259-339">Тлсминимумверсион</span><span class="sxs-lookup"><span data-stu-id="d7259-339">tlsMinimumVersion</span></span>|<span data-ttu-id="d7259-340">String</span><span class="sxs-lookup"><span data-stu-id="d7259-340">String</span></span>|<span data-ttu-id="d7259-341">Минимальная версия протокола TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="d7259-341">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="d7259-342">АлловдефаултсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="d7259-342">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="d7259-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7259-343">Boolean</span></span>|<span data-ttu-id="d7259-344">Разрешает использование параметров сопоставления безопасности путем установки всех параметров для устройства по умолчанию, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="d7259-344">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="d7259-345">АлловдефаултчилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="d7259-345">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="d7259-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7259-346">Boolean</span></span>|<span data-ttu-id="d7259-347">Разрешает использование параметров дочернего сопоставления безопасности, устанавливая все параметры по умолчанию устройства, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="d7259-347">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|



## <a name="response"></a><span data-ttu-id="d7259-348">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7259-348">Response</span></span>
<span data-ttu-id="d7259-349">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d7259-349">If successful, this method returns a `200 OK` response code and an updated [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7259-350">Пример</span><span class="sxs-lookup"><span data-stu-id="d7259-350">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7259-351">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7259-351">Request</span></span>
<span data-ttu-id="d7259-352">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7259-352">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4237

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
  "localIdentifier": "deviceFQDN",
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
  "allowDefaultChildSecurityAssociationParameters": true
}
```

### <a name="response"></a><span data-ttu-id="d7259-353">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7259-353">Response</span></span>
<span data-ttu-id="d7259-p139">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7259-p139">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4409

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
  "localIdentifier": "deviceFQDN",
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
  "allowDefaultChildSecurityAssociationParameters": true
}
```





