---
title: Создание windowsPhone81VpnConfiguration
description: Создайте новый объект WindowsPhone81VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d4c1578dfa97cd73a22e72308a7eead0b43fd73
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150950"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="b3022-103">Создание windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3022-103">Create windowsPhone81VpnConfiguration</span></span>

<span data-ttu-id="b3022-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3022-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3022-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3022-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3022-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3022-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3022-107">Создайте [новый объект WindowsPhone81VpnConfiguration.](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3022-107">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3022-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b3022-108">Prerequisites</span></span>
<span data-ttu-id="b3022-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3022-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3022-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3022-111">Permission type</span></span>|<span data-ttu-id="b3022-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3022-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3022-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3022-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3022-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3022-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3022-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3022-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3022-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3022-116">Not supported.</span></span>|
|<span data-ttu-id="b3022-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b3022-117">Application</span></span>|<span data-ttu-id="b3022-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3022-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3022-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3022-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b3022-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b3022-120">Request headers</span></span>
|<span data-ttu-id="b3022-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3022-121">Header</span></span>|<span data-ttu-id="b3022-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b3022-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3022-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3022-123">Authorization</span></span>|<span data-ttu-id="b3022-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3022-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3022-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b3022-125">Accept</span></span>|<span data-ttu-id="b3022-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3022-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3022-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3022-127">Request body</span></span>
<span data-ttu-id="b3022-128">В теле запроса предоставляем представление JSON для объекта windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b3022-128">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="b3022-129">В следующей таблице показаны свойства, необходимые при создании windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b3022-129">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="b3022-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3022-130">Property</span></span>|<span data-ttu-id="b3022-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b3022-131">Type</span></span>|<span data-ttu-id="b3022-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b3022-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3022-133">id</span><span class="sxs-lookup"><span data-stu-id="b3022-133">id</span></span>|<span data-ttu-id="b3022-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b3022-134">String</span></span>|<span data-ttu-id="b3022-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b3022-135">Key of the entity.</span></span> <span data-ttu-id="b3022-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3022-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3022-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3022-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b3022-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3022-138">DateTimeOffset</span></span>|<span data-ttu-id="b3022-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b3022-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b3022-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3022-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3022-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b3022-141">roleScopeTagIds</span></span>|<span data-ttu-id="b3022-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b3022-142">String collection</span></span>|<span data-ttu-id="b3022-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="b3022-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b3022-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3022-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3022-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b3022-145">supportsScopeTags</span></span>|<span data-ttu-id="b3022-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3022-146">Boolean</span></span>|<span data-ttu-id="b3022-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b3022-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b3022-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="b3022-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b3022-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b3022-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b3022-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b3022-150">This property is read-only.</span></span> <span data-ttu-id="b3022-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3022-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3022-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b3022-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b3022-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b3022-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b3022-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b3022-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b3022-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3022-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3022-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b3022-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b3022-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b3022-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b3022-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b3022-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b3022-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3022-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3022-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b3022-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b3022-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b3022-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b3022-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b3022-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b3022-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3022-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3022-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3022-164">createdDateTime</span></span>|<span data-ttu-id="b3022-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3022-165">DateTimeOffset</span></span>|<span data-ttu-id="b3022-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b3022-166">DateTime the object was created.</span></span> <span data-ttu-id="b3022-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3022-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3022-168">description</span><span class="sxs-lookup"><span data-stu-id="b3022-168">description</span></span>|<span data-ttu-id="b3022-169">Строка</span><span class="sxs-lookup"><span data-stu-id="b3022-169">String</span></span>|<span data-ttu-id="b3022-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b3022-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b3022-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3022-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3022-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b3022-172">displayName</span></span>|<span data-ttu-id="b3022-173">Строка</span><span class="sxs-lookup"><span data-stu-id="b3022-173">String</span></span>|<span data-ttu-id="b3022-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b3022-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b3022-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3022-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3022-176">version</span><span class="sxs-lookup"><span data-stu-id="b3022-176">version</span></span>|<span data-ttu-id="b3022-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b3022-177">Int32</span></span>|<span data-ttu-id="b3022-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b3022-178">Version of the device configuration.</span></span> <span data-ttu-id="b3022-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3022-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3022-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="b3022-180">connectionName</span></span>|<span data-ttu-id="b3022-181">Строка</span><span class="sxs-lookup"><span data-stu-id="b3022-181">String</span></span>|<span data-ttu-id="b3022-182">Имя подключения, отображаемая пользователю.</span><span class="sxs-lookup"><span data-stu-id="b3022-182">Connection name displayed to the user.</span></span> <span data-ttu-id="b3022-183">Унаследованный от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3022-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b3022-184">серверы</span><span class="sxs-lookup"><span data-stu-id="b3022-184">servers</span></span>|<span data-ttu-id="b3022-185">[коллекция vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="b3022-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="b3022-186">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="b3022-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="b3022-187">Убедитесь, что конечные пользователи могут получить доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="b3022-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="b3022-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="b3022-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b3022-189">Унаследованный от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3022-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b3022-190">customXml</span><span class="sxs-lookup"><span data-stu-id="b3022-190">customXml</span></span>|<span data-ttu-id="b3022-191">Binary</span><span class="sxs-lookup"><span data-stu-id="b3022-191">Binary</span></span>|<span data-ttu-id="b3022-192">Настраиваемые XML-команды, настраиваемые vpn-подключением.</span><span class="sxs-lookup"><span data-stu-id="b3022-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="b3022-193">(массив byte, закодированный UTF8) Унаследованный от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3022-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b3022-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="b3022-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="b3022-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3022-195">Boolean</span></span>|<span data-ttu-id="b3022-196">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="b3022-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="b3022-197">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b3022-197">This property is read-only.</span></span> <span data-ttu-id="b3022-198">Унаследованный от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3022-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="b3022-199">connectionType</span><span class="sxs-lookup"><span data-stu-id="b3022-199">connectionType</span></span>|[<span data-ttu-id="b3022-200">WindowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="b3022-200">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="b3022-201">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="b3022-201">Connection type.</span></span> <span data-ttu-id="b3022-202">Унаследовано от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3022-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="b3022-203">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="b3022-203">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="b3022-204">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="b3022-204">loginGroupOrDomain</span></span>|<span data-ttu-id="b3022-205">Строка</span><span class="sxs-lookup"><span data-stu-id="b3022-205">String</span></span>|<span data-ttu-id="b3022-206">Группа входа или домен при наборе типа подключения к мобильному подключению Dell SonicWALL.</span><span class="sxs-lookup"><span data-stu-id="b3022-206">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="b3022-207">Унаследованный от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3022-207">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="b3022-208">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="b3022-208">enableSplitTunneling</span></span>|<span data-ttu-id="b3022-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3022-209">Boolean</span></span>|<span data-ttu-id="b3022-210">Включить раздельный туннель для VPN.</span><span class="sxs-lookup"><span data-stu-id="b3022-210">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="b3022-211">Унаследованный от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3022-211">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="b3022-212">proxyServer</span><span class="sxs-lookup"><span data-stu-id="b3022-212">proxyServer</span></span>|[<span data-ttu-id="b3022-213">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="b3022-213">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="b3022-214">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="b3022-214">Proxy Server.</span></span> <span data-ttu-id="b3022-215">Унаследованный от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3022-215">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="b3022-216">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="b3022-216">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="b3022-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3022-217">Boolean</span></span>|<span data-ttu-id="b3022-218">Обход VPN в фирме Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b3022-218">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="b3022-219">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="b3022-219">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="b3022-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3022-220">Boolean</span></span>|<span data-ttu-id="b3022-221">Обход VPN в домашнем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b3022-221">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="b3022-222">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b3022-222">authenticationMethod</span></span>|[<span data-ttu-id="b3022-223">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b3022-223">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="b3022-224">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b3022-224">Authentication method.</span></span> <span data-ttu-id="b3022-225">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="b3022-225">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="b3022-226">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="b3022-226">rememberUserCredentials</span></span>|<span data-ttu-id="b3022-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3022-227">Boolean</span></span>|<span data-ttu-id="b3022-228">Помните учетные данные пользователей.</span><span class="sxs-lookup"><span data-stu-id="b3022-228">Remember user credentials.</span></span>|
|<span data-ttu-id="b3022-229">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="b3022-229">dnsSuffixSearchList</span></span>|<span data-ttu-id="b3022-230">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b3022-230">String collection</span></span>|<span data-ttu-id="b3022-231">Список поиска Суффикса DNS.</span><span class="sxs-lookup"><span data-stu-id="b3022-231">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="b3022-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3022-232">Response</span></span>
<span data-ttu-id="b3022-233">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b3022-233">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3022-234">Пример</span><span class="sxs-lookup"><span data-stu-id="b3022-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3022-235">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3022-235">Request</span></span>
<span data-ttu-id="b3022-236">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3022-236">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b3022-237">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3022-237">Response</span></span>
<span data-ttu-id="b3022-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3022-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




