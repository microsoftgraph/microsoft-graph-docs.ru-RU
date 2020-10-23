---
title: Обновление Иосвпнконфигуратион
description: Обновление свойств объекта Иосвпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e815135ee99251d715ae2776b65eb15e9af7bc79
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729238"
---
# <a name="update-iosvpnconfiguration"></a><span data-ttu-id="659c1-103">Обновление Иосвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="659c1-103">Update iosVpnConfiguration</span></span>

<span data-ttu-id="659c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="659c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="659c1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="659c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="659c1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="659c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="659c1-107">Обновление свойств объекта [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="659c1-107">Update the properties of a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="659c1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="659c1-108">Prerequisites</span></span>
<span data-ttu-id="659c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="659c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="659c1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="659c1-111">Permission type</span></span>|<span data-ttu-id="659c1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="659c1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="659c1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="659c1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="659c1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="659c1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="659c1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="659c1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="659c1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="659c1-116">Not supported.</span></span>|
|<span data-ttu-id="659c1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="659c1-117">Application</span></span>|<span data-ttu-id="659c1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="659c1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="659c1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="659c1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="659c1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="659c1-120">Request headers</span></span>
|<span data-ttu-id="659c1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="659c1-121">Header</span></span>|<span data-ttu-id="659c1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="659c1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="659c1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="659c1-123">Authorization</span></span>|<span data-ttu-id="659c1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="659c1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="659c1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="659c1-125">Accept</span></span>|<span data-ttu-id="659c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="659c1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="659c1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="659c1-127">Request body</span></span>
<span data-ttu-id="659c1-128">В тексте запроса добавьте представление объекта [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="659c1-128">In the request body, supply a JSON representation for the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="659c1-129">В следующей таблице приведены свойства, необходимые при создании [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="659c1-129">The following table shows the properties that are required when you create the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span>

|<span data-ttu-id="659c1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="659c1-130">Property</span></span>|<span data-ttu-id="659c1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="659c1-131">Type</span></span>|<span data-ttu-id="659c1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="659c1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="659c1-133">id</span><span class="sxs-lookup"><span data-stu-id="659c1-133">id</span></span>|<span data-ttu-id="659c1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="659c1-134">String</span></span>|<span data-ttu-id="659c1-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="659c1-135">Key of the entity.</span></span> <span data-ttu-id="659c1-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="659c1-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="659c1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="659c1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="659c1-138">DateTimeOffset</span></span>|<span data-ttu-id="659c1-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="659c1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="659c1-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="659c1-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="659c1-141">roleScopeTagIds</span></span>|<span data-ttu-id="659c1-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="659c1-142">String collection</span></span>|<span data-ttu-id="659c1-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="659c1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="659c1-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="659c1-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="659c1-145">supportsScopeTags</span></span>|<span data-ttu-id="659c1-146">Логический</span><span class="sxs-lookup"><span data-stu-id="659c1-146">Boolean</span></span>|<span data-ttu-id="659c1-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="659c1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="659c1-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="659c1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="659c1-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="659c1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="659c1-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="659c1-150">This property is read-only.</span></span> <span data-ttu-id="659c1-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="659c1-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="659c1-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="659c1-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="659c1-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="659c1-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="659c1-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="659c1-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="659c1-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="659c1-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="659c1-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="659c1-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="659c1-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="659c1-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="659c1-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="659c1-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="659c1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="659c1-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="659c1-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="659c1-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="659c1-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="659c1-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="659c1-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="659c1-164">createdDateTime</span></span>|<span data-ttu-id="659c1-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="659c1-165">DateTimeOffset</span></span>|<span data-ttu-id="659c1-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="659c1-166">DateTime the object was created.</span></span> <span data-ttu-id="659c1-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="659c1-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-168">description</span><span class="sxs-lookup"><span data-stu-id="659c1-168">description</span></span>|<span data-ttu-id="659c1-169">Строка</span><span class="sxs-lookup"><span data-stu-id="659c1-169">String</span></span>|<span data-ttu-id="659c1-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="659c1-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="659c1-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="659c1-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-172">displayName</span><span class="sxs-lookup"><span data-stu-id="659c1-172">displayName</span></span>|<span data-ttu-id="659c1-173">Строка</span><span class="sxs-lookup"><span data-stu-id="659c1-173">String</span></span>|<span data-ttu-id="659c1-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="659c1-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="659c1-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="659c1-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-176">version</span><span class="sxs-lookup"><span data-stu-id="659c1-176">version</span></span>|<span data-ttu-id="659c1-177">Int32</span><span class="sxs-lookup"><span data-stu-id="659c1-177">Int32</span></span>|<span data-ttu-id="659c1-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="659c1-178">Version of the device configuration.</span></span> <span data-ttu-id="659c1-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="659c1-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="659c1-180">connectionName</span></span>|<span data-ttu-id="659c1-181">Строка</span><span class="sxs-lookup"><span data-stu-id="659c1-181">String</span></span>|<span data-ttu-id="659c1-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="659c1-182">Connection name displayed to the user.</span></span> <span data-ttu-id="659c1-183">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="659c1-184">connectionType</span></span>|[<span data-ttu-id="659c1-185">апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="659c1-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="659c1-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="659c1-186">Connection type.</span></span> <span data-ttu-id="659c1-187">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="659c1-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="659c1-188">Возможные значения:,,,,,,,,,, `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` ,, `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` , `paloAltoGlobalProtectV2` , `ikEv2` , `alwaysOn` `microsoftTunnel` `netMotionMobility` ,,.</span><span class="sxs-lookup"><span data-stu-id="659c1-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="659c1-189">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="659c1-189">loginGroupOrDomain</span></span>|<span data-ttu-id="659c1-190">Строка</span><span class="sxs-lookup"><span data-stu-id="659c1-190">String</span></span>|<span data-ttu-id="659c1-191">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="659c1-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="659c1-192">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-193">role</span><span class="sxs-lookup"><span data-stu-id="659c1-193">role</span></span>|<span data-ttu-id="659c1-194">Строка</span><span class="sxs-lookup"><span data-stu-id="659c1-194">String</span></span>|<span data-ttu-id="659c1-195">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="659c1-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="659c1-196">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-197">область</span><span class="sxs-lookup"><span data-stu-id="659c1-197">realm</span></span>|<span data-ttu-id="659c1-198">Строка</span><span class="sxs-lookup"><span data-stu-id="659c1-198">String</span></span>|<span data-ttu-id="659c1-199">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="659c1-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="659c1-200">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-201">сервер</span><span class="sxs-lookup"><span data-stu-id="659c1-201">server</span></span>|[<span data-ttu-id="659c1-202">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="659c1-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="659c1-203">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="659c1-203">VPN Server on the network.</span></span> <span data-ttu-id="659c1-204">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="659c1-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="659c1-205">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="659c1-206">identifier</span></span>|<span data-ttu-id="659c1-207">Строка</span><span class="sxs-lookup"><span data-stu-id="659c1-207">String</span></span>|<span data-ttu-id="659c1-208">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="659c1-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="659c1-209">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-210">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="659c1-210">customData</span></span>|<span data-ttu-id="659c1-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="659c1-212">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="659c1-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="659c1-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="659c1-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="659c1-214">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="659c1-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="659c1-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="659c1-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="659c1-216">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="659c1-217">customKeyValueData</span></span>|<span data-ttu-id="659c1-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="659c1-219">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="659c1-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="659c1-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="659c1-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="659c1-221">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="659c1-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="659c1-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="659c1-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="659c1-223">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-224">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="659c1-224">enableSplitTunneling</span></span>|<span data-ttu-id="659c1-225">Логический</span><span class="sxs-lookup"><span data-stu-id="659c1-225">Boolean</span></span>|<span data-ttu-id="659c1-226">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="659c1-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="659c1-227">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-228">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="659c1-228">authenticationMethod</span></span>|[<span data-ttu-id="659c1-229">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="659c1-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="659c1-230">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="659c1-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="659c1-231">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="659c1-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="659c1-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="659c1-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="659c1-233">енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="659c1-233">enablePerApp</span></span>|<span data-ttu-id="659c1-234">Логический</span><span class="sxs-lookup"><span data-stu-id="659c1-234">Boolean</span></span>|<span data-ttu-id="659c1-235">Если задать для этого параметра значение true, будут созданы Per-App полезные данные VPN, которые позже могут быть связаны с приложениями, которые могут запускать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="659c1-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="659c1-236">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-237">сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="659c1-237">safariDomains</span></span>|<span data-ttu-id="659c1-238">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="659c1-238">String collection</span></span>|<span data-ttu-id="659c1-239">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="659c1-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="659c1-240">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="659c1-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="659c1-241">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-242">ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="659c1-242">onDemandRules</span></span>|<span data-ttu-id="659c1-243">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="659c1-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="659c1-244">On-Demand Rules.</span></span> <span data-ttu-id="659c1-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="659c1-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="659c1-246">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-247">providerType</span><span class="sxs-lookup"><span data-stu-id="659c1-247">providerType</span></span>|[<span data-ttu-id="659c1-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="659c1-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="659c1-249">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="659c1-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="659c1-250">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="659c1-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="659c1-251">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="659c1-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="659c1-252">ексклудеддомаинс</span><span class="sxs-lookup"><span data-stu-id="659c1-252">excludedDomains</span></span>|<span data-ttu-id="659c1-253">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="659c1-253">String collection</span></span>|<span data-ttu-id="659c1-254">Домены, доступ к которым осуществляется через общедоступный Интернет, а не через VPN, даже если VPN для каждого приложения активируется наследуемой от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-254">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-255">дисаблеондемандусероверриде</span><span class="sxs-lookup"><span data-stu-id="659c1-255">disableOnDemandUserOverride</span></span>|<span data-ttu-id="659c1-256">Логический</span><span class="sxs-lookup"><span data-stu-id="659c1-256">Boolean</span></span>|<span data-ttu-id="659c1-257">Переключатель, чтобы запретить пользователям отключать автоматическое VPN в приложении "Параметры", унаследованном от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-257">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-258">проксисервер</span><span class="sxs-lookup"><span data-stu-id="659c1-258">proxyServer</span></span>|[<span data-ttu-id="659c1-259">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="659c1-259">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="659c1-260">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="659c1-260">Proxy Server.</span></span> <span data-ttu-id="659c1-261">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-261">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-262">оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="659c1-262">optInToDeviceIdSharing</span></span>|<span data-ttu-id="659c1-263">Логический</span><span class="sxs-lookup"><span data-stu-id="659c1-263">Boolean</span></span>|<span data-ttu-id="659c1-264">Opt-In для предоставления доступа к идентификатору устройства сторонним VPN-клиентам для использования в процессе проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="659c1-264">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="659c1-265">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-265">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="659c1-266">userDomain</span><span class="sxs-lookup"><span data-stu-id="659c1-266">userDomain</span></span>|<span data-ttu-id="659c1-267">Строка</span><span class="sxs-lookup"><span data-stu-id="659c1-267">String</span></span>|<span data-ttu-id="659c1-268">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="659c1-268">Zscaler only.</span></span> <span data-ttu-id="659c1-269">Введите статический домен для предварительного заполнения поля Login в приложении Зскалер.</span><span class="sxs-lookup"><span data-stu-id="659c1-269">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="659c1-270">Если оставить это поле пустым, вместо этого будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="659c1-270">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="659c1-271">стриктенфорцемент</span><span class="sxs-lookup"><span data-stu-id="659c1-271">strictEnforcement</span></span>|<span data-ttu-id="659c1-272">Логический</span><span class="sxs-lookup"><span data-stu-id="659c1-272">Boolean</span></span>|<span data-ttu-id="659c1-273">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="659c1-273">Zscaler only.</span></span> <span data-ttu-id="659c1-274">Блокирует сетевой трафик до тех пор, пока пользователь не войдет в приложение Зскалер.</span><span class="sxs-lookup"><span data-stu-id="659c1-274">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="659c1-275">"True" означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="659c1-275">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="659c1-276">клауднаме</span><span class="sxs-lookup"><span data-stu-id="659c1-276">cloudName</span></span>|<span data-ttu-id="659c1-277">Строка</span><span class="sxs-lookup"><span data-stu-id="659c1-277">String</span></span>|<span data-ttu-id="659c1-278">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="659c1-278">Zscaler only.</span></span> <span data-ttu-id="659c1-279">Облако зскалер, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="659c1-279">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="659c1-280">excludeList</span><span class="sxs-lookup"><span data-stu-id="659c1-280">excludeList</span></span>|<span data-ttu-id="659c1-281">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="659c1-281">String collection</span></span>|<span data-ttu-id="659c1-282">Только зскалер.</span><span class="sxs-lookup"><span data-stu-id="659c1-282">Zscaler only.</span></span> <span data-ttu-id="659c1-283">Список сетевых адресов, которые не отправляются через облако Зскалер.</span><span class="sxs-lookup"><span data-stu-id="659c1-283">List of network addresses which are not sent through the Zscaler cloud.</span></span>|
|<span data-ttu-id="659c1-284">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="659c1-284">targetedMobileApps</span></span>|<span data-ttu-id="659c1-285">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="659c1-285">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="659c1-286">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="659c1-286">Targeted mobile apps.</span></span> <span data-ttu-id="659c1-287">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="659c1-287">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="659c1-288">микрософттуннелситеид</span><span class="sxs-lookup"><span data-stu-id="659c1-288">microsoftTunnelSiteId</span></span>|<span data-ttu-id="659c1-289">Строка</span><span class="sxs-lookup"><span data-stu-id="659c1-289">String</span></span>|<span data-ttu-id="659c1-290">Идентификатор сайта туннеля (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="659c1-290">Microsoft Tunnel site ID.</span></span>|



## <a name="response"></a><span data-ttu-id="659c1-291">Ответ</span><span class="sxs-lookup"><span data-stu-id="659c1-291">Response</span></span>
<span data-ttu-id="659c1-292">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="659c1-292">If successful, this method returns a `200 OK` response code and an updated [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="659c1-293">Пример</span><span class="sxs-lookup"><span data-stu-id="659c1-293">Example</span></span>

### <a name="request"></a><span data-ttu-id="659c1-294">Запрос</span><span class="sxs-lookup"><span data-stu-id="659c1-294">Request</span></span>
<span data-ttu-id="659c1-295">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="659c1-295">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3234

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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```

### <a name="response"></a><span data-ttu-id="659c1-296">Отклик</span><span class="sxs-lookup"><span data-stu-id="659c1-296">Response</span></span>
<span data-ttu-id="659c1-p135">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="659c1-p135">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3406

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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```





