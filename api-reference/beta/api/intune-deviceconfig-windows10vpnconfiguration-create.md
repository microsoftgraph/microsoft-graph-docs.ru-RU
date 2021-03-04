---
title: Создание windows10VpnConfiguration
description: Создайте новый объект Windows10VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 007f2c90d63ec2e3b6e9139a27fdc2c19bd44591
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435016"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="ef9e2-103">Создание windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ef9e2-103">Create windows10VpnConfiguration</span></span>

<span data-ttu-id="ef9e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef9e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef9e2-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef9e2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef9e2-107">Создайте [новый объект Windows10VpnConfiguration.](../resources/intune-deviceconfig-windows10vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9e2-107">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef9e2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ef9e2-108">Prerequisites</span></span>
<span data-ttu-id="ef9e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef9e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef9e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef9e2-111">Permission type</span></span>|<span data-ttu-id="ef9e2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef9e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef9e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef9e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef9e2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef9e2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef9e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef9e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef9e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-116">Not supported.</span></span>|
|<span data-ttu-id="ef9e2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ef9e2-117">Application</span></span>|<span data-ttu-id="ef9e2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef9e2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef9e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef9e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ef9e2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ef9e2-120">Request headers</span></span>
|<span data-ttu-id="ef9e2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef9e2-121">Header</span></span>|<span data-ttu-id="ef9e2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ef9e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef9e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef9e2-123">Authorization</span></span>|<span data-ttu-id="ef9e2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef9e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ef9e2-125">Accept</span></span>|<span data-ttu-id="ef9e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef9e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef9e2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef9e2-127">Request body</span></span>
<span data-ttu-id="ef9e2-128">В теле запроса предоставляем представление JSON для объекта Windows10VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-128">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="ef9e2-129">В следующей таблице показаны свойства, необходимые при создании windows10VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-129">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="ef9e2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef9e2-130">Property</span></span>|<span data-ttu-id="ef9e2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ef9e2-131">Type</span></span>|<span data-ttu-id="ef9e2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ef9e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef9e2-133">id</span><span class="sxs-lookup"><span data-stu-id="ef9e2-133">id</span></span>|<span data-ttu-id="ef9e2-134">String</span><span class="sxs-lookup"><span data-stu-id="ef9e2-134">String</span></span>|<span data-ttu-id="ef9e2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-135">Key of the entity.</span></span> <span data-ttu-id="ef9e2-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef9e2-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9e2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef9e2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ef9e2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef9e2-138">DateTimeOffset</span></span>|<span data-ttu-id="ef9e2-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ef9e2-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef9e2-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9e2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ef9e2-141">roleScopeTagIds</span></span>|<span data-ttu-id="ef9e2-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ef9e2-142">String collection</span></span>|<span data-ttu-id="ef9e2-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ef9e2-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef9e2-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9e2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ef9e2-145">supportsScopeTags</span></span>|<span data-ttu-id="ef9e2-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9e2-146">Boolean</span></span>|<span data-ttu-id="ef9e2-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ef9e2-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ef9e2-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ef9e2-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-150">This property is read-only.</span></span> <span data-ttu-id="ef9e2-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef9e2-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9e2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ef9e2-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ef9e2-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ef9e2-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ef9e2-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ef9e2-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef9e2-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9e2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ef9e2-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ef9e2-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ef9e2-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ef9e2-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ef9e2-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef9e2-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9e2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ef9e2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ef9e2-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ef9e2-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ef9e2-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ef9e2-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef9e2-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9e2-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef9e2-164">createdDateTime</span></span>|<span data-ttu-id="ef9e2-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef9e2-165">DateTimeOffset</span></span>|<span data-ttu-id="ef9e2-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-166">DateTime the object was created.</span></span> <span data-ttu-id="ef9e2-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef9e2-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9e2-168">description</span><span class="sxs-lookup"><span data-stu-id="ef9e2-168">description</span></span>|<span data-ttu-id="ef9e2-169">String</span><span class="sxs-lookup"><span data-stu-id="ef9e2-169">String</span></span>|<span data-ttu-id="ef9e2-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ef9e2-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef9e2-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9e2-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ef9e2-172">displayName</span></span>|<span data-ttu-id="ef9e2-173">String</span><span class="sxs-lookup"><span data-stu-id="ef9e2-173">String</span></span>|<span data-ttu-id="ef9e2-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ef9e2-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef9e2-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9e2-176">version</span><span class="sxs-lookup"><span data-stu-id="ef9e2-176">version</span></span>|<span data-ttu-id="ef9e2-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ef9e2-177">Int32</span></span>|<span data-ttu-id="ef9e2-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-178">Version of the device configuration.</span></span> <span data-ttu-id="ef9e2-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef9e2-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef9e2-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="ef9e2-180">connectionName</span></span>|<span data-ttu-id="ef9e2-181">String</span><span class="sxs-lookup"><span data-stu-id="ef9e2-181">String</span></span>|<span data-ttu-id="ef9e2-182">Имя подключения, отображаемая пользователю.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-182">Connection name displayed to the user.</span></span> <span data-ttu-id="ef9e2-183">Унаследованный от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9e2-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ef9e2-184">серверы</span><span class="sxs-lookup"><span data-stu-id="ef9e2-184">servers</span></span>|<span data-ttu-id="ef9e2-185">[коллекция vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="ef9e2-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="ef9e2-186">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="ef9e2-187">Убедитесь, что конечные пользователи могут получить доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="ef9e2-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ef9e2-189">Унаследованный от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9e2-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ef9e2-190">customXml</span><span class="sxs-lookup"><span data-stu-id="ef9e2-190">customXml</span></span>|<span data-ttu-id="ef9e2-191">Binary</span><span class="sxs-lookup"><span data-stu-id="ef9e2-191">Binary</span></span>|<span data-ttu-id="ef9e2-192">Настраиваемые XML-команды, настраиваемые vpn-подключением.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="ef9e2-193">(массив byte, закодированный UTF8) Унаследованный от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef9e2-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ef9e2-194">profileTarget</span><span class="sxs-lookup"><span data-stu-id="ef9e2-194">profileTarget</span></span>|[<span data-ttu-id="ef9e2-195">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="ef9e2-195">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="ef9e2-196">Тип целевого профиля.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-196">Profile target type.</span></span> <span data-ttu-id="ef9e2-197">Возможные значения: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-197">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="ef9e2-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="ef9e2-198">connectionType</span></span>|[<span data-ttu-id="ef9e2-199">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="ef9e2-199">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="ef9e2-200">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-200">Connection type.</span></span> <span data-ttu-id="ef9e2-201">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`, `ciscoAnyConnect`.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`, `ciscoAnyConnect`.</span></span>|
|<span data-ttu-id="ef9e2-202">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="ef9e2-202">enableSplitTunneling</span></span>|<span data-ttu-id="ef9e2-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9e2-203">Boolean</span></span>|<span data-ttu-id="ef9e2-204">Включить раздельный туннель.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-204">Enable split tunneling.</span></span>|
|<span data-ttu-id="ef9e2-205">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="ef9e2-205">enableAlwaysOn</span></span>|<span data-ttu-id="ef9e2-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9e2-206">Boolean</span></span>|<span data-ttu-id="ef9e2-207">Включить режим Always On.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-207">Enable Always On mode.</span></span>|
|<span data-ttu-id="ef9e2-208">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="ef9e2-208">enableDeviceTunnel</span></span>|<span data-ttu-id="ef9e2-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9e2-209">Boolean</span></span>|<span data-ttu-id="ef9e2-210">Включить туннель устройства.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-210">Enable device tunnel.</span></span>|
|<span data-ttu-id="ef9e2-211">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="ef9e2-211">enableDnsRegistration</span></span>|<span data-ttu-id="ef9e2-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9e2-212">Boolean</span></span>|<span data-ttu-id="ef9e2-213">Включить регистрацию IP-адресов с помощью внутреннего DNS.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-213">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="ef9e2-214">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="ef9e2-214">dnsSuffixes</span></span>|<span data-ttu-id="ef9e2-215">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ef9e2-215">String collection</span></span>|<span data-ttu-id="ef9e2-216">Укажите суффиксы DNS, чтобы добавить их в список поиска DNS, чтобы правильно маршрутизировать короткие имена.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-216">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="ef9e2-217">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ef9e2-217">authenticationMethod</span></span>|[<span data-ttu-id="ef9e2-218">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ef9e2-218">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="ef9e2-219">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-219">Authentication method.</span></span> <span data-ttu-id="ef9e2-220">Возможные значения: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-220">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span></span>|
|<span data-ttu-id="ef9e2-221">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="ef9e2-221">rememberUserCredentials</span></span>|<span data-ttu-id="ef9e2-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9e2-222">Boolean</span></span>|<span data-ttu-id="ef9e2-223">Помните учетные данные пользователей.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-223">Remember user credentials.</span></span>|
|<span data-ttu-id="ef9e2-224">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="ef9e2-224">enableConditionalAccess</span></span>|<span data-ttu-id="ef9e2-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9e2-225">Boolean</span></span>|<span data-ttu-id="ef9e2-226">Включить условный доступ.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-226">Enable conditional access.</span></span>|
|<span data-ttu-id="ef9e2-227">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="ef9e2-227">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="ef9e2-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9e2-228">Boolean</span></span>|<span data-ttu-id="ef9e2-229">Включить один вход (SSO) с помощью альтернативного сертификата.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-229">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="ef9e2-230">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="ef9e2-230">singleSignOnEku</span></span>|[<span data-ttu-id="ef9e2-231">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="ef9e2-231">extendedKeyUsage</span></span>](../resources/intune-shared-extendedkeyusage.md)|<span data-ttu-id="ef9e2-232">Использование расширенного ключа с одним входом (EKU).</span><span class="sxs-lookup"><span data-stu-id="ef9e2-232">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="ef9e2-233">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="ef9e2-233">singleSignOnIssuerHash</span></span>|<span data-ttu-id="ef9e2-234">String</span><span class="sxs-lookup"><span data-stu-id="ef9e2-234">String</span></span>|<span data-ttu-id="ef9e2-235">Hash одного входного эмитента.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-235">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="ef9e2-236">eapXml</span><span class="sxs-lookup"><span data-stu-id="ef9e2-236">eapXml</span></span>|<span data-ttu-id="ef9e2-237">Binary</span><span class="sxs-lookup"><span data-stu-id="ef9e2-237">Binary</span></span>|<span data-ttu-id="ef9e2-238">XML-протокол экстратензивной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="ef9e2-238">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="ef9e2-239">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="ef9e2-239">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="ef9e2-240">proxyServer</span><span class="sxs-lookup"><span data-stu-id="ef9e2-240">proxyServer</span></span>|[<span data-ttu-id="ef9e2-241">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="ef9e2-241">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="ef9e2-242">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-242">Proxy Server.</span></span>|
|<span data-ttu-id="ef9e2-243">associatedApps</span><span class="sxs-lookup"><span data-stu-id="ef9e2-243">associatedApps</span></span>|<span data-ttu-id="ef9e2-244">[коллекция windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="ef9e2-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="ef9e2-245">Связанные приложения.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-245">Associated Apps.</span></span> <span data-ttu-id="ef9e2-246">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-246">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ef9e2-247">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="ef9e2-247">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="ef9e2-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef9e2-248">Boolean</span></span>|<span data-ttu-id="ef9e2-249">Только связанные приложения могут использовать подключение (VPN для каждого приложения).</span><span class="sxs-lookup"><span data-stu-id="ef9e2-249">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="ef9e2-250">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="ef9e2-250">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="ef9e2-251">String</span><span class="sxs-lookup"><span data-stu-id="ef9e2-251">String</span></span>|<span data-ttu-id="ef9e2-252">Домен Windows Information Protection (WIP) для связи с этим подключением.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-252">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="ef9e2-253">trafficRules</span><span class="sxs-lookup"><span data-stu-id="ef9e2-253">trafficRules</span></span>|<span data-ttu-id="ef9e2-254">[коллекция vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="ef9e2-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="ef9e2-255">Правила дорожного движения.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-255">Traffic rules.</span></span> <span data-ttu-id="ef9e2-256">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-256">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="ef9e2-257">маршруты</span><span class="sxs-lookup"><span data-stu-id="ef9e2-257">routes</span></span>|<span data-ttu-id="ef9e2-258">[коллекция vpnRoute](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="ef9e2-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="ef9e2-259">Маршруты (необязательные для сторонних поставщиков).</span><span class="sxs-lookup"><span data-stu-id="ef9e2-259">Routes (optional for third-party providers).</span></span> <span data-ttu-id="ef9e2-260">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-260">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="ef9e2-261">dnsRules</span><span class="sxs-lookup"><span data-stu-id="ef9e2-261">dnsRules</span></span>|<span data-ttu-id="ef9e2-262">[коллекция vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="ef9e2-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="ef9e2-263">Правила DNS.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-263">DNS rules.</span></span> <span data-ttu-id="ef9e2-264">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-264">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="ef9e2-265">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="ef9e2-265">trustedNetworkDomains</span></span>|<span data-ttu-id="ef9e2-266">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ef9e2-266">String collection</span></span>|<span data-ttu-id="ef9e2-267">Доверенные сетевые домены</span><span class="sxs-lookup"><span data-stu-id="ef9e2-267">Trusted Network Domains</span></span>|
|<span data-ttu-id="ef9e2-268">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="ef9e2-268">cryptographySuite</span></span>|[<span data-ttu-id="ef9e2-269">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="ef9e2-269">cryptographySuite</span></span>](../resources/intune-deviceconfig-cryptographysuite.md)|<span data-ttu-id="ef9e2-270">Параметры безопасности пакета шифрования для VPN IKEv2 в Windows10 и выше</span><span class="sxs-lookup"><span data-stu-id="ef9e2-270">Cryptography Suite security settings for IKEv2 VPN in Windows10 and above</span></span> |



## <a name="response"></a><span data-ttu-id="ef9e2-271">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef9e2-271">Response</span></span>
<span data-ttu-id="ef9e2-272">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-272">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef9e2-273">Пример</span><span class="sxs-lookup"><span data-stu-id="ef9e2-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef9e2-274">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef9e2-274">Request</span></span>
<span data-ttu-id="ef9e2-275">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-275">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="ef9e2-276">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef9e2-276">Response</span></span>
<span data-ttu-id="ef9e2-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef9e2-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




