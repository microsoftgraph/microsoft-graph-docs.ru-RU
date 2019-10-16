---
title: Обновление iosikEv2VpnConfiguration
description: Обновление свойств объекта iosikEv2VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2e570faa7a2861edfb98e4e487db994b6893c3f0
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533800"
---
# <a name="update-iosikev2vpnconfiguration"></a><span data-ttu-id="ac286-103">Обновление iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ac286-103">Update iosikEv2VpnConfiguration</span></span>

> <span data-ttu-id="ac286-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac286-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac286-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ac286-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac286-106">Обновление свойств объекта [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ac286-106">Update the properties of a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac286-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ac286-107">Prerequisites</span></span>
<span data-ttu-id="ac286-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac286-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac286-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac286-110">Permission type</span></span>|<span data-ttu-id="ac286-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac286-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac286-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac286-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ac286-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac286-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ac286-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac286-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac286-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac286-115">Not supported.</span></span>|
|<span data-ttu-id="ac286-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ac286-116">Application</span></span>|<span data-ttu-id="ac286-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac286-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac286-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac286-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ac286-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac286-119">Request headers</span></span>
|<span data-ttu-id="ac286-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ac286-120">Header</span></span>|<span data-ttu-id="ac286-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ac286-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac286-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac286-122">Authorization</span></span>|<span data-ttu-id="ac286-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac286-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac286-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ac286-124">Accept</span></span>|<span data-ttu-id="ac286-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ac286-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac286-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac286-126">Request body</span></span>
<span data-ttu-id="ac286-127">В тексте запроса добавьте представление объекта [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac286-127">In the request body, supply a JSON representation for the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

<span data-ttu-id="ac286-128">В следующей таблице приведены свойства, необходимые при создании [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac286-128">The following table shows the properties that are required when you create the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span></span>

|<span data-ttu-id="ac286-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac286-129">Property</span></span>|<span data-ttu-id="ac286-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ac286-130">Type</span></span>|<span data-ttu-id="ac286-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ac286-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac286-132">id</span><span class="sxs-lookup"><span data-stu-id="ac286-132">id</span></span>|<span data-ttu-id="ac286-133">String</span><span class="sxs-lookup"><span data-stu-id="ac286-133">String</span></span>|<span data-ttu-id="ac286-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ac286-134">Key of the entity.</span></span> <span data-ttu-id="ac286-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac286-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac286-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ac286-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac286-137">DateTimeOffset</span></span>|<span data-ttu-id="ac286-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ac286-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ac286-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac286-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ac286-140">roleScopeTagIds</span></span>|<span data-ttu-id="ac286-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ac286-141">String collection</span></span>|<span data-ttu-id="ac286-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ac286-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ac286-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac286-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="ac286-144">supportsScopeTags</span></span>|<span data-ttu-id="ac286-145">Логический</span><span class="sxs-lookup"><span data-stu-id="ac286-145">Boolean</span></span>|<span data-ttu-id="ac286-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ac286-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ac286-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="ac286-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ac286-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ac286-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ac286-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac286-149">This property is read-only.</span></span> <span data-ttu-id="ac286-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac286-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ac286-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ac286-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ac286-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ac286-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ac286-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ac286-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac286-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ac286-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ac286-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ac286-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ac286-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ac286-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ac286-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac286-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ac286-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ac286-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ac286-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ac286-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ac286-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ac286-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac286-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac286-163">createdDateTime</span></span>|<span data-ttu-id="ac286-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac286-164">DateTimeOffset</span></span>|<span data-ttu-id="ac286-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ac286-165">DateTime the object was created.</span></span> <span data-ttu-id="ac286-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac286-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-167">description</span><span class="sxs-lookup"><span data-stu-id="ac286-167">description</span></span>|<span data-ttu-id="ac286-168">String</span><span class="sxs-lookup"><span data-stu-id="ac286-168">String</span></span>|<span data-ttu-id="ac286-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ac286-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ac286-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac286-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ac286-171">displayName</span></span>|<span data-ttu-id="ac286-172">Строка</span><span class="sxs-lookup"><span data-stu-id="ac286-172">String</span></span>|<span data-ttu-id="ac286-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ac286-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ac286-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac286-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-175">version</span><span class="sxs-lookup"><span data-stu-id="ac286-175">version</span></span>|<span data-ttu-id="ac286-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ac286-176">Int32</span></span>|<span data-ttu-id="ac286-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ac286-177">Version of the device configuration.</span></span> <span data-ttu-id="ac286-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac286-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-179">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="ac286-179">connectionName</span></span>|<span data-ttu-id="ac286-180">String</span><span class="sxs-lookup"><span data-stu-id="ac286-180">String</span></span>|<span data-ttu-id="ac286-181">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="ac286-181">Connection name displayed to the user.</span></span> <span data-ttu-id="ac286-182">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-182">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="ac286-183">connectionType</span></span>|[<span data-ttu-id="ac286-184">апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="ac286-184">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="ac286-185">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="ac286-185">Connection type.</span></span> <span data-ttu-id="ac286-186">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac286-186">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="ac286-187">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`,. `ikEv2`</span><span class="sxs-lookup"><span data-stu-id="ac286-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`.</span></span>|
|<span data-ttu-id="ac286-188">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="ac286-188">loginGroupOrDomain</span></span>|<span data-ttu-id="ac286-189">String</span><span class="sxs-lookup"><span data-stu-id="ac286-189">String</span></span>|<span data-ttu-id="ac286-190">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="ac286-190">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="ac286-191">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-191">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-192">role</span><span class="sxs-lookup"><span data-stu-id="ac286-192">role</span></span>|<span data-ttu-id="ac286-193">String</span><span class="sxs-lookup"><span data-stu-id="ac286-193">String</span></span>|<span data-ttu-id="ac286-194">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="ac286-194">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="ac286-195">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-195">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-196">область</span><span class="sxs-lookup"><span data-stu-id="ac286-196">realm</span></span>|<span data-ttu-id="ac286-197">String</span><span class="sxs-lookup"><span data-stu-id="ac286-197">String</span></span>|<span data-ttu-id="ac286-198">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="ac286-198">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="ac286-199">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-199">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-200">сервер</span><span class="sxs-lookup"><span data-stu-id="ac286-200">server</span></span>|[<span data-ttu-id="ac286-201">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="ac286-201">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="ac286-202">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="ac286-202">VPN Server on the network.</span></span> <span data-ttu-id="ac286-203">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="ac286-203">Make sure end users can access this network location.</span></span> <span data-ttu-id="ac286-204">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-205">идентификатор</span><span class="sxs-lookup"><span data-stu-id="ac286-205">identifier</span></span>|<span data-ttu-id="ac286-206">String</span><span class="sxs-lookup"><span data-stu-id="ac286-206">String</span></span>|<span data-ttu-id="ac286-207">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="ac286-207">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ac286-208">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-208">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-209">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="ac286-209">customData</span></span>|<span data-ttu-id="ac286-210">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="ac286-211">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="ac286-211">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ac286-212">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="ac286-212">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="ac286-213">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="ac286-213">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="ac286-214">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="ac286-214">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="ac286-215">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-216">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="ac286-216">customKeyValueData</span></span>|<span data-ttu-id="ac286-217">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ac286-218">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="ac286-218">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ac286-219">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="ac286-219">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="ac286-220">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="ac286-220">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="ac286-221">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="ac286-221">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="ac286-222">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-222">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-223">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="ac286-223">enableSplitTunneling</span></span>|<span data-ttu-id="ac286-224">Логический</span><span class="sxs-lookup"><span data-stu-id="ac286-224">Boolean</span></span>|<span data-ttu-id="ac286-225">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="ac286-225">Send all network traffic through VPN.</span></span> <span data-ttu-id="ac286-226">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-226">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-227">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="ac286-227">authenticationMethod</span></span>|[<span data-ttu-id="ac286-228">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="ac286-228">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="ac286-229">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="ac286-229">Authentication method for this VPN connection.</span></span> <span data-ttu-id="ac286-230">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac286-230">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="ac286-231">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="ac286-231">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="ac286-232">енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="ac286-232">enablePerApp</span></span>|<span data-ttu-id="ac286-233">Логический</span><span class="sxs-lookup"><span data-stu-id="ac286-233">Boolean</span></span>|<span data-ttu-id="ac286-234">Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ac286-234">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="ac286-235">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-235">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-236">сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="ac286-236">safariDomains</span></span>|<span data-ttu-id="ac286-237">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ac286-237">String collection</span></span>|<span data-ttu-id="ac286-238">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="ac286-238">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="ac286-239">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="ac286-239">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="ac286-240">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-240">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-241">ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="ac286-241">onDemandRules</span></span>|<span data-ttu-id="ac286-242">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="ac286-243">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="ac286-243">On-Demand Rules.</span></span> <span data-ttu-id="ac286-244">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ac286-244">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ac286-245">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-245">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-246">проксисервер</span><span class="sxs-lookup"><span data-stu-id="ac286-246">proxyServer</span></span>|[<span data-ttu-id="ac286-247">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="ac286-247">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="ac286-248">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="ac286-248">Proxy Server.</span></span> <span data-ttu-id="ac286-249">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-249">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-250">оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="ac286-250">optInToDeviceIdSharing</span></span>|<span data-ttu-id="ac286-251">Логический</span><span class="sxs-lookup"><span data-stu-id="ac286-251">Boolean</span></span>|<span data-ttu-id="ac286-252">Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="ac286-252">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="ac286-253">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-253">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-254">providerType</span><span class="sxs-lookup"><span data-stu-id="ac286-254">providerType</span></span>|[<span data-ttu-id="ac286-255">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="ac286-255">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="ac286-256">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="ac286-256">Provider type for per-app VPN.</span></span> <span data-ttu-id="ac286-257">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac286-257">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="ac286-258">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="ac286-258">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="ac286-259">userDomain</span><span class="sxs-lookup"><span data-stu-id="ac286-259">userDomain</span></span>|<span data-ttu-id="ac286-260">String</span><span class="sxs-lookup"><span data-stu-id="ac286-260">String</span></span>|<span data-ttu-id="ac286-261">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="ac286-261">Zscaler only.</span></span> <span data-ttu-id="ac286-262">Введите статический домен для предварительного заполнения поля Login в приложении Зскалер.</span><span class="sxs-lookup"><span data-stu-id="ac286-262">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="ac286-263">Если оставить это поле пустым, вместо этого будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="ac286-263">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="ac286-264">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-264">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-265">стриктенфорцемент</span><span class="sxs-lookup"><span data-stu-id="ac286-265">strictEnforcement</span></span>|<span data-ttu-id="ac286-266">Логический</span><span class="sxs-lookup"><span data-stu-id="ac286-266">Boolean</span></span>|<span data-ttu-id="ac286-267">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="ac286-267">Zscaler only.</span></span> <span data-ttu-id="ac286-268">Блокирует сетевой трафик до тех пор, пока пользователь не войдет в приложение Зскалер.</span><span class="sxs-lookup"><span data-stu-id="ac286-268">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="ac286-269">"True" означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="ac286-269">"True" means traffic is blocked.</span></span> <span data-ttu-id="ac286-270">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-270">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-271">клауднаме</span><span class="sxs-lookup"><span data-stu-id="ac286-271">cloudName</span></span>|<span data-ttu-id="ac286-272">String</span><span class="sxs-lookup"><span data-stu-id="ac286-272">String</span></span>|<span data-ttu-id="ac286-273">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="ac286-273">Zscaler only.</span></span> <span data-ttu-id="ac286-274">Облако зскалер, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="ac286-274">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="ac286-275">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-275">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-276">excludeList</span><span class="sxs-lookup"><span data-stu-id="ac286-276">excludeList</span></span>|<span data-ttu-id="ac286-277">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ac286-277">String collection</span></span>|<span data-ttu-id="ac286-278">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="ac286-278">Zscaler only.</span></span> <span data-ttu-id="ac286-279">Список сетевых адресов, которые не отправляются через облако Зскалер.</span><span class="sxs-lookup"><span data-stu-id="ac286-279">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="ac286-280">Наследуется от [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac286-280">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ac286-281">чилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="ac286-281">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="ac286-282">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="ac286-282">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="ac286-283">Дочерние параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="ac286-283">Child Security Association Parameters</span></span>|
|<span data-ttu-id="ac286-284">клиентаусентикатионтипе</span><span class="sxs-lookup"><span data-stu-id="ac286-284">clientAuthenticationType</span></span>|[<span data-ttu-id="ac286-285">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="ac286-285">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="ac286-286">Тип проверки подлинности клиента, который будет использоваться VPN-клиентом.</span><span class="sxs-lookup"><span data-stu-id="ac286-286">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="ac286-287">Возможные значения: `userAuthentication`, `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="ac286-287">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="ac286-288">деадпирдетектионрате</span><span class="sxs-lookup"><span data-stu-id="ac286-288">deadPeerDetectionRate</span></span>|[<span data-ttu-id="ac286-289">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="ac286-289">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="ac286-290">Определите, как часто следует проверять, активен ли одноранговый сеанс.</span><span class="sxs-lookup"><span data-stu-id="ac286-290">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="ac286-291">.</span><span class="sxs-lookup"><span data-stu-id="ac286-291"></span></span> <span data-ttu-id="ac286-292">Возможные значения: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="ac286-292">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="ac286-293">дисаблемобилитяндмултихоминг</span><span class="sxs-lookup"><span data-stu-id="ac286-293">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="ac286-294">Логический</span><span class="sxs-lookup"><span data-stu-id="ac286-294">Boolean</span></span>|<span data-ttu-id="ac286-295">Отключение МОБИКЕ</span><span class="sxs-lookup"><span data-stu-id="ac286-295">Disable MOBIKE</span></span>|
|<span data-ttu-id="ac286-296">дисаблередирект</span><span class="sxs-lookup"><span data-stu-id="ac286-296">disableRedirect</span></span>|<span data-ttu-id="ac286-297">Логический</span><span class="sxs-lookup"><span data-stu-id="ac286-297">Boolean</span></span>|<span data-ttu-id="ac286-298">Отключение перенаправления</span><span class="sxs-lookup"><span data-stu-id="ac286-298">Disable Redirect</span></span>|
|<span data-ttu-id="ac286-299">енаблецертификатеревокатиончекк</span><span class="sxs-lookup"><span data-stu-id="ac286-299">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="ac286-300">Логический</span><span class="sxs-lookup"><span data-stu-id="ac286-300">Boolean</span></span>|<span data-ttu-id="ac286-301">Включает проверку отзывов и действий. время ожидания отклика сервера не приведет к сбою</span><span class="sxs-lookup"><span data-stu-id="ac286-301">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="ac286-302">енаблиап</span><span class="sxs-lookup"><span data-stu-id="ac286-302">enableEAP</span></span>|<span data-ttu-id="ac286-303">Логический</span><span class="sxs-lookup"><span data-stu-id="ac286-303">Boolean</span></span>|<span data-ttu-id="ac286-304">Включает проверку подлинности только EAP</span><span class="sxs-lookup"><span data-stu-id="ac286-304">Enables EAP only authentication</span></span>|
|<span data-ttu-id="ac286-305">енаблеперфектфорвардсекреци</span><span class="sxs-lookup"><span data-stu-id="ac286-305">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="ac286-306">Логический</span><span class="sxs-lookup"><span data-stu-id="ac286-306">Boolean</span></span>|<span data-ttu-id="ac286-307">Включить безопасную пересылку (PFS).</span><span class="sxs-lookup"><span data-stu-id="ac286-307">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="ac286-308">енаблеусеинтерналсубнетаттрибутес</span><span class="sxs-lookup"><span data-stu-id="ac286-308">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="ac286-309">Логический</span><span class="sxs-lookup"><span data-stu-id="ac286-309">Boolean</span></span>|<span data-ttu-id="ac286-310">Включите использование атрибутов внутренней подсети.</span><span class="sxs-lookup"><span data-stu-id="ac286-310">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="ac286-311">локалидентифиер</span><span class="sxs-lookup"><span data-stu-id="ac286-311">localIdentifier</span></span>|[<span data-ttu-id="ac286-312">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="ac286-312">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="ac286-313">Метод идентификации клиента, который пытается подключиться через VPN.</span><span class="sxs-lookup"><span data-stu-id="ac286-313">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="ac286-314">.</span><span class="sxs-lookup"><span data-stu-id="ac286-314"></span></span> <span data-ttu-id="ac286-315">Возможные значения: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="ac286-315">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="ac286-316">ремотеидентифиер</span><span class="sxs-lookup"><span data-stu-id="ac286-316">remoteIdentifier</span></span>|<span data-ttu-id="ac286-317">String</span><span class="sxs-lookup"><span data-stu-id="ac286-317">String</span></span>|<span data-ttu-id="ac286-318">Адрес сервера IKEv2.</span><span class="sxs-lookup"><span data-stu-id="ac286-318">Address of the IKEv2 server.</span></span> <span data-ttu-id="ac286-319">Должно быть полным доменным именем, Усерфкдн, сетевым адресом или ASN1DN</span><span class="sxs-lookup"><span data-stu-id="ac286-319">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="ac286-320">секуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="ac286-320">securityAssociationParameters</span></span>|[<span data-ttu-id="ac286-321">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="ac286-321">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="ac286-322">Параметры сопоставления безопасности</span><span class="sxs-lookup"><span data-stu-id="ac286-322">Security Association Parameters</span></span>|
|<span data-ttu-id="ac286-323">серверцертификатекоммоннаме</span><span class="sxs-lookup"><span data-stu-id="ac286-323">serverCertificateCommonName</span></span>|<span data-ttu-id="ac286-324">String</span><span class="sxs-lookup"><span data-stu-id="ac286-324">String</span></span>|<span data-ttu-id="ac286-325">Общее имя сертификата сервера IKEv2, используемого при проверке подлинности сервера</span><span class="sxs-lookup"><span data-stu-id="ac286-325">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="ac286-326">серверцертификатеиссуеркоммоннаме</span><span class="sxs-lookup"><span data-stu-id="ac286-326">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="ac286-327">String</span><span class="sxs-lookup"><span data-stu-id="ac286-327">String</span></span>|<span data-ttu-id="ac286-328">Общее имя поставщика сертификата сервера IKEv2, используемого при проверке подлинности</span><span class="sxs-lookup"><span data-stu-id="ac286-328">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="ac286-329">серверцертификатетипе</span><span class="sxs-lookup"><span data-stu-id="ac286-329">serverCertificateType</span></span>|[<span data-ttu-id="ac286-330">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="ac286-330">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="ac286-331">Тип сертификата, который VPN-сервер будет предоставлять VPN-клиенту для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ac286-331">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="ac286-332">Возможные значения: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="ac286-332">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="ac286-333">шаредсекрет</span><span class="sxs-lookup"><span data-stu-id="ac286-333">sharedSecret</span></span>|<span data-ttu-id="ac286-334">String</span><span class="sxs-lookup"><span data-stu-id="ac286-334">String</span></span>|<span data-ttu-id="ac286-335">Используется, когда выбрана общая секретная проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="ac286-335">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="ac286-336">тлсмаксимумверсион</span><span class="sxs-lookup"><span data-stu-id="ac286-336">tlsMaximumVersion</span></span>|<span data-ttu-id="ac286-337">String</span><span class="sxs-lookup"><span data-stu-id="ac286-337">String</span></span>|<span data-ttu-id="ac286-338">Максимальная версия TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="ac286-338">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="ac286-339">тлсминимумверсион</span><span class="sxs-lookup"><span data-stu-id="ac286-339">tlsMinimumVersion</span></span>|<span data-ttu-id="ac286-340">String</span><span class="sxs-lookup"><span data-stu-id="ac286-340">String</span></span>|<span data-ttu-id="ac286-341">Минимальная версия протокола TLS, используемая для проверки подлинности EAP – TLS</span><span class="sxs-lookup"><span data-stu-id="ac286-341">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="ac286-342">алловдефаултсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="ac286-342">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="ac286-343">Логический</span><span class="sxs-lookup"><span data-stu-id="ac286-343">Boolean</span></span>|<span data-ttu-id="ac286-344">Разрешает использование параметров сопоставления безопасности путем установки всех параметров для устройства по умолчанию, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="ac286-344">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="ac286-345">алловдефаултчилдсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="ac286-345">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="ac286-346">Логический</span><span class="sxs-lookup"><span data-stu-id="ac286-346">Boolean</span></span>|<span data-ttu-id="ac286-347">Разрешает использование параметров дочернего сопоставления безопасности, устанавливая все параметры по умолчанию устройства, если явно не указано иное.</span><span class="sxs-lookup"><span data-stu-id="ac286-347">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|



## <a name="response"></a><span data-ttu-id="ac286-348">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac286-348">Response</span></span>
<span data-ttu-id="ac286-349">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ac286-349">If successful, this method returns a `200 OK` response code and an updated [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac286-350">Пример</span><span class="sxs-lookup"><span data-stu-id="ac286-350">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac286-351">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac286-351">Request</span></span>
<span data-ttu-id="ac286-352">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac286-352">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4232

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
  "allowDefaultChildSecurityAssociationParameters": true
}
```

### <a name="response"></a><span data-ttu-id="ac286-353">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac286-353">Response</span></span>
<span data-ttu-id="ac286-p139">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ac286-p139">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4404

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
  "allowDefaultChildSecurityAssociationParameters": true
}
```






