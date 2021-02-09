---
title: Обновление macOSVpnConfiguration
description: Обновление свойств объекта macOSVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 13b2a4c9b02edc8207909e2dfb26030e7812f202
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155169"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="2936b-103">Обновление macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="2936b-103">Update macOSVpnConfiguration</span></span>

<span data-ttu-id="2936b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2936b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2936b-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2936b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2936b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2936b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2936b-107">Обновление свойств объекта [macOSVpnConfiguration.](../resources/intune-deviceconfig-macosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-107">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2936b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2936b-108">Prerequisites</span></span>
<span data-ttu-id="2936b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2936b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2936b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2936b-111">Permission type</span></span>|<span data-ttu-id="2936b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2936b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2936b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2936b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2936b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2936b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2936b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2936b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2936b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2936b-116">Not supported.</span></span>|
|<span data-ttu-id="2936b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2936b-117">Application</span></span>|<span data-ttu-id="2936b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2936b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2936b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2936b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2936b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2936b-120">Request headers</span></span>
|<span data-ttu-id="2936b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2936b-121">Header</span></span>|<span data-ttu-id="2936b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2936b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2936b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2936b-123">Authorization</span></span>|<span data-ttu-id="2936b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2936b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2936b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2936b-125">Accept</span></span>|<span data-ttu-id="2936b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2936b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2936b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2936b-127">Request body</span></span>
<span data-ttu-id="2936b-128">В теле запроса предоставляем представление объекта [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="2936b-128">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="2936b-129">В следующей таблице показаны свойства, необходимые при создании [объекта macOSVpnConfiguration.](../resources/intune-deviceconfig-macosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-129">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="2936b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2936b-130">Property</span></span>|<span data-ttu-id="2936b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2936b-131">Type</span></span>|<span data-ttu-id="2936b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2936b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2936b-133">id</span><span class="sxs-lookup"><span data-stu-id="2936b-133">id</span></span>|<span data-ttu-id="2936b-134">String</span><span class="sxs-lookup"><span data-stu-id="2936b-134">String</span></span>|<span data-ttu-id="2936b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2936b-135">Key of the entity.</span></span> <span data-ttu-id="2936b-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2936b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2936b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2936b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2936b-138">DateTimeOffset</span></span>|<span data-ttu-id="2936b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2936b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2936b-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2936b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2936b-141">roleScopeTagIds</span></span>|<span data-ttu-id="2936b-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2936b-142">String collection</span></span>|<span data-ttu-id="2936b-143">Список тегов области для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2936b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2936b-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2936b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2936b-145">supportsScopeTags</span></span>|<span data-ttu-id="2936b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2936b-146">Boolean</span></span>|<span data-ttu-id="2936b-147">Указывает, поддерживает ли конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="2936b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2936b-148">Назначение свойству ScopeTags не допускается, если это значение имеет значение false, а сущности не будут видны пользователям с заданной областью действия.</span><span class="sxs-lookup"><span data-stu-id="2936b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2936b-149">Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2936b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2936b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2936b-150">This property is read-only.</span></span> <span data-ttu-id="2936b-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2936b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2936b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2936b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2936b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2936b-154">Применимость выпуска ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2936b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2936b-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2936b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2936b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2936b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2936b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2936b-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2936b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2936b-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2936b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2936b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2936b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2936b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2936b-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2936b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2936b-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2936b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2936b-164">createdDateTime</span></span>|<span data-ttu-id="2936b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2936b-165">DateTimeOffset</span></span>|<span data-ttu-id="2936b-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2936b-166">DateTime the object was created.</span></span> <span data-ttu-id="2936b-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2936b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-168">description</span><span class="sxs-lookup"><span data-stu-id="2936b-168">description</span></span>|<span data-ttu-id="2936b-169">String</span><span class="sxs-lookup"><span data-stu-id="2936b-169">String</span></span>|<span data-ttu-id="2936b-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2936b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2936b-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2936b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="2936b-172">displayName</span></span>|<span data-ttu-id="2936b-173">String</span><span class="sxs-lookup"><span data-stu-id="2936b-173">String</span></span>|<span data-ttu-id="2936b-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2936b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2936b-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2936b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-176">version</span><span class="sxs-lookup"><span data-stu-id="2936b-176">version</span></span>|<span data-ttu-id="2936b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="2936b-177">Int32</span></span>|<span data-ttu-id="2936b-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2936b-178">Version of the device configuration.</span></span> <span data-ttu-id="2936b-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2936b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="2936b-180">connectionName</span></span>|<span data-ttu-id="2936b-181">String</span><span class="sxs-lookup"><span data-stu-id="2936b-181">String</span></span>|<span data-ttu-id="2936b-182">Имя подключения, отображаемая для пользователя.</span><span class="sxs-lookup"><span data-stu-id="2936b-182">Connection name displayed to the user.</span></span> <span data-ttu-id="2936b-183">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="2936b-184">connectionType</span></span>|[<span data-ttu-id="2936b-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="2936b-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="2936b-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="2936b-186">Connection type.</span></span> <span data-ttu-id="2936b-187">Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="2936b-188">Возможные значения: `ciscoAnyConnect` , , , , , , , `pulseSecure` , , `f5EdgeClient` , `dellSonicWallMobileConnect` , , , `checkPointCapsuleVpn` , `customVpn` , , `ciscoIPSec` `citrix` `ciscoAnyConnectV2` , `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` .</span><span class="sxs-lookup"><span data-stu-id="2936b-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="2936b-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="2936b-189">loginGroupOrDomain</span></span>|<span data-ttu-id="2936b-190">String</span><span class="sxs-lookup"><span data-stu-id="2936b-190">String</span></span>|<span data-ttu-id="2936b-191">Группа входа или домен, если для типа подключения установлено мобильное подключение Dell SonicWALL.</span><span class="sxs-lookup"><span data-stu-id="2936b-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="2936b-192">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-193">role</span><span class="sxs-lookup"><span data-stu-id="2936b-193">role</span></span>|<span data-ttu-id="2936b-194">String</span><span class="sxs-lookup"><span data-stu-id="2936b-194">String</span></span>|<span data-ttu-id="2936b-195">Роль, если для типа подключения установлено значение Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="2936b-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="2936b-196">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-197">realm</span><span class="sxs-lookup"><span data-stu-id="2936b-197">realm</span></span>|<span data-ttu-id="2936b-198">String</span><span class="sxs-lookup"><span data-stu-id="2936b-198">String</span></span>|<span data-ttu-id="2936b-199">Область, когда для типа подключения установлено безопасное пульса.</span><span class="sxs-lookup"><span data-stu-id="2936b-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="2936b-200">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-201">server</span><span class="sxs-lookup"><span data-stu-id="2936b-201">server</span></span>|[<span data-ttu-id="2936b-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="2936b-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="2936b-203">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="2936b-203">VPN Server on the network.</span></span> <span data-ttu-id="2936b-204">Убедитесь, что конечные пользователи могут получить доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="2936b-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="2936b-205">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="2936b-206">identifier</span></span>|<span data-ttu-id="2936b-207">String</span><span class="sxs-lookup"><span data-stu-id="2936b-207">String</span></span>|<span data-ttu-id="2936b-208">Идентификатор, предоставляемый поставщиком VPN, если для типа подключения установлено настраиваемая VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="2936b-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="2936b-209">Например: Cisco AnyConnect использует идентификатор формы com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-210">customData</span><span class="sxs-lookup"><span data-stu-id="2936b-210">customData</span></span>|<span data-ttu-id="2936b-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="2936b-212">Пользовательские данные, если для типа подключения установлено настраиваемая VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="2936b-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="2936b-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в vpn-решении.</span><span class="sxs-lookup"><span data-stu-id="2936b-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="2936b-214">Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="2936b-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="2936b-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="2936b-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="2936b-216">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="2936b-217">customKeyValueData</span></span>|<span data-ttu-id="2936b-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="2936b-219">Пользовательские данные, если для типа подключения установлено настраиваемая VPN-сеть.</span><span class="sxs-lookup"><span data-stu-id="2936b-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="2936b-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в vpn-решении.</span><span class="sxs-lookup"><span data-stu-id="2936b-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="2936b-221">Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары ключ-значение.</span><span class="sxs-lookup"><span data-stu-id="2936b-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="2936b-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="2936b-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="2936b-223">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="2936b-224">enableSplitTunneling</span></span>|<span data-ttu-id="2936b-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="2936b-225">Boolean</span></span>|<span data-ttu-id="2936b-226">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="2936b-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="2936b-227">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2936b-228">authenticationMethod</span></span>|[<span data-ttu-id="2936b-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2936b-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="2936b-230">Метод проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="2936b-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="2936b-231">Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="2936b-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="2936b-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="2936b-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="2936b-233">enablePerApp</span></span>|<span data-ttu-id="2936b-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="2936b-234">Boolean</span></span>|<span data-ttu-id="2936b-235">Если установить для этого параметра Per-App vpn, которые впоследствии могут быть связаны с приложениями, которые могут активирует этот коннекциатор VPN на устройстве конечного пользователя с iOS.</span><span class="sxs-lookup"><span data-stu-id="2936b-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="2936b-236">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="2936b-237">safariDomains</span></span>|<span data-ttu-id="2936b-238">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2936b-238">String collection</span></span>|<span data-ttu-id="2936b-239">Домены Safari, если этот параметр VPN для каждого приложения включен.</span><span class="sxs-lookup"><span data-stu-id="2936b-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="2936b-240">Помимо приложений, связанных с этим VPN, указанные здесь домены Safari также смогут запускать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="2936b-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="2936b-241">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="2936b-242">onDemandRules</span></span>|<span data-ttu-id="2936b-243">[Коллекция vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="2936b-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="2936b-244">On-Demand Rules.</span></span> <span data-ttu-id="2936b-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="2936b-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="2936b-246">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-247">providerType</span><span class="sxs-lookup"><span data-stu-id="2936b-247">providerType</span></span>|[<span data-ttu-id="2936b-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="2936b-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="2936b-249">Тип поставщика для VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="2936b-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="2936b-250">Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="2936b-251">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="2936b-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="2936b-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="2936b-252">associatedDomains</span></span>|<span data-ttu-id="2936b-253">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2936b-253">String collection</span></span>|<span data-ttu-id="2936b-254">Связанные домены, унаследованные от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="2936b-255">excludedDomains</span></span>|<span data-ttu-id="2936b-256">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2936b-256">String collection</span></span>|<span data-ttu-id="2936b-257">Домены, которые доступны через общедоступный Интернет, а не через VPN, даже если активирован VPN для каждого приложения. Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="2936b-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="2936b-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="2936b-259">Boolean</span></span>|<span data-ttu-id="2936b-260">Переключение, чтобы запретить пользователю отключать автоматическую vpn-сеть в приложении "Параметры". Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-261">proxyServer</span><span class="sxs-lookup"><span data-stu-id="2936b-261">proxyServer</span></span>|[<span data-ttu-id="2936b-262">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="2936b-262">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="2936b-263">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="2936b-263">Proxy Server.</span></span> <span data-ttu-id="2936b-264">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-264">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2936b-265">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="2936b-265">optInToDeviceIdSharing</span></span>|<span data-ttu-id="2936b-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="2936b-266">Boolean</span></span>|<span data-ttu-id="2936b-267">Opt-In к совместному использованию удостоверения устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="2936b-267">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="2936b-268">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2936b-268">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2936b-269">Отклик</span><span class="sxs-lookup"><span data-stu-id="2936b-269">Response</span></span>
<span data-ttu-id="2936b-270">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2936b-270">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2936b-271">Пример</span><span class="sxs-lookup"><span data-stu-id="2936b-271">Example</span></span>

### <a name="request"></a><span data-ttu-id="2936b-272">Запрос</span><span class="sxs-lookup"><span data-stu-id="2936b-272">Request</span></span>
<span data-ttu-id="2936b-273">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2936b-273">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2825

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
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true
}
```

### <a name="response"></a><span data-ttu-id="2936b-274">Отклик</span><span class="sxs-lookup"><span data-stu-id="2936b-274">Response</span></span>
<span data-ttu-id="2936b-p130">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2936b-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2997

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
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true
}
```




