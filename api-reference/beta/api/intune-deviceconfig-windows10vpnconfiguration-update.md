---
title: Обновление windows10VpnConfiguration
description: Обновление свойств объекта windows10VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 67020189730fef27e4427057f8767590466c22b9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48005455"
---
# <a name="update-windows10vpnconfiguration"></a><span data-ttu-id="c138e-103">Обновление windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c138e-103">Update windows10VpnConfiguration</span></span>

<span data-ttu-id="c138e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c138e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c138e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c138e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c138e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c138e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c138e-107">Обновление свойств объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c138e-107">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c138e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c138e-108">Prerequisites</span></span>
<span data-ttu-id="c138e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c138e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c138e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c138e-111">Permission type</span></span>|<span data-ttu-id="c138e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c138e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c138e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c138e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c138e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c138e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c138e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c138e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c138e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c138e-116">Not supported.</span></span>|
|<span data-ttu-id="c138e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c138e-117">Application</span></span>|<span data-ttu-id="c138e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c138e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c138e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c138e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c138e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c138e-120">Request headers</span></span>
|<span data-ttu-id="c138e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c138e-121">Header</span></span>|<span data-ttu-id="c138e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c138e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c138e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c138e-123">Authorization</span></span>|<span data-ttu-id="c138e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c138e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c138e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c138e-125">Accept</span></span>|<span data-ttu-id="c138e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c138e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c138e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c138e-127">Request body</span></span>
<span data-ttu-id="c138e-128">В тексте запроса добавьте представление объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c138e-128">In the request body, supply a JSON representation for the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

<span data-ttu-id="c138e-129">В следующей таблице приведены свойства, необходимые при создании [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c138e-129">The following table shows the properties that are required when you create the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>

|<span data-ttu-id="c138e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c138e-130">Property</span></span>|<span data-ttu-id="c138e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c138e-131">Type</span></span>|<span data-ttu-id="c138e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c138e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c138e-133">id</span><span class="sxs-lookup"><span data-stu-id="c138e-133">id</span></span>|<span data-ttu-id="c138e-134">String</span><span class="sxs-lookup"><span data-stu-id="c138e-134">String</span></span>|<span data-ttu-id="c138e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c138e-135">Key of the entity.</span></span> <span data-ttu-id="c138e-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c138e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c138e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c138e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c138e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c138e-138">DateTimeOffset</span></span>|<span data-ttu-id="c138e-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c138e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c138e-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c138e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c138e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c138e-141">roleScopeTagIds</span></span>|<span data-ttu-id="c138e-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c138e-142">String collection</span></span>|<span data-ttu-id="c138e-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c138e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c138e-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c138e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c138e-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c138e-145">supportsScopeTags</span></span>|<span data-ttu-id="c138e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c138e-146">Boolean</span></span>|<span data-ttu-id="c138e-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c138e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c138e-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c138e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c138e-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c138e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c138e-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c138e-150">This property is read-only.</span></span> <span data-ttu-id="c138e-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c138e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c138e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c138e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c138e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c138e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c138e-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c138e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c138e-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c138e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c138e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c138e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c138e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c138e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c138e-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c138e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c138e-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c138e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c138e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c138e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c138e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c138e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c138e-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c138e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c138e-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c138e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c138e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c138e-164">createdDateTime</span></span>|<span data-ttu-id="c138e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c138e-165">DateTimeOffset</span></span>|<span data-ttu-id="c138e-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c138e-166">DateTime the object was created.</span></span> <span data-ttu-id="c138e-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c138e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c138e-168">description</span><span class="sxs-lookup"><span data-stu-id="c138e-168">description</span></span>|<span data-ttu-id="c138e-169">String</span><span class="sxs-lookup"><span data-stu-id="c138e-169">String</span></span>|<span data-ttu-id="c138e-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c138e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c138e-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c138e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c138e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c138e-172">displayName</span></span>|<span data-ttu-id="c138e-173">String</span><span class="sxs-lookup"><span data-stu-id="c138e-173">String</span></span>|<span data-ttu-id="c138e-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c138e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c138e-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c138e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c138e-176">version</span><span class="sxs-lookup"><span data-stu-id="c138e-176">version</span></span>|<span data-ttu-id="c138e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c138e-177">Int32</span></span>|<span data-ttu-id="c138e-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c138e-178">Version of the device configuration.</span></span> <span data-ttu-id="c138e-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c138e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c138e-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="c138e-180">connectionName</span></span>|<span data-ttu-id="c138e-181">String</span><span class="sxs-lookup"><span data-stu-id="c138e-181">String</span></span>|<span data-ttu-id="c138e-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="c138e-182">Connection name displayed to the user.</span></span> <span data-ttu-id="c138e-183">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c138e-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c138e-184">серверами</span><span class="sxs-lookup"><span data-stu-id="c138e-184">servers</span></span>|<span data-ttu-id="c138e-185">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="c138e-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="c138e-186">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="c138e-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="c138e-187">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="c138e-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="c138e-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c138e-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c138e-189">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c138e-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c138e-190">customXml</span><span class="sxs-lookup"><span data-stu-id="c138e-190">customXml</span></span>|<span data-ttu-id="c138e-191">Binary</span><span class="sxs-lookup"><span data-stu-id="c138e-191">Binary</span></span>|<span data-ttu-id="c138e-192">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="c138e-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="c138e-193">(Массив байтов в кодировке UTF8) Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c138e-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c138e-194">профилетаржет</span><span class="sxs-lookup"><span data-stu-id="c138e-194">profileTarget</span></span>|[<span data-ttu-id="c138e-195">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="c138e-195">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="c138e-196">Тип целевого объекта профиля.</span><span class="sxs-lookup"><span data-stu-id="c138e-196">Profile target type.</span></span> <span data-ttu-id="c138e-197">Возможные значения: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="c138e-197">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="c138e-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="c138e-198">connectionType</span></span>|[<span data-ttu-id="c138e-199">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="c138e-199">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="c138e-200">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="c138e-200">Connection type.</span></span> <span data-ttu-id="c138e-201">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="c138e-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="c138e-202">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="c138e-202">enableSplitTunneling</span></span>|<span data-ttu-id="c138e-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="c138e-203">Boolean</span></span>|<span data-ttu-id="c138e-204">Включение Расщепленного туннелирования.</span><span class="sxs-lookup"><span data-stu-id="c138e-204">Enable split tunneling.</span></span>|
|<span data-ttu-id="c138e-205">енаблеалвайсон</span><span class="sxs-lookup"><span data-stu-id="c138e-205">enableAlwaysOn</span></span>|<span data-ttu-id="c138e-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="c138e-206">Boolean</span></span>|<span data-ttu-id="c138e-207">Включение режима "всегда включено".</span><span class="sxs-lookup"><span data-stu-id="c138e-207">Enable Always On mode.</span></span>|
|<span data-ttu-id="c138e-208">енабледевицетуннел</span><span class="sxs-lookup"><span data-stu-id="c138e-208">enableDeviceTunnel</span></span>|<span data-ttu-id="c138e-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="c138e-209">Boolean</span></span>|<span data-ttu-id="c138e-210">Включите туннель устройства.</span><span class="sxs-lookup"><span data-stu-id="c138e-210">Enable device tunnel.</span></span>|
|<span data-ttu-id="c138e-211">енабледнсрегистратион</span><span class="sxs-lookup"><span data-stu-id="c138e-211">enableDnsRegistration</span></span>|<span data-ttu-id="c138e-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="c138e-212">Boolean</span></span>|<span data-ttu-id="c138e-213">Включить регистрацию IP-адресов с использованием внутренней DNS.</span><span class="sxs-lookup"><span data-stu-id="c138e-213">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="c138e-214">днссуффиксес</span><span class="sxs-lookup"><span data-stu-id="c138e-214">dnsSuffixes</span></span>|<span data-ttu-id="c138e-215">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c138e-215">String collection</span></span>|<span data-ttu-id="c138e-216">Укажите DNS-суффиксы, которые необходимо добавить в список поиска DNS, чтобы правильно маршрутизировать короткие имена.</span><span class="sxs-lookup"><span data-stu-id="c138e-216">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="c138e-217">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="c138e-217">authenticationMethod</span></span>|[<span data-ttu-id="c138e-218">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c138e-218">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="c138e-219">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="c138e-219">Authentication method.</span></span> <span data-ttu-id="c138e-220">Возможные значения: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="c138e-220">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span></span>|
|<span data-ttu-id="c138e-221">ремемберусеркредентиалс</span><span class="sxs-lookup"><span data-stu-id="c138e-221">rememberUserCredentials</span></span>|<span data-ttu-id="c138e-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="c138e-222">Boolean</span></span>|<span data-ttu-id="c138e-223">Запомнить учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="c138e-223">Remember user credentials.</span></span>|
|<span data-ttu-id="c138e-224">енаблекондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="c138e-224">enableConditionalAccess</span></span>|<span data-ttu-id="c138e-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="c138e-225">Boolean</span></span>|<span data-ttu-id="c138e-226">Включение условного доступа.</span><span class="sxs-lookup"><span data-stu-id="c138e-226">Enable conditional access.</span></span>|
|<span data-ttu-id="c138e-227">енаблесинглесигнонвисалтернатецертификате</span><span class="sxs-lookup"><span data-stu-id="c138e-227">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="c138e-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="c138e-228">Boolean</span></span>|<span data-ttu-id="c138e-229">Включите единый вход (SSO) с альтернативным сертификатом.</span><span class="sxs-lookup"><span data-stu-id="c138e-229">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="c138e-230">синглесигнонеку</span><span class="sxs-lookup"><span data-stu-id="c138e-230">singleSignOnEku</span></span>|[<span data-ttu-id="c138e-231">екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="c138e-231">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="c138e-232">Расширенное использование ключа (EKU) единого входа.</span><span class="sxs-lookup"><span data-stu-id="c138e-232">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="c138e-233">синглесигнониссуерхаш</span><span class="sxs-lookup"><span data-stu-id="c138e-233">singleSignOnIssuerHash</span></span>|<span data-ttu-id="c138e-234">String</span><span class="sxs-lookup"><span data-stu-id="c138e-234">String</span></span>|<span data-ttu-id="c138e-235">Хэш поставщика единого входа.</span><span class="sxs-lookup"><span data-stu-id="c138e-235">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="c138e-236">еапксмл</span><span class="sxs-lookup"><span data-stu-id="c138e-236">eapXml</span></span>|<span data-ttu-id="c138e-237">Binary</span><span class="sxs-lookup"><span data-stu-id="c138e-237">Binary</span></span>|<span data-ttu-id="c138e-238">XML-файл протокола расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="c138e-238">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="c138e-239">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="c138e-239">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="c138e-240">проксисервер</span><span class="sxs-lookup"><span data-stu-id="c138e-240">proxyServer</span></span>|[<span data-ttu-id="c138e-241">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="c138e-241">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="c138e-242">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="c138e-242">Proxy Server.</span></span>|
|<span data-ttu-id="c138e-243">ассоЦиатедаппс</span><span class="sxs-lookup"><span data-stu-id="c138e-243">associatedApps</span></span>|<span data-ttu-id="c138e-244">Коллекция [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="c138e-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="c138e-245">Связанные приложения.</span><span class="sxs-lookup"><span data-stu-id="c138e-245">Associated Apps.</span></span> <span data-ttu-id="c138e-246">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="c138e-246">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c138e-247">онляссоЦиатедаппсканусеконнектион</span><span class="sxs-lookup"><span data-stu-id="c138e-247">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="c138e-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="c138e-248">Boolean</span></span>|<span data-ttu-id="c138e-249">Подключение можно использовать только для связанных приложений (VPN для каждого приложения).</span><span class="sxs-lookup"><span data-stu-id="c138e-249">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="c138e-250">виндовсинформатионпротектиондомаин</span><span class="sxs-lookup"><span data-stu-id="c138e-250">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="c138e-251">String</span><span class="sxs-lookup"><span data-stu-id="c138e-251">String</span></span>|<span data-ttu-id="c138e-252">Домен Windows Information Protection (WIP) для связи с этим подключением.</span><span class="sxs-lookup"><span data-stu-id="c138e-252">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="c138e-253">траффикрулес</span><span class="sxs-lookup"><span data-stu-id="c138e-253">trafficRules</span></span>|<span data-ttu-id="c138e-254">Коллекция [впнтраффикруле](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="c138e-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="c138e-255">Правила трафика.</span><span class="sxs-lookup"><span data-stu-id="c138e-255">Traffic rules.</span></span> <span data-ttu-id="c138e-256">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="c138e-256">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="c138e-257">сылает</span><span class="sxs-lookup"><span data-stu-id="c138e-257">routes</span></span>|<span data-ttu-id="c138e-258">Коллекция [впнрауте](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="c138e-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="c138e-259">Маршруты (необязательно для сторонних поставщиков).</span><span class="sxs-lookup"><span data-stu-id="c138e-259">Routes (optional for third-party providers).</span></span> <span data-ttu-id="c138e-260">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="c138e-260">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="c138e-261">днсрулес</span><span class="sxs-lookup"><span data-stu-id="c138e-261">dnsRules</span></span>|<span data-ttu-id="c138e-262">Коллекция [впнднсруле](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="c138e-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="c138e-263">Правила DNS.</span><span class="sxs-lookup"><span data-stu-id="c138e-263">DNS rules.</span></span> <span data-ttu-id="c138e-264">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="c138e-264">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="c138e-265">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="c138e-265">trustedNetworkDomains</span></span>|<span data-ttu-id="c138e-266">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c138e-266">String collection</span></span>|<span data-ttu-id="c138e-267">Доверенные сетевые домены</span><span class="sxs-lookup"><span data-stu-id="c138e-267">Trusted Network Domains</span></span>|
|<span data-ttu-id="c138e-268">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="c138e-268">cryptographySuite</span></span>|[<span data-ttu-id="c138e-269">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="c138e-269">cryptographySuite</span></span>](../resources/intune-deviceconfig-cryptographysuite.md)|<span data-ttu-id="c138e-270">Параметры безопасности комплекта шифрования для VPN-подключения по протоколу IKEv2 в Windows10 и более поздних версий</span><span class="sxs-lookup"><span data-stu-id="c138e-270">Cryptography Suite security settings for IKEv2 VPN in Windows10 and above</span></span> |



## <a name="response"></a><span data-ttu-id="c138e-271">Отклик</span><span class="sxs-lookup"><span data-stu-id="c138e-271">Response</span></span>
<span data-ttu-id="c138e-272">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c138e-272">If successful, this method returns a `200 OK` response code and an updated [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c138e-273">Пример</span><span class="sxs-lookup"><span data-stu-id="c138e-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="c138e-274">Запрос</span><span class="sxs-lookup"><span data-stu-id="c138e-274">Request</span></span>
<span data-ttu-id="c138e-275">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c138e-275">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4463

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
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
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ],
  "cryptographySuite": {
    "@odata.type": "microsoft.graph.cryptographySuite",
    "encryptionMethod": "des",
    "integrityCheckMethod": "sha1_96",
    "dhGroup": "group2",
    "cipherTransformConstants": "des",
    "authenticationTransformConstants": "sha1_96",
    "pfsGroup": "pfs2"
  }
}
```

### <a name="response"></a><span data-ttu-id="c138e-276">Отклик</span><span class="sxs-lookup"><span data-stu-id="c138e-276">Response</span></span>
<span data-ttu-id="c138e-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c138e-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4635

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
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
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ],
  "cryptographySuite": {
    "@odata.type": "microsoft.graph.cryptographySuite",
    "encryptionMethod": "des",
    "integrityCheckMethod": "sha1_96",
    "dhGroup": "group2",
    "cipherTransformConstants": "des",
    "authenticationTransformConstants": "sha1_96",
    "pfsGroup": "pfs2"
  }
}
```






