---
title: Создание macOSVpnConfiguration
description: Создание объекта macOSVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d5b22cb759459599118632047e12e9693910ad9f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157990"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="279b0-103">Создание macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="279b0-103">Create macOSVpnConfiguration</span></span>

<span data-ttu-id="279b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="279b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="279b0-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="279b0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="279b0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="279b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="279b0-107">Создание объекта [macOSVpnConfiguration.](../resources/intune-deviceconfig-macosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-107">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="279b0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="279b0-108">Prerequisites</span></span>
<span data-ttu-id="279b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="279b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="279b0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="279b0-111">Permission type</span></span>|<span data-ttu-id="279b0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="279b0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="279b0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="279b0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="279b0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="279b0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="279b0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="279b0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="279b0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="279b0-116">Not supported.</span></span>|
|<span data-ttu-id="279b0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="279b0-117">Application</span></span>|<span data-ttu-id="279b0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="279b0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="279b0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="279b0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="279b0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="279b0-120">Request headers</span></span>
|<span data-ttu-id="279b0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="279b0-121">Header</span></span>|<span data-ttu-id="279b0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="279b0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="279b0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="279b0-123">Authorization</span></span>|<span data-ttu-id="279b0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="279b0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="279b0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="279b0-125">Accept</span></span>|<span data-ttu-id="279b0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="279b0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="279b0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="279b0-127">Request body</span></span>
<span data-ttu-id="279b0-128">В теле запроса предоставляем представление объекта macOSVpnConfiguration в JSON.</span><span class="sxs-lookup"><span data-stu-id="279b0-128">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="279b0-129">В следующей таблице показаны свойства, необходимые при создании объекта macOSVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="279b0-129">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="279b0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="279b0-130">Property</span></span>|<span data-ttu-id="279b0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="279b0-131">Type</span></span>|<span data-ttu-id="279b0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="279b0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="279b0-133">id</span><span class="sxs-lookup"><span data-stu-id="279b0-133">id</span></span>|<span data-ttu-id="279b0-134">String</span><span class="sxs-lookup"><span data-stu-id="279b0-134">String</span></span>|<span data-ttu-id="279b0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="279b0-135">Key of the entity.</span></span> <span data-ttu-id="279b0-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="279b0-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="279b0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="279b0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="279b0-138">DateTimeOffset</span></span>|<span data-ttu-id="279b0-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="279b0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="279b0-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="279b0-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="279b0-141">roleScopeTagIds</span></span>|<span data-ttu-id="279b0-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="279b0-142">String collection</span></span>|<span data-ttu-id="279b0-143">Список тегов области для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="279b0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="279b0-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="279b0-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="279b0-145">supportsScopeTags</span></span>|<span data-ttu-id="279b0-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="279b0-146">Boolean</span></span>|<span data-ttu-id="279b0-147">Указывает, поддерживает ли конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="279b0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="279b0-148">Назначение свойству ScopeTags не допускается, если это значение имеет значение false, а сущности не будут видны пользователям с заданной областью действия.</span><span class="sxs-lookup"><span data-stu-id="279b0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="279b0-149">Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="279b0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="279b0-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="279b0-150">This property is read-only.</span></span> <span data-ttu-id="279b0-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="279b0-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="279b0-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="279b0-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="279b0-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="279b0-154">Применимость выпуска ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="279b0-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="279b0-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="279b0-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="279b0-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="279b0-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="279b0-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="279b0-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="279b0-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="279b0-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="279b0-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="279b0-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="279b0-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="279b0-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="279b0-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="279b0-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="279b0-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="279b0-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="279b0-164">createdDateTime</span></span>|<span data-ttu-id="279b0-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="279b0-165">DateTimeOffset</span></span>|<span data-ttu-id="279b0-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="279b0-166">DateTime the object was created.</span></span> <span data-ttu-id="279b0-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="279b0-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-168">description</span><span class="sxs-lookup"><span data-stu-id="279b0-168">description</span></span>|<span data-ttu-id="279b0-169">String</span><span class="sxs-lookup"><span data-stu-id="279b0-169">String</span></span>|<span data-ttu-id="279b0-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="279b0-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="279b0-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="279b0-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-172">displayName</span><span class="sxs-lookup"><span data-stu-id="279b0-172">displayName</span></span>|<span data-ttu-id="279b0-173">String</span><span class="sxs-lookup"><span data-stu-id="279b0-173">String</span></span>|<span data-ttu-id="279b0-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="279b0-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="279b0-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="279b0-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-176">version</span><span class="sxs-lookup"><span data-stu-id="279b0-176">version</span></span>|<span data-ttu-id="279b0-177">Int32</span><span class="sxs-lookup"><span data-stu-id="279b0-177">Int32</span></span>|<span data-ttu-id="279b0-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="279b0-178">Version of the device configuration.</span></span> <span data-ttu-id="279b0-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="279b0-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="279b0-180">connectionName</span></span>|<span data-ttu-id="279b0-181">String</span><span class="sxs-lookup"><span data-stu-id="279b0-181">String</span></span>|<span data-ttu-id="279b0-182">Имя подключения, отображаемая для пользователя.</span><span class="sxs-lookup"><span data-stu-id="279b0-182">Connection name displayed to the user.</span></span> <span data-ttu-id="279b0-183">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="279b0-184">connectionType</span></span>|[<span data-ttu-id="279b0-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="279b0-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="279b0-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="279b0-186">Connection type.</span></span> <span data-ttu-id="279b0-187">Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="279b0-188">Возможные значения: `ciscoAnyConnect` , , , , , , , `pulseSecure` , , `f5EdgeClient` , `dellSonicWallMobileConnect` , , , `checkPointCapsuleVpn` , `customVpn` , , `ciscoIPSec` `citrix` `ciscoAnyConnectV2` , `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` .</span><span class="sxs-lookup"><span data-stu-id="279b0-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="279b0-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="279b0-189">loginGroupOrDomain</span></span>|<span data-ttu-id="279b0-190">String</span><span class="sxs-lookup"><span data-stu-id="279b0-190">String</span></span>|<span data-ttu-id="279b0-191">Группа входа или домен, если для типа подключения установлено мобильное подключение Dell SonicWALL.</span><span class="sxs-lookup"><span data-stu-id="279b0-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="279b0-192">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-193">role</span><span class="sxs-lookup"><span data-stu-id="279b0-193">role</span></span>|<span data-ttu-id="279b0-194">String</span><span class="sxs-lookup"><span data-stu-id="279b0-194">String</span></span>|<span data-ttu-id="279b0-195">Роль, если для типа подключения установлено значение Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="279b0-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="279b0-196">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-197">realm</span><span class="sxs-lookup"><span data-stu-id="279b0-197">realm</span></span>|<span data-ttu-id="279b0-198">String</span><span class="sxs-lookup"><span data-stu-id="279b0-198">String</span></span>|<span data-ttu-id="279b0-199">Область, когда для типа подключения установлено "Pulse Secure".</span><span class="sxs-lookup"><span data-stu-id="279b0-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="279b0-200">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-201">server</span><span class="sxs-lookup"><span data-stu-id="279b0-201">server</span></span>|[<span data-ttu-id="279b0-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="279b0-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="279b0-203">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="279b0-203">VPN Server on the network.</span></span> <span data-ttu-id="279b0-204">Убедитесь, что конечные пользователи могут получить доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="279b0-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="279b0-205">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="279b0-206">identifier</span></span>|<span data-ttu-id="279b0-207">String</span><span class="sxs-lookup"><span data-stu-id="279b0-207">String</span></span>|<span data-ttu-id="279b0-208">Идентификатор, предоставляемый поставщиком VPN, если для типа подключения за установлено настраиваемого VPN.</span><span class="sxs-lookup"><span data-stu-id="279b0-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="279b0-209">Например: Cisco AnyConnect использует идентификатор формы com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-210">customData</span><span class="sxs-lookup"><span data-stu-id="279b0-210">customData</span></span>|<span data-ttu-id="279b0-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="279b0-212">Пользовательские данные, если для типа подключения установлено настраиваемая VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="279b0-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="279b0-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в вашем VPN-решении.</span><span class="sxs-lookup"><span data-stu-id="279b0-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="279b0-214">Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары ключ-значение.</span><span class="sxs-lookup"><span data-stu-id="279b0-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="279b0-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="279b0-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="279b0-216">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="279b0-217">customKeyValueData</span></span>|<span data-ttu-id="279b0-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="279b0-219">Пользовательские данные, если для типа подключения установлено настраиваемая VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="279b0-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="279b0-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в vpn-решении.</span><span class="sxs-lookup"><span data-stu-id="279b0-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="279b0-221">Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="279b0-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="279b0-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="279b0-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="279b0-223">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="279b0-224">enableSplitTunneling</span></span>|<span data-ttu-id="279b0-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="279b0-225">Boolean</span></span>|<span data-ttu-id="279b0-226">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="279b0-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="279b0-227">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="279b0-228">authenticationMethod</span></span>|[<span data-ttu-id="279b0-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="279b0-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="279b0-230">Метод проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="279b0-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="279b0-231">Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="279b0-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="279b0-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="279b0-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="279b0-233">enablePerApp</span></span>|<span data-ttu-id="279b0-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="279b0-234">Boolean</span></span>|<span data-ttu-id="279b0-235">Если установить для этого параметра Per-App vpn, которые впоследствии могут быть связаны с приложениями, которые могут активирует этот коннекциатор VPN на устройстве пользователя с iOS.</span><span class="sxs-lookup"><span data-stu-id="279b0-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="279b0-236">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="279b0-237">safariDomains</span></span>|<span data-ttu-id="279b0-238">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="279b0-238">String collection</span></span>|<span data-ttu-id="279b0-239">Домены Safari, если этот параметр VPN для каждого приложения включен.</span><span class="sxs-lookup"><span data-stu-id="279b0-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="279b0-240">Помимо приложений, связанных с этим VPN, указанные здесь домены Safari также смогут запускать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="279b0-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="279b0-241">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="279b0-242">onDemandRules</span></span>|<span data-ttu-id="279b0-243">[Коллекция vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="279b0-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="279b0-244">On-Demand Rules.</span></span> <span data-ttu-id="279b0-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="279b0-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="279b0-246">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-247">providerType</span><span class="sxs-lookup"><span data-stu-id="279b0-247">providerType</span></span>|[<span data-ttu-id="279b0-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="279b0-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="279b0-249">Тип поставщика для VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="279b0-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="279b0-250">Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="279b0-251">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="279b0-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="279b0-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="279b0-252">associatedDomains</span></span>|<span data-ttu-id="279b0-253">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="279b0-253">String collection</span></span>|<span data-ttu-id="279b0-254">Связанные домены, унаследованные от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="279b0-255">excludedDomains</span></span>|<span data-ttu-id="279b0-256">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="279b0-256">String collection</span></span>|<span data-ttu-id="279b0-257">Домены, которые доступны через общедоступный Интернет, а не через VPN, даже если активирован VPN для каждого приложения. Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="279b0-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="279b0-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="279b0-259">Boolean</span></span>|<span data-ttu-id="279b0-260">Переключение, чтобы запретить пользователю отключать автоматическую vpn-сеть в приложении "Параметры". Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-261">proxyServer</span><span class="sxs-lookup"><span data-stu-id="279b0-261">proxyServer</span></span>|[<span data-ttu-id="279b0-262">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="279b0-262">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="279b0-263">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="279b0-263">Proxy Server.</span></span> <span data-ttu-id="279b0-264">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-264">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="279b0-265">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="279b0-265">optInToDeviceIdSharing</span></span>|<span data-ttu-id="279b0-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="279b0-266">Boolean</span></span>|<span data-ttu-id="279b0-267">Opt-In к совместному использованию удостоверения устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="279b0-267">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="279b0-268">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="279b0-268">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="279b0-269">Отклик</span><span class="sxs-lookup"><span data-stu-id="279b0-269">Response</span></span>
<span data-ttu-id="279b0-270">В случае успеха этот метод возвращает код отклика и объект `201 Created` [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="279b0-270">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="279b0-271">Пример</span><span class="sxs-lookup"><span data-stu-id="279b0-271">Example</span></span>

### <a name="request"></a><span data-ttu-id="279b0-272">Запрос</span><span class="sxs-lookup"><span data-stu-id="279b0-272">Request</span></span>
<span data-ttu-id="279b0-273">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="279b0-273">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="279b0-274">Отклик</span><span class="sxs-lookup"><span data-stu-id="279b0-274">Response</span></span>
<span data-ttu-id="279b0-p130">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="279b0-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




