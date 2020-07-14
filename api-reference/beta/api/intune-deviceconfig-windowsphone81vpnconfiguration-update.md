---
title: Обновление windowsPhone81VpnConfiguration
description: Обновление свойств объекта windowsPhone81VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f02fd9ff1e7821cdff099971ffa04127717537b6
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122765"
---
# <a name="update-windowsphone81vpnconfiguration"></a><span data-ttu-id="15b87-103">Обновление windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="15b87-103">Update windowsPhone81VpnConfiguration</span></span>

<span data-ttu-id="15b87-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15b87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15b87-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15b87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15b87-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15b87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15b87-107">Обновление свойств объекта [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="15b87-107">Update the properties of a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15b87-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="15b87-108">Prerequisites</span></span>
<span data-ttu-id="15b87-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="15b87-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="15b87-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15b87-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15b87-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15b87-111">Permission type</span></span>|<span data-ttu-id="15b87-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="15b87-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15b87-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15b87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15b87-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15b87-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="15b87-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15b87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15b87-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15b87-116">Not supported.</span></span>|
|<span data-ttu-id="15b87-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15b87-117">Application</span></span>|<span data-ttu-id="15b87-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15b87-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15b87-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15b87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="15b87-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="15b87-120">Request headers</span></span>
|<span data-ttu-id="15b87-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15b87-121">Header</span></span>|<span data-ttu-id="15b87-122">Значение</span><span class="sxs-lookup"><span data-stu-id="15b87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15b87-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15b87-123">Authorization</span></span>|<span data-ttu-id="15b87-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15b87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15b87-125">Accept</span><span class="sxs-lookup"><span data-stu-id="15b87-125">Accept</span></span>|<span data-ttu-id="15b87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15b87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15b87-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15b87-127">Request body</span></span>
<span data-ttu-id="15b87-128">В тексте запроса добавьте представление объекта [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15b87-128">In the request body, supply a JSON representation for the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="15b87-129">В следующей таблице приведены свойства, необходимые при создании [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15b87-129">The following table shows the properties that are required when you create the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span></span>

|<span data-ttu-id="15b87-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="15b87-130">Property</span></span>|<span data-ttu-id="15b87-131">Тип</span><span class="sxs-lookup"><span data-stu-id="15b87-131">Type</span></span>|<span data-ttu-id="15b87-132">Описание</span><span class="sxs-lookup"><span data-stu-id="15b87-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15b87-133">id</span><span class="sxs-lookup"><span data-stu-id="15b87-133">id</span></span>|<span data-ttu-id="15b87-134">String</span><span class="sxs-lookup"><span data-stu-id="15b87-134">String</span></span>|<span data-ttu-id="15b87-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="15b87-135">Key of the entity.</span></span> <span data-ttu-id="15b87-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15b87-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15b87-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15b87-137">lastModifiedDateTime</span></span>|<span data-ttu-id="15b87-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15b87-138">DateTimeOffset</span></span>|<span data-ttu-id="15b87-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="15b87-139">DateTime the object was last modified.</span></span> <span data-ttu-id="15b87-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15b87-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15b87-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="15b87-141">roleScopeTagIds</span></span>|<span data-ttu-id="15b87-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="15b87-142">String collection</span></span>|<span data-ttu-id="15b87-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="15b87-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="15b87-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15b87-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15b87-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="15b87-145">supportsScopeTags</span></span>|<span data-ttu-id="15b87-146">Логический</span><span class="sxs-lookup"><span data-stu-id="15b87-146">Boolean</span></span>|<span data-ttu-id="15b87-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="15b87-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="15b87-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="15b87-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="15b87-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="15b87-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="15b87-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="15b87-150">This property is read-only.</span></span> <span data-ttu-id="15b87-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15b87-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15b87-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="15b87-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="15b87-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="15b87-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="15b87-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="15b87-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="15b87-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15b87-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15b87-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="15b87-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="15b87-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="15b87-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="15b87-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="15b87-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="15b87-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15b87-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15b87-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="15b87-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="15b87-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="15b87-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="15b87-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="15b87-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="15b87-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15b87-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15b87-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15b87-164">createdDateTime</span></span>|<span data-ttu-id="15b87-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15b87-165">DateTimeOffset</span></span>|<span data-ttu-id="15b87-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="15b87-166">DateTime the object was created.</span></span> <span data-ttu-id="15b87-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15b87-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15b87-168">description</span><span class="sxs-lookup"><span data-stu-id="15b87-168">description</span></span>|<span data-ttu-id="15b87-169">String</span><span class="sxs-lookup"><span data-stu-id="15b87-169">String</span></span>|<span data-ttu-id="15b87-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="15b87-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="15b87-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15b87-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15b87-172">displayName</span><span class="sxs-lookup"><span data-stu-id="15b87-172">displayName</span></span>|<span data-ttu-id="15b87-173">Строка</span><span class="sxs-lookup"><span data-stu-id="15b87-173">String</span></span>|<span data-ttu-id="15b87-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="15b87-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="15b87-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15b87-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15b87-176">version</span><span class="sxs-lookup"><span data-stu-id="15b87-176">version</span></span>|<span data-ttu-id="15b87-177">Int32</span><span class="sxs-lookup"><span data-stu-id="15b87-177">Int32</span></span>|<span data-ttu-id="15b87-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="15b87-178">Version of the device configuration.</span></span> <span data-ttu-id="15b87-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15b87-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15b87-180">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="15b87-180">connectionName</span></span>|<span data-ttu-id="15b87-181">String</span><span class="sxs-lookup"><span data-stu-id="15b87-181">String</span></span>|<span data-ttu-id="15b87-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="15b87-182">Connection name displayed to the user.</span></span> <span data-ttu-id="15b87-183">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15b87-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="15b87-184">серверами</span><span class="sxs-lookup"><span data-stu-id="15b87-184">servers</span></span>|<span data-ttu-id="15b87-185">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="15b87-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="15b87-186">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="15b87-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="15b87-187">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="15b87-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="15b87-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="15b87-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="15b87-189">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15b87-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="15b87-190">customXml</span><span class="sxs-lookup"><span data-stu-id="15b87-190">customXml</span></span>|<span data-ttu-id="15b87-191">Binary</span><span class="sxs-lookup"><span data-stu-id="15b87-191">Binary</span></span>|<span data-ttu-id="15b87-192">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="15b87-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="15b87-193">(Массив байтов в кодировке UTF8) Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15b87-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="15b87-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="15b87-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="15b87-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="15b87-195">Boolean</span></span>|<span data-ttu-id="15b87-196">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="15b87-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="15b87-197">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="15b87-197">This property is read-only.</span></span> <span data-ttu-id="15b87-198">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15b87-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="15b87-199">connectionType</span><span class="sxs-lookup"><span data-stu-id="15b87-199">connectionType</span></span>|[<span data-ttu-id="15b87-200">виндовсвпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="15b87-200">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="15b87-201">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="15b87-201">Connection type.</span></span> <span data-ttu-id="15b87-202">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15b87-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="15b87-203">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="15b87-203">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="15b87-204">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="15b87-204">loginGroupOrDomain</span></span>|<span data-ttu-id="15b87-205">String</span><span class="sxs-lookup"><span data-stu-id="15b87-205">String</span></span>|<span data-ttu-id="15b87-206">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="15b87-206">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="15b87-207">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15b87-207">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="15b87-208">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="15b87-208">enableSplitTunneling</span></span>|<span data-ttu-id="15b87-209">Логический</span><span class="sxs-lookup"><span data-stu-id="15b87-209">Boolean</span></span>|<span data-ttu-id="15b87-210">Включение Расщепленного туннелирования для VPN.</span><span class="sxs-lookup"><span data-stu-id="15b87-210">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="15b87-211">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15b87-211">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="15b87-212">проксисервер</span><span class="sxs-lookup"><span data-stu-id="15b87-212">proxyServer</span></span>|[<span data-ttu-id="15b87-213">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="15b87-213">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="15b87-214">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="15b87-214">Proxy Server.</span></span> <span data-ttu-id="15b87-215">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15b87-215">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="15b87-216">бипассвпнонкомпанивифи</span><span class="sxs-lookup"><span data-stu-id="15b87-216">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="15b87-217">Логический</span><span class="sxs-lookup"><span data-stu-id="15b87-217">Boolean</span></span>|<span data-ttu-id="15b87-218">Обход VPN в сети Wi-Fi компании.</span><span class="sxs-lookup"><span data-stu-id="15b87-218">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="15b87-219">бипассвпнонхомевифи</span><span class="sxs-lookup"><span data-stu-id="15b87-219">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="15b87-220">Логический</span><span class="sxs-lookup"><span data-stu-id="15b87-220">Boolean</span></span>|<span data-ttu-id="15b87-221">Обход VPN для домашнего Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="15b87-221">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="15b87-222">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="15b87-222">authenticationMethod</span></span>|[<span data-ttu-id="15b87-223">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="15b87-223">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="15b87-224">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="15b87-224">Authentication method.</span></span> <span data-ttu-id="15b87-225">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="15b87-225">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="15b87-226">ремемберусеркредентиалс</span><span class="sxs-lookup"><span data-stu-id="15b87-226">rememberUserCredentials</span></span>|<span data-ttu-id="15b87-227">Логический</span><span class="sxs-lookup"><span data-stu-id="15b87-227">Boolean</span></span>|<span data-ttu-id="15b87-228">Запомнить учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="15b87-228">Remember user credentials.</span></span>|
|<span data-ttu-id="15b87-229">днссуффикссеарчлист</span><span class="sxs-lookup"><span data-stu-id="15b87-229">dnsSuffixSearchList</span></span>|<span data-ttu-id="15b87-230">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="15b87-230">String collection</span></span>|<span data-ttu-id="15b87-231">Список поиска DNS-суффиксов.</span><span class="sxs-lookup"><span data-stu-id="15b87-231">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="15b87-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="15b87-232">Response</span></span>
<span data-ttu-id="15b87-233">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="15b87-233">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15b87-234">Пример</span><span class="sxs-lookup"><span data-stu-id="15b87-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="15b87-235">Запрос</span><span class="sxs-lookup"><span data-stu-id="15b87-235">Request</span></span>
<span data-ttu-id="15b87-236">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15b87-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="15b87-237">Отклик</span><span class="sxs-lookup"><span data-stu-id="15b87-237">Response</span></span>
<span data-ttu-id="15b87-238">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="15b87-238">Here is an example of the response.</span></span> <span data-ttu-id="15b87-239">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="15b87-239">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="15b87-240">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="15b87-240">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



