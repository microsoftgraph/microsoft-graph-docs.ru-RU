---
title: Обновление windows81VpnConfiguration
description: Обновление свойств объекта Windows81VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7dcd84bc12639cd20620d028514e4787e50dafc7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154940"
---
# <a name="update-windows81vpnconfiguration"></a><span data-ttu-id="3eb12-103">Обновление windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3eb12-103">Update windows81VpnConfiguration</span></span>

<span data-ttu-id="3eb12-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3eb12-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3eb12-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3eb12-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3eb12-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3eb12-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3eb12-107">Обновление свойств объекта [Windows81VpnConfiguration.](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb12-107">Update the properties of a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3eb12-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3eb12-108">Prerequisites</span></span>
<span data-ttu-id="3eb12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eb12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eb12-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3eb12-111">Permission type</span></span>|<span data-ttu-id="3eb12-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3eb12-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3eb12-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3eb12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3eb12-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb12-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3eb12-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3eb12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3eb12-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3eb12-116">Not supported.</span></span>|
|<span data-ttu-id="3eb12-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3eb12-117">Application</span></span>|<span data-ttu-id="3eb12-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb12-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3eb12-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3eb12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3eb12-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3eb12-120">Request headers</span></span>
|<span data-ttu-id="3eb12-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3eb12-121">Header</span></span>|<span data-ttu-id="3eb12-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3eb12-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3eb12-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3eb12-123">Authorization</span></span>|<span data-ttu-id="3eb12-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3eb12-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3eb12-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3eb12-125">Accept</span></span>|<span data-ttu-id="3eb12-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3eb12-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3eb12-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3eb12-127">Request body</span></span>
<span data-ttu-id="3eb12-128">В теле запроса поставляем представление JSON для [объекта Windows81VpnConfiguration.](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb12-128">In the request body, supply a JSON representation for the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="3eb12-129">В следующей таблице показаны свойства, необходимые при создании [windows81VpnConfiguration.](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb12-129">The following table shows the properties that are required when you create the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span>

|<span data-ttu-id="3eb12-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3eb12-130">Property</span></span>|<span data-ttu-id="3eb12-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3eb12-131">Type</span></span>|<span data-ttu-id="3eb12-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3eb12-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3eb12-133">id</span><span class="sxs-lookup"><span data-stu-id="3eb12-133">id</span></span>|<span data-ttu-id="3eb12-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3eb12-134">String</span></span>|<span data-ttu-id="3eb12-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3eb12-135">Key of the entity.</span></span> <span data-ttu-id="3eb12-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3eb12-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb12-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3eb12-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3eb12-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3eb12-138">DateTimeOffset</span></span>|<span data-ttu-id="3eb12-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3eb12-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3eb12-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3eb12-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb12-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3eb12-141">roleScopeTagIds</span></span>|<span data-ttu-id="3eb12-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3eb12-142">String collection</span></span>|<span data-ttu-id="3eb12-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="3eb12-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3eb12-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3eb12-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb12-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3eb12-145">supportsScopeTags</span></span>|<span data-ttu-id="3eb12-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3eb12-146">Boolean</span></span>|<span data-ttu-id="3eb12-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="3eb12-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3eb12-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="3eb12-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3eb12-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3eb12-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3eb12-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3eb12-150">This property is read-only.</span></span> <span data-ttu-id="3eb12-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3eb12-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb12-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3eb12-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3eb12-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3eb12-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3eb12-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3eb12-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3eb12-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3eb12-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb12-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3eb12-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3eb12-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3eb12-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3eb12-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3eb12-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3eb12-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3eb12-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb12-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3eb12-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3eb12-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3eb12-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3eb12-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3eb12-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3eb12-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3eb12-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb12-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3eb12-164">createdDateTime</span></span>|<span data-ttu-id="3eb12-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3eb12-165">DateTimeOffset</span></span>|<span data-ttu-id="3eb12-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3eb12-166">DateTime the object was created.</span></span> <span data-ttu-id="3eb12-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3eb12-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb12-168">description</span><span class="sxs-lookup"><span data-stu-id="3eb12-168">description</span></span>|<span data-ttu-id="3eb12-169">Строка</span><span class="sxs-lookup"><span data-stu-id="3eb12-169">String</span></span>|<span data-ttu-id="3eb12-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3eb12-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3eb12-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3eb12-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb12-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3eb12-172">displayName</span></span>|<span data-ttu-id="3eb12-173">Строка</span><span class="sxs-lookup"><span data-stu-id="3eb12-173">String</span></span>|<span data-ttu-id="3eb12-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3eb12-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3eb12-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3eb12-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb12-176">version</span><span class="sxs-lookup"><span data-stu-id="3eb12-176">version</span></span>|<span data-ttu-id="3eb12-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3eb12-177">Int32</span></span>|<span data-ttu-id="3eb12-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3eb12-178">Version of the device configuration.</span></span> <span data-ttu-id="3eb12-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3eb12-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb12-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="3eb12-180">connectionName</span></span>|<span data-ttu-id="3eb12-181">Строка</span><span class="sxs-lookup"><span data-stu-id="3eb12-181">String</span></span>|<span data-ttu-id="3eb12-182">Имя подключения, отображаемая пользователю.</span><span class="sxs-lookup"><span data-stu-id="3eb12-182">Connection name displayed to the user.</span></span> <span data-ttu-id="3eb12-183">Унаследованный от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb12-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="3eb12-184">серверы</span><span class="sxs-lookup"><span data-stu-id="3eb12-184">servers</span></span>|<span data-ttu-id="3eb12-185">[коллекция vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="3eb12-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="3eb12-186">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="3eb12-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="3eb12-187">Убедитесь, что конечные пользователи могут получить доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="3eb12-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="3eb12-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3eb12-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="3eb12-189">Унаследованный от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb12-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="3eb12-190">customXml</span><span class="sxs-lookup"><span data-stu-id="3eb12-190">customXml</span></span>|<span data-ttu-id="3eb12-191">Binary</span><span class="sxs-lookup"><span data-stu-id="3eb12-191">Binary</span></span>|<span data-ttu-id="3eb12-192">Настраиваемые XML-команды, настраиваемые vpn-подключением.</span><span class="sxs-lookup"><span data-stu-id="3eb12-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="3eb12-193">(массив byte, закодированный UTF8) Унаследованный от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb12-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="3eb12-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="3eb12-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="3eb12-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="3eb12-195">Boolean</span></span>|<span data-ttu-id="3eb12-196">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="3eb12-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="3eb12-197">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3eb12-197">This property is read-only.</span></span>|
|<span data-ttu-id="3eb12-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="3eb12-198">connectionType</span></span>|[<span data-ttu-id="3eb12-199">WindowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="3eb12-199">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="3eb12-200">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="3eb12-200">Connection type.</span></span> <span data-ttu-id="3eb12-201">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="3eb12-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="3eb12-202">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="3eb12-202">loginGroupOrDomain</span></span>|<span data-ttu-id="3eb12-203">Строка</span><span class="sxs-lookup"><span data-stu-id="3eb12-203">String</span></span>|<span data-ttu-id="3eb12-204">Группа входа или домен при наборе типа подключения к мобильному подключению Dell SonicWALL.</span><span class="sxs-lookup"><span data-stu-id="3eb12-204">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="3eb12-205">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="3eb12-205">enableSplitTunneling</span></span>|<span data-ttu-id="3eb12-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="3eb12-206">Boolean</span></span>|<span data-ttu-id="3eb12-207">Включить раздельный туннель для VPN.</span><span class="sxs-lookup"><span data-stu-id="3eb12-207">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="3eb12-208">proxyServer</span><span class="sxs-lookup"><span data-stu-id="3eb12-208">proxyServer</span></span>|[<span data-ttu-id="3eb12-209">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="3eb12-209">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="3eb12-210">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="3eb12-210">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="3eb12-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="3eb12-211">Response</span></span>
<span data-ttu-id="3eb12-212">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3eb12-212">If successful, this method returns a `200 OK` response code and an updated [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3eb12-213">Пример</span><span class="sxs-lookup"><span data-stu-id="3eb12-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="3eb12-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="3eb12-214">Request</span></span>
<span data-ttu-id="3eb12-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3eb12-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3eb12-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="3eb12-216">Response</span></span>
<span data-ttu-id="3eb12-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3eb12-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




