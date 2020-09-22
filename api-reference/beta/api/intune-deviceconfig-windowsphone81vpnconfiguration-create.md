---
title: Создание windowsPhone81VpnConfiguration
description: Создание нового объекта windowsPhone81VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b479189f6b27bb1c8cac07ab36b78d757d23d74d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48043537"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="d6915-103">Создание windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d6915-103">Create windowsPhone81VpnConfiguration</span></span>

<span data-ttu-id="d6915-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6915-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6915-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6915-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6915-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6915-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6915-107">Создание нового объекта [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d6915-107">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6915-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d6915-108">Prerequisites</span></span>
<span data-ttu-id="d6915-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6915-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6915-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6915-111">Permission type</span></span>|<span data-ttu-id="d6915-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6915-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6915-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6915-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6915-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6915-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6915-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6915-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6915-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6915-116">Not supported.</span></span>|
|<span data-ttu-id="d6915-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6915-117">Application</span></span>|<span data-ttu-id="d6915-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6915-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6915-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6915-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d6915-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d6915-120">Request headers</span></span>
|<span data-ttu-id="d6915-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6915-121">Header</span></span>|<span data-ttu-id="d6915-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d6915-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6915-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6915-123">Authorization</span></span>|<span data-ttu-id="d6915-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6915-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6915-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d6915-125">Accept</span></span>|<span data-ttu-id="d6915-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6915-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6915-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d6915-127">Request body</span></span>
<span data-ttu-id="d6915-128">В тексте запроса добавьте представление объекта windowsPhone81VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6915-128">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="d6915-129">В следующей таблице приведены свойства, необходимые при создании windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d6915-129">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="d6915-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6915-130">Property</span></span>|<span data-ttu-id="d6915-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d6915-131">Type</span></span>|<span data-ttu-id="d6915-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d6915-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6915-133">id</span><span class="sxs-lookup"><span data-stu-id="d6915-133">id</span></span>|<span data-ttu-id="d6915-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d6915-134">String</span></span>|<span data-ttu-id="d6915-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d6915-135">Key of the entity.</span></span> <span data-ttu-id="d6915-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6915-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6915-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6915-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d6915-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6915-138">DateTimeOffset</span></span>|<span data-ttu-id="d6915-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d6915-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d6915-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6915-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6915-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d6915-141">roleScopeTagIds</span></span>|<span data-ttu-id="d6915-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d6915-142">String collection</span></span>|<span data-ttu-id="d6915-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d6915-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d6915-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6915-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6915-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d6915-145">supportsScopeTags</span></span>|<span data-ttu-id="d6915-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6915-146">Boolean</span></span>|<span data-ttu-id="d6915-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d6915-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d6915-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d6915-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d6915-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d6915-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d6915-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d6915-150">This property is read-only.</span></span> <span data-ttu-id="d6915-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6915-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6915-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d6915-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d6915-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d6915-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d6915-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d6915-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d6915-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6915-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6915-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d6915-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d6915-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d6915-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d6915-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d6915-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d6915-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6915-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6915-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d6915-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d6915-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d6915-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d6915-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d6915-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d6915-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6915-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6915-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6915-164">createdDateTime</span></span>|<span data-ttu-id="d6915-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6915-165">DateTimeOffset</span></span>|<span data-ttu-id="d6915-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d6915-166">DateTime the object was created.</span></span> <span data-ttu-id="d6915-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6915-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6915-168">description</span><span class="sxs-lookup"><span data-stu-id="d6915-168">description</span></span>|<span data-ttu-id="d6915-169">String</span><span class="sxs-lookup"><span data-stu-id="d6915-169">String</span></span>|<span data-ttu-id="d6915-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d6915-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d6915-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6915-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6915-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d6915-172">displayName</span></span>|<span data-ttu-id="d6915-173">Строка</span><span class="sxs-lookup"><span data-stu-id="d6915-173">String</span></span>|<span data-ttu-id="d6915-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d6915-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d6915-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6915-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6915-176">version</span><span class="sxs-lookup"><span data-stu-id="d6915-176">version</span></span>|<span data-ttu-id="d6915-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d6915-177">Int32</span></span>|<span data-ttu-id="d6915-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d6915-178">Version of the device configuration.</span></span> <span data-ttu-id="d6915-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6915-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6915-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="d6915-180">connectionName</span></span>|<span data-ttu-id="d6915-181">Строка</span><span class="sxs-lookup"><span data-stu-id="d6915-181">String</span></span>|<span data-ttu-id="d6915-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6915-182">Connection name displayed to the user.</span></span> <span data-ttu-id="d6915-183">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6915-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d6915-184">серверами</span><span class="sxs-lookup"><span data-stu-id="d6915-184">servers</span></span>|<span data-ttu-id="d6915-185">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="d6915-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="d6915-186">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="d6915-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="d6915-187">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="d6915-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="d6915-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="d6915-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d6915-189">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6915-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d6915-190">customXml</span><span class="sxs-lookup"><span data-stu-id="d6915-190">customXml</span></span>|<span data-ttu-id="d6915-191">Binary</span><span class="sxs-lookup"><span data-stu-id="d6915-191">Binary</span></span>|<span data-ttu-id="d6915-192">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="d6915-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="d6915-193">(Массив байтов в кодировке UTF8) Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6915-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d6915-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="d6915-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="d6915-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6915-195">Boolean</span></span>|<span data-ttu-id="d6915-196">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="d6915-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="d6915-197">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d6915-197">This property is read-only.</span></span> <span data-ttu-id="d6915-198">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6915-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="d6915-199">connectionType</span><span class="sxs-lookup"><span data-stu-id="d6915-199">connectionType</span></span>|[<span data-ttu-id="d6915-200">виндовсвпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="d6915-200">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="d6915-201">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="d6915-201">Connection type.</span></span> <span data-ttu-id="d6915-202">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6915-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="d6915-203">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="d6915-203">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="d6915-204">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="d6915-204">loginGroupOrDomain</span></span>|<span data-ttu-id="d6915-205">Строка</span><span class="sxs-lookup"><span data-stu-id="d6915-205">String</span></span>|<span data-ttu-id="d6915-206">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="d6915-206">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="d6915-207">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6915-207">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="d6915-208">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="d6915-208">enableSplitTunneling</span></span>|<span data-ttu-id="d6915-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6915-209">Boolean</span></span>|<span data-ttu-id="d6915-210">Включение Расщепленного туннелирования для VPN.</span><span class="sxs-lookup"><span data-stu-id="d6915-210">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="d6915-211">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6915-211">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="d6915-212">проксисервер</span><span class="sxs-lookup"><span data-stu-id="d6915-212">proxyServer</span></span>|[<span data-ttu-id="d6915-213">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="d6915-213">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="d6915-214">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="d6915-214">Proxy Server.</span></span> <span data-ttu-id="d6915-215">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6915-215">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="d6915-216">бипассвпнонкомпанивифи</span><span class="sxs-lookup"><span data-stu-id="d6915-216">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="d6915-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6915-217">Boolean</span></span>|<span data-ttu-id="d6915-218">Обход VPN в сети Wi-Fi компании.</span><span class="sxs-lookup"><span data-stu-id="d6915-218">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="d6915-219">бипассвпнонхомевифи</span><span class="sxs-lookup"><span data-stu-id="d6915-219">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="d6915-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6915-220">Boolean</span></span>|<span data-ttu-id="d6915-221">Обход VPN для домашнего Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="d6915-221">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="d6915-222">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="d6915-222">authenticationMethod</span></span>|[<span data-ttu-id="d6915-223">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="d6915-223">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="d6915-224">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d6915-224">Authentication method.</span></span> <span data-ttu-id="d6915-225">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="d6915-225">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="d6915-226">ремемберусеркредентиалс</span><span class="sxs-lookup"><span data-stu-id="d6915-226">rememberUserCredentials</span></span>|<span data-ttu-id="d6915-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6915-227">Boolean</span></span>|<span data-ttu-id="d6915-228">Запомнить учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6915-228">Remember user credentials.</span></span>|
|<span data-ttu-id="d6915-229">днссуффикссеарчлист</span><span class="sxs-lookup"><span data-stu-id="d6915-229">dnsSuffixSearchList</span></span>|<span data-ttu-id="d6915-230">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d6915-230">String collection</span></span>|<span data-ttu-id="d6915-231">Список поиска DNS-суффиксов.</span><span class="sxs-lookup"><span data-stu-id="d6915-231">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="d6915-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6915-232">Response</span></span>
<span data-ttu-id="d6915-233">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6915-233">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6915-234">Пример</span><span class="sxs-lookup"><span data-stu-id="d6915-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6915-235">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6915-235">Request</span></span>
<span data-ttu-id="d6915-236">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6915-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2016

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
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
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="d6915-237">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6915-237">Response</span></span>
<span data-ttu-id="d6915-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6915-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2188

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
  "id": "7cecc0db-c0db-7cec-dbc0-ec7cdbc0ec7c",
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
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```






