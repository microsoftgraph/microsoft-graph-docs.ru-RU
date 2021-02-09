---
title: Обновление iosikEv2VpnConfiguration
description: Обновление свойств объекта iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b7ad685e3bf5340e3026b5f3ccd07b217c809856
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156051"
---
# <a name="update-iosikev2vpnconfiguration"></a><span data-ttu-id="41115-103">Обновление iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="41115-103">Update iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="41115-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41115-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41115-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41115-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41115-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="41115-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41115-107">Обновление свойств объекта [iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-107">Update the properties of a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41115-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="41115-108">Prerequisites</span></span>
<span data-ttu-id="41115-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41115-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41115-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41115-111">Permission type</span></span>|<span data-ttu-id="41115-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="41115-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41115-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41115-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41115-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41115-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41115-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41115-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41115-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41115-116">Not supported.</span></span>|
|<span data-ttu-id="41115-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41115-117">Application</span></span>|<span data-ttu-id="41115-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41115-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41115-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41115-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="41115-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="41115-120">Request headers</span></span>
|<span data-ttu-id="41115-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41115-121">Header</span></span>|<span data-ttu-id="41115-122">Значение</span><span class="sxs-lookup"><span data-stu-id="41115-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41115-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41115-123">Authorization</span></span>|<span data-ttu-id="41115-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41115-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41115-125">Accept</span><span class="sxs-lookup"><span data-stu-id="41115-125">Accept</span></span>|<span data-ttu-id="41115-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41115-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41115-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41115-127">Request body</span></span>
<span data-ttu-id="41115-128">В теле запроса предоставляем представление объекта [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="41115-128">In the request body, supply a JSON representation for the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

<span data-ttu-id="41115-129">В следующей таблице показаны свойства, необходимые при создании [iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-129">The following table shows the properties that are required when you create the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span></span>

|<span data-ttu-id="41115-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="41115-130">Property</span></span>|<span data-ttu-id="41115-131">Тип</span><span class="sxs-lookup"><span data-stu-id="41115-131">Type</span></span>|<span data-ttu-id="41115-132">Описание</span><span class="sxs-lookup"><span data-stu-id="41115-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41115-133">id</span><span class="sxs-lookup"><span data-stu-id="41115-133">id</span></span>|<span data-ttu-id="41115-134">String</span><span class="sxs-lookup"><span data-stu-id="41115-134">String</span></span>|<span data-ttu-id="41115-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="41115-135">Key of the entity.</span></span> <span data-ttu-id="41115-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41115-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41115-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41115-137">lastModifiedDateTime</span></span>|<span data-ttu-id="41115-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41115-138">DateTimeOffset</span></span>|<span data-ttu-id="41115-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="41115-139">DateTime the object was last modified.</span></span> <span data-ttu-id="41115-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41115-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41115-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="41115-141">roleScopeTagIds</span></span>|<span data-ttu-id="41115-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="41115-142">String collection</span></span>|<span data-ttu-id="41115-143">Список тегов области для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="41115-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="41115-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41115-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41115-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="41115-145">supportsScopeTags</span></span>|<span data-ttu-id="41115-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="41115-146">Boolean</span></span>|<span data-ttu-id="41115-147">Указывает, поддерживает ли конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="41115-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="41115-148">Назначение свойству ScopeTags запрещено, если это значение имеет значение false, а сущности не будут видны пользователям с заданной областью действия.</span><span class="sxs-lookup"><span data-stu-id="41115-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="41115-149">Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить, удавшись и повторно создав политику на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="41115-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="41115-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41115-150">This property is read-only.</span></span> <span data-ttu-id="41115-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41115-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41115-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="41115-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="41115-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="41115-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="41115-154">Применимость выпуска ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="41115-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="41115-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41115-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41115-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="41115-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="41115-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="41115-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="41115-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="41115-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="41115-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41115-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41115-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="41115-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="41115-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="41115-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="41115-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="41115-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="41115-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41115-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41115-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41115-164">createdDateTime</span></span>|<span data-ttu-id="41115-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41115-165">DateTimeOffset</span></span>|<span data-ttu-id="41115-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="41115-166">DateTime the object was created.</span></span> <span data-ttu-id="41115-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41115-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41115-168">description</span><span class="sxs-lookup"><span data-stu-id="41115-168">description</span></span>|<span data-ttu-id="41115-169">String</span><span class="sxs-lookup"><span data-stu-id="41115-169">String</span></span>|<span data-ttu-id="41115-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="41115-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="41115-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41115-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41115-172">displayName</span><span class="sxs-lookup"><span data-stu-id="41115-172">displayName</span></span>|<span data-ttu-id="41115-173">String</span><span class="sxs-lookup"><span data-stu-id="41115-173">String</span></span>|<span data-ttu-id="41115-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="41115-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="41115-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41115-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41115-176">version</span><span class="sxs-lookup"><span data-stu-id="41115-176">version</span></span>|<span data-ttu-id="41115-177">Int32</span><span class="sxs-lookup"><span data-stu-id="41115-177">Int32</span></span>|<span data-ttu-id="41115-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="41115-178">Version of the device configuration.</span></span> <span data-ttu-id="41115-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41115-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41115-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="41115-180">connectionName</span></span>|<span data-ttu-id="41115-181">String</span><span class="sxs-lookup"><span data-stu-id="41115-181">String</span></span>|<span data-ttu-id="41115-182">Имя подключения, отображаемая для пользователя.</span><span class="sxs-lookup"><span data-stu-id="41115-182">Connection name displayed to the user.</span></span> <span data-ttu-id="41115-183">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="41115-184">connectionType</span></span>|[<span data-ttu-id="41115-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="41115-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="41115-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="41115-186">Connection type.</span></span> <span data-ttu-id="41115-187">Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="41115-188">Возможные значения: `ciscoAnyConnect` , , , , , , , `pulseSecure` , , `f5EdgeClient` , `dellSonicWallMobileConnect` , , , `checkPointCapsuleVpn` , `customVpn` , , `ciscoIPSec` `citrix` `ciscoAnyConnectV2` , `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` .</span><span class="sxs-lookup"><span data-stu-id="41115-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="41115-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="41115-189">loginGroupOrDomain</span></span>|<span data-ttu-id="41115-190">String</span><span class="sxs-lookup"><span data-stu-id="41115-190">String</span></span>|<span data-ttu-id="41115-191">Группа входа или домен, если для типа подключения установлено мобильное подключение Dell SonicWALL.</span><span class="sxs-lookup"><span data-stu-id="41115-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="41115-192">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-193">role</span><span class="sxs-lookup"><span data-stu-id="41115-193">role</span></span>|<span data-ttu-id="41115-194">String</span><span class="sxs-lookup"><span data-stu-id="41115-194">String</span></span>|<span data-ttu-id="41115-195">Роль, если для типа подключения установлено значение Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="41115-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="41115-196">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-197">realm</span><span class="sxs-lookup"><span data-stu-id="41115-197">realm</span></span>|<span data-ttu-id="41115-198">String</span><span class="sxs-lookup"><span data-stu-id="41115-198">String</span></span>|<span data-ttu-id="41115-199">Область, когда для типа подключения установлено "Pulse Secure".</span><span class="sxs-lookup"><span data-stu-id="41115-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="41115-200">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-201">server</span><span class="sxs-lookup"><span data-stu-id="41115-201">server</span></span>|[<span data-ttu-id="41115-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="41115-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="41115-203">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="41115-203">VPN Server on the network.</span></span> <span data-ttu-id="41115-204">Убедитесь, что конечные пользователи могут получить доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="41115-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="41115-205">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="41115-206">identifier</span></span>|<span data-ttu-id="41115-207">String</span><span class="sxs-lookup"><span data-stu-id="41115-207">String</span></span>|<span data-ttu-id="41115-208">Идентификатор, предоставляемый поставщиком VPN, если для типа подключения за установлено настраиваемого VPN.</span><span class="sxs-lookup"><span data-stu-id="41115-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="41115-209">Например: Cisco AnyConnect использует идентификатор формы com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-210">customData</span><span class="sxs-lookup"><span data-stu-id="41115-210">customData</span></span>|<span data-ttu-id="41115-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="41115-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="41115-212">Пользовательские данные, если для типа подключения установлено настраиваемая VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="41115-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="41115-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в вашем VPN-решении.</span><span class="sxs-lookup"><span data-stu-id="41115-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="41115-214">Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="41115-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="41115-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="41115-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="41115-216">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="41115-217">customKeyValueData</span></span>|<span data-ttu-id="41115-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="41115-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="41115-219">Пользовательские данные, если для типа подключения установлено настраиваемая VPN-сеть.</span><span class="sxs-lookup"><span data-stu-id="41115-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="41115-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в vpn-решении.</span><span class="sxs-lookup"><span data-stu-id="41115-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="41115-221">Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="41115-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="41115-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="41115-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="41115-223">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="41115-224">enableSplitTunneling</span></span>|<span data-ttu-id="41115-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="41115-225">Boolean</span></span>|<span data-ttu-id="41115-226">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="41115-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="41115-227">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="41115-228">authenticationMethod</span></span>|[<span data-ttu-id="41115-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="41115-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="41115-230">Метод проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="41115-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="41115-231">Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="41115-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="41115-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="41115-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="41115-233">enablePerApp</span></span>|<span data-ttu-id="41115-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="41115-234">Boolean</span></span>|<span data-ttu-id="41115-235">Если установить для этого параметра Per-App vpn, которые впоследствии могут быть связаны с приложениями, которые могут активирует этот коннекциатор VPN на устройстве пользователя с iOS.</span><span class="sxs-lookup"><span data-stu-id="41115-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="41115-236">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="41115-237">safariDomains</span></span>|<span data-ttu-id="41115-238">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="41115-238">String collection</span></span>|<span data-ttu-id="41115-239">Домены Safari, если этот параметр VPN для каждого приложения включен.</span><span class="sxs-lookup"><span data-stu-id="41115-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="41115-240">Помимо приложений, связанных с этим VPN, указанные здесь домены Safari также смогут запускать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="41115-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="41115-241">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="41115-242">onDemandRules</span></span>|<span data-ttu-id="41115-243">[Коллекция vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="41115-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="41115-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="41115-244">On-Demand Rules.</span></span> <span data-ttu-id="41115-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="41115-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="41115-246">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-247">providerType</span><span class="sxs-lookup"><span data-stu-id="41115-247">providerType</span></span>|[<span data-ttu-id="41115-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="41115-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="41115-249">Тип поставщика для VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="41115-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="41115-250">Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="41115-251">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="41115-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="41115-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="41115-252">associatedDomains</span></span>|<span data-ttu-id="41115-253">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="41115-253">String collection</span></span>|<span data-ttu-id="41115-254">Связанные домены, унаследованные от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="41115-255">excludedDomains</span></span>|<span data-ttu-id="41115-256">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="41115-256">String collection</span></span>|<span data-ttu-id="41115-257">Домены, которые доступны через общедоступный Интернет, а не через VPN, даже если активирован VPN для каждого приложения. Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="41115-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="41115-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="41115-259">Boolean</span></span>|<span data-ttu-id="41115-260">Переключение, чтобы запретить пользователю отключать автоматическую VPN-сеть в приложении "Параметры". Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-261">proxyServer</span><span class="sxs-lookup"><span data-stu-id="41115-261">proxyServer</span></span>|[<span data-ttu-id="41115-262">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="41115-262">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="41115-263">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="41115-263">Proxy Server.</span></span> <span data-ttu-id="41115-264">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-264">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-265">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="41115-265">optInToDeviceIdSharing</span></span>|<span data-ttu-id="41115-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="41115-266">Boolean</span></span>|<span data-ttu-id="41115-267">Opt-In к совместному использованию удостоверения устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="41115-267">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="41115-268">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-268">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-269">userDomain</span><span class="sxs-lookup"><span data-stu-id="41115-269">userDomain</span></span>|<span data-ttu-id="41115-270">String</span><span class="sxs-lookup"><span data-stu-id="41115-270">String</span></span>|<span data-ttu-id="41115-271">Только Zscaler.</span><span class="sxs-lookup"><span data-stu-id="41115-271">Zscaler only.</span></span> <span data-ttu-id="41115-272">Введите статический домен для предварительного заполнения поля входа в приложение Zscaler.</span><span class="sxs-lookup"><span data-stu-id="41115-272">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="41115-273">Если оставить его пустым, будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="41115-273">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="41115-274">Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-274">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-275">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="41115-275">strictEnforcement</span></span>|<span data-ttu-id="41115-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="41115-276">Boolean</span></span>|<span data-ttu-id="41115-277">Только Zscaler.</span><span class="sxs-lookup"><span data-stu-id="41115-277">Zscaler only.</span></span> <span data-ttu-id="41115-278">Блокирует сетевой трафик, пока пользователь не войди в приложение Zscaler.</span><span class="sxs-lookup"><span data-stu-id="41115-278">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="41115-279">"True" означает, что трафик заблокирован.</span><span class="sxs-lookup"><span data-stu-id="41115-279">"True" means traffic is blocked.</span></span> <span data-ttu-id="41115-280">Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-280">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-281">cloudName</span><span class="sxs-lookup"><span data-stu-id="41115-281">cloudName</span></span>|<span data-ttu-id="41115-282">String</span><span class="sxs-lookup"><span data-stu-id="41115-282">String</span></span>|<span data-ttu-id="41115-283">Только Zscaler.</span><span class="sxs-lookup"><span data-stu-id="41115-283">Zscaler only.</span></span> <span data-ttu-id="41115-284">Облако Zscaler, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="41115-284">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="41115-285">Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-285">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-286">excludeList</span><span class="sxs-lookup"><span data-stu-id="41115-286">excludeList</span></span>|<span data-ttu-id="41115-287">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="41115-287">String collection</span></span>|<span data-ttu-id="41115-288">Только Zscaler.</span><span class="sxs-lookup"><span data-stu-id="41115-288">Zscaler only.</span></span> <span data-ttu-id="41115-289">Список сетевых адресов, которые не отправляются через облако Zscaler.</span><span class="sxs-lookup"><span data-stu-id="41115-289">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="41115-290">Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-290">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-291">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="41115-291">targetedMobileApps</span></span>|<span data-ttu-id="41115-292">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="41115-292">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="41115-293">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="41115-293">Targeted mobile apps.</span></span> <span data-ttu-id="41115-294">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="41115-294">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="41115-295">Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-295">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-296">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="41115-296">microsoftTunnelSiteId</span></span>|<span data-ttu-id="41115-297">String</span><span class="sxs-lookup"><span data-stu-id="41115-297">String</span></span>|<span data-ttu-id="41115-298">Microsoft Tunnel site ID.</span><span class="sxs-lookup"><span data-stu-id="41115-298">Microsoft Tunnel site ID.</span></span> <span data-ttu-id="41115-299">Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41115-299">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="41115-300">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="41115-300">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="41115-301">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="41115-301">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="41115-302">Параметры связи между безопасностью и безопасностью</span><span class="sxs-lookup"><span data-stu-id="41115-302">Child Security Association Parameters</span></span>|
|<span data-ttu-id="41115-303">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="41115-303">clientAuthenticationType</span></span>|[<span data-ttu-id="41115-304">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="41115-304">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="41115-305">Тип проверки подлинности клиента, который будет использовать VPN-клиент.</span><span class="sxs-lookup"><span data-stu-id="41115-305">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="41115-306">Возможные значения: `userAuthentication`, `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="41115-306">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="41115-307">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="41115-307">deadPeerDetectionRate</span></span>|[<span data-ttu-id="41115-308">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="41115-308">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="41115-309">Определите, как часто проверяется активность одноранговых подключений.</span><span class="sxs-lookup"><span data-stu-id="41115-309">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="41115-310">.</span><span class="sxs-lookup"><span data-stu-id="41115-310">.</span></span> <span data-ttu-id="41115-311">Возможные значения: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="41115-311">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="41115-312">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="41115-312">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="41115-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="41115-313">Boolean</span></span>|<span data-ttu-id="41115-314">Отключение MOBIKE</span><span class="sxs-lookup"><span data-stu-id="41115-314">Disable MOBIKE</span></span>|
|<span data-ttu-id="41115-315">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="41115-315">disableRedirect</span></span>|<span data-ttu-id="41115-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="41115-316">Boolean</span></span>|<span data-ttu-id="41115-317">Отключение перенаправления</span><span class="sxs-lookup"><span data-stu-id="41115-317">Disable Redirect</span></span>|
|<span data-ttu-id="41115-318">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="41115-318">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="41115-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="41115-319">Boolean</span></span>|<span data-ttu-id="41115-320">Включает проверку отзыва с наилучшими усилиями; Время отклика сервера не приведет к сбойу</span><span class="sxs-lookup"><span data-stu-id="41115-320">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="41115-321">enableEAP</span><span class="sxs-lookup"><span data-stu-id="41115-321">enableEAP</span></span>|<span data-ttu-id="41115-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="41115-322">Boolean</span></span>|<span data-ttu-id="41115-323">Включает только проверку подлинности EAP</span><span class="sxs-lookup"><span data-stu-id="41115-323">Enables EAP only authentication</span></span>|
|<span data-ttu-id="41115-324">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="41115-324">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="41115-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="41115-325">Boolean</span></span>|<span data-ttu-id="41115-326">Включить PFS.</span><span class="sxs-lookup"><span data-stu-id="41115-326">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="41115-327">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="41115-327">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="41115-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="41115-328">Boolean</span></span>|<span data-ttu-id="41115-329">Включить использование атрибутов внутренней подсети.</span><span class="sxs-lookup"><span data-stu-id="41115-329">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="41115-330">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="41115-330">localIdentifier</span></span>|[<span data-ttu-id="41115-331">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="41115-331">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="41115-332">Способ идентификации клиента, который пытается подключиться через VPN.</span><span class="sxs-lookup"><span data-stu-id="41115-332">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="41115-333">.</span><span class="sxs-lookup"><span data-stu-id="41115-333">.</span></span> <span data-ttu-id="41115-334">Возможные значения: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="41115-334">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="41115-335">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="41115-335">remoteIdentifier</span></span>|<span data-ttu-id="41115-336">String</span><span class="sxs-lookup"><span data-stu-id="41115-336">String</span></span>|<span data-ttu-id="41115-337">Адрес сервера IKEv2.</span><span class="sxs-lookup"><span data-stu-id="41115-337">Address of the IKEv2 server.</span></span> <span data-ttu-id="41115-338">Должно быть FQDN, UserFQDN, сетевой адрес или ASN1DN</span><span class="sxs-lookup"><span data-stu-id="41115-338">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="41115-339">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="41115-339">securityAssociationParameters</span></span>|[<span data-ttu-id="41115-340">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="41115-340">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="41115-341">Параметры ассоциации безопасности</span><span class="sxs-lookup"><span data-stu-id="41115-341">Security Association Parameters</span></span>|
|<span data-ttu-id="41115-342">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="41115-342">serverCertificateCommonName</span></span>|<span data-ttu-id="41115-343">String</span><span class="sxs-lookup"><span data-stu-id="41115-343">String</span></span>|<span data-ttu-id="41115-344">Общее имя сертификата сервера IKEv2, используемого при проверке подлинности сервера</span><span class="sxs-lookup"><span data-stu-id="41115-344">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="41115-345">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="41115-345">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="41115-346">String</span><span class="sxs-lookup"><span data-stu-id="41115-346">String</span></span>|<span data-ttu-id="41115-347">Общее имя выпуска сертификата сервера IKEv2, используемого при проверке подлинности</span><span class="sxs-lookup"><span data-stu-id="41115-347">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="41115-348">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="41115-348">serverCertificateType</span></span>|[<span data-ttu-id="41115-349">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="41115-349">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="41115-350">Тип сертификата, который VPN-сервер будет представлять VPN-клиенту для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="41115-350">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="41115-351">Возможные значения: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="41115-351">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="41115-352">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="41115-352">sharedSecret</span></span>|<span data-ttu-id="41115-353">String</span><span class="sxs-lookup"><span data-stu-id="41115-353">String</span></span>|<span data-ttu-id="41115-354">Используется при выборе проверки подлинности с общим секретом</span><span class="sxs-lookup"><span data-stu-id="41115-354">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="41115-355">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="41115-355">tlsMaximumVersion</span></span>|<span data-ttu-id="41115-356">String</span><span class="sxs-lookup"><span data-stu-id="41115-356">String</span></span>|<span data-ttu-id="41115-357">Максимальная версия TLS, используемая для проверки подлинности EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="41115-357">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="41115-358">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="41115-358">tlsMinimumVersion</span></span>|<span data-ttu-id="41115-359">String</span><span class="sxs-lookup"><span data-stu-id="41115-359">String</span></span>|<span data-ttu-id="41115-360">Минимальная версия TLS, используемая для проверки подлинности EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="41115-360">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="41115-361">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="41115-361">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="41115-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="41115-362">Boolean</span></span>|<span data-ttu-id="41115-363">Разрешает использование параметров связи безопасности, устанавливая для всех параметров значение по умолчанию устройства, если не указано явно.</span><span class="sxs-lookup"><span data-stu-id="41115-363">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="41115-364">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="41115-364">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="41115-365">Boolean</span><span class="sxs-lookup"><span data-stu-id="41115-365">Boolean</span></span>|<span data-ttu-id="41115-366">Разрешает использование параметров связи между безопасностью, устанавливая для всех параметров значение по умолчанию устройства, если не указано явно.</span><span class="sxs-lookup"><span data-stu-id="41115-366">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="41115-367">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="41115-367">alwaysOnConfiguration</span></span>|[<span data-ttu-id="41115-368">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="41115-368">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="41115-369">Конфигурация AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="41115-369">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="41115-370">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="41115-370">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="41115-371">Boolean</span><span class="sxs-lookup"><span data-stu-id="41115-371">Boolean</span></span>|<span data-ttu-id="41115-372">Определяет, включена ли always on VPN</span><span class="sxs-lookup"><span data-stu-id="41115-372">Determines if Always on VPN is enabled</span></span>|
|<span data-ttu-id="41115-373">mtuSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="41115-373">mtuSizeInBytes</span></span>|<span data-ttu-id="41115-374">Int32</span><span class="sxs-lookup"><span data-stu-id="41115-374">Int32</span></span>|<span data-ttu-id="41115-375">Максимальная единица передачи.</span><span class="sxs-lookup"><span data-stu-id="41115-375">Maximum transmission unit.</span></span> <span data-ttu-id="41115-376">Допустимые значения: от 1280 до 1400</span><span class="sxs-lookup"><span data-stu-id="41115-376">Valid values 1280 to 1400</span></span>|



## <a name="response"></a><span data-ttu-id="41115-377">Отклик</span><span class="sxs-lookup"><span data-stu-id="41115-377">Response</span></span>
<span data-ttu-id="41115-378">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="41115-378">If successful, this method returns a `200 OK` response code and an updated [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41115-379">Пример</span><span class="sxs-lookup"><span data-stu-id="41115-379">Example</span></span>

### <a name="request"></a><span data-ttu-id="41115-380">Запрос</span><span class="sxs-lookup"><span data-stu-id="41115-380">Request</span></span>
<span data-ttu-id="41115-381">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41115-381">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 5492

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
  "associatedDomains": [
    "Associated Domains value"
  ],
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

### <a name="response"></a><span data-ttu-id="41115-382">Отклик</span><span class="sxs-lookup"><span data-stu-id="41115-382">Response</span></span>
<span data-ttu-id="41115-p142">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="41115-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5664

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
  "associatedDomains": [
    "Associated Domains value"
  ],
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




