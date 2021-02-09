---
title: Создание iosikEv2VpnConfiguration
description: Создание объекта iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f545a135f7b17978f38b17d32c71718f80e43763
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156079"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="77d9f-103">Создание iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="77d9f-103">Create iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="77d9f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77d9f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77d9f-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77d9f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77d9f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77d9f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77d9f-107">Создание объекта [iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-107">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77d9f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="77d9f-108">Prerequisites</span></span>
<span data-ttu-id="77d9f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77d9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77d9f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77d9f-111">Permission type</span></span>|<span data-ttu-id="77d9f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="77d9f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77d9f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77d9f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77d9f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d9f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77d9f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77d9f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77d9f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77d9f-116">Not supported.</span></span>|
|<span data-ttu-id="77d9f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77d9f-117">Application</span></span>|<span data-ttu-id="77d9f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d9f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77d9f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77d9f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="77d9f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="77d9f-120">Request headers</span></span>
|<span data-ttu-id="77d9f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77d9f-121">Header</span></span>|<span data-ttu-id="77d9f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="77d9f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77d9f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77d9f-123">Authorization</span></span>|<span data-ttu-id="77d9f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77d9f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77d9f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="77d9f-125">Accept</span></span>|<span data-ttu-id="77d9f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77d9f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77d9f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77d9f-127">Request body</span></span>
<span data-ttu-id="77d9f-128">В теле запроса предоставляем представление объекта iosikEv2VpnConfiguration в JSON.</span><span class="sxs-lookup"><span data-stu-id="77d9f-128">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="77d9f-129">В следующей таблице показаны свойства, необходимые при создании объекта iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="77d9f-129">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="77d9f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="77d9f-130">Property</span></span>|<span data-ttu-id="77d9f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="77d9f-131">Type</span></span>|<span data-ttu-id="77d9f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="77d9f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77d9f-133">id</span><span class="sxs-lookup"><span data-stu-id="77d9f-133">id</span></span>|<span data-ttu-id="77d9f-134">String</span><span class="sxs-lookup"><span data-stu-id="77d9f-134">String</span></span>|<span data-ttu-id="77d9f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="77d9f-135">Key of the entity.</span></span> <span data-ttu-id="77d9f-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77d9f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77d9f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="77d9f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77d9f-138">DateTimeOffset</span></span>|<span data-ttu-id="77d9f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="77d9f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="77d9f-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77d9f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="77d9f-141">roleScopeTagIds</span></span>|<span data-ttu-id="77d9f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="77d9f-142">String collection</span></span>|<span data-ttu-id="77d9f-143">Список тегов области для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="77d9f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="77d9f-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77d9f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="77d9f-145">supportsScopeTags</span></span>|<span data-ttu-id="77d9f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="77d9f-146">Boolean</span></span>|<span data-ttu-id="77d9f-147">Указывает, поддерживает ли конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="77d9f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="77d9f-148">Назначение свойству ScopeTags не допускается, если это значение имеет значение false, а сущности не будут видны пользователям с заданной областью действия.</span><span class="sxs-lookup"><span data-stu-id="77d9f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="77d9f-149">Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="77d9f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="77d9f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77d9f-150">This property is read-only.</span></span> <span data-ttu-id="77d9f-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77d9f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="77d9f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="77d9f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="77d9f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="77d9f-154">Применимость выпуска ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="77d9f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="77d9f-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77d9f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="77d9f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="77d9f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="77d9f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="77d9f-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="77d9f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="77d9f-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77d9f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="77d9f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="77d9f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="77d9f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="77d9f-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="77d9f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="77d9f-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77d9f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77d9f-164">createdDateTime</span></span>|<span data-ttu-id="77d9f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77d9f-165">DateTimeOffset</span></span>|<span data-ttu-id="77d9f-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="77d9f-166">DateTime the object was created.</span></span> <span data-ttu-id="77d9f-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77d9f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-168">description</span><span class="sxs-lookup"><span data-stu-id="77d9f-168">description</span></span>|<span data-ttu-id="77d9f-169">String</span><span class="sxs-lookup"><span data-stu-id="77d9f-169">String</span></span>|<span data-ttu-id="77d9f-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="77d9f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="77d9f-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77d9f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="77d9f-172">displayName</span></span>|<span data-ttu-id="77d9f-173">String</span><span class="sxs-lookup"><span data-stu-id="77d9f-173">String</span></span>|<span data-ttu-id="77d9f-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="77d9f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="77d9f-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77d9f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-176">version</span><span class="sxs-lookup"><span data-stu-id="77d9f-176">version</span></span>|<span data-ttu-id="77d9f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="77d9f-177">Int32</span></span>|<span data-ttu-id="77d9f-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="77d9f-178">Version of the device configuration.</span></span> <span data-ttu-id="77d9f-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="77d9f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="77d9f-180">connectionName</span></span>|<span data-ttu-id="77d9f-181">String</span><span class="sxs-lookup"><span data-stu-id="77d9f-181">String</span></span>|<span data-ttu-id="77d9f-182">Имя подключения, отображаемая для пользователя.</span><span class="sxs-lookup"><span data-stu-id="77d9f-182">Connection name displayed to the user.</span></span> <span data-ttu-id="77d9f-183">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="77d9f-184">connectionType</span></span>|[<span data-ttu-id="77d9f-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="77d9f-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="77d9f-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="77d9f-186">Connection type.</span></span> <span data-ttu-id="77d9f-187">Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="77d9f-188">Возможные значения: `ciscoAnyConnect` , , , , , , , `pulseSecure` , , `f5EdgeClient` , `dellSonicWallMobileConnect` , , , `checkPointCapsuleVpn` , `customVpn` , , `ciscoIPSec` `citrix` `ciscoAnyConnectV2` , `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` .</span><span class="sxs-lookup"><span data-stu-id="77d9f-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="77d9f-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="77d9f-189">loginGroupOrDomain</span></span>|<span data-ttu-id="77d9f-190">String</span><span class="sxs-lookup"><span data-stu-id="77d9f-190">String</span></span>|<span data-ttu-id="77d9f-191">Группа входа или домен, если для типа подключения установлено мобильное подключение Dell SonicWALL.</span><span class="sxs-lookup"><span data-stu-id="77d9f-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="77d9f-192">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-193">role</span><span class="sxs-lookup"><span data-stu-id="77d9f-193">role</span></span>|<span data-ttu-id="77d9f-194">String</span><span class="sxs-lookup"><span data-stu-id="77d9f-194">String</span></span>|<span data-ttu-id="77d9f-195">Роль, если для типа подключения установлено значение Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="77d9f-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="77d9f-196">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-197">realm</span><span class="sxs-lookup"><span data-stu-id="77d9f-197">realm</span></span>|<span data-ttu-id="77d9f-198">String</span><span class="sxs-lookup"><span data-stu-id="77d9f-198">String</span></span>|<span data-ttu-id="77d9f-199">Область, когда для типа подключения установлено "Pulse Secure".</span><span class="sxs-lookup"><span data-stu-id="77d9f-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="77d9f-200">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-201">server</span><span class="sxs-lookup"><span data-stu-id="77d9f-201">server</span></span>|[<span data-ttu-id="77d9f-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="77d9f-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="77d9f-203">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="77d9f-203">VPN Server on the network.</span></span> <span data-ttu-id="77d9f-204">Убедитесь, что конечные пользователи могут получить доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="77d9f-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="77d9f-205">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="77d9f-206">identifier</span></span>|<span data-ttu-id="77d9f-207">String</span><span class="sxs-lookup"><span data-stu-id="77d9f-207">String</span></span>|<span data-ttu-id="77d9f-208">Идентификатор, предоставляемый поставщиком VPN, если для типа подключения за установлено настраиваемого VPN.</span><span class="sxs-lookup"><span data-stu-id="77d9f-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="77d9f-209">Например: Cisco AnyConnect использует идентификатор формы com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-210">customData</span><span class="sxs-lookup"><span data-stu-id="77d9f-210">customData</span></span>|<span data-ttu-id="77d9f-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="77d9f-212">Пользовательские данные, если для типа подключения установлено настраиваемая VPN-сеть.</span><span class="sxs-lookup"><span data-stu-id="77d9f-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="77d9f-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в vpn-решении.</span><span class="sxs-lookup"><span data-stu-id="77d9f-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="77d9f-214">Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары ключ-значение.</span><span class="sxs-lookup"><span data-stu-id="77d9f-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="77d9f-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="77d9f-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="77d9f-216">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="77d9f-217">customKeyValueData</span></span>|<span data-ttu-id="77d9f-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="77d9f-219">Пользовательские данные, если для типа подключения установлено настраиваемая VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="77d9f-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="77d9f-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в вашем VPN-решении.</span><span class="sxs-lookup"><span data-stu-id="77d9f-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="77d9f-221">Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары ключ-значение.</span><span class="sxs-lookup"><span data-stu-id="77d9f-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="77d9f-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="77d9f-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="77d9f-223">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="77d9f-224">enableSplitTunneling</span></span>|<span data-ttu-id="77d9f-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="77d9f-225">Boolean</span></span>|<span data-ttu-id="77d9f-226">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="77d9f-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="77d9f-227">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="77d9f-228">authenticationMethod</span></span>|[<span data-ttu-id="77d9f-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="77d9f-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="77d9f-230">Метод проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="77d9f-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="77d9f-231">Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="77d9f-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="77d9f-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="77d9f-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="77d9f-233">enablePerApp</span></span>|<span data-ttu-id="77d9f-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="77d9f-234">Boolean</span></span>|<span data-ttu-id="77d9f-235">Если установить для этого параметра Per-App vpn, которые впоследствии могут быть связаны с приложениями, которые могут активирует этот коннекциатор VPN на устройстве пользователя с iOS.</span><span class="sxs-lookup"><span data-stu-id="77d9f-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="77d9f-236">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="77d9f-237">safariDomains</span></span>|<span data-ttu-id="77d9f-238">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="77d9f-238">String collection</span></span>|<span data-ttu-id="77d9f-239">Домены Safari, если этот параметр VPN для каждого приложения включен.</span><span class="sxs-lookup"><span data-stu-id="77d9f-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="77d9f-240">Помимо приложений, связанных с этим VPN, указанные здесь домены Safari также смогут запускать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="77d9f-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="77d9f-241">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="77d9f-242">onDemandRules</span></span>|<span data-ttu-id="77d9f-243">[Коллекция vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="77d9f-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="77d9f-244">On-Demand Rules.</span></span> <span data-ttu-id="77d9f-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="77d9f-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="77d9f-246">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-247">providerType</span><span class="sxs-lookup"><span data-stu-id="77d9f-247">providerType</span></span>|[<span data-ttu-id="77d9f-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="77d9f-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="77d9f-249">Тип поставщика для VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="77d9f-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="77d9f-250">Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="77d9f-251">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="77d9f-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="77d9f-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="77d9f-252">associatedDomains</span></span>|<span data-ttu-id="77d9f-253">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="77d9f-253">String collection</span></span>|<span data-ttu-id="77d9f-254">Связанные домены, унаследованные от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="77d9f-255">excludedDomains</span></span>|<span data-ttu-id="77d9f-256">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="77d9f-256">String collection</span></span>|<span data-ttu-id="77d9f-257">Домены, которые доступны через общедоступный Интернет, а не через VPN, даже если активирован VPN для каждого приложения. Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="77d9f-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="77d9f-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="77d9f-259">Boolean</span></span>|<span data-ttu-id="77d9f-260">Переключение, чтобы запретить пользователю отключать автоматическую VPN-сеть в приложении "Параметры". Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-261">proxyServer</span><span class="sxs-lookup"><span data-stu-id="77d9f-261">proxyServer</span></span>|[<span data-ttu-id="77d9f-262">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="77d9f-262">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="77d9f-263">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="77d9f-263">Proxy Server.</span></span> <span data-ttu-id="77d9f-264">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-264">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-265">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="77d9f-265">optInToDeviceIdSharing</span></span>|<span data-ttu-id="77d9f-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="77d9f-266">Boolean</span></span>|<span data-ttu-id="77d9f-267">Opt-In к совместному использованию удостоверения устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="77d9f-267">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="77d9f-268">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-268">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-269">userDomain</span><span class="sxs-lookup"><span data-stu-id="77d9f-269">userDomain</span></span>|<span data-ttu-id="77d9f-270">String</span><span class="sxs-lookup"><span data-stu-id="77d9f-270">String</span></span>|<span data-ttu-id="77d9f-271">Только Zscaler.</span><span class="sxs-lookup"><span data-stu-id="77d9f-271">Zscaler only.</span></span> <span data-ttu-id="77d9f-272">Введите статический домен для предварительного заполнения поля входа в приложение Zscaler.</span><span class="sxs-lookup"><span data-stu-id="77d9f-272">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="77d9f-273">Если оставить его пустым, будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="77d9f-273">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="77d9f-274">Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-274">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-275">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="77d9f-275">strictEnforcement</span></span>|<span data-ttu-id="77d9f-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="77d9f-276">Boolean</span></span>|<span data-ttu-id="77d9f-277">Только Zscaler.</span><span class="sxs-lookup"><span data-stu-id="77d9f-277">Zscaler only.</span></span> <span data-ttu-id="77d9f-278">Блокирует сетевой трафик, пока пользователь не войди в приложение Zscaler.</span><span class="sxs-lookup"><span data-stu-id="77d9f-278">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="77d9f-279">"True" означает, что трафик заблокирован.</span><span class="sxs-lookup"><span data-stu-id="77d9f-279">"True" means traffic is blocked.</span></span> <span data-ttu-id="77d9f-280">Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-280">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-281">cloudName</span><span class="sxs-lookup"><span data-stu-id="77d9f-281">cloudName</span></span>|<span data-ttu-id="77d9f-282">String</span><span class="sxs-lookup"><span data-stu-id="77d9f-282">String</span></span>|<span data-ttu-id="77d9f-283">Только Zscaler.</span><span class="sxs-lookup"><span data-stu-id="77d9f-283">Zscaler only.</span></span> <span data-ttu-id="77d9f-284">Облако Zscaler, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="77d9f-284">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="77d9f-285">Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-285">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-286">excludeList</span><span class="sxs-lookup"><span data-stu-id="77d9f-286">excludeList</span></span>|<span data-ttu-id="77d9f-287">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="77d9f-287">String collection</span></span>|<span data-ttu-id="77d9f-288">Только Zscaler.</span><span class="sxs-lookup"><span data-stu-id="77d9f-288">Zscaler only.</span></span> <span data-ttu-id="77d9f-289">Список сетевых адресов, которые не отправляются через облако Zscaler.</span><span class="sxs-lookup"><span data-stu-id="77d9f-289">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="77d9f-290">Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-290">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-291">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="77d9f-291">targetedMobileApps</span></span>|<span data-ttu-id="77d9f-292">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-292">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="77d9f-293">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="77d9f-293">Targeted mobile apps.</span></span> <span data-ttu-id="77d9f-294">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="77d9f-294">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="77d9f-295">Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-295">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-296">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="77d9f-296">microsoftTunnelSiteId</span></span>|<span data-ttu-id="77d9f-297">String</span><span class="sxs-lookup"><span data-stu-id="77d9f-297">String</span></span>|<span data-ttu-id="77d9f-298">Microsoft Tunnel site ID.</span><span class="sxs-lookup"><span data-stu-id="77d9f-298">Microsoft Tunnel site ID.</span></span> <span data-ttu-id="77d9f-299">Наследуется от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77d9f-299">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="77d9f-300">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="77d9f-300">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="77d9f-301">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="77d9f-301">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="77d9f-302">Параметры связи между безопасностью и безопасностью</span><span class="sxs-lookup"><span data-stu-id="77d9f-302">Child Security Association Parameters</span></span>|
|<span data-ttu-id="77d9f-303">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="77d9f-303">clientAuthenticationType</span></span>|[<span data-ttu-id="77d9f-304">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="77d9f-304">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="77d9f-305">Тип проверки подлинности клиента, который будет использовать VPN-клиент.</span><span class="sxs-lookup"><span data-stu-id="77d9f-305">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="77d9f-306">Возможные значения: `userAuthentication`, `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="77d9f-306">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="77d9f-307">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="77d9f-307">deadPeerDetectionRate</span></span>|[<span data-ttu-id="77d9f-308">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="77d9f-308">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="77d9f-309">Определите, как часто проверяется активность одноранговых подключений.</span><span class="sxs-lookup"><span data-stu-id="77d9f-309">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="77d9f-310">.</span><span class="sxs-lookup"><span data-stu-id="77d9f-310">.</span></span> <span data-ttu-id="77d9f-311">Возможные значения: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="77d9f-311">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="77d9f-312">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="77d9f-312">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="77d9f-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="77d9f-313">Boolean</span></span>|<span data-ttu-id="77d9f-314">Отключение MOBIKE</span><span class="sxs-lookup"><span data-stu-id="77d9f-314">Disable MOBIKE</span></span>|
|<span data-ttu-id="77d9f-315">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="77d9f-315">disableRedirect</span></span>|<span data-ttu-id="77d9f-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="77d9f-316">Boolean</span></span>|<span data-ttu-id="77d9f-317">Отключение перенаправления</span><span class="sxs-lookup"><span data-stu-id="77d9f-317">Disable Redirect</span></span>|
|<span data-ttu-id="77d9f-318">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="77d9f-318">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="77d9f-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="77d9f-319">Boolean</span></span>|<span data-ttu-id="77d9f-320">Включает проверку отзыва с наилучшими усилиями; Время отклика сервера не приведет к сбойу</span><span class="sxs-lookup"><span data-stu-id="77d9f-320">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="77d9f-321">enableEAP</span><span class="sxs-lookup"><span data-stu-id="77d9f-321">enableEAP</span></span>|<span data-ttu-id="77d9f-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="77d9f-322">Boolean</span></span>|<span data-ttu-id="77d9f-323">Включает только проверку подлинности EAP</span><span class="sxs-lookup"><span data-stu-id="77d9f-323">Enables EAP only authentication</span></span>|
|<span data-ttu-id="77d9f-324">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="77d9f-324">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="77d9f-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="77d9f-325">Boolean</span></span>|<span data-ttu-id="77d9f-326">Включить PFS.</span><span class="sxs-lookup"><span data-stu-id="77d9f-326">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="77d9f-327">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="77d9f-327">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="77d9f-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="77d9f-328">Boolean</span></span>|<span data-ttu-id="77d9f-329">Включить использование атрибутов внутренней подсети.</span><span class="sxs-lookup"><span data-stu-id="77d9f-329">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="77d9f-330">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="77d9f-330">localIdentifier</span></span>|[<span data-ttu-id="77d9f-331">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="77d9f-331">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="77d9f-332">Способ идентификации клиента, который пытается подключиться через VPN.</span><span class="sxs-lookup"><span data-stu-id="77d9f-332">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="77d9f-333">.</span><span class="sxs-lookup"><span data-stu-id="77d9f-333">.</span></span> <span data-ttu-id="77d9f-334">Возможные значения: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="77d9f-334">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="77d9f-335">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="77d9f-335">remoteIdentifier</span></span>|<span data-ttu-id="77d9f-336">String</span><span class="sxs-lookup"><span data-stu-id="77d9f-336">String</span></span>|<span data-ttu-id="77d9f-337">Адрес сервера IKEv2.</span><span class="sxs-lookup"><span data-stu-id="77d9f-337">Address of the IKEv2 server.</span></span> <span data-ttu-id="77d9f-338">Должно быть FQDN, UserFQDN, сетевой адрес или ASN1DN</span><span class="sxs-lookup"><span data-stu-id="77d9f-338">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="77d9f-339">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="77d9f-339">securityAssociationParameters</span></span>|[<span data-ttu-id="77d9f-340">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="77d9f-340">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="77d9f-341">Параметры ассоциации безопасности</span><span class="sxs-lookup"><span data-stu-id="77d9f-341">Security Association Parameters</span></span>|
|<span data-ttu-id="77d9f-342">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="77d9f-342">serverCertificateCommonName</span></span>|<span data-ttu-id="77d9f-343">String</span><span class="sxs-lookup"><span data-stu-id="77d9f-343">String</span></span>|<span data-ttu-id="77d9f-344">Общее имя сертификата сервера IKEv2, используемого при проверке подлинности сервера</span><span class="sxs-lookup"><span data-stu-id="77d9f-344">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="77d9f-345">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="77d9f-345">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="77d9f-346">String</span><span class="sxs-lookup"><span data-stu-id="77d9f-346">String</span></span>|<span data-ttu-id="77d9f-347">Общее имя выпуска сертификата сервера IKEv2, используемого при проверке подлинности</span><span class="sxs-lookup"><span data-stu-id="77d9f-347">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="77d9f-348">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="77d9f-348">serverCertificateType</span></span>|[<span data-ttu-id="77d9f-349">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="77d9f-349">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="77d9f-350">Тип сертификата, который VPN-сервер будет представлять VPN-клиенту для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="77d9f-350">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="77d9f-351">Возможные значения: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="77d9f-351">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="77d9f-352">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="77d9f-352">sharedSecret</span></span>|<span data-ttu-id="77d9f-353">String</span><span class="sxs-lookup"><span data-stu-id="77d9f-353">String</span></span>|<span data-ttu-id="77d9f-354">Используется при выборе проверки подлинности с общим секретом</span><span class="sxs-lookup"><span data-stu-id="77d9f-354">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="77d9f-355">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="77d9f-355">tlsMaximumVersion</span></span>|<span data-ttu-id="77d9f-356">String</span><span class="sxs-lookup"><span data-stu-id="77d9f-356">String</span></span>|<span data-ttu-id="77d9f-357">Максимальная версия TLS, используемая для проверки подлинности EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="77d9f-357">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="77d9f-358">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="77d9f-358">tlsMinimumVersion</span></span>|<span data-ttu-id="77d9f-359">String</span><span class="sxs-lookup"><span data-stu-id="77d9f-359">String</span></span>|<span data-ttu-id="77d9f-360">Минимальная версия TLS, используемая для проверки подлинности EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="77d9f-360">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="77d9f-361">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="77d9f-361">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="77d9f-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="77d9f-362">Boolean</span></span>|<span data-ttu-id="77d9f-363">Разрешает использование параметров связи безопасности, устанавливая для всех параметров значение по умолчанию устройства, если не указано явно.</span><span class="sxs-lookup"><span data-stu-id="77d9f-363">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="77d9f-364">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="77d9f-364">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="77d9f-365">Boolean</span><span class="sxs-lookup"><span data-stu-id="77d9f-365">Boolean</span></span>|<span data-ttu-id="77d9f-366">Разрешает использование параметров связи между безопасностью, устанавливая для всех параметров значение по умолчанию устройства, если не указано явно.</span><span class="sxs-lookup"><span data-stu-id="77d9f-366">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="77d9f-367">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="77d9f-367">alwaysOnConfiguration</span></span>|[<span data-ttu-id="77d9f-368">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="77d9f-368">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="77d9f-369">Конфигурация AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="77d9f-369">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="77d9f-370">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="77d9f-370">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="77d9f-371">Boolean</span><span class="sxs-lookup"><span data-stu-id="77d9f-371">Boolean</span></span>|<span data-ttu-id="77d9f-372">Определяет, включена ли always on VPN</span><span class="sxs-lookup"><span data-stu-id="77d9f-372">Determines if Always on VPN is enabled</span></span>|
|<span data-ttu-id="77d9f-373">mtuSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="77d9f-373">mtuSizeInBytes</span></span>|<span data-ttu-id="77d9f-374">Int32</span><span class="sxs-lookup"><span data-stu-id="77d9f-374">Int32</span></span>|<span data-ttu-id="77d9f-375">Максимальная единица передачи.</span><span class="sxs-lookup"><span data-stu-id="77d9f-375">Maximum transmission unit.</span></span> <span data-ttu-id="77d9f-376">Допустимые значения: от 1280 до 1400</span><span class="sxs-lookup"><span data-stu-id="77d9f-376">Valid values 1280 to 1400</span></span>|



## <a name="response"></a><span data-ttu-id="77d9f-377">Отклик</span><span class="sxs-lookup"><span data-stu-id="77d9f-377">Response</span></span>
<span data-ttu-id="77d9f-378">В случае успеха этот метод возвращает код отклика и объект `201 Created` [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="77d9f-378">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77d9f-379">Пример</span><span class="sxs-lookup"><span data-stu-id="77d9f-379">Example</span></span>

### <a name="request"></a><span data-ttu-id="77d9f-380">Запрос</span><span class="sxs-lookup"><span data-stu-id="77d9f-380">Request</span></span>
<span data-ttu-id="77d9f-381">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77d9f-381">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="77d9f-382">Отклик</span><span class="sxs-lookup"><span data-stu-id="77d9f-382">Response</span></span>
<span data-ttu-id="77d9f-p142">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77d9f-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




