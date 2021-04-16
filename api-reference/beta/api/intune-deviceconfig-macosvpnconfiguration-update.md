---
title: Обновление macOSVpnConfiguration
description: Обновление свойств объекта macOSVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ba55a346a2e597bfdce4d74e20df5eb5b671ab9c
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866533"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="ada5c-103">Обновление macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ada5c-103">Update macOSVpnConfiguration</span></span>

<span data-ttu-id="ada5c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ada5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ada5c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ada5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ada5c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ada5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ada5c-107">Обновление свойств объекта [macOSVpnConfiguration.](../resources/intune-deviceconfig-macosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-107">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ada5c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ada5c-108">Prerequisites</span></span>
<span data-ttu-id="ada5c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ada5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ada5c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ada5c-111">Permission type</span></span>|<span data-ttu-id="ada5c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ada5c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ada5c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ada5c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ada5c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ada5c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ada5c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ada5c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ada5c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ada5c-116">Not supported.</span></span>|
|<span data-ttu-id="ada5c-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ada5c-117">Application</span></span>|<span data-ttu-id="ada5c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ada5c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ada5c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ada5c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ada5c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ada5c-120">Request headers</span></span>
|<span data-ttu-id="ada5c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ada5c-121">Header</span></span>|<span data-ttu-id="ada5c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ada5c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ada5c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ada5c-123">Authorization</span></span>|<span data-ttu-id="ada5c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ada5c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ada5c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ada5c-125">Accept</span></span>|<span data-ttu-id="ada5c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ada5c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ada5c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ada5c-127">Request body</span></span>
<span data-ttu-id="ada5c-128">В теле запроса поставляем представление JSON для [объекта macOSVpnConfiguration.](../resources/intune-deviceconfig-macosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-128">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="ada5c-129">В следующей таблице показаны свойства, необходимые при создании [macOSVpnConfiguration.](../resources/intune-deviceconfig-macosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-129">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="ada5c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ada5c-130">Property</span></span>|<span data-ttu-id="ada5c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ada5c-131">Type</span></span>|<span data-ttu-id="ada5c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ada5c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ada5c-133">id</span><span class="sxs-lookup"><span data-stu-id="ada5c-133">id</span></span>|<span data-ttu-id="ada5c-134">String</span><span class="sxs-lookup"><span data-stu-id="ada5c-134">String</span></span>|<span data-ttu-id="ada5c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ada5c-135">Key of the entity.</span></span> <span data-ttu-id="ada5c-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ada5c-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ada5c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ada5c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ada5c-138">DateTimeOffset</span></span>|<span data-ttu-id="ada5c-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ada5c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ada5c-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ada5c-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ada5c-141">roleScopeTagIds</span></span>|<span data-ttu-id="ada5c-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ada5c-142">String collection</span></span>|<span data-ttu-id="ada5c-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="ada5c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ada5c-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ada5c-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ada5c-145">supportsScopeTags</span></span>|<span data-ttu-id="ada5c-146">Логический</span><span class="sxs-lookup"><span data-stu-id="ada5c-146">Boolean</span></span>|<span data-ttu-id="ada5c-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ada5c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ada5c-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="ada5c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ada5c-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ada5c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ada5c-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ada5c-150">This property is read-only.</span></span> <span data-ttu-id="ada5c-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ada5c-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ada5c-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ada5c-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ada5c-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ada5c-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ada5c-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ada5c-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ada5c-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ada5c-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ada5c-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ada5c-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ada5c-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ada5c-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ada5c-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ada5c-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ada5c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ada5c-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ada5c-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ada5c-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ada5c-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ada5c-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ada5c-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ada5c-164">createdDateTime</span></span>|<span data-ttu-id="ada5c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ada5c-165">DateTimeOffset</span></span>|<span data-ttu-id="ada5c-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ada5c-166">DateTime the object was created.</span></span> <span data-ttu-id="ada5c-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ada5c-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-168">description</span><span class="sxs-lookup"><span data-stu-id="ada5c-168">description</span></span>|<span data-ttu-id="ada5c-169">String</span><span class="sxs-lookup"><span data-stu-id="ada5c-169">String</span></span>|<span data-ttu-id="ada5c-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ada5c-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ada5c-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ada5c-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ada5c-172">displayName</span></span>|<span data-ttu-id="ada5c-173">String</span><span class="sxs-lookup"><span data-stu-id="ada5c-173">String</span></span>|<span data-ttu-id="ada5c-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ada5c-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ada5c-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ada5c-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-176">version</span><span class="sxs-lookup"><span data-stu-id="ada5c-176">version</span></span>|<span data-ttu-id="ada5c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ada5c-177">Int32</span></span>|<span data-ttu-id="ada5c-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ada5c-178">Version of the device configuration.</span></span> <span data-ttu-id="ada5c-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ada5c-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="ada5c-180">connectionName</span></span>|<span data-ttu-id="ada5c-181">String</span><span class="sxs-lookup"><span data-stu-id="ada5c-181">String</span></span>|<span data-ttu-id="ada5c-182">Имя подключения, отображаемая пользователю.</span><span class="sxs-lookup"><span data-stu-id="ada5c-182">Connection name displayed to the user.</span></span> <span data-ttu-id="ada5c-183">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="ada5c-184">connectionType</span></span>|[<span data-ttu-id="ada5c-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="ada5c-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="ada5c-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="ada5c-186">Connection type.</span></span> <span data-ttu-id="ada5c-187">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ada5c-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="ada5c-188">Возможные значения: `ciscoAnyConnect` `pulseSecure` , , , , , `f5EdgeClient` , , , `dellSonicWallMobileConnect` `checkPointCapsuleVpn` , , `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` , `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` .</span><span class="sxs-lookup"><span data-stu-id="ada5c-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="ada5c-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="ada5c-189">loginGroupOrDomain</span></span>|<span data-ttu-id="ada5c-190">String</span><span class="sxs-lookup"><span data-stu-id="ada5c-190">String</span></span>|<span data-ttu-id="ada5c-191">Группа входа или домен при наборе типа подключения к мобильному подключению Dell SonicWALL.</span><span class="sxs-lookup"><span data-stu-id="ada5c-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="ada5c-192">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-193">role</span><span class="sxs-lookup"><span data-stu-id="ada5c-193">role</span></span>|<span data-ttu-id="ada5c-194">String</span><span class="sxs-lookup"><span data-stu-id="ada5c-194">String</span></span>|<span data-ttu-id="ada5c-195">Роль при наборе типа подключения к Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="ada5c-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="ada5c-196">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-197">realm</span><span class="sxs-lookup"><span data-stu-id="ada5c-197">realm</span></span>|<span data-ttu-id="ada5c-198">String</span><span class="sxs-lookup"><span data-stu-id="ada5c-198">String</span></span>|<span data-ttu-id="ada5c-199">Realm, когда тип подключения за установлен в Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="ada5c-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="ada5c-200">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-201">сервер</span><span class="sxs-lookup"><span data-stu-id="ada5c-201">server</span></span>|[<span data-ttu-id="ada5c-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="ada5c-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="ada5c-203">VPN Server в сети.</span><span class="sxs-lookup"><span data-stu-id="ada5c-203">VPN Server on the network.</span></span> <span data-ttu-id="ada5c-204">Убедитесь, что конечные пользователи могут получить доступ к этому расположению сети.</span><span class="sxs-lookup"><span data-stu-id="ada5c-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="ada5c-205">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="ada5c-206">identifier</span></span>|<span data-ttu-id="ada5c-207">String</span><span class="sxs-lookup"><span data-stu-id="ada5c-207">String</span></span>|<span data-ttu-id="ada5c-208">Идентификатор, предоставляемый поставщиком VPN при наборе типа подключения к настраиваемой VPN.</span><span class="sxs-lookup"><span data-stu-id="ada5c-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ada5c-209">Например: Cisco AnyConnect использует идентификатор формы com.cisco.anyconnect.applevpn.plugin, унаследованный от [appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-210">customData</span><span class="sxs-lookup"><span data-stu-id="ada5c-210">customData</span></span>|<span data-ttu-id="ada5c-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="ada5c-212">Настраиваемые данные при наборе типа подключения к настраиваемой VPN.</span><span class="sxs-lookup"><span data-stu-id="ada5c-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ada5c-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в vpn-решении.</span><span class="sxs-lookup"><span data-stu-id="ada5c-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="ada5c-214">Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары ключей и значений.</span><span class="sxs-lookup"><span data-stu-id="ada5c-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="ada5c-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="ada5c-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="ada5c-216">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="ada5c-217">customKeyValueData</span></span>|<span data-ttu-id="ada5c-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ada5c-219">Настраиваемые данные при наборе типа подключения к настраиваемой VPN.</span><span class="sxs-lookup"><span data-stu-id="ada5c-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ada5c-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в vpn-решении.</span><span class="sxs-lookup"><span data-stu-id="ada5c-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="ada5c-221">Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары ключей и значений.</span><span class="sxs-lookup"><span data-stu-id="ada5c-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="ada5c-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="ada5c-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="ada5c-223">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="ada5c-224">enableSplitTunneling</span></span>|<span data-ttu-id="ada5c-225">Логический</span><span class="sxs-lookup"><span data-stu-id="ada5c-225">Boolean</span></span>|<span data-ttu-id="ada5c-226">Отправка всего сетевого трафика через VPN.</span><span class="sxs-lookup"><span data-stu-id="ada5c-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="ada5c-227">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ada5c-228">authenticationMethod</span></span>|[<span data-ttu-id="ada5c-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ada5c-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="ada5c-230">Метод проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="ada5c-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="ada5c-231">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ada5c-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="ada5c-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="ada5c-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="ada5c-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="ada5c-233">enablePerApp</span></span>|<span data-ttu-id="ada5c-234">Логический</span><span class="sxs-lookup"><span data-stu-id="ada5c-234">Boolean</span></span>|<span data-ttu-id="ada5c-235">Настройка этого параметра создает Per-App, которая впоследствии может быть связана с приложениями, которые могут запускать этот VPN-коннекцитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ada5c-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="ada5c-236">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="ada5c-237">safariDomains</span></span>|<span data-ttu-id="ada5c-238">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ada5c-238">String collection</span></span>|<span data-ttu-id="ada5c-239">Домены Safari при включении этого параметра VPN для приложения.</span><span class="sxs-lookup"><span data-stu-id="ada5c-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="ada5c-240">Помимо приложений, связанных с этим VPN, указанные здесь домены Safari также смогут запускать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="ada5c-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="ada5c-241">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="ada5c-242">onDemandRules</span></span>|<span data-ttu-id="ada5c-243">[коллекция vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="ada5c-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="ada5c-244">On-Demand Rules.</span></span> <span data-ttu-id="ada5c-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ada5c-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ada5c-246">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-247">providerType</span><span class="sxs-lookup"><span data-stu-id="ada5c-247">providerType</span></span>|[<span data-ttu-id="ada5c-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="ada5c-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="ada5c-249">Тип поставщика для VPN-приложения.</span><span class="sxs-lookup"><span data-stu-id="ada5c-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="ada5c-250">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ada5c-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="ada5c-251">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="ada5c-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="ada5c-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="ada5c-252">associatedDomains</span></span>|<span data-ttu-id="ada5c-253">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ada5c-253">String collection</span></span>|<span data-ttu-id="ada5c-254">Связанные домены, унаследованные от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="ada5c-255">excludedDomains</span></span>|<span data-ttu-id="ada5c-256">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ada5c-256">String collection</span></span>|<span data-ttu-id="ada5c-257">Домены, которые доступны через общедоступный интернет, а не через VPN, даже если VPN для каждого приложения активируется, наследуется [из appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="ada5c-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="ada5c-259">Логический</span><span class="sxs-lookup"><span data-stu-id="ada5c-259">Boolean</span></span>|<span data-ttu-id="ada5c-260">Переключение, чтобы предотвратить отключение автоматического VPN в приложении "Параметры", унаследованных от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-261">disconnectOnIdle</span><span class="sxs-lookup"><span data-stu-id="ada5c-261">disconnectOnIdle</span></span>|<span data-ttu-id="ada5c-262">Логический</span><span class="sxs-lookup"><span data-stu-id="ada5c-262">Boolean</span></span>|<span data-ttu-id="ada5c-263">Отключение после простоя подключения по требованию, унаследованной от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-263">Whether to disconnect after on-demand connection idles Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-264">disconnectOnIdleTimerInSeconds</span><span class="sxs-lookup"><span data-stu-id="ada5c-264">disconnectOnIdleTimerInSeconds</span></span>|<span data-ttu-id="ada5c-265">Int32</span><span class="sxs-lookup"><span data-stu-id="ada5c-265">Int32</span></span>|<span data-ttu-id="ada5c-266">Время в секундах, необходимое для ожидания перед отключением подключения по запросу.</span><span class="sxs-lookup"><span data-stu-id="ada5c-266">The length of time in seconds to wait before disconnecting an on-demand connection.</span></span> <span data-ttu-id="ada5c-267">Допустимые значения от 0 до 65535, унаследованные от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-267">Valid values 0 to 65535 Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-268">proxyServer</span><span class="sxs-lookup"><span data-stu-id="ada5c-268">proxyServer</span></span>|[<span data-ttu-id="ada5c-269">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="ada5c-269">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="ada5c-270">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="ada5c-270">Proxy Server.</span></span> <span data-ttu-id="ada5c-271">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-271">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ada5c-272">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="ada5c-272">optInToDeviceIdSharing</span></span>|<span data-ttu-id="ada5c-273">Логический</span><span class="sxs-lookup"><span data-stu-id="ada5c-273">Boolean</span></span>|<span data-ttu-id="ada5c-274">Opt-In совместное использование Id устройства сторонним vpn-клиентам для использования во время проверки контроля доступа к сети.</span><span class="sxs-lookup"><span data-stu-id="ada5c-274">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="ada5c-275">Унаследованный от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ada5c-275">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ada5c-276">Отклик</span><span class="sxs-lookup"><span data-stu-id="ada5c-276">Response</span></span>
<span data-ttu-id="ada5c-277">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ada5c-277">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ada5c-278">Пример</span><span class="sxs-lookup"><span data-stu-id="ada5c-278">Example</span></span>

### <a name="request"></a><span data-ttu-id="ada5c-279">Запрос</span><span class="sxs-lookup"><span data-stu-id="ada5c-279">Request</span></span>
<span data-ttu-id="ada5c-280">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ada5c-280">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2895

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
  "optInToDeviceIdSharing": true
}
```

### <a name="response"></a><span data-ttu-id="ada5c-281">Отклик</span><span class="sxs-lookup"><span data-stu-id="ada5c-281">Response</span></span>
<span data-ttu-id="ada5c-p131">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ada5c-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3067

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
  "optInToDeviceIdSharing": true
}
```




