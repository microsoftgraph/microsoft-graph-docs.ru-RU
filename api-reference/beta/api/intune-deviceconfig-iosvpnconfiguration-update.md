---
title: Обновление iosVpnConfiguration
description: Обновление свойств объекта iosVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 88b7cc4f9a719afbc293b714c3319dfda750829d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154609"
---
# <a name="update-iosvpnconfiguration"></a><span data-ttu-id="da9a9-103">Обновление iosVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="da9a9-103">Update iosVpnConfiguration</span></span>

<span data-ttu-id="da9a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da9a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da9a9-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da9a9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da9a9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="da9a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da9a9-107">Обновление свойств объекта [iosVpnConfiguration.](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-107">Update the properties of a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da9a9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="da9a9-108">Prerequisites</span></span>
<span data-ttu-id="da9a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da9a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da9a9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da9a9-111">Permission type</span></span>|<span data-ttu-id="da9a9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="da9a9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da9a9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da9a9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da9a9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da9a9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da9a9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da9a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da9a9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da9a9-116">Not supported.</span></span>|
|<span data-ttu-id="da9a9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da9a9-117">Application</span></span>|<span data-ttu-id="da9a9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da9a9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da9a9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da9a9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="da9a9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="da9a9-120">Request headers</span></span>
|<span data-ttu-id="da9a9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="da9a9-121">Header</span></span>|<span data-ttu-id="da9a9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="da9a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da9a9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da9a9-123">Authorization</span></span>|<span data-ttu-id="da9a9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da9a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da9a9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="da9a9-125">Accept</span></span>|<span data-ttu-id="da9a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da9a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da9a9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da9a9-127">Request body</span></span>
<span data-ttu-id="da9a9-128">В теле запроса предоставляем представление объекта [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="da9a9-128">In the request body, supply a JSON representation for the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="da9a9-129">В следующей таблице показаны свойства, необходимые при создании [объекта iosVpnConfiguration.](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-129">The following table shows the properties that are required when you create the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span>

|<span data-ttu-id="da9a9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="da9a9-130">Property</span></span>|<span data-ttu-id="da9a9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="da9a9-131">Type</span></span>|<span data-ttu-id="da9a9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="da9a9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da9a9-133">id</span><span class="sxs-lookup"><span data-stu-id="da9a9-133">id</span></span>|<span data-ttu-id="da9a9-134">String</span><span class="sxs-lookup"><span data-stu-id="da9a9-134">String</span></span>|<span data-ttu-id="da9a9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="da9a9-135">Key of the entity.</span></span> <span data-ttu-id="da9a9-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da9a9-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da9a9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="da9a9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da9a9-138">DateTimeOffset</span></span>|<span data-ttu-id="da9a9-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="da9a9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="da9a9-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da9a9-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="da9a9-141">roleScopeTagIds</span></span>|<span data-ttu-id="da9a9-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="da9a9-142">String collection</span></span>|<span data-ttu-id="da9a9-143">Список тегов области для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="da9a9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="da9a9-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da9a9-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="da9a9-145">supportsScopeTags</span></span>|<span data-ttu-id="da9a9-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="da9a9-146">Boolean</span></span>|<span data-ttu-id="da9a9-147">Указывает, поддерживает ли конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="da9a9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="da9a9-148">Назначение свойству ScopeTags запрещено, если это значение имеет значение false, а сущности не будут видны пользователям с заданной областью действия.</span><span class="sxs-lookup"><span data-stu-id="da9a9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="da9a9-149">Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить, удавшись и повторно создав политику на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="da9a9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="da9a9-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da9a9-150">This property is read-only.</span></span> <span data-ttu-id="da9a9-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da9a9-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="da9a9-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="da9a9-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="da9a9-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="da9a9-154">Применимость выпуска ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="da9a9-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="da9a9-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da9a9-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="da9a9-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="da9a9-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="da9a9-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="da9a9-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="da9a9-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="da9a9-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da9a9-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="da9a9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="da9a9-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="da9a9-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="da9a9-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="da9a9-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="da9a9-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da9a9-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da9a9-164">createdDateTime</span></span>|<span data-ttu-id="da9a9-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da9a9-165">DateTimeOffset</span></span>|<span data-ttu-id="da9a9-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="da9a9-166">DateTime the object was created.</span></span> <span data-ttu-id="da9a9-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da9a9-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-168">description</span><span class="sxs-lookup"><span data-stu-id="da9a9-168">description</span></span>|<span data-ttu-id="da9a9-169">String</span><span class="sxs-lookup"><span data-stu-id="da9a9-169">String</span></span>|<span data-ttu-id="da9a9-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="da9a9-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="da9a9-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da9a9-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-172">displayName</span><span class="sxs-lookup"><span data-stu-id="da9a9-172">displayName</span></span>|<span data-ttu-id="da9a9-173">String</span><span class="sxs-lookup"><span data-stu-id="da9a9-173">String</span></span>|<span data-ttu-id="da9a9-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="da9a9-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="da9a9-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da9a9-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-176">version</span><span class="sxs-lookup"><span data-stu-id="da9a9-176">version</span></span>|<span data-ttu-id="da9a9-177">Int32</span><span class="sxs-lookup"><span data-stu-id="da9a9-177">Int32</span></span>|<span data-ttu-id="da9a9-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="da9a9-178">Version of the device configuration.</span></span> <span data-ttu-id="da9a9-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="da9a9-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="da9a9-180">connectionName</span></span>|<span data-ttu-id="da9a9-181">String</span><span class="sxs-lookup"><span data-stu-id="da9a9-181">String</span></span>|<span data-ttu-id="da9a9-182">Имя подключения, отображаемая для пользователя.</span><span class="sxs-lookup"><span data-stu-id="da9a9-182">Connection name displayed to the user.</span></span> <span data-ttu-id="da9a9-183">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="da9a9-184">connectionType</span></span>|[<span data-ttu-id="da9a9-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="da9a9-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="da9a9-186">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="da9a9-186">Connection type.</span></span> <span data-ttu-id="da9a9-187">Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="da9a9-188">Возможные значения: `ciscoAnyConnect` , , , , , , , `pulseSecure` , , `f5EdgeClient` , , , `dellSonicWallMobileConnect` , , , , `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` , `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` .</span><span class="sxs-lookup"><span data-stu-id="da9a9-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="da9a9-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="da9a9-189">loginGroupOrDomain</span></span>|<span data-ttu-id="da9a9-190">String</span><span class="sxs-lookup"><span data-stu-id="da9a9-190">String</span></span>|<span data-ttu-id="da9a9-191">Группа входа или домен, если для типа подключения установлено мобильное подключение Dell SonicWALL.</span><span class="sxs-lookup"><span data-stu-id="da9a9-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="da9a9-192">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-193">role</span><span class="sxs-lookup"><span data-stu-id="da9a9-193">role</span></span>|<span data-ttu-id="da9a9-194">String</span><span class="sxs-lookup"><span data-stu-id="da9a9-194">String</span></span>|<span data-ttu-id="da9a9-195">Роль, если для типа подключения установлено значение Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="da9a9-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="da9a9-196">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-197">realm</span><span class="sxs-lookup"><span data-stu-id="da9a9-197">realm</span></span>|<span data-ttu-id="da9a9-198">String</span><span class="sxs-lookup"><span data-stu-id="da9a9-198">String</span></span>|<span data-ttu-id="da9a9-199">Область, когда для типа подключения установлено безопасное пульса.</span><span class="sxs-lookup"><span data-stu-id="da9a9-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="da9a9-200">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-201">server</span><span class="sxs-lookup"><span data-stu-id="da9a9-201">server</span></span>|[<span data-ttu-id="da9a9-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="da9a9-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="da9a9-203">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="da9a9-203">VPN Server on the network.</span></span> <span data-ttu-id="da9a9-204">Убедитесь, что конечные пользователи могут получить доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="da9a9-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="da9a9-205">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-206">идентификатор</span><span class="sxs-lookup"><span data-stu-id="da9a9-206">identifier</span></span>|<span data-ttu-id="da9a9-207">String</span><span class="sxs-lookup"><span data-stu-id="da9a9-207">String</span></span>|<span data-ttu-id="da9a9-208">Идентификатор, предоставляемый поставщиком VPN, если для типа подключения установлено настраиваемая VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="da9a9-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="da9a9-209">Например: Cisco AnyConnect использует идентификатор формы com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-210">customData</span><span class="sxs-lookup"><span data-stu-id="da9a9-210">customData</span></span>|<span data-ttu-id="da9a9-211">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="da9a9-212">Пользовательские данные, если для типа подключения установлено настраиваемая VPN-сеть.</span><span class="sxs-lookup"><span data-stu-id="da9a9-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="da9a9-213">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в vpn-решении.</span><span class="sxs-lookup"><span data-stu-id="da9a9-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="da9a9-214">Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="da9a9-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="da9a9-215">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="da9a9-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="da9a9-216">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="da9a9-217">customKeyValueData</span></span>|<span data-ttu-id="da9a9-218">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="da9a9-219">Пользовательские данные, если для типа подключения установлено настраиваемая VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="da9a9-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="da9a9-220">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в вашем VPN-решении.</span><span class="sxs-lookup"><span data-stu-id="da9a9-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="da9a9-221">Обратитесь к поставщику VPN, чтобы узнать, как добавить эти пары ключ-значение.</span><span class="sxs-lookup"><span data-stu-id="da9a9-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="da9a9-222">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="da9a9-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="da9a9-223">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="da9a9-224">enableSplitTunneling</span></span>|<span data-ttu-id="da9a9-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="da9a9-225">Boolean</span></span>|<span data-ttu-id="da9a9-226">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="da9a9-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="da9a9-227">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="da9a9-228">authenticationMethod</span></span>|[<span data-ttu-id="da9a9-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="da9a9-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="da9a9-230">Метод проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="da9a9-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="da9a9-231">Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="da9a9-232">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="da9a9-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="da9a9-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="da9a9-233">enablePerApp</span></span>|<span data-ttu-id="da9a9-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="da9a9-234">Boolean</span></span>|<span data-ttu-id="da9a9-235">Если установить для этого параметра Per-App vpn, которые впоследствии могут быть связаны с приложениями, которые могут активирует этот коннекциатор VPN на устройстве пользователя с iOS.</span><span class="sxs-lookup"><span data-stu-id="da9a9-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="da9a9-236">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="da9a9-237">safariDomains</span></span>|<span data-ttu-id="da9a9-238">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="da9a9-238">String collection</span></span>|<span data-ttu-id="da9a9-239">Домены Safari, если этот параметр VPN для каждого приложения включен.</span><span class="sxs-lookup"><span data-stu-id="da9a9-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="da9a9-240">Помимо приложений, связанных с этим VPN, указанные здесь домены Safari также смогут запускать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="da9a9-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="da9a9-241">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="da9a9-242">onDemandRules</span></span>|<span data-ttu-id="da9a9-243">[Коллекция vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="da9a9-244">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="da9a9-244">On-Demand Rules.</span></span> <span data-ttu-id="da9a9-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="da9a9-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="da9a9-246">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-247">providerType</span><span class="sxs-lookup"><span data-stu-id="da9a9-247">providerType</span></span>|[<span data-ttu-id="da9a9-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="da9a9-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="da9a9-249">Тип поставщика для VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="da9a9-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="da9a9-250">Наследуется [от appleVpnConfiguration.](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="da9a9-251">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="da9a9-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="da9a9-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="da9a9-252">associatedDomains</span></span>|<span data-ttu-id="da9a9-253">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="da9a9-253">String collection</span></span>|<span data-ttu-id="da9a9-254">Связанные домены, унаследованные [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="da9a9-255">excludedDomains</span></span>|<span data-ttu-id="da9a9-256">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="da9a9-256">String collection</span></span>|<span data-ttu-id="da9a9-257">Домены, которые доступны через общедоступный Интернет, а не через VPN, даже если активирован VPN для каждого приложения. Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="da9a9-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="da9a9-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="da9a9-259">Boolean</span></span>|<span data-ttu-id="da9a9-260">Переключение, чтобы запретить пользователю отключать автоматическую vpn-сеть в приложении "Параметры". Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-261">proxyServer</span><span class="sxs-lookup"><span data-stu-id="da9a9-261">proxyServer</span></span>|[<span data-ttu-id="da9a9-262">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="da9a9-262">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="da9a9-263">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="da9a9-263">Proxy Server.</span></span> <span data-ttu-id="da9a9-264">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-264">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-265">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="da9a9-265">optInToDeviceIdSharing</span></span>|<span data-ttu-id="da9a9-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="da9a9-266">Boolean</span></span>|<span data-ttu-id="da9a9-267">Opt-In к совместному использованию удостоверения устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="da9a9-267">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="da9a9-268">Наследуется [от appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-268">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="da9a9-269">userDomain</span><span class="sxs-lookup"><span data-stu-id="da9a9-269">userDomain</span></span>|<span data-ttu-id="da9a9-270">String</span><span class="sxs-lookup"><span data-stu-id="da9a9-270">String</span></span>|<span data-ttu-id="da9a9-271">Только Zscaler.</span><span class="sxs-lookup"><span data-stu-id="da9a9-271">Zscaler only.</span></span> <span data-ttu-id="da9a9-272">Введите статический домен для предварительного заполнения поля входа в приложение Zscaler.</span><span class="sxs-lookup"><span data-stu-id="da9a9-272">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="da9a9-273">Если оставить его пустым, будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="da9a9-273">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="da9a9-274">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="da9a9-274">strictEnforcement</span></span>|<span data-ttu-id="da9a9-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="da9a9-275">Boolean</span></span>|<span data-ttu-id="da9a9-276">Только Zscaler.</span><span class="sxs-lookup"><span data-stu-id="da9a9-276">Zscaler only.</span></span> <span data-ttu-id="da9a9-277">Блокирует сетевой трафик, пока пользователь не войди в приложение Zscaler.</span><span class="sxs-lookup"><span data-stu-id="da9a9-277">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="da9a9-278">"True" означает, что трафик заблокирован.</span><span class="sxs-lookup"><span data-stu-id="da9a9-278">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="da9a9-279">cloudName</span><span class="sxs-lookup"><span data-stu-id="da9a9-279">cloudName</span></span>|<span data-ttu-id="da9a9-280">String</span><span class="sxs-lookup"><span data-stu-id="da9a9-280">String</span></span>|<span data-ttu-id="da9a9-281">Только Zscaler.</span><span class="sxs-lookup"><span data-stu-id="da9a9-281">Zscaler only.</span></span> <span data-ttu-id="da9a9-282">Облако Zscaler, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="da9a9-282">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="da9a9-283">excludeList</span><span class="sxs-lookup"><span data-stu-id="da9a9-283">excludeList</span></span>|<span data-ttu-id="da9a9-284">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="da9a9-284">String collection</span></span>|<span data-ttu-id="da9a9-285">Только Zscaler.</span><span class="sxs-lookup"><span data-stu-id="da9a9-285">Zscaler only.</span></span> <span data-ttu-id="da9a9-286">Список сетевых адресов, которые не отправляются через облако Zscaler.</span><span class="sxs-lookup"><span data-stu-id="da9a9-286">List of network addresses which are not sent through the Zscaler cloud.</span></span>|
|<span data-ttu-id="da9a9-287">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="da9a9-287">targetedMobileApps</span></span>|<span data-ttu-id="da9a9-288">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="da9a9-288">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="da9a9-289">Целевые мобильные приложения.</span><span class="sxs-lookup"><span data-stu-id="da9a9-289">Targeted mobile apps.</span></span> <span data-ttu-id="da9a9-290">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="da9a9-290">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="da9a9-291">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="da9a9-291">microsoftTunnelSiteId</span></span>|<span data-ttu-id="da9a9-292">String</span><span class="sxs-lookup"><span data-stu-id="da9a9-292">String</span></span>|<span data-ttu-id="da9a9-293">Microsoft Tunnel site ID.</span><span class="sxs-lookup"><span data-stu-id="da9a9-293">Microsoft Tunnel site ID.</span></span>|



## <a name="response"></a><span data-ttu-id="da9a9-294">Отклик</span><span class="sxs-lookup"><span data-stu-id="da9a9-294">Response</span></span>
<span data-ttu-id="da9a9-295">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="da9a9-295">If successful, this method returns a `200 OK` response code and an updated [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da9a9-296">Пример</span><span class="sxs-lookup"><span data-stu-id="da9a9-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="da9a9-297">Запрос</span><span class="sxs-lookup"><span data-stu-id="da9a9-297">Request</span></span>
<span data-ttu-id="da9a9-298">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da9a9-298">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="da9a9-299">Отклик</span><span class="sxs-lookup"><span data-stu-id="da9a9-299">Response</span></span>
<span data-ttu-id="da9a9-p135">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da9a9-p135">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




