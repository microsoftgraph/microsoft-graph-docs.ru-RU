---
title: Создание iosVpnConfiguration
description: Создание объекта iosVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 62fbdb6406d2c33541ca82a324836d1f66c265ed
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155806"
---
# <a name="create-iosvpnconfiguration"></a><span data-ttu-id="c1a01-103">Создание iosVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c1a01-103">Create iosVpnConfiguration</span></span>

<span data-ttu-id="c1a01-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1a01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1a01-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1a01-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1a01-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1a01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1a01-107">Создание объекта [iosVpnConfiguration.](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-107">Create a new [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1a01-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c1a01-108">Prerequisites</span></span>
<span data-ttu-id="c1a01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1a01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1a01-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1a01-111">Permission type</span></span>|<span data-ttu-id="c1a01-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1a01-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1a01-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1a01-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1a01-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1a01-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1a01-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1a01-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1a01-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1a01-116">Not supported.</span></span>|
|<span data-ttu-id="c1a01-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1a01-117">Application</span></span>|<span data-ttu-id="c1a01-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1a01-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1a01-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1a01-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c1a01-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c1a01-120">Request headers</span></span>
|<span data-ttu-id="c1a01-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1a01-121">Header</span></span>|<span data-ttu-id="c1a01-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c1a01-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1a01-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1a01-123">Authorization</span></span>|<span data-ttu-id="c1a01-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1a01-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1a01-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c1a01-125">Accept</span></span>|<span data-ttu-id="c1a01-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1a01-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1a01-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1a01-127">Request body</span></span>
<span data-ttu-id="c1a01-128">В теле запроса предоставляем представление объекта iosVpnConfiguration в JSON.</span><span class="sxs-lookup"><span data-stu-id="c1a01-128">In the request body, supply a JSON representation for the iosVpnConfiguration object.</span></span>

<span data-ttu-id="c1a01-129">В следующей таблице показаны свойства, необходимые при создании объекта iosVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c1a01-129">The following table shows the properties that are required when you create the iosVpnConfiguration.</span></span>

|<span data-ttu-id="c1a01-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1a01-130">Property</span></span>|<span data-ttu-id="c1a01-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c1a01-131">Type</span></span>|<span data-ttu-id="c1a01-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c1a01-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1a01-133">id</span><span class="sxs-lookup"><span data-stu-id="c1a01-133">id</span></span>|<span data-ttu-id="c1a01-134">String</span><span class="sxs-lookup"><span data-stu-id="c1a01-134">String</span></span>|<span data-ttu-id="c1a01-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c1a01-135">Key of the entity.</span></span> <span data-ttu-id="c1a01-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1a01-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1a01-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c1a01-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1a01-138">DateTimeOffset</span></span>|<span data-ttu-id="c1a01-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c1a01-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c1a01-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1a01-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c1a01-141">roleScopeTagIds</span></span>|<span data-ttu-id="c1a01-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c1a01-142">String collection</span></span>|<span data-ttu-id="c1a01-143">Список тегов области для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c1a01-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c1a01-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1a01-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c1a01-145">supportsScopeTags</span></span>|<span data-ttu-id="c1a01-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1a01-146">Boolean</span></span>|<span data-ttu-id="c1a01-147">Указывает, поддерживает ли конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c1a01-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c1a01-148">Назначение свойству ScopeTags запрещено, если это значение имеет значение false, а сущности не будут видны пользователям с заданной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c1a01-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c1a01-149">Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить, удавшись и повторно создав политику на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c1a01-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c1a01-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1a01-150">This property is read-only.</span></span> <span data-ttu-id="c1a01-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1a01-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c1a01-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c1a01-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c1a01-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c1a01-154">Применимость выпуска ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c1a01-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c1a01-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1a01-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c1a01-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c1a01-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c1a01-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c1a01-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c1a01-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c1a01-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1a01-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c1a01-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c1a01-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c1a01-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c1a01-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c1a01-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c1a01-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1a01-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1a01-164">createdDateTime</span></span>|<span data-ttu-id="c1a01-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1a01-165">DateTimeOffset</span></span>|<span data-ttu-id="c1a01-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c1a01-166">DateTime the object was created.</span></span> <span data-ttu-id="c1a01-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1a01-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-168">description</span><span class="sxs-lookup"><span data-stu-id="c1a01-168">description</span></span>|<span data-ttu-id="c1a01-169">String</span><span class="sxs-lookup"><span data-stu-id="c1a01-169">String</span></span>|<span data-ttu-id="c1a01-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c1a01-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c1a01-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1a01-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c1a01-172">displayName</span></span>|<span data-ttu-id="c1a01-173">String</span><span class="sxs-lookup"><span data-stu-id="c1a01-173">String</span></span>|<span data-ttu-id="c1a01-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c1a01-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c1a01-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1a01-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-176">version</span><span class="sxs-lookup"><span data-stu-id="c1a01-176">version</span></span>|<span data-ttu-id="c1a01-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c1a01-177">Int32</span></span>|<span data-ttu-id="c1a01-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c1a01-178">Version of the device configuration.</span></span> <span data-ttu-id="c1a01-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c1a01-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="c1a01-180">connectionName</span></span>|<span data-ttu-id="c1a01-181">String</span><span class="sxs-lookup"><span data-stu-id="c1a01-181">String</span></span>|<span data-ttu-id="c1a01-182">Имя подключения, отображаемая для пользователя.</span><span class="sxs-lookup"><span data-stu-id="c1a01-182">Connection name displayed to the user.</span></span> <span data-ttu-id="c1a01-183">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="c1a01-184">connectionType</span></span>|[<span data-ttu-id="c1a01-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="c1a01-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="c1a01-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="c1a01-186">Connection type.</span></span> <span data-ttu-id="c1a01-187">Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="c1a01-188">Возможные значения: `ciscoAnyConnect` , , , , , , , `pulseSecure` , , `f5EdgeClient` , `dellSonicWallMobileConnect` , , , `checkPointCapsuleVpn` , `customVpn` , , `ciscoIPSec` `citrix` `ciscoAnyConnectV2` , `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` .</span><span class="sxs-lookup"><span data-stu-id="c1a01-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="c1a01-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="c1a01-189">loginGroupOrDomain</span></span>|<span data-ttu-id="c1a01-190">String</span><span class="sxs-lookup"><span data-stu-id="c1a01-190">String</span></span>|<span data-ttu-id="c1a01-191">Группа входа или домен, если для типа подключения установлено мобильное подключение Dell SonicWALL.</span><span class="sxs-lookup"><span data-stu-id="c1a01-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="c1a01-192">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-193">role</span><span class="sxs-lookup"><span data-stu-id="c1a01-193">role</span></span>|<span data-ttu-id="c1a01-194">String</span><span class="sxs-lookup"><span data-stu-id="c1a01-194">String</span></span>|<span data-ttu-id="c1a01-195">Роль, если для типа подключения установлено значение Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="c1a01-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="c1a01-196">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-197">realm</span><span class="sxs-lookup"><span data-stu-id="c1a01-197">realm</span></span>|<span data-ttu-id="c1a01-198">String</span><span class="sxs-lookup"><span data-stu-id="c1a01-198">String</span></span>|<span data-ttu-id="c1a01-199">Область, когда для типа подключения установлено "Pulse Secure".</span><span class="sxs-lookup"><span data-stu-id="c1a01-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="c1a01-200">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-201">server</span><span class="sxs-lookup"><span data-stu-id="c1a01-201">server</span></span>|[<span data-ttu-id="c1a01-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="c1a01-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="c1a01-203">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="c1a01-203">VPN Server on the network.</span></span> <span data-ttu-id="c1a01-204">Убедитесь, что конечные пользователи могут получить доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="c1a01-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="c1a01-205">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="c1a01-206">identifier</span></span>|<span data-ttu-id="c1a01-207">String</span><span class="sxs-lookup"><span data-stu-id="c1a01-207">String</span></span>|<span data-ttu-id="c1a01-208">Идентификатор, предоставляемый поставщиком VPN, если для типа подключения за установлено настраиваемого VPN.</span><span class="sxs-lookup"><span data-stu-id="c1a01-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="c1a01-209">Например: Cisco AnyConnect использует идентификатор формы com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-210">customData</span><span class="sxs-lookup"><span data-stu-id="c1a01-210">customData</span></span>|<span data-ttu-id="c1a01-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="c1a01-212">Пользовательские данные, если для типа подключения установлено настраиваемая VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="c1a01-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="c1a01-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в вашем VPN-решении.</span><span class="sxs-lookup"><span data-stu-id="c1a01-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="c1a01-214">Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="c1a01-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="c1a01-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="c1a01-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="c1a01-216">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="c1a01-217">customKeyValueData</span></span>|<span data-ttu-id="c1a01-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c1a01-219">Пользовательские данные, если для типа подключения установлено настраиваемая VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="c1a01-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="c1a01-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в vpn-решении.</span><span class="sxs-lookup"><span data-stu-id="c1a01-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="c1a01-221">Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="c1a01-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="c1a01-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="c1a01-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="c1a01-223">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="c1a01-224">enableSplitTunneling</span></span>|<span data-ttu-id="c1a01-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1a01-225">Boolean</span></span>|<span data-ttu-id="c1a01-226">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="c1a01-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="c1a01-227">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c1a01-228">authenticationMethod</span></span>|[<span data-ttu-id="c1a01-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c1a01-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="c1a01-230">Метод проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="c1a01-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="c1a01-231">Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="c1a01-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="c1a01-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="c1a01-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="c1a01-233">enablePerApp</span></span>|<span data-ttu-id="c1a01-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1a01-234">Boolean</span></span>|<span data-ttu-id="c1a01-235">Если установить для этого параметра Per-App vpn, которые впоследствии могут быть связаны с приложениями, которые могут активирует этот коннекциатор VPN на устройстве конечного пользователя с iOS.</span><span class="sxs-lookup"><span data-stu-id="c1a01-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="c1a01-236">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="c1a01-237">safariDomains</span></span>|<span data-ttu-id="c1a01-238">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c1a01-238">String collection</span></span>|<span data-ttu-id="c1a01-239">Домены Safari, если этот параметр VPN для каждого приложения включен.</span><span class="sxs-lookup"><span data-stu-id="c1a01-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="c1a01-240">Помимо приложений, связанных с этим VPN, указанные здесь домены Safari также смогут запускать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="c1a01-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="c1a01-241">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="c1a01-242">onDemandRules</span></span>|<span data-ttu-id="c1a01-243">[Коллекция vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="c1a01-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="c1a01-244">On-Demand Rules.</span></span> <span data-ttu-id="c1a01-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c1a01-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c1a01-246">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-247">providerType</span><span class="sxs-lookup"><span data-stu-id="c1a01-247">providerType</span></span>|[<span data-ttu-id="c1a01-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="c1a01-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="c1a01-249">Тип поставщика для VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="c1a01-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="c1a01-250">Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="c1a01-251">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="c1a01-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="c1a01-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="c1a01-252">associatedDomains</span></span>|<span data-ttu-id="c1a01-253">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c1a01-253">String collection</span></span>|<span data-ttu-id="c1a01-254">Связанные домены, унаследованные [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="c1a01-255">excludedDomains</span></span>|<span data-ttu-id="c1a01-256">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c1a01-256">String collection</span></span>|<span data-ttu-id="c1a01-257">Домены, которые доступны через общедоступный Интернет, а не через VPN, даже если активирован VPN для каждого приложения. Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="c1a01-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="c1a01-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1a01-259">Boolean</span></span>|<span data-ttu-id="c1a01-260">Переключение, чтобы запретить пользователю отключать автоматическую vpn-сеть в приложении "Параметры". Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-261">proxyServer</span><span class="sxs-lookup"><span data-stu-id="c1a01-261">proxyServer</span></span>|[<span data-ttu-id="c1a01-262">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="c1a01-262">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="c1a01-263">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="c1a01-263">Proxy Server.</span></span> <span data-ttu-id="c1a01-264">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-264">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-265">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="c1a01-265">optInToDeviceIdSharing</span></span>|<span data-ttu-id="c1a01-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1a01-266">Boolean</span></span>|<span data-ttu-id="c1a01-267">Opt-In к совместному использованию удостоверения устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="c1a01-267">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="c1a01-268">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-268">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="c1a01-269">userDomain</span><span class="sxs-lookup"><span data-stu-id="c1a01-269">userDomain</span></span>|<span data-ttu-id="c1a01-270">String</span><span class="sxs-lookup"><span data-stu-id="c1a01-270">String</span></span>|<span data-ttu-id="c1a01-271">Только Zscaler.</span><span class="sxs-lookup"><span data-stu-id="c1a01-271">Zscaler only.</span></span> <span data-ttu-id="c1a01-272">Введите статический домен для предварительного заполнения поля входа в приложение Zscaler.</span><span class="sxs-lookup"><span data-stu-id="c1a01-272">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="c1a01-273">Если оставить его пустым, будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="c1a01-273">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="c1a01-274">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="c1a01-274">strictEnforcement</span></span>|<span data-ttu-id="c1a01-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1a01-275">Boolean</span></span>|<span data-ttu-id="c1a01-276">Только Zscaler.</span><span class="sxs-lookup"><span data-stu-id="c1a01-276">Zscaler only.</span></span> <span data-ttu-id="c1a01-277">Блокирует сетевой трафик, пока пользователь не войди в приложение Zscaler.</span><span class="sxs-lookup"><span data-stu-id="c1a01-277">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="c1a01-278">"True" означает, что трафик заблокирован.</span><span class="sxs-lookup"><span data-stu-id="c1a01-278">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="c1a01-279">cloudName</span><span class="sxs-lookup"><span data-stu-id="c1a01-279">cloudName</span></span>|<span data-ttu-id="c1a01-280">String</span><span class="sxs-lookup"><span data-stu-id="c1a01-280">String</span></span>|<span data-ttu-id="c1a01-281">Только Zscaler.</span><span class="sxs-lookup"><span data-stu-id="c1a01-281">Zscaler only.</span></span> <span data-ttu-id="c1a01-282">Облако Zscaler, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="c1a01-282">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="c1a01-283">excludeList</span><span class="sxs-lookup"><span data-stu-id="c1a01-283">excludeList</span></span>|<span data-ttu-id="c1a01-284">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c1a01-284">String collection</span></span>|<span data-ttu-id="c1a01-285">Только Zscaler.</span><span class="sxs-lookup"><span data-stu-id="c1a01-285">Zscaler only.</span></span> <span data-ttu-id="c1a01-286">Список сетевых адресов, которые не отправляются через облако Zscaler.</span><span class="sxs-lookup"><span data-stu-id="c1a01-286">List of network addresses which are not sent through the Zscaler cloud.</span></span>|
|<span data-ttu-id="c1a01-287">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="c1a01-287">targetedMobileApps</span></span>|<span data-ttu-id="c1a01-288">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c1a01-288">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c1a01-289">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="c1a01-289">Targeted mobile apps.</span></span> <span data-ttu-id="c1a01-290">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c1a01-290">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c1a01-291">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="c1a01-291">microsoftTunnelSiteId</span></span>|<span data-ttu-id="c1a01-292">String</span><span class="sxs-lookup"><span data-stu-id="c1a01-292">String</span></span>|<span data-ttu-id="c1a01-293">Microsoft Tunnel site ID.</span><span class="sxs-lookup"><span data-stu-id="c1a01-293">Microsoft Tunnel site ID.</span></span>|



## <a name="response"></a><span data-ttu-id="c1a01-294">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1a01-294">Response</span></span>
<span data-ttu-id="c1a01-295">В случае успеха этот метод возвращает код отклика и объект `201 Created` [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c1a01-295">If successful, this method returns a `201 Created` response code and a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1a01-296">Пример</span><span class="sxs-lookup"><span data-stu-id="c1a01-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1a01-297">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1a01-297">Request</span></span>
<span data-ttu-id="c1a01-298">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1a01-298">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3298

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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```

### <a name="response"></a><span data-ttu-id="c1a01-299">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1a01-299">Response</span></span>
<span data-ttu-id="c1a01-p135">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1a01-p135">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3470

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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```




