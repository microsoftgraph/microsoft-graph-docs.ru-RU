---
title: Создание iosikEv2VpnConfiguration
description: Создайте новый объект iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 46959bc18368658faff157cb592e8b23b505b70d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867220"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="6e8ef-103">Создание iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e8ef-103">Create iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="6e8ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e8ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e8ef-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e8ef-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e8ef-107">Создайте новый [объект iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-107">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e8ef-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6e8ef-108">Prerequisites</span></span>
<span data-ttu-id="6e8ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e8ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e8ef-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e8ef-111">Permission type</span></span>|<span data-ttu-id="6e8ef-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e8ef-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e8ef-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e8ef-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e8ef-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e8ef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-116">Not supported.</span></span>|
|<span data-ttu-id="6e8ef-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6e8ef-117">Application</span></span>|<span data-ttu-id="6e8ef-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e8ef-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e8ef-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e8ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6e8ef-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6e8ef-120">Request headers</span></span>
|<span data-ttu-id="6e8ef-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e8ef-121">Header</span></span>|<span data-ttu-id="6e8ef-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6e8ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e8ef-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e8ef-123">Authorization</span></span>|<span data-ttu-id="6e8ef-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e8ef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6e8ef-125">Accept</span></span>|<span data-ttu-id="6e8ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e8ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e8ef-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e8ef-127">Request body</span></span>
<span data-ttu-id="6e8ef-128">В теле запроса поставляем представление JSON для объекта iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-128">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="6e8ef-129">В следующей таблице показаны свойства, необходимые при создании iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-129">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="6e8ef-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e8ef-130">Property</span></span>|<span data-ttu-id="6e8ef-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6e8ef-131">Type</span></span>|<span data-ttu-id="6e8ef-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6e8ef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e8ef-133">id</span><span class="sxs-lookup"><span data-stu-id="6e8ef-133">id</span></span>|<span data-ttu-id="6e8ef-134">String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-134">String</span></span>|<span data-ttu-id="6e8ef-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-135">Key of the entity.</span></span> <span data-ttu-id="6e8ef-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ef-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e8ef-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6e8ef-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e8ef-138">DateTimeOffset</span></span>|<span data-ttu-id="6e8ef-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6e8ef-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ef-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6e8ef-141">roleScopeTagIds</span></span>|<span data-ttu-id="6e8ef-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-142">String collection</span></span>|<span data-ttu-id="6e8ef-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6e8ef-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ef-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6e8ef-145">supportsScopeTags</span></span>|<span data-ttu-id="6e8ef-146">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ef-146">Boolean</span></span>|<span data-ttu-id="6e8ef-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6e8ef-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6e8ef-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6e8ef-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-150">This property is read-only.</span></span> <span data-ttu-id="6e8ef-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ef-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6e8ef-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6e8ef-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6e8ef-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6e8ef-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6e8ef-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ef-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6e8ef-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6e8ef-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6e8ef-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6e8ef-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6e8ef-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ef-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6e8ef-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6e8ef-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6e8ef-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6e8ef-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6e8ef-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ef-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e8ef-164">createdDateTime</span></span>|<span data-ttu-id="6e8ef-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e8ef-165">DateTimeOffset</span></span>|<span data-ttu-id="6e8ef-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-166">DateTime the object was created.</span></span> <span data-ttu-id="6e8ef-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ef-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-168">description</span><span class="sxs-lookup"><span data-stu-id="6e8ef-168">description</span></span>|<span data-ttu-id="6e8ef-169">String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-169">String</span></span>|<span data-ttu-id="6e8ef-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6e8ef-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ef-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-172">displayName</span><span class="sxs-lookup"><span data-stu-id="6e8ef-172">displayName</span></span>|<span data-ttu-id="6e8ef-173">String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-173">String</span></span>|<span data-ttu-id="6e8ef-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6e8ef-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ef-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-176">version</span><span class="sxs-lookup"><span data-stu-id="6e8ef-176">version</span></span>|<span data-ttu-id="6e8ef-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6e8ef-177">Int32</span></span>|<span data-ttu-id="6e8ef-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-178">Version of the device configuration.</span></span> <span data-ttu-id="6e8ef-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ef-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="6e8ef-180">connectionName</span></span>|<span data-ttu-id="6e8ef-181">String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-181">String</span></span>|<span data-ttu-id="6e8ef-182">Имя подключения, отображаемая пользователю.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-182">Connection name displayed to the user.</span></span> <span data-ttu-id="6e8ef-183">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="6e8ef-184">connectionType</span></span>|[<span data-ttu-id="6e8ef-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="6e8ef-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="6e8ef-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-186">Connection type.</span></span> <span data-ttu-id="6e8ef-187">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ef-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="6e8ef-188">Возможные значения: `ciscoAnyConnect` `pulseSecure` , , , , , `f5EdgeClient` , , , `dellSonicWallMobileConnect` `checkPointCapsuleVpn` , , `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` , `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` .</span><span class="sxs-lookup"><span data-stu-id="6e8ef-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="6e8ef-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="6e8ef-189">loginGroupOrDomain</span></span>|<span data-ttu-id="6e8ef-190">String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-190">String</span></span>|<span data-ttu-id="6e8ef-191">Группа входа или домен при наборе типа подключения к мобильному подключению Dell SonicWALL.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="6e8ef-192">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-193">role</span><span class="sxs-lookup"><span data-stu-id="6e8ef-193">role</span></span>|<span data-ttu-id="6e8ef-194">String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-194">String</span></span>|<span data-ttu-id="6e8ef-195">Роль при наборе типа подключения к Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="6e8ef-196">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-197">realm</span><span class="sxs-lookup"><span data-stu-id="6e8ef-197">realm</span></span>|<span data-ttu-id="6e8ef-198">String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-198">String</span></span>|<span data-ttu-id="6e8ef-199">Realm, когда тип подключения за установлен в Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="6e8ef-200">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-201">сервер</span><span class="sxs-lookup"><span data-stu-id="6e8ef-201">server</span></span>|[<span data-ttu-id="6e8ef-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="6e8ef-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="6e8ef-203">VPN Server в сети.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-203">VPN Server on the network.</span></span> <span data-ttu-id="6e8ef-204">Убедитесь, что конечные пользователи могут получить доступ к этому расположению сети.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="6e8ef-205">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="6e8ef-206">identifier</span></span>|<span data-ttu-id="6e8ef-207">String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-207">String</span></span>|<span data-ttu-id="6e8ef-208">Идентификатор, предоставляемый поставщиком VPN при наборе типа подключения к настраиваемой VPN.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="6e8ef-209">Например: Cisco AnyConnect использует идентификатор формы com.cisco.anyconnect.applevpn.plugin, унаследованный от [appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-210">customData</span><span class="sxs-lookup"><span data-stu-id="6e8ef-210">customData</span></span>|<span data-ttu-id="6e8ef-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="6e8ef-212">Настраиваемые данные при наборе типа подключения к настраиваемой VPN.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="6e8ef-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в vpn-решении.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="6e8ef-214">Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары ключей и значений.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="6e8ef-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="6e8ef-216">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="6e8ef-217">customKeyValueData</span></span>|<span data-ttu-id="6e8ef-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6e8ef-219">Настраиваемые данные при наборе типа подключения к настраиваемой VPN.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="6e8ef-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в vpn-решении.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="6e8ef-221">Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары ключей и значений.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="6e8ef-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="6e8ef-223">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="6e8ef-224">enableSplitTunneling</span></span>|<span data-ttu-id="6e8ef-225">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ef-225">Boolean</span></span>|<span data-ttu-id="6e8ef-226">Отправка всего сетевого трафика через VPN.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="6e8ef-227">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6e8ef-228">authenticationMethod</span></span>|[<span data-ttu-id="6e8ef-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6e8ef-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="6e8ef-230">Метод проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="6e8ef-231">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ef-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="6e8ef-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="6e8ef-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="6e8ef-233">enablePerApp</span></span>|<span data-ttu-id="6e8ef-234">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ef-234">Boolean</span></span>|<span data-ttu-id="6e8ef-235">Настройка этого параметра создает Per-App, которая впоследствии может быть связана с приложениями, которые могут запускать этот VPN-коннекцитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="6e8ef-236">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="6e8ef-237">safariDomains</span></span>|<span data-ttu-id="6e8ef-238">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-238">String collection</span></span>|<span data-ttu-id="6e8ef-239">Домены Safari при включении этого параметра VPN для приложения.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="6e8ef-240">Помимо приложений, связанных с этим VPN, указанные здесь домены Safari также смогут запускать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="6e8ef-241">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="6e8ef-242">onDemandRules</span></span>|<span data-ttu-id="6e8ef-243">[коллекция vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="6e8ef-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-244">On-Demand Rules.</span></span> <span data-ttu-id="6e8ef-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6e8ef-246">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-247">providerType</span><span class="sxs-lookup"><span data-stu-id="6e8ef-247">providerType</span></span>|[<span data-ttu-id="6e8ef-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="6e8ef-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="6e8ef-249">Тип поставщика для VPN-приложения.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="6e8ef-250">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e8ef-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="6e8ef-251">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="6e8ef-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="6e8ef-252">associatedDomains</span></span>|<span data-ttu-id="6e8ef-253">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-253">String collection</span></span>|<span data-ttu-id="6e8ef-254">Связанные домены, унаследованные от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="6e8ef-255">excludedDomains</span></span>|<span data-ttu-id="6e8ef-256">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-256">String collection</span></span>|<span data-ttu-id="6e8ef-257">Домены, которые доступны через общедоступный интернет, а не через VPN, даже если VPN для каждого приложения активируется, наследуется [из appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="6e8ef-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="6e8ef-259">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ef-259">Boolean</span></span>|<span data-ttu-id="6e8ef-260">Переключение, чтобы предотвратить отключение автоматического VPN в приложении "Параметры", унаследованных от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-261">disconnectOnIdle</span><span class="sxs-lookup"><span data-stu-id="6e8ef-261">disconnectOnIdle</span></span>|<span data-ttu-id="6e8ef-262">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ef-262">Boolean</span></span>|<span data-ttu-id="6e8ef-263">Отключение после простоя подключения по требованию, унаследованной от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-263">Whether to disconnect after on-demand connection idles Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-264">disconnectOnIdleTimerInSeconds</span><span class="sxs-lookup"><span data-stu-id="6e8ef-264">disconnectOnIdleTimerInSeconds</span></span>|<span data-ttu-id="6e8ef-265">Int32</span><span class="sxs-lookup"><span data-stu-id="6e8ef-265">Int32</span></span>|<span data-ttu-id="6e8ef-266">Время в секундах, необходимое для ожидания перед отключением подключения по запросу.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-266">The length of time in seconds to wait before disconnecting an on-demand connection.</span></span> <span data-ttu-id="6e8ef-267">Допустимые значения от 0 до 65535, унаследованные от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-267">Valid values 0 to 65535 Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-268">proxyServer</span><span class="sxs-lookup"><span data-stu-id="6e8ef-268">proxyServer</span></span>|[<span data-ttu-id="6e8ef-269">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="6e8ef-269">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="6e8ef-270">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-270">Proxy Server.</span></span> <span data-ttu-id="6e8ef-271">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-271">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-272">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="6e8ef-272">optInToDeviceIdSharing</span></span>|<span data-ttu-id="6e8ef-273">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ef-273">Boolean</span></span>|<span data-ttu-id="6e8ef-274">Opt-In совместное использование Id устройства сторонним vpn-клиентам для использования во время проверки контроля доступа к сети.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-274">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="6e8ef-275">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-275">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-276">userDomain</span><span class="sxs-lookup"><span data-stu-id="6e8ef-276">userDomain</span></span>|<span data-ttu-id="6e8ef-277">String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-277">String</span></span>|<span data-ttu-id="6e8ef-278">Zscaler только.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-278">Zscaler only.</span></span> <span data-ttu-id="6e8ef-279">Введите статический домен для предварительного заполнения поля входа в приложение Zscaler.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-279">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="6e8ef-280">Если этот домен останется пустым, вместо него будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-280">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="6e8ef-281">Унаследованный от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-281">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-282">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="6e8ef-282">strictEnforcement</span></span>|<span data-ttu-id="6e8ef-283">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ef-283">Boolean</span></span>|<span data-ttu-id="6e8ef-284">Zscaler только.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-284">Zscaler only.</span></span> <span data-ttu-id="6e8ef-285">Блокирует сетевой трафик до тех пор, пока пользователь не впишется в приложение Zscaler.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-285">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="6e8ef-286">"True" означает, что трафик заблокирован.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-286">"True" means traffic is blocked.</span></span> <span data-ttu-id="6e8ef-287">Унаследованный от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-287">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-288">cloudName</span><span class="sxs-lookup"><span data-stu-id="6e8ef-288">cloudName</span></span>|<span data-ttu-id="6e8ef-289">String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-289">String</span></span>|<span data-ttu-id="6e8ef-290">Zscaler только.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-290">Zscaler only.</span></span> <span data-ttu-id="6e8ef-291">Облако Zscaler, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-291">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="6e8ef-292">Унаследованный от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-292">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-293">excludeList</span><span class="sxs-lookup"><span data-stu-id="6e8ef-293">excludeList</span></span>|<span data-ttu-id="6e8ef-294">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-294">String collection</span></span>|<span data-ttu-id="6e8ef-295">Zscaler только.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-295">Zscaler only.</span></span> <span data-ttu-id="6e8ef-296">Список сетевых адресов, которые не отправляются через облако Zscaler.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-296">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="6e8ef-297">Унаследованный от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-297">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-298">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="6e8ef-298">targetedMobileApps</span></span>|<span data-ttu-id="6e8ef-299">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-299">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6e8ef-300">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-300">Targeted mobile apps.</span></span> <span data-ttu-id="6e8ef-301">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-301">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6e8ef-302">Унаследованный от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-302">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-303">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="6e8ef-303">microsoftTunnelSiteId</span></span>|<span data-ttu-id="6e8ef-304">String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-304">String</span></span>|<span data-ttu-id="6e8ef-305">Microsoft Tunnel site ID.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-305">Microsoft Tunnel site ID.</span></span> <span data-ttu-id="6e8ef-306">Унаследованный от [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e8ef-306">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6e8ef-307">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="6e8ef-307">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="6e8ef-308">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="6e8ef-308">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="6e8ef-309">Параметры ассоциации безопасности детей</span><span class="sxs-lookup"><span data-stu-id="6e8ef-309">Child Security Association Parameters</span></span>|
|<span data-ttu-id="6e8ef-310">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="6e8ef-310">clientAuthenticationType</span></span>|[<span data-ttu-id="6e8ef-311">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="6e8ef-311">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="6e8ef-312">Тип проверки подлинности клиента, который будет использовать VPN-клиент.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-312">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="6e8ef-313">Возможные значения: `userAuthentication`, `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-313">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="6e8ef-314">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="6e8ef-314">deadPeerDetectionRate</span></span>|[<span data-ttu-id="6e8ef-315">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="6e8ef-315">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="6e8ef-316">Определите, как часто проверять, активна ли одноранговая связь.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-316">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="6e8ef-317">.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-317">.</span></span> <span data-ttu-id="6e8ef-318">Возможные значения: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-318">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="6e8ef-319">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="6e8ef-319">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="6e8ef-320">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ef-320">Boolean</span></span>|<span data-ttu-id="6e8ef-321">Отключение MOBIKE</span><span class="sxs-lookup"><span data-stu-id="6e8ef-321">Disable MOBIKE</span></span>|
|<span data-ttu-id="6e8ef-322">отключениеRedirect</span><span class="sxs-lookup"><span data-stu-id="6e8ef-322">disableRedirect</span></span>|<span data-ttu-id="6e8ef-323">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ef-323">Boolean</span></span>|<span data-ttu-id="6e8ef-324">Отключение перенаправления</span><span class="sxs-lookup"><span data-stu-id="6e8ef-324">Disable Redirect</span></span>|
|<span data-ttu-id="6e8ef-325">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="6e8ef-325">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="6e8ef-326">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ef-326">Boolean</span></span>|<span data-ttu-id="6e8ef-327">Включает проверку отзыва с наилучшими усилиями; Время ото времени отклика сервера не приведет к сбой</span><span class="sxs-lookup"><span data-stu-id="6e8ef-327">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="6e8ef-328">enableEAP</span><span class="sxs-lookup"><span data-stu-id="6e8ef-328">enableEAP</span></span>|<span data-ttu-id="6e8ef-329">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ef-329">Boolean</span></span>|<span data-ttu-id="6e8ef-330">Включает только проверку подлинности EAP</span><span class="sxs-lookup"><span data-stu-id="6e8ef-330">Enables EAP only authentication</span></span>|
|<span data-ttu-id="6e8ef-331">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="6e8ef-331">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="6e8ef-332">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ef-332">Boolean</span></span>|<span data-ttu-id="6e8ef-333">Включить совершенную секретность вперед (PFS).</span><span class="sxs-lookup"><span data-stu-id="6e8ef-333">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="6e8ef-334">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="6e8ef-334">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="6e8ef-335">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ef-335">Boolean</span></span>|<span data-ttu-id="6e8ef-336">Включить использование атрибутов внутренней подсети.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-336">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="6e8ef-337">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="6e8ef-337">localIdentifier</span></span>|[<span data-ttu-id="6e8ef-338">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="6e8ef-338">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="6e8ef-339">Метод идентификации клиента, который пытается подключиться с помощью VPN.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-339">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="6e8ef-340">.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-340">.</span></span> <span data-ttu-id="6e8ef-341">Возможные значения: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-341">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="6e8ef-342">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="6e8ef-342">remoteIdentifier</span></span>|<span data-ttu-id="6e8ef-343">String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-343">String</span></span>|<span data-ttu-id="6e8ef-344">Адрес сервера IKEv2.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-344">Address of the IKEv2 server.</span></span> <span data-ttu-id="6e8ef-345">Должен быть FQDN, UserFQDN, сетевой адрес или ASN1DN</span><span class="sxs-lookup"><span data-stu-id="6e8ef-345">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="6e8ef-346">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="6e8ef-346">securityAssociationParameters</span></span>|[<span data-ttu-id="6e8ef-347">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="6e8ef-347">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="6e8ef-348">Параметры ассоциации безопасности</span><span class="sxs-lookup"><span data-stu-id="6e8ef-348">Security Association Parameters</span></span>|
|<span data-ttu-id="6e8ef-349">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="6e8ef-349">serverCertificateCommonName</span></span>|<span data-ttu-id="6e8ef-350">String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-350">String</span></span>|<span data-ttu-id="6e8ef-351">Общее имя сертификата сервера IKEv2, используемого в проверке подлинности сервера</span><span class="sxs-lookup"><span data-stu-id="6e8ef-351">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="6e8ef-352">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="6e8ef-352">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="6e8ef-353">String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-353">String</span></span>|<span data-ttu-id="6e8ef-354">Общее имя эмитента сертификата IKEv2 Server, используемого в проверке подлинности</span><span class="sxs-lookup"><span data-stu-id="6e8ef-354">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="6e8ef-355">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="6e8ef-355">serverCertificateType</span></span>|[<span data-ttu-id="6e8ef-356">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="6e8ef-356">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="6e8ef-357">Тип сертификата, который VPN-сервер представит VPN-клиенту для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-357">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="6e8ef-358">Возможные значения: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-358">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="6e8ef-359">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="6e8ef-359">sharedSecret</span></span>|<span data-ttu-id="6e8ef-360">String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-360">String</span></span>|<span data-ttu-id="6e8ef-361">Используется при выборе общей секретной проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="6e8ef-361">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="6e8ef-362">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6e8ef-362">tlsMaximumVersion</span></span>|<span data-ttu-id="6e8ef-363">String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-363">String</span></span>|<span data-ttu-id="6e8ef-364">Максимальная версия TLS, используемая для проверки подлинности EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="6e8ef-364">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="6e8ef-365">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6e8ef-365">tlsMinimumVersion</span></span>|<span data-ttu-id="6e8ef-366">String</span><span class="sxs-lookup"><span data-stu-id="6e8ef-366">String</span></span>|<span data-ttu-id="6e8ef-367">Минимальная версия TLS, используемая для проверки подлинности EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="6e8ef-367">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="6e8ef-368">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="6e8ef-368">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="6e8ef-369">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ef-369">Boolean</span></span>|<span data-ttu-id="6e8ef-370">Позволяет использовать параметры ассоциации безопасности, устанавливая все параметры по умолчанию устройства, если явно не указано.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-370">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="6e8ef-371">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="6e8ef-371">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="6e8ef-372">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ef-372">Boolean</span></span>|<span data-ttu-id="6e8ef-373">Позволяет использовать параметры ассоциации детской безопасности, устанавливая все параметры по умолчанию устройства, если явно не указано.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-373">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="6e8ef-374">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e8ef-374">alwaysOnConfiguration</span></span>|[<span data-ttu-id="6e8ef-375">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e8ef-375">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="6e8ef-376">Конфигурация AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="6e8ef-376">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="6e8ef-377">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e8ef-377">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="6e8ef-378">Логический</span><span class="sxs-lookup"><span data-stu-id="6e8ef-378">Boolean</span></span>|<span data-ttu-id="6e8ef-379">Определяет, включен ли always на VPN</span><span class="sxs-lookup"><span data-stu-id="6e8ef-379">Determines if Always on VPN is enabled</span></span>|
|<span data-ttu-id="6e8ef-380">mtuSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="6e8ef-380">mtuSizeInBytes</span></span>|<span data-ttu-id="6e8ef-381">Int32</span><span class="sxs-lookup"><span data-stu-id="6e8ef-381">Int32</span></span>|<span data-ttu-id="6e8ef-382">Максимальный блок передачи.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-382">Maximum transmission unit.</span></span> <span data-ttu-id="6e8ef-383">Допустимые значения от 1280 до 1400</span><span class="sxs-lookup"><span data-stu-id="6e8ef-383">Valid values 1280 to 1400</span></span>|



## <a name="response"></a><span data-ttu-id="6e8ef-384">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e8ef-384">Response</span></span>
<span data-ttu-id="6e8ef-385">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-385">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e8ef-386">Пример</span><span class="sxs-lookup"><span data-stu-id="6e8ef-386">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e8ef-387">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e8ef-387">Request</span></span>
<span data-ttu-id="6e8ef-388">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-388">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 5562

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
  "disconnectOnIdle": true,
  "disconnectOnIdleTimerInSeconds": 14,
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

### <a name="response"></a><span data-ttu-id="6e8ef-389">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e8ef-389">Response</span></span>
<span data-ttu-id="6e8ef-p143">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e8ef-p143">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 5734

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
  "disconnectOnIdle": true,
  "disconnectOnIdleTimerInSeconds": 14,
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




