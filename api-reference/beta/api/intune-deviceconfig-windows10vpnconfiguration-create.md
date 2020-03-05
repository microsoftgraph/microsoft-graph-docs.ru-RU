---
title: Создание windows10VpnConfiguration
description: Создание нового объекта windows10VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bff78f58039cbe4be3c471d81a783ba6f8fcde01
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42477702"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="fc024-103">Создание windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="fc024-103">Create windows10VpnConfiguration</span></span>

<span data-ttu-id="fc024-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fc024-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc024-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc024-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc024-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc024-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc024-107">Создание нового объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fc024-107">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc024-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fc024-108">Prerequisites</span></span>
<span data-ttu-id="fc024-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc024-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc024-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc024-111">Permission type</span></span>|<span data-ttu-id="fc024-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc024-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc024-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc024-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc024-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc024-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fc024-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc024-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc024-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc024-116">Not supported.</span></span>|
|<span data-ttu-id="fc024-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-117">Application</span></span>|<span data-ttu-id="fc024-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc024-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc024-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc024-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fc024-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fc024-120">Request headers</span></span>
|<span data-ttu-id="fc024-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc024-121">Header</span></span>|<span data-ttu-id="fc024-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fc024-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc024-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc024-123">Authorization</span></span>|<span data-ttu-id="fc024-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc024-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc024-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fc024-125">Accept</span></span>|<span data-ttu-id="fc024-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc024-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc024-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc024-127">Request body</span></span>
<span data-ttu-id="fc024-128">В тексте запроса добавьте представление объекта windows10VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc024-128">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="fc024-129">В следующей таблице приведены свойства, необходимые при создании windows10VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fc024-129">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="fc024-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc024-130">Property</span></span>|<span data-ttu-id="fc024-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fc024-131">Type</span></span>|<span data-ttu-id="fc024-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fc024-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc024-133">id</span><span class="sxs-lookup"><span data-stu-id="fc024-133">id</span></span>|<span data-ttu-id="fc024-134">String</span><span class="sxs-lookup"><span data-stu-id="fc024-134">String</span></span>|<span data-ttu-id="fc024-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fc024-135">Key of the entity.</span></span> <span data-ttu-id="fc024-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc024-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc024-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc024-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fc024-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc024-138">DateTimeOffset</span></span>|<span data-ttu-id="fc024-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fc024-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fc024-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc024-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc024-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fc024-141">roleScopeTagIds</span></span>|<span data-ttu-id="fc024-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fc024-142">String collection</span></span>|<span data-ttu-id="fc024-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fc024-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fc024-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc024-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc024-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="fc024-145">supportsScopeTags</span></span>|<span data-ttu-id="fc024-146">Логический</span><span class="sxs-lookup"><span data-stu-id="fc024-146">Boolean</span></span>|<span data-ttu-id="fc024-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="fc024-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fc024-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="fc024-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fc024-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fc024-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fc024-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc024-150">This property is read-only.</span></span> <span data-ttu-id="fc024-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc024-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc024-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fc024-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fc024-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fc024-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fc024-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fc024-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fc024-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc024-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc024-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fc024-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fc024-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fc024-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fc024-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fc024-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fc024-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc024-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc024-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fc024-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fc024-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fc024-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fc024-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fc024-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fc024-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc024-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc024-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fc024-164">createdDateTime</span></span>|<span data-ttu-id="fc024-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc024-165">DateTimeOffset</span></span>|<span data-ttu-id="fc024-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fc024-166">DateTime the object was created.</span></span> <span data-ttu-id="fc024-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc024-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc024-168">description</span><span class="sxs-lookup"><span data-stu-id="fc024-168">description</span></span>|<span data-ttu-id="fc024-169">String</span><span class="sxs-lookup"><span data-stu-id="fc024-169">String</span></span>|<span data-ttu-id="fc024-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fc024-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fc024-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc024-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc024-172">displayName</span><span class="sxs-lookup"><span data-stu-id="fc024-172">displayName</span></span>|<span data-ttu-id="fc024-173">Строка</span><span class="sxs-lookup"><span data-stu-id="fc024-173">String</span></span>|<span data-ttu-id="fc024-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fc024-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fc024-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc024-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc024-176">version</span><span class="sxs-lookup"><span data-stu-id="fc024-176">version</span></span>|<span data-ttu-id="fc024-177">Int32</span><span class="sxs-lookup"><span data-stu-id="fc024-177">Int32</span></span>|<span data-ttu-id="fc024-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fc024-178">Version of the device configuration.</span></span> <span data-ttu-id="fc024-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc024-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc024-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="fc024-180">connectionName</span></span>|<span data-ttu-id="fc024-181">String</span><span class="sxs-lookup"><span data-stu-id="fc024-181">String</span></span>|<span data-ttu-id="fc024-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="fc024-182">Connection name displayed to the user.</span></span> <span data-ttu-id="fc024-183">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc024-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="fc024-184">серверами</span><span class="sxs-lookup"><span data-stu-id="fc024-184">servers</span></span>|<span data-ttu-id="fc024-185">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="fc024-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="fc024-186">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="fc024-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="fc024-187">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="fc024-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="fc024-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="fc024-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="fc024-189">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc024-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="fc024-190">customXml</span><span class="sxs-lookup"><span data-stu-id="fc024-190">customXml</span></span>|<span data-ttu-id="fc024-191">Binary</span><span class="sxs-lookup"><span data-stu-id="fc024-191">Binary</span></span>|<span data-ttu-id="fc024-192">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="fc024-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="fc024-193">(Массив байтов в кодировке UTF8) Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc024-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="fc024-194">профилетаржет</span><span class="sxs-lookup"><span data-stu-id="fc024-194">profileTarget</span></span>|[<span data-ttu-id="fc024-195">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="fc024-195">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="fc024-196">Тип целевого объекта профиля.</span><span class="sxs-lookup"><span data-stu-id="fc024-196">Profile target type.</span></span> <span data-ttu-id="fc024-197">Возможные значения: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="fc024-197">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="fc024-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="fc024-198">connectionType</span></span>|[<span data-ttu-id="fc024-199">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="fc024-199">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="fc024-200">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="fc024-200">Connection type.</span></span> <span data-ttu-id="fc024-201">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="fc024-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="fc024-202">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="fc024-202">enableSplitTunneling</span></span>|<span data-ttu-id="fc024-203">Логический</span><span class="sxs-lookup"><span data-stu-id="fc024-203">Boolean</span></span>|<span data-ttu-id="fc024-204">Включение Расщепленного туннелирования.</span><span class="sxs-lookup"><span data-stu-id="fc024-204">Enable split tunneling.</span></span>|
|<span data-ttu-id="fc024-205">енаблеалвайсон</span><span class="sxs-lookup"><span data-stu-id="fc024-205">enableAlwaysOn</span></span>|<span data-ttu-id="fc024-206">Логический</span><span class="sxs-lookup"><span data-stu-id="fc024-206">Boolean</span></span>|<span data-ttu-id="fc024-207">Включение режима "всегда включено".</span><span class="sxs-lookup"><span data-stu-id="fc024-207">Enable Always On mode.</span></span>|
|<span data-ttu-id="fc024-208">енабледевицетуннел</span><span class="sxs-lookup"><span data-stu-id="fc024-208">enableDeviceTunnel</span></span>|<span data-ttu-id="fc024-209">Логический</span><span class="sxs-lookup"><span data-stu-id="fc024-209">Boolean</span></span>|<span data-ttu-id="fc024-210">Включите туннель устройства.</span><span class="sxs-lookup"><span data-stu-id="fc024-210">Enable device tunnel.</span></span>|
|<span data-ttu-id="fc024-211">енабледнсрегистратион</span><span class="sxs-lookup"><span data-stu-id="fc024-211">enableDnsRegistration</span></span>|<span data-ttu-id="fc024-212">Логический</span><span class="sxs-lookup"><span data-stu-id="fc024-212">Boolean</span></span>|<span data-ttu-id="fc024-213">Включить регистрацию IP-адресов с использованием внутренней DNS.</span><span class="sxs-lookup"><span data-stu-id="fc024-213">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="fc024-214">днссуффиксес</span><span class="sxs-lookup"><span data-stu-id="fc024-214">dnsSuffixes</span></span>|<span data-ttu-id="fc024-215">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fc024-215">String collection</span></span>|<span data-ttu-id="fc024-216">Укажите DNS-суффиксы, которые необходимо добавить в список поиска DNS, чтобы правильно маршрутизировать короткие имена.</span><span class="sxs-lookup"><span data-stu-id="fc024-216">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="fc024-217">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="fc024-217">authenticationMethod</span></span>|[<span data-ttu-id="fc024-218">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fc024-218">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="fc024-219">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="fc024-219">Authentication method.</span></span> <span data-ttu-id="fc024-220">Возможные значения: `certificate`, `usernameAndPassword`, `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="fc024-220">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="fc024-221">ремемберусеркредентиалс</span><span class="sxs-lookup"><span data-stu-id="fc024-221">rememberUserCredentials</span></span>|<span data-ttu-id="fc024-222">Логический</span><span class="sxs-lookup"><span data-stu-id="fc024-222">Boolean</span></span>|<span data-ttu-id="fc024-223">Запомнить учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="fc024-223">Remember user credentials.</span></span>|
|<span data-ttu-id="fc024-224">енаблекондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="fc024-224">enableConditionalAccess</span></span>|<span data-ttu-id="fc024-225">Логический</span><span class="sxs-lookup"><span data-stu-id="fc024-225">Boolean</span></span>|<span data-ttu-id="fc024-226">Включение условного доступа.</span><span class="sxs-lookup"><span data-stu-id="fc024-226">Enable conditional access.</span></span>|
|<span data-ttu-id="fc024-227">енаблесинглесигнонвисалтернатецертификате</span><span class="sxs-lookup"><span data-stu-id="fc024-227">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="fc024-228">Логический</span><span class="sxs-lookup"><span data-stu-id="fc024-228">Boolean</span></span>|<span data-ttu-id="fc024-229">Включите единый вход (SSO) с альтернативным сертификатом.</span><span class="sxs-lookup"><span data-stu-id="fc024-229">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="fc024-230">синглесигнонеку</span><span class="sxs-lookup"><span data-stu-id="fc024-230">singleSignOnEku</span></span>|[<span data-ttu-id="fc024-231">екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="fc024-231">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="fc024-232">Расширенное использование ключа (EKU) единого входа.</span><span class="sxs-lookup"><span data-stu-id="fc024-232">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="fc024-233">синглесигнониссуерхаш</span><span class="sxs-lookup"><span data-stu-id="fc024-233">singleSignOnIssuerHash</span></span>|<span data-ttu-id="fc024-234">String</span><span class="sxs-lookup"><span data-stu-id="fc024-234">String</span></span>|<span data-ttu-id="fc024-235">Хэш поставщика единого входа.</span><span class="sxs-lookup"><span data-stu-id="fc024-235">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="fc024-236">еапксмл</span><span class="sxs-lookup"><span data-stu-id="fc024-236">eapXml</span></span>|<span data-ttu-id="fc024-237">Binary</span><span class="sxs-lookup"><span data-stu-id="fc024-237">Binary</span></span>|<span data-ttu-id="fc024-238">XML-файл протокола расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="fc024-238">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="fc024-239">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="fc024-239">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="fc024-240">проксисервер</span><span class="sxs-lookup"><span data-stu-id="fc024-240">proxyServer</span></span>|[<span data-ttu-id="fc024-241">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="fc024-241">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="fc024-242">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="fc024-242">Proxy Server.</span></span>|
|<span data-ttu-id="fc024-243">ассоЦиатедаппс</span><span class="sxs-lookup"><span data-stu-id="fc024-243">associatedApps</span></span>|<span data-ttu-id="fc024-244">Коллекция [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="fc024-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="fc024-245">Связанные приложения.</span><span class="sxs-lookup"><span data-stu-id="fc024-245">Associated Apps.</span></span> <span data-ttu-id="fc024-246">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="fc024-246">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="fc024-247">онляссоЦиатедаппсканусеконнектион</span><span class="sxs-lookup"><span data-stu-id="fc024-247">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="fc024-248">Логический</span><span class="sxs-lookup"><span data-stu-id="fc024-248">Boolean</span></span>|<span data-ttu-id="fc024-249">Подключение можно использовать только для связанных приложений (VPN для каждого приложения).</span><span class="sxs-lookup"><span data-stu-id="fc024-249">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="fc024-250">виндовсинформатионпротектиондомаин</span><span class="sxs-lookup"><span data-stu-id="fc024-250">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="fc024-251">String</span><span class="sxs-lookup"><span data-stu-id="fc024-251">String</span></span>|<span data-ttu-id="fc024-252">Домен Windows Information Protection (WIP) для связи с этим подключением.</span><span class="sxs-lookup"><span data-stu-id="fc024-252">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="fc024-253">траффикрулес</span><span class="sxs-lookup"><span data-stu-id="fc024-253">trafficRules</span></span>|<span data-ttu-id="fc024-254">Коллекция [впнтраффикруле](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="fc024-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="fc024-255">Правила трафика.</span><span class="sxs-lookup"><span data-stu-id="fc024-255">Traffic rules.</span></span> <span data-ttu-id="fc024-256">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="fc024-256">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="fc024-257">сылает</span><span class="sxs-lookup"><span data-stu-id="fc024-257">routes</span></span>|<span data-ttu-id="fc024-258">Коллекция [впнрауте](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="fc024-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="fc024-259">Маршруты (необязательно для сторонних поставщиков).</span><span class="sxs-lookup"><span data-stu-id="fc024-259">Routes (optional for third-party providers).</span></span> <span data-ttu-id="fc024-260">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="fc024-260">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="fc024-261">днсрулес</span><span class="sxs-lookup"><span data-stu-id="fc024-261">dnsRules</span></span>|<span data-ttu-id="fc024-262">Коллекция [впнднсруле](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="fc024-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="fc024-263">Правила DNS.</span><span class="sxs-lookup"><span data-stu-id="fc024-263">DNS rules.</span></span> <span data-ttu-id="fc024-264">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="fc024-264">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="fc024-265">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="fc024-265">trustedNetworkDomains</span></span>|<span data-ttu-id="fc024-266">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fc024-266">String collection</span></span>|<span data-ttu-id="fc024-267">Доверенные сетевые домены</span><span class="sxs-lookup"><span data-stu-id="fc024-267">Trusted Network Domains</span></span>|



## <a name="response"></a><span data-ttu-id="fc024-268">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc024-268">Response</span></span>
<span data-ttu-id="fc024-269">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc024-269">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc024-270">Пример</span><span class="sxs-lookup"><span data-stu-id="fc024-270">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc024-271">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc024-271">Request</span></span>
<span data-ttu-id="fc024-272">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc024-272">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4160

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
  ]
}
```

### <a name="response"></a><span data-ttu-id="fc024-273">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc024-273">Response</span></span>
<span data-ttu-id="fc024-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc024-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4332

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
  ]
}
```





