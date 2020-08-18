---
title: Обновление Иосвпнконфигуратион
description: Обновление свойств объекта Иосвпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eaca743801259af26ff414707b07553b142f2e60
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790905"
---
# <a name="update-iosvpnconfiguration"></a><span data-ttu-id="130f5-103">Обновление Иосвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="130f5-103">Update iosVpnConfiguration</span></span>

<span data-ttu-id="130f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="130f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="130f5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="130f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="130f5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="130f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="130f5-107">Обновление свойств объекта [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="130f5-107">Update the properties of a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="130f5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="130f5-108">Prerequisites</span></span>
<span data-ttu-id="130f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="130f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="130f5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="130f5-111">Permission type</span></span>|<span data-ttu-id="130f5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="130f5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="130f5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="130f5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="130f5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="130f5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="130f5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="130f5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="130f5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="130f5-116">Not supported.</span></span>|
|<span data-ttu-id="130f5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="130f5-117">Application</span></span>|<span data-ttu-id="130f5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="130f5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="130f5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="130f5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="130f5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="130f5-120">Request headers</span></span>
|<span data-ttu-id="130f5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="130f5-121">Header</span></span>|<span data-ttu-id="130f5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="130f5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="130f5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="130f5-123">Authorization</span></span>|<span data-ttu-id="130f5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="130f5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="130f5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="130f5-125">Accept</span></span>|<span data-ttu-id="130f5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="130f5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="130f5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="130f5-127">Request body</span></span>
<span data-ttu-id="130f5-128">В тексте запроса добавьте представление объекта [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="130f5-128">In the request body, supply a JSON representation for the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="130f5-129">В следующей таблице приведены свойства, необходимые при создании [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="130f5-129">The following table shows the properties that are required when you create the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span>

|<span data-ttu-id="130f5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="130f5-130">Property</span></span>|<span data-ttu-id="130f5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="130f5-131">Type</span></span>|<span data-ttu-id="130f5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="130f5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="130f5-133">id</span><span class="sxs-lookup"><span data-stu-id="130f5-133">id</span></span>|<span data-ttu-id="130f5-134">String</span><span class="sxs-lookup"><span data-stu-id="130f5-134">String</span></span>|<span data-ttu-id="130f5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="130f5-135">Key of the entity.</span></span> <span data-ttu-id="130f5-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="130f5-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="130f5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="130f5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="130f5-138">DateTimeOffset</span></span>|<span data-ttu-id="130f5-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="130f5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="130f5-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="130f5-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="130f5-141">roleScopeTagIds</span></span>|<span data-ttu-id="130f5-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="130f5-142">String collection</span></span>|<span data-ttu-id="130f5-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="130f5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="130f5-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="130f5-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="130f5-145">supportsScopeTags</span></span>|<span data-ttu-id="130f5-146">Логический</span><span class="sxs-lookup"><span data-stu-id="130f5-146">Boolean</span></span>|<span data-ttu-id="130f5-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="130f5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="130f5-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="130f5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="130f5-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="130f5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="130f5-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="130f5-150">This property is read-only.</span></span> <span data-ttu-id="130f5-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="130f5-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="130f5-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="130f5-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="130f5-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="130f5-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="130f5-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="130f5-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="130f5-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="130f5-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="130f5-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="130f5-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="130f5-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="130f5-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="130f5-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="130f5-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="130f5-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="130f5-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="130f5-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="130f5-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="130f5-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="130f5-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="130f5-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="130f5-164">createdDateTime</span></span>|<span data-ttu-id="130f5-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="130f5-165">DateTimeOffset</span></span>|<span data-ttu-id="130f5-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="130f5-166">DateTime the object was created.</span></span> <span data-ttu-id="130f5-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="130f5-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-168">description</span><span class="sxs-lookup"><span data-stu-id="130f5-168">description</span></span>|<span data-ttu-id="130f5-169">String</span><span class="sxs-lookup"><span data-stu-id="130f5-169">String</span></span>|<span data-ttu-id="130f5-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="130f5-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="130f5-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="130f5-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-172">displayName</span><span class="sxs-lookup"><span data-stu-id="130f5-172">displayName</span></span>|<span data-ttu-id="130f5-173">String</span><span class="sxs-lookup"><span data-stu-id="130f5-173">String</span></span>|<span data-ttu-id="130f5-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="130f5-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="130f5-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="130f5-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-176">version</span><span class="sxs-lookup"><span data-stu-id="130f5-176">version</span></span>|<span data-ttu-id="130f5-177">Int32</span><span class="sxs-lookup"><span data-stu-id="130f5-177">Int32</span></span>|<span data-ttu-id="130f5-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="130f5-178">Version of the device configuration.</span></span> <span data-ttu-id="130f5-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="130f5-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="130f5-180">connectionName</span></span>|<span data-ttu-id="130f5-181">String</span><span class="sxs-lookup"><span data-stu-id="130f5-181">String</span></span>|<span data-ttu-id="130f5-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="130f5-182">Connection name displayed to the user.</span></span> <span data-ttu-id="130f5-183">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="130f5-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="130f5-184">connectionType</span></span>|[<span data-ttu-id="130f5-185">апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="130f5-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="130f5-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="130f5-186">Connection type.</span></span> <span data-ttu-id="130f5-187">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="130f5-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="130f5-188">Возможные значения:,,,,,,,,,, `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` ,, `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` , `paloAltoGlobalProtectV2` , `ikEv2` , `alwaysOn` `microsoftTunnel` `netMotionMobility` ,,.</span><span class="sxs-lookup"><span data-stu-id="130f5-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="130f5-189">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="130f5-189">loginGroupOrDomain</span></span>|<span data-ttu-id="130f5-190">String</span><span class="sxs-lookup"><span data-stu-id="130f5-190">String</span></span>|<span data-ttu-id="130f5-191">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="130f5-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="130f5-192">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="130f5-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-193">role</span><span class="sxs-lookup"><span data-stu-id="130f5-193">role</span></span>|<span data-ttu-id="130f5-194">String</span><span class="sxs-lookup"><span data-stu-id="130f5-194">String</span></span>|<span data-ttu-id="130f5-195">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="130f5-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="130f5-196">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="130f5-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-197">область</span><span class="sxs-lookup"><span data-stu-id="130f5-197">realm</span></span>|<span data-ttu-id="130f5-198">String</span><span class="sxs-lookup"><span data-stu-id="130f5-198">String</span></span>|<span data-ttu-id="130f5-199">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="130f5-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="130f5-200">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="130f5-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-201">сервер</span><span class="sxs-lookup"><span data-stu-id="130f5-201">server</span></span>|[<span data-ttu-id="130f5-202">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="130f5-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="130f5-203">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="130f5-203">VPN Server on the network.</span></span> <span data-ttu-id="130f5-204">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="130f5-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="130f5-205">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="130f5-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="130f5-206">identifier</span></span>|<span data-ttu-id="130f5-207">String</span><span class="sxs-lookup"><span data-stu-id="130f5-207">String</span></span>|<span data-ttu-id="130f5-208">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="130f5-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="130f5-209">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="130f5-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-210">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="130f5-210">customData</span></span>|<span data-ttu-id="130f5-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="130f5-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="130f5-212">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="130f5-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="130f5-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="130f5-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="130f5-214">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="130f5-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="130f5-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="130f5-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="130f5-216">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="130f5-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="130f5-217">customKeyValueData</span></span>|<span data-ttu-id="130f5-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="130f5-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="130f5-219">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="130f5-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="130f5-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="130f5-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="130f5-221">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="130f5-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="130f5-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="130f5-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="130f5-223">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="130f5-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-224">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="130f5-224">enableSplitTunneling</span></span>|<span data-ttu-id="130f5-225">Логический</span><span class="sxs-lookup"><span data-stu-id="130f5-225">Boolean</span></span>|<span data-ttu-id="130f5-226">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="130f5-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="130f5-227">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="130f5-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-228">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="130f5-228">authenticationMethod</span></span>|[<span data-ttu-id="130f5-229">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="130f5-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="130f5-230">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="130f5-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="130f5-231">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="130f5-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="130f5-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="130f5-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="130f5-233">енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="130f5-233">enablePerApp</span></span>|<span data-ttu-id="130f5-234">Логический</span><span class="sxs-lookup"><span data-stu-id="130f5-234">Boolean</span></span>|<span data-ttu-id="130f5-235">Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="130f5-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="130f5-236">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="130f5-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-237">сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="130f5-237">safariDomains</span></span>|<span data-ttu-id="130f5-238">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="130f5-238">String collection</span></span>|<span data-ttu-id="130f5-239">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="130f5-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="130f5-240">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="130f5-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="130f5-241">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="130f5-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-242">ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="130f5-242">onDemandRules</span></span>|<span data-ttu-id="130f5-243">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="130f5-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="130f5-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="130f5-244">On-Demand Rules.</span></span> <span data-ttu-id="130f5-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="130f5-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="130f5-246">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="130f5-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-247">providerType</span><span class="sxs-lookup"><span data-stu-id="130f5-247">providerType</span></span>|[<span data-ttu-id="130f5-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="130f5-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="130f5-249">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="130f5-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="130f5-250">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="130f5-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="130f5-251">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="130f5-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="130f5-252">проксисервер</span><span class="sxs-lookup"><span data-stu-id="130f5-252">proxyServer</span></span>|[<span data-ttu-id="130f5-253">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="130f5-253">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="130f5-254">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="130f5-254">Proxy Server.</span></span> <span data-ttu-id="130f5-255">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="130f5-255">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-256">оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="130f5-256">optInToDeviceIdSharing</span></span>|<span data-ttu-id="130f5-257">Логический</span><span class="sxs-lookup"><span data-stu-id="130f5-257">Boolean</span></span>|<span data-ttu-id="130f5-258">Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="130f5-258">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="130f5-259">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="130f5-259">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="130f5-260">userDomain</span><span class="sxs-lookup"><span data-stu-id="130f5-260">userDomain</span></span>|<span data-ttu-id="130f5-261">String</span><span class="sxs-lookup"><span data-stu-id="130f5-261">String</span></span>|<span data-ttu-id="130f5-262">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="130f5-262">Zscaler only.</span></span> <span data-ttu-id="130f5-263">Введите статический домен для предварительного заполнения поля Login в приложении Зскалер.</span><span class="sxs-lookup"><span data-stu-id="130f5-263">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="130f5-264">Если оставить это поле пустым, вместо этого будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="130f5-264">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="130f5-265">стриктенфорцемент</span><span class="sxs-lookup"><span data-stu-id="130f5-265">strictEnforcement</span></span>|<span data-ttu-id="130f5-266">Логический</span><span class="sxs-lookup"><span data-stu-id="130f5-266">Boolean</span></span>|<span data-ttu-id="130f5-267">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="130f5-267">Zscaler only.</span></span> <span data-ttu-id="130f5-268">Блокирует сетевой трафик до тех пор, пока пользователь не войдет в приложение Зскалер.</span><span class="sxs-lookup"><span data-stu-id="130f5-268">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="130f5-269">"True" означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="130f5-269">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="130f5-270">клауднаме</span><span class="sxs-lookup"><span data-stu-id="130f5-270">cloudName</span></span>|<span data-ttu-id="130f5-271">String</span><span class="sxs-lookup"><span data-stu-id="130f5-271">String</span></span>|<span data-ttu-id="130f5-272">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="130f5-272">Zscaler only.</span></span> <span data-ttu-id="130f5-273">Облако зскалер, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="130f5-273">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="130f5-274">excludeList</span><span class="sxs-lookup"><span data-stu-id="130f5-274">excludeList</span></span>|<span data-ttu-id="130f5-275">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="130f5-275">String collection</span></span>|<span data-ttu-id="130f5-276">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="130f5-276">Zscaler only.</span></span> <span data-ttu-id="130f5-277">Список сетевых адресов, которые не отправляются через облако Зскалер.</span><span class="sxs-lookup"><span data-stu-id="130f5-277">List of network addresses which are not sent through the Zscaler cloud.</span></span>|
|<span data-ttu-id="130f5-278">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="130f5-278">targetedMobileApps</span></span>|<span data-ttu-id="130f5-279">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="130f5-279">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="130f5-280">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="130f5-280">Targeted mobile apps.</span></span> <span data-ttu-id="130f5-281">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="130f5-281">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="130f5-282">Ответ</span><span class="sxs-lookup"><span data-stu-id="130f5-282">Response</span></span>
<span data-ttu-id="130f5-283">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="130f5-283">If successful, this method returns a `200 OK` response code and an updated [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="130f5-284">Пример</span><span class="sxs-lookup"><span data-stu-id="130f5-284">Example</span></span>

### <a name="request"></a><span data-ttu-id="130f5-285">Запрос</span><span class="sxs-lookup"><span data-stu-id="130f5-285">Request</span></span>
<span data-ttu-id="130f5-286">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="130f5-286">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3072

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="130f5-287">Отклик</span><span class="sxs-lookup"><span data-stu-id="130f5-287">Response</span></span>
<span data-ttu-id="130f5-p135">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="130f5-p135">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3244

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
  "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
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
  ]
}
```



