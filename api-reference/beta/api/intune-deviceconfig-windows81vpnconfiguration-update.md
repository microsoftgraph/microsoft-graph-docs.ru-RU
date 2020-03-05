---
title: Обновление windows81VpnConfiguration
description: Обновление свойств объекта windows81VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 94ec74cb949effd5af502ad2a1cddbebe9c993e2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42476652"
---
# <a name="update-windows81vpnconfiguration"></a><span data-ttu-id="b9662-103">Обновление windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b9662-103">Update windows81VpnConfiguration</span></span>

<span data-ttu-id="b9662-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b9662-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9662-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9662-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9662-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9662-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9662-107">Обновление свойств объекта [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b9662-107">Update the properties of a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9662-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b9662-108">Prerequisites</span></span>
<span data-ttu-id="b9662-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9662-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9662-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9662-111">Permission type</span></span>|<span data-ttu-id="b9662-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9662-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9662-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9662-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9662-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9662-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9662-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9662-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9662-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9662-116">Not supported.</span></span>|
|<span data-ttu-id="b9662-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9662-117">Application</span></span>|<span data-ttu-id="b9662-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9662-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9662-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9662-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b9662-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b9662-120">Request headers</span></span>
|<span data-ttu-id="b9662-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9662-121">Header</span></span>|<span data-ttu-id="b9662-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b9662-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9662-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9662-123">Authorization</span></span>|<span data-ttu-id="b9662-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9662-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9662-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b9662-125">Accept</span></span>|<span data-ttu-id="b9662-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9662-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9662-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9662-127">Request body</span></span>
<span data-ttu-id="b9662-128">В тексте запроса добавьте представление объекта [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9662-128">In the request body, supply a JSON representation for the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="b9662-129">В следующей таблице приведены свойства, необходимые при создании [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9662-129">The following table shows the properties that are required when you create the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span>

|<span data-ttu-id="b9662-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9662-130">Property</span></span>|<span data-ttu-id="b9662-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b9662-131">Type</span></span>|<span data-ttu-id="b9662-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b9662-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9662-133">id</span><span class="sxs-lookup"><span data-stu-id="b9662-133">id</span></span>|<span data-ttu-id="b9662-134">String</span><span class="sxs-lookup"><span data-stu-id="b9662-134">String</span></span>|<span data-ttu-id="b9662-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b9662-135">Key of the entity.</span></span> <span data-ttu-id="b9662-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9662-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9662-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9662-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b9662-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9662-138">DateTimeOffset</span></span>|<span data-ttu-id="b9662-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b9662-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b9662-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9662-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9662-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b9662-141">roleScopeTagIds</span></span>|<span data-ttu-id="b9662-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b9662-142">String collection</span></span>|<span data-ttu-id="b9662-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b9662-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b9662-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9662-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9662-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="b9662-145">supportsScopeTags</span></span>|<span data-ttu-id="b9662-146">Логический</span><span class="sxs-lookup"><span data-stu-id="b9662-146">Boolean</span></span>|<span data-ttu-id="b9662-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b9662-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b9662-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="b9662-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b9662-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b9662-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b9662-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9662-150">This property is read-only.</span></span> <span data-ttu-id="b9662-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9662-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9662-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b9662-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b9662-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b9662-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b9662-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b9662-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b9662-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9662-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9662-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b9662-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b9662-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b9662-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b9662-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b9662-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b9662-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9662-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9662-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b9662-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b9662-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b9662-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b9662-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b9662-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b9662-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9662-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9662-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9662-164">createdDateTime</span></span>|<span data-ttu-id="b9662-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9662-165">DateTimeOffset</span></span>|<span data-ttu-id="b9662-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b9662-166">DateTime the object was created.</span></span> <span data-ttu-id="b9662-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9662-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9662-168">description</span><span class="sxs-lookup"><span data-stu-id="b9662-168">description</span></span>|<span data-ttu-id="b9662-169">String</span><span class="sxs-lookup"><span data-stu-id="b9662-169">String</span></span>|<span data-ttu-id="b9662-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b9662-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b9662-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9662-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9662-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b9662-172">displayName</span></span>|<span data-ttu-id="b9662-173">Строка</span><span class="sxs-lookup"><span data-stu-id="b9662-173">String</span></span>|<span data-ttu-id="b9662-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b9662-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b9662-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9662-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9662-176">version</span><span class="sxs-lookup"><span data-stu-id="b9662-176">version</span></span>|<span data-ttu-id="b9662-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b9662-177">Int32</span></span>|<span data-ttu-id="b9662-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b9662-178">Version of the device configuration.</span></span> <span data-ttu-id="b9662-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9662-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b9662-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="b9662-180">connectionName</span></span>|<span data-ttu-id="b9662-181">String</span><span class="sxs-lookup"><span data-stu-id="b9662-181">String</span></span>|<span data-ttu-id="b9662-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9662-182">Connection name displayed to the user.</span></span> <span data-ttu-id="b9662-183">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9662-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b9662-184">серверами</span><span class="sxs-lookup"><span data-stu-id="b9662-184">servers</span></span>|<span data-ttu-id="b9662-185">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="b9662-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="b9662-186">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="b9662-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="b9662-187">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="b9662-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="b9662-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="b9662-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b9662-189">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9662-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b9662-190">customXml</span><span class="sxs-lookup"><span data-stu-id="b9662-190">customXml</span></span>|<span data-ttu-id="b9662-191">Binary</span><span class="sxs-lookup"><span data-stu-id="b9662-191">Binary</span></span>|<span data-ttu-id="b9662-192">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="b9662-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="b9662-193">(Массив байтов в кодировке UTF8) Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b9662-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b9662-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="b9662-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="b9662-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9662-195">Boolean</span></span>|<span data-ttu-id="b9662-196">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="b9662-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="b9662-197">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9662-197">This property is read-only.</span></span>|
|<span data-ttu-id="b9662-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="b9662-198">connectionType</span></span>|[<span data-ttu-id="b9662-199">виндовсвпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="b9662-199">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="b9662-200">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="b9662-200">Connection type.</span></span> <span data-ttu-id="b9662-201">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="b9662-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="b9662-202">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="b9662-202">loginGroupOrDomain</span></span>|<span data-ttu-id="b9662-203">String</span><span class="sxs-lookup"><span data-stu-id="b9662-203">String</span></span>|<span data-ttu-id="b9662-204">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="b9662-204">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="b9662-205">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="b9662-205">enableSplitTunneling</span></span>|<span data-ttu-id="b9662-206">Логический</span><span class="sxs-lookup"><span data-stu-id="b9662-206">Boolean</span></span>|<span data-ttu-id="b9662-207">Включение Расщепленного туннелирования для VPN.</span><span class="sxs-lookup"><span data-stu-id="b9662-207">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="b9662-208">проксисервер</span><span class="sxs-lookup"><span data-stu-id="b9662-208">proxyServer</span></span>|[<span data-ttu-id="b9662-209">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="b9662-209">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="b9662-210">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="b9662-210">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="b9662-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9662-211">Response</span></span>
<span data-ttu-id="b9662-212">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b9662-212">If successful, this method returns a `200 OK` response code and an updated [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9662-213">Пример</span><span class="sxs-lookup"><span data-stu-id="b9662-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9662-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9662-214">Request</span></span>
<span data-ttu-id="b9662-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9662-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1788

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
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
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  }
}
```

### <a name="response"></a><span data-ttu-id="b9662-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9662-216">Response</span></span>
<span data-ttu-id="b9662-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9662-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1960

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
  "id": "6aa07da3-7da3-6aa0-a37d-a06aa37da06a",
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
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  }
}
```





