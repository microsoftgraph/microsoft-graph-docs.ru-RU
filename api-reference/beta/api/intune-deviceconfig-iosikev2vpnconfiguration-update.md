---
title: Обновление iosikEv2VpnConfiguration
description: Обновление свойств объекта iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 70099b8e64ba6076b1e63610df5ee58a5b7aa3f2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43438914"
---
# <a name="update-iosikev2vpnconfiguration"></a><span data-ttu-id="6ad80-103">Обновление iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6ad80-103">Update iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="6ad80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ad80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ad80-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ad80-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ad80-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ad80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ad80-107">Обновление свойств объекта [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6ad80-107">Update the properties of a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ad80-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6ad80-108">Prerequisites</span></span>
<span data-ttu-id="6ad80-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ad80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ad80-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ad80-111">Permission type</span></span>|<span data-ttu-id="6ad80-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ad80-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ad80-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ad80-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ad80-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ad80-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ad80-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ad80-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ad80-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ad80-116">Not supported.</span></span>|
|<span data-ttu-id="6ad80-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6ad80-117">Application</span></span>|<span data-ttu-id="6ad80-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ad80-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ad80-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ad80-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6ad80-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6ad80-120">Request headers</span></span>
|<span data-ttu-id="6ad80-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ad80-121">Header</span></span>|<span data-ttu-id="6ad80-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6ad80-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ad80-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ad80-123">Authorization</span></span>|<span data-ttu-id="6ad80-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ad80-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ad80-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6ad80-125">Accept</span></span>|<span data-ttu-id="6ad80-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ad80-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ad80-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ad80-127">Request body</span></span>
<span data-ttu-id="6ad80-128">В тексте запроса добавьте представление объекта [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ad80-128">In the request body, supply a JSON representation for the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

<span data-ttu-id="6ad80-129">В следующей таблице приведены свойства, необходимые при создании [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ad80-129">The following table shows the properties that are required when you create the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span></span>

|<span data-ttu-id="6ad80-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ad80-130">Property</span></span>|<span data-ttu-id="6ad80-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6ad80-131">Type</span></span>|<span data-ttu-id="6ad80-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6ad80-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ad80-133">id</span><span class="sxs-lookup"><span data-stu-id="6ad80-133">id</span></span>|<span data-ttu-id="6ad80-134">String</span><span class="sxs-lookup"><span data-stu-id="6ad80-134">String</span></span>|<span data-ttu-id="6ad80-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6ad80-135">Key of the entity.</span></span> <span data-ttu-id="6ad80-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ad80-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ad80-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6ad80-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ad80-138">DateTimeOffset</span></span>|<span data-ttu-id="6ad80-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6ad80-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6ad80-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ad80-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6ad80-141">roleScopeTagIds</span></span>|<span data-ttu-id="6ad80-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6ad80-142">String collection</span></span>|<span data-ttu-id="6ad80-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6ad80-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6ad80-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ad80-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="6ad80-145">supportsScopeTags</span></span>|<span data-ttu-id="6ad80-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="6ad80-146">Boolean</span></span>|<span data-ttu-id="6ad80-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="6ad80-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6ad80-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="6ad80-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6ad80-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6ad80-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6ad80-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ad80-150">This property is read-only.</span></span> <span data-ttu-id="6ad80-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ad80-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6ad80-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6ad80-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6ad80-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6ad80-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6ad80-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6ad80-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ad80-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6ad80-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6ad80-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6ad80-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6ad80-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6ad80-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6ad80-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ad80-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6ad80-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6ad80-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6ad80-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6ad80-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6ad80-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6ad80-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ad80-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ad80-164">createdDateTime</span></span>|<span data-ttu-id="6ad80-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ad80-165">DateTimeOffset</span></span>|<span data-ttu-id="6ad80-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6ad80-166">DateTime the object was created.</span></span> <span data-ttu-id="6ad80-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ad80-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-168">description</span><span class="sxs-lookup"><span data-stu-id="6ad80-168">description</span></span>|<span data-ttu-id="6ad80-169">String</span><span class="sxs-lookup"><span data-stu-id="6ad80-169">String</span></span>|<span data-ttu-id="6ad80-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6ad80-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6ad80-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ad80-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-172">displayName</span><span class="sxs-lookup"><span data-stu-id="6ad80-172">displayName</span></span>|<span data-ttu-id="6ad80-173">Строка</span><span class="sxs-lookup"><span data-stu-id="6ad80-173">String</span></span>|<span data-ttu-id="6ad80-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6ad80-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6ad80-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ad80-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-176">version</span><span class="sxs-lookup"><span data-stu-id="6ad80-176">version</span></span>|<span data-ttu-id="6ad80-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6ad80-177">Int32</span></span>|<span data-ttu-id="6ad80-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6ad80-178">Version of the device configuration.</span></span> <span data-ttu-id="6ad80-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ad80-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="6ad80-180">connectionName</span></span>|<span data-ttu-id="6ad80-181">String</span><span class="sxs-lookup"><span data-stu-id="6ad80-181">String</span></span>|<span data-ttu-id="6ad80-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ad80-182">Connection name displayed to the user.</span></span> <span data-ttu-id="6ad80-183">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="6ad80-184">connectionType</span></span>|[<span data-ttu-id="6ad80-185">апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="6ad80-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="6ad80-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="6ad80-186">Connection type.</span></span> <span data-ttu-id="6ad80-187">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ad80-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="6ad80-188">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span><span class="sxs-lookup"><span data-stu-id="6ad80-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span></span>|
|<span data-ttu-id="6ad80-189">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="6ad80-189">loginGroupOrDomain</span></span>|<span data-ttu-id="6ad80-190">String</span><span class="sxs-lookup"><span data-stu-id="6ad80-190">String</span></span>|<span data-ttu-id="6ad80-191">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="6ad80-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="6ad80-192">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-193">role</span><span class="sxs-lookup"><span data-stu-id="6ad80-193">role</span></span>|<span data-ttu-id="6ad80-194">String</span><span class="sxs-lookup"><span data-stu-id="6ad80-194">String</span></span>|<span data-ttu-id="6ad80-195">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="6ad80-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="6ad80-196">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-197">область</span><span class="sxs-lookup"><span data-stu-id="6ad80-197">realm</span></span>|<span data-ttu-id="6ad80-198">String</span><span class="sxs-lookup"><span data-stu-id="6ad80-198">String</span></span>|<span data-ttu-id="6ad80-199">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="6ad80-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="6ad80-200">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-201">сервер</span><span class="sxs-lookup"><span data-stu-id="6ad80-201">server</span></span>|[<span data-ttu-id="6ad80-202">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="6ad80-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="6ad80-203">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="6ad80-203">VPN Server on the network.</span></span> <span data-ttu-id="6ad80-204">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="6ad80-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="6ad80-205">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="6ad80-206">identifier</span></span>|<span data-ttu-id="6ad80-207">String</span><span class="sxs-lookup"><span data-stu-id="6ad80-207">String</span></span>|<span data-ttu-id="6ad80-208">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="6ad80-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="6ad80-209">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-210">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="6ad80-210">customData</span></span>|<span data-ttu-id="6ad80-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="6ad80-212">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="6ad80-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="6ad80-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="6ad80-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="6ad80-214">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="6ad80-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="6ad80-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="6ad80-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="6ad80-216">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="6ad80-217">customKeyValueData</span></span>|<span data-ttu-id="6ad80-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6ad80-219">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="6ad80-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="6ad80-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="6ad80-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="6ad80-221">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="6ad80-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="6ad80-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="6ad80-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="6ad80-223">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-224">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="6ad80-224">enableSplitTunneling</span></span>|<span data-ttu-id="6ad80-225">Логическое</span><span class="sxs-lookup"><span data-stu-id="6ad80-225">Boolean</span></span>|<span data-ttu-id="6ad80-226">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="6ad80-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="6ad80-227">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-228">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="6ad80-228">authenticationMethod</span></span>|[<span data-ttu-id="6ad80-229">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="6ad80-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="6ad80-230">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="6ad80-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="6ad80-231">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ad80-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="6ad80-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="6ad80-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="6ad80-233">енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="6ad80-233">enablePerApp</span></span>|<span data-ttu-id="6ad80-234">Логическое</span><span class="sxs-lookup"><span data-stu-id="6ad80-234">Boolean</span></span>|<span data-ttu-id="6ad80-235">Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ad80-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="6ad80-236">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-237">сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="6ad80-237">safariDomains</span></span>|<span data-ttu-id="6ad80-238">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6ad80-238">String collection</span></span>|<span data-ttu-id="6ad80-239">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="6ad80-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="6ad80-240">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="6ad80-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="6ad80-241">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-242">ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="6ad80-242">onDemandRules</span></span>|<span data-ttu-id="6ad80-243">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="6ad80-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="6ad80-244">On-Demand Rules.</span></span> <span data-ttu-id="6ad80-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6ad80-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6ad80-246">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-247">проксисервер</span><span class="sxs-lookup"><span data-stu-id="6ad80-247">proxyServer</span></span>|[<span data-ttu-id="6ad80-248">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="6ad80-248">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="6ad80-249">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="6ad80-249">Proxy Server.</span></span> <span data-ttu-id="6ad80-250">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-251">оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="6ad80-251">optInToDeviceIdSharing</span></span>|<span data-ttu-id="6ad80-252">Логическое</span><span class="sxs-lookup"><span data-stu-id="6ad80-252">Boolean</span></span>|<span data-ttu-id="6ad80-253">Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="6ad80-253">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="6ad80-254">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-254">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-255">providerType</span><span class="sxs-lookup"><span data-stu-id="6ad80-255">providerType</span></span>|[<span data-ttu-id="6ad80-256">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="6ad80-256">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="6ad80-257">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="6ad80-257">Provider type for per-app VPN.</span></span> <span data-ttu-id="6ad80-258">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ad80-258">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="6ad80-259">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="6ad80-259">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="6ad80-260">userDomain</span><span class="sxs-lookup"><span data-stu-id="6ad80-260">userDomain</span></span>|<span data-ttu-id="6ad80-261">String</span><span class="sxs-lookup"><span data-stu-id="6ad80-261">String</span></span>|<span data-ttu-id="6ad80-262">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="6ad80-262">Zscaler only.</span></span> <span data-ttu-id="6ad80-263">Введите статический домен для предварительного заполнения поля Login в приложении Зскалер.</span><span class="sxs-lookup"><span data-stu-id="6ad80-263">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="6ad80-264">Если оставить это поле пустым, вместо этого будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ad80-264">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="6ad80-265">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-265">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-266">стриктенфорцемент</span><span class="sxs-lookup"><span data-stu-id="6ad80-266">strictEnforcement</span></span>|<span data-ttu-id="6ad80-267">Логическое</span><span class="sxs-lookup"><span data-stu-id="6ad80-267">Boolean</span></span>|<span data-ttu-id="6ad80-268">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="6ad80-268">Zscaler only.</span></span> <span data-ttu-id="6ad80-269">Блокирует сетевой трафик до тех пор, пока пользователь не войдет в приложение Зскалер.</span><span class="sxs-lookup"><span data-stu-id="6ad80-269">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="6ad80-270">"True" означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="6ad80-270">"True" means traffic is blocked.</span></span> <span data-ttu-id="6ad80-271">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-272">клауднаме</span><span class="sxs-lookup"><span data-stu-id="6ad80-272">cloudName</span></span>|<span data-ttu-id="6ad80-273">String</span><span class="sxs-lookup"><span data-stu-id="6ad80-273">String</span></span>|<span data-ttu-id="6ad80-274">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="6ad80-274">Zscaler only.</span></span> <span data-ttu-id="6ad80-275">Облако зскалер, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="6ad80-275">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="6ad80-276">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-276">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-277">excludeList</span><span class="sxs-lookup"><span data-stu-id="6ad80-277">excludeList</span></span>|<span data-ttu-id="6ad80-278">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6ad80-278">String collection</span></span>|<span data-ttu-id="6ad80-279">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="6ad80-279">Zscaler only.</span></span> <span data-ttu-id="6ad80-280">Список сетевых адресов, которые не отправляются через облако Зскалер.</span><span class="sxs-lookup"><span data-stu-id="6ad80-280">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="6ad80-281">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ad80-281">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ad80-282">чилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="6ad80-282">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="6ad80-283">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="6ad80-283">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="6ad80-284">Дочерние параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="6ad80-284">Child Security Association Parameters</span></span>|
|<span data-ttu-id="6ad80-285">клиентаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="6ad80-285">clientAuthenticationType</span></span>|[<span data-ttu-id="6ad80-286">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="6ad80-286">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="6ad80-287">Тип проверки подлинности клиента, который будет использоваться VPN-клиентом.</span><span class="sxs-lookup"><span data-stu-id="6ad80-287">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="6ad80-288">Возможные значения: `userAuthentication`, `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="6ad80-288">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="6ad80-289">деадпирдетектионрате</span><span class="sxs-lookup"><span data-stu-id="6ad80-289">deadPeerDetectionRate</span></span>|[<span data-ttu-id="6ad80-290">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="6ad80-290">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="6ad80-291">Определите, как часто следует проверять, активен ли одноранговый сеанс.</span><span class="sxs-lookup"><span data-stu-id="6ad80-291">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="6ad80-292">.</span><span class="sxs-lookup"><span data-stu-id="6ad80-292">.</span></span> <span data-ttu-id="6ad80-293">Возможные значения: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="6ad80-293">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="6ad80-294">дисаблемобилитяндмултихоминг</span><span class="sxs-lookup"><span data-stu-id="6ad80-294">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="6ad80-295">Логическое</span><span class="sxs-lookup"><span data-stu-id="6ad80-295">Boolean</span></span>|<span data-ttu-id="6ad80-296">Отключение МОБИКЕ</span><span class="sxs-lookup"><span data-stu-id="6ad80-296">Disable MOBIKE</span></span>|
|<span data-ttu-id="6ad80-297">дисаблередирект</span><span class="sxs-lookup"><span data-stu-id="6ad80-297">disableRedirect</span></span>|<span data-ttu-id="6ad80-298">Логическое</span><span class="sxs-lookup"><span data-stu-id="6ad80-298">Boolean</span></span>|<span data-ttu-id="6ad80-299">Отключение перенаправления</span><span class="sxs-lookup"><span data-stu-id="6ad80-299">Disable Redirect</span></span>|
|<span data-ttu-id="6ad80-300">енаблецертификатеревокатиончекк</span><span class="sxs-lookup"><span data-stu-id="6ad80-300">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="6ad80-301">Логическое</span><span class="sxs-lookup"><span data-stu-id="6ad80-301">Boolean</span></span>|<span data-ttu-id="6ad80-302">Включает проверку отзывов и действий. время ожидания отклика сервера не приведет к сбою</span><span class="sxs-lookup"><span data-stu-id="6ad80-302">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="6ad80-303">енаблиап</span><span class="sxs-lookup"><span data-stu-id="6ad80-303">enableEAP</span></span>|<span data-ttu-id="6ad80-304">Логическое</span><span class="sxs-lookup"><span data-stu-id="6ad80-304">Boolean</span></span>|<span data-ttu-id="6ad80-305">Включает проверку подлинности только EAP</span><span class="sxs-lookup"><span data-stu-id="6ad80-305">Enables EAP only authentication</span></span>|
|<span data-ttu-id="6ad80-306">енаблеперфектфорвардсекреци</span><span class="sxs-lookup"><span data-stu-id="6ad80-306">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="6ad80-307">Логическое</span><span class="sxs-lookup"><span data-stu-id="6ad80-307">Boolean</span></span>|<span data-ttu-id="6ad80-308">Включить безопасную пересылку (PFS).</span><span class="sxs-lookup"><span data-stu-id="6ad80-308">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="6ad80-309">енаблеусеинтерналсубнетаттрибутес</span><span class="sxs-lookup"><span data-stu-id="6ad80-309">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="6ad80-310">Логическое</span><span class="sxs-lookup"><span data-stu-id="6ad80-310">Boolean</span></span>|<span data-ttu-id="6ad80-311">Включите использование атрибутов внутренней подсети.</span><span class="sxs-lookup"><span data-stu-id="6ad80-311">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="6ad80-312">локалидентифиер</span><span class="sxs-lookup"><span data-stu-id="6ad80-312">localIdentifier</span></span>|[<span data-ttu-id="6ad80-313">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="6ad80-313">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="6ad80-314">Метод идентификации клиента, который пытается подключиться через VPN.</span><span class="sxs-lookup"><span data-stu-id="6ad80-314">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="6ad80-315">.</span><span class="sxs-lookup"><span data-stu-id="6ad80-315">.</span></span> <span data-ttu-id="6ad80-316">Возможные значения: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="6ad80-316">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="6ad80-317">ремотеидентифиер</span><span class="sxs-lookup"><span data-stu-id="6ad80-317">remoteIdentifier</span></span>|<span data-ttu-id="6ad80-318">String</span><span class="sxs-lookup"><span data-stu-id="6ad80-318">String</span></span>|<span data-ttu-id="6ad80-319">Адрес сервера IKEv2.</span><span class="sxs-lookup"><span data-stu-id="6ad80-319">Address of the IKEv2 server.</span></span> <span data-ttu-id="6ad80-320">Должно быть полным доменным именем, Усерфкдн, сетевым адресом или ASN1DN</span><span class="sxs-lookup"><span data-stu-id="6ad80-320">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="6ad80-321">секуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="6ad80-321">securityAssociationParameters</span></span>|[<span data-ttu-id="6ad80-322">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="6ad80-322">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="6ad80-323">Параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="6ad80-323">Security Association Parameters</span></span>|
|<span data-ttu-id="6ad80-324">серверцертификатекоммоннаме</span><span class="sxs-lookup"><span data-stu-id="6ad80-324">serverCertificateCommonName</span></span>|<span data-ttu-id="6ad80-325">String</span><span class="sxs-lookup"><span data-stu-id="6ad80-325">String</span></span>|<span data-ttu-id="6ad80-326">Общее имя сертификата сервера IKEv2, используемого при проверке подлинности сервера</span><span class="sxs-lookup"><span data-stu-id="6ad80-326">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="6ad80-327">серверцертификатеиссуеркоммоннаме</span><span class="sxs-lookup"><span data-stu-id="6ad80-327">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="6ad80-328">String</span><span class="sxs-lookup"><span data-stu-id="6ad80-328">String</span></span>|<span data-ttu-id="6ad80-329">Общее имя поставщика сертификата сервера IKEv2, используемого при проверке подлинности</span><span class="sxs-lookup"><span data-stu-id="6ad80-329">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="6ad80-330">серверцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="6ad80-330">serverCertificateType</span></span>|[<span data-ttu-id="6ad80-331">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="6ad80-331">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="6ad80-332">Тип сертификата, который VPN-сервер будет предоставлять VPN-клиенту для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="6ad80-332">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="6ad80-333">Возможные значения: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="6ad80-333">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="6ad80-334">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="6ad80-334">sharedSecret</span></span>|<span data-ttu-id="6ad80-335">String</span><span class="sxs-lookup"><span data-stu-id="6ad80-335">String</span></span>|<span data-ttu-id="6ad80-336">Используется, когда выбрана общая секретная проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="6ad80-336">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="6ad80-337">тлсмаксимумверсион</span><span class="sxs-lookup"><span data-stu-id="6ad80-337">tlsMaximumVersion</span></span>|<span data-ttu-id="6ad80-338">String</span><span class="sxs-lookup"><span data-stu-id="6ad80-338">String</span></span>|<span data-ttu-id="6ad80-339">Максимальная версия TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="6ad80-339">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="6ad80-340">тлсминимумверсион</span><span class="sxs-lookup"><span data-stu-id="6ad80-340">tlsMinimumVersion</span></span>|<span data-ttu-id="6ad80-341">String</span><span class="sxs-lookup"><span data-stu-id="6ad80-341">String</span></span>|<span data-ttu-id="6ad80-342">Минимальная версия протокола TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="6ad80-342">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="6ad80-343">алловдефаултсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="6ad80-343">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="6ad80-344">Логическое</span><span class="sxs-lookup"><span data-stu-id="6ad80-344">Boolean</span></span>|<span data-ttu-id="6ad80-345">Разрешает использование параметров сопоставления безопасности путем установки всех параметров для устройства по умолчанию, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="6ad80-345">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="6ad80-346">алловдефаултчилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="6ad80-346">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="6ad80-347">Логическое</span><span class="sxs-lookup"><span data-stu-id="6ad80-347">Boolean</span></span>|<span data-ttu-id="6ad80-348">Разрешает использование параметров дочернего сопоставления безопасности, устанавливая все параметры по умолчанию устройства, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="6ad80-348">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="6ad80-349">алвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="6ad80-349">alwaysOnConfiguration</span></span>|[<span data-ttu-id="6ad80-350">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6ad80-350">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="6ad80-351">Конфигурация AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="6ad80-351">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="6ad80-352">енаблеалвайсонконфигуратион</span><span class="sxs-lookup"><span data-stu-id="6ad80-352">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="6ad80-353">Логическое</span><span class="sxs-lookup"><span data-stu-id="6ad80-353">Boolean</span></span>|<span data-ttu-id="6ad80-354">Определяет, включена ли функция "всегда включено" VPN</span><span class="sxs-lookup"><span data-stu-id="6ad80-354">Determines if Always on VPN is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="6ad80-355">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ad80-355">Response</span></span>
<span data-ttu-id="6ad80-356">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6ad80-356">If successful, this method returns a `200 OK` response code and an updated [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ad80-357">Пример</span><span class="sxs-lookup"><span data-stu-id="6ad80-357">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ad80-358">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ad80-358">Request</span></span>
<span data-ttu-id="6ad80-359">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ad80-359">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6ad80-360">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ad80-360">Response</span></span>
<span data-ttu-id="6ad80-p139">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ad80-p139">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



