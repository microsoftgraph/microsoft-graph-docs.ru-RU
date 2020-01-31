---
title: Обновление Макосвпнконфигуратион
description: Обновление свойств объекта Макосвпнконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b91550af75c8841f0484dd070cbfe54cc348d34c
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41635813"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="e6755-103">Обновление Макосвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e6755-103">Update macOSVpnConfiguration</span></span>

> <span data-ttu-id="e6755-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6755-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6755-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6755-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6755-106">Обновление свойств объекта [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e6755-106">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6755-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e6755-107">Prerequisites</span></span>
<span data-ttu-id="e6755-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6755-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6755-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6755-110">Permission type</span></span>|<span data-ttu-id="e6755-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6755-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6755-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6755-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e6755-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6755-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e6755-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6755-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6755-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6755-115">Not supported.</span></span>|
|<span data-ttu-id="e6755-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6755-116">Application</span></span>|<span data-ttu-id="e6755-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6755-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6755-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6755-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e6755-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e6755-119">Request headers</span></span>
|<span data-ttu-id="e6755-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6755-120">Header</span></span>|<span data-ttu-id="e6755-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e6755-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6755-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6755-122">Authorization</span></span>|<span data-ttu-id="e6755-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6755-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6755-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e6755-124">Accept</span></span>|<span data-ttu-id="e6755-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e6755-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6755-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6755-126">Request body</span></span>
<span data-ttu-id="e6755-127">В тексте запроса добавьте представление объекта [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6755-127">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="e6755-128">В следующей таблице приведены свойства, необходимые при создании [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6755-128">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="e6755-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6755-129">Property</span></span>|<span data-ttu-id="e6755-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e6755-130">Type</span></span>|<span data-ttu-id="e6755-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e6755-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6755-132">id</span><span class="sxs-lookup"><span data-stu-id="e6755-132">id</span></span>|<span data-ttu-id="e6755-133">String</span><span class="sxs-lookup"><span data-stu-id="e6755-133">String</span></span>|<span data-ttu-id="e6755-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e6755-134">Key of the entity.</span></span> <span data-ttu-id="e6755-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6755-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6755-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e6755-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6755-137">DateTimeOffset</span></span>|<span data-ttu-id="e6755-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e6755-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e6755-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6755-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e6755-140">roleScopeTagIds</span></span>|<span data-ttu-id="e6755-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e6755-141">String collection</span></span>|<span data-ttu-id="e6755-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e6755-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e6755-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6755-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e6755-144">supportsScopeTags</span></span>|<span data-ttu-id="e6755-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6755-145">Boolean</span></span>|<span data-ttu-id="e6755-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e6755-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e6755-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e6755-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e6755-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e6755-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e6755-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e6755-149">This property is read-only.</span></span> <span data-ttu-id="e6755-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6755-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e6755-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e6755-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e6755-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e6755-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e6755-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e6755-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6755-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e6755-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e6755-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e6755-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e6755-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e6755-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e6755-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6755-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e6755-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e6755-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e6755-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e6755-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e6755-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e6755-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6755-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6755-163">createdDateTime</span></span>|<span data-ttu-id="e6755-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6755-164">DateTimeOffset</span></span>|<span data-ttu-id="e6755-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e6755-165">DateTime the object was created.</span></span> <span data-ttu-id="e6755-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6755-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-167">description</span><span class="sxs-lookup"><span data-stu-id="e6755-167">description</span></span>|<span data-ttu-id="e6755-168">String</span><span class="sxs-lookup"><span data-stu-id="e6755-168">String</span></span>|<span data-ttu-id="e6755-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e6755-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e6755-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6755-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-171">displayName</span><span class="sxs-lookup"><span data-stu-id="e6755-171">displayName</span></span>|<span data-ttu-id="e6755-172">Строка</span><span class="sxs-lookup"><span data-stu-id="e6755-172">String</span></span>|<span data-ttu-id="e6755-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e6755-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e6755-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6755-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-175">version</span><span class="sxs-lookup"><span data-stu-id="e6755-175">version</span></span>|<span data-ttu-id="e6755-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e6755-176">Int32</span></span>|<span data-ttu-id="e6755-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e6755-177">Version of the device configuration.</span></span> <span data-ttu-id="e6755-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6755-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-179">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="e6755-179">connectionName</span></span>|<span data-ttu-id="e6755-180">Строка</span><span class="sxs-lookup"><span data-stu-id="e6755-180">String</span></span>|<span data-ttu-id="e6755-181">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="e6755-181">Connection name displayed to the user.</span></span> <span data-ttu-id="e6755-182">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6755-182">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="e6755-183">connectionType</span></span>|[<span data-ttu-id="e6755-184">апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="e6755-184">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="e6755-185">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="e6755-185">Connection type.</span></span> <span data-ttu-id="e6755-186">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6755-186">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="e6755-187">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span><span class="sxs-lookup"><span data-stu-id="e6755-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span></span>|
|<span data-ttu-id="e6755-188">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="e6755-188">loginGroupOrDomain</span></span>|<span data-ttu-id="e6755-189">Строка</span><span class="sxs-lookup"><span data-stu-id="e6755-189">String</span></span>|<span data-ttu-id="e6755-190">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="e6755-190">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="e6755-191">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6755-191">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-192">role</span><span class="sxs-lookup"><span data-stu-id="e6755-192">role</span></span>|<span data-ttu-id="e6755-193">Строка</span><span class="sxs-lookup"><span data-stu-id="e6755-193">String</span></span>|<span data-ttu-id="e6755-194">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="e6755-194">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="e6755-195">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6755-195">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-196">область</span><span class="sxs-lookup"><span data-stu-id="e6755-196">realm</span></span>|<span data-ttu-id="e6755-197">Строка</span><span class="sxs-lookup"><span data-stu-id="e6755-197">String</span></span>|<span data-ttu-id="e6755-198">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="e6755-198">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="e6755-199">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6755-199">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-200">сервер</span><span class="sxs-lookup"><span data-stu-id="e6755-200">server</span></span>|[<span data-ttu-id="e6755-201">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="e6755-201">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="e6755-202">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="e6755-202">VPN Server on the network.</span></span> <span data-ttu-id="e6755-203">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="e6755-203">Make sure end users can access this network location.</span></span> <span data-ttu-id="e6755-204">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6755-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-205">идентификатор</span><span class="sxs-lookup"><span data-stu-id="e6755-205">identifier</span></span>|<span data-ttu-id="e6755-206">Строка</span><span class="sxs-lookup"><span data-stu-id="e6755-206">String</span></span>|<span data-ttu-id="e6755-207">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="e6755-207">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="e6755-208">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6755-208">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-209">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="e6755-209">customData</span></span>|<span data-ttu-id="e6755-210">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e6755-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="e6755-211">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="e6755-211">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="e6755-212">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="e6755-212">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="e6755-213">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="e6755-213">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="e6755-214">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="e6755-214">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="e6755-215">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6755-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-216">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="e6755-216">customKeyValueData</span></span>|<span data-ttu-id="e6755-217">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="e6755-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e6755-218">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="e6755-218">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="e6755-219">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="e6755-219">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="e6755-220">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="e6755-220">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="e6755-221">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="e6755-221">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="e6755-222">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6755-222">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-223">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="e6755-223">enableSplitTunneling</span></span>|<span data-ttu-id="e6755-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6755-224">Boolean</span></span>|<span data-ttu-id="e6755-225">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="e6755-225">Send all network traffic through VPN.</span></span> <span data-ttu-id="e6755-226">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6755-226">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-227">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="e6755-227">authenticationMethod</span></span>|[<span data-ttu-id="e6755-228">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="e6755-228">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="e6755-229">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="e6755-229">Authentication method for this VPN connection.</span></span> <span data-ttu-id="e6755-230">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6755-230">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="e6755-231">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="e6755-231">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="e6755-232">енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="e6755-232">enablePerApp</span></span>|<span data-ttu-id="e6755-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6755-233">Boolean</span></span>|<span data-ttu-id="e6755-234">Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="e6755-234">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="e6755-235">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6755-235">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-236">сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="e6755-236">safariDomains</span></span>|<span data-ttu-id="e6755-237">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e6755-237">String collection</span></span>|<span data-ttu-id="e6755-238">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="e6755-238">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="e6755-239">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="e6755-239">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="e6755-240">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6755-240">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-241">ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="e6755-241">onDemandRules</span></span>|<span data-ttu-id="e6755-242">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="e6755-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="e6755-243">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="e6755-243">On-Demand Rules.</span></span> <span data-ttu-id="e6755-244">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e6755-244">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="e6755-245">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6755-245">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-246">проксисервер</span><span class="sxs-lookup"><span data-stu-id="e6755-246">proxyServer</span></span>|[<span data-ttu-id="e6755-247">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="e6755-247">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="e6755-248">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="e6755-248">Proxy Server.</span></span> <span data-ttu-id="e6755-249">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6755-249">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6755-250">оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="e6755-250">optInToDeviceIdSharing</span></span>|<span data-ttu-id="e6755-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6755-251">Boolean</span></span>|<span data-ttu-id="e6755-252">Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="e6755-252">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="e6755-253">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6755-253">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e6755-254">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6755-254">Response</span></span>
<span data-ttu-id="e6755-255">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e6755-255">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6755-256">Пример</span><span class="sxs-lookup"><span data-stu-id="e6755-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6755-257">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6755-257">Request</span></span>
<span data-ttu-id="e6755-258">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6755-258">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2630

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
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true
}
```

### <a name="response"></a><span data-ttu-id="e6755-259">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6755-259">Response</span></span>
<span data-ttu-id="e6755-p129">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6755-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2802

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
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true
}
```





