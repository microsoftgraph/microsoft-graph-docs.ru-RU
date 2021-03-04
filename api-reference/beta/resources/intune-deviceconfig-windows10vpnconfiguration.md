---
title: тип ресурса windows10VpnConfiguration
description: Предоставляя конфигурации в этом профиле, можно поручить устройству Windows 10 (настольному или мобильному) подключиться к нужной конечной точке VPN. Указав метод проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, можно сделать подключение VPN бесшовным для конечного пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c9cfc4fb3fc36ba2187458ded6072b992c278e7b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444541"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="ae7a3-104">тип ресурса windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae7a3-104">windows10VpnConfiguration resource type</span></span>

<span data-ttu-id="ae7a3-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae7a3-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae7a3-106">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae7a3-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae7a3-108">Предоставляя конфигурации в этом профиле, можно поручить устройству Windows 10 (настольному или мобильному) подключиться к нужной конечной точке VPN.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-108">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="ae7a3-109">Указав метод проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, можно сделать подключение VPN бесшовным для конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-109">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="ae7a3-110">Наследуется [от windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-110">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ae7a3-111">Методы</span><span class="sxs-lookup"><span data-stu-id="ae7a3-111">Methods</span></span>
|<span data-ttu-id="ae7a3-112">Метод</span><span class="sxs-lookup"><span data-stu-id="ae7a3-112">Method</span></span>|<span data-ttu-id="ae7a3-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ae7a3-113">Return Type</span></span>|<span data-ttu-id="ae7a3-114">Описание</span><span class="sxs-lookup"><span data-stu-id="ae7a3-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ae7a3-115">Список windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="ae7a3-115">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="ae7a3-116">[коллекция windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="ae7a3-117">Список свойств и связей [объектов Windows10VpnConfiguration.](../resources/intune-deviceconfig-windows10vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-117">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="ae7a3-118">Получить windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae7a3-118">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="ae7a3-119">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae7a3-119">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="ae7a3-120">Чтение свойств и связей [объекта Windows10VpnConfiguration.](../resources/intune-deviceconfig-windows10vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-120">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ae7a3-121">Создание windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae7a3-121">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="ae7a3-122">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae7a3-122">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="ae7a3-123">Создайте [новый объект Windows10VpnConfiguration.](../resources/intune-deviceconfig-windows10vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-123">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ae7a3-124">Удаление windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae7a3-124">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="ae7a3-125">Нет</span><span class="sxs-lookup"><span data-stu-id="ae7a3-125">None</span></span>|<span data-ttu-id="ae7a3-126">Удаляет [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-126">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="ae7a3-127">Обновление windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae7a3-127">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="ae7a3-128">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae7a3-128">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="ae7a3-129">Обновление свойств объекта [Windows10VpnConfiguration.](../resources/intune-deviceconfig-windows10vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-129">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ae7a3-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae7a3-130">Properties</span></span>
|<span data-ttu-id="ae7a3-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae7a3-131">Property</span></span>|<span data-ttu-id="ae7a3-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ae7a3-132">Type</span></span>|<span data-ttu-id="ae7a3-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ae7a3-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae7a3-134">id</span><span class="sxs-lookup"><span data-stu-id="ae7a3-134">id</span></span>|<span data-ttu-id="ae7a3-135">String</span><span class="sxs-lookup"><span data-stu-id="ae7a3-135">String</span></span>|<span data-ttu-id="ae7a3-136">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-136">Key of the entity.</span></span> <span data-ttu-id="ae7a3-137">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-137">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae7a3-138">lastModifiedDateTime</span></span>|<span data-ttu-id="ae7a3-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae7a3-139">DateTimeOffset</span></span>|<span data-ttu-id="ae7a3-140">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-140">DateTime the object was last modified.</span></span> <span data-ttu-id="ae7a3-141">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-141">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ae7a3-142">roleScopeTagIds</span></span>|<span data-ttu-id="ae7a3-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ae7a3-143">String collection</span></span>|<span data-ttu-id="ae7a3-144">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-144">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ae7a3-145">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-146">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ae7a3-146">supportsScopeTags</span></span>|<span data-ttu-id="ae7a3-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae7a3-147">Boolean</span></span>|<span data-ttu-id="ae7a3-148">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-148">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ae7a3-149">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-149">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ae7a3-150">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-150">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ae7a3-151">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-151">This property is read-only.</span></span> <span data-ttu-id="ae7a3-152">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-152">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ae7a3-153">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ae7a3-154">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ae7a3-154">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ae7a3-155">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-155">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ae7a3-156">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-156">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ae7a3-157">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ae7a3-158">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ae7a3-158">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ae7a3-159">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-159">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ae7a3-160">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-160">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ae7a3-161">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ae7a3-162">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ae7a3-162">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ae7a3-163">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-163">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ae7a3-164">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-164">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-165">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae7a3-165">createdDateTime</span></span>|<span data-ttu-id="ae7a3-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae7a3-166">DateTimeOffset</span></span>|<span data-ttu-id="ae7a3-167">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-167">DateTime the object was created.</span></span> <span data-ttu-id="ae7a3-168">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-168">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-169">description</span><span class="sxs-lookup"><span data-stu-id="ae7a3-169">description</span></span>|<span data-ttu-id="ae7a3-170">String</span><span class="sxs-lookup"><span data-stu-id="ae7a3-170">String</span></span>|<span data-ttu-id="ae7a3-171">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-171">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ae7a3-172">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-172">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-173">displayName</span><span class="sxs-lookup"><span data-stu-id="ae7a3-173">displayName</span></span>|<span data-ttu-id="ae7a3-174">String</span><span class="sxs-lookup"><span data-stu-id="ae7a3-174">String</span></span>|<span data-ttu-id="ae7a3-175">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-175">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ae7a3-176">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-176">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-177">version</span><span class="sxs-lookup"><span data-stu-id="ae7a3-177">version</span></span>|<span data-ttu-id="ae7a3-178">Int32</span><span class="sxs-lookup"><span data-stu-id="ae7a3-178">Int32</span></span>|<span data-ttu-id="ae7a3-179">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-179">Version of the device configuration.</span></span> <span data-ttu-id="ae7a3-180">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-180">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-181">connectionName</span><span class="sxs-lookup"><span data-stu-id="ae7a3-181">connectionName</span></span>|<span data-ttu-id="ae7a3-182">String</span><span class="sxs-lookup"><span data-stu-id="ae7a3-182">String</span></span>|<span data-ttu-id="ae7a3-183">Имя подключения, отображаемая пользователю.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-183">Connection name displayed to the user.</span></span> <span data-ttu-id="ae7a3-184">Унаследованный от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-184">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-185">серверы</span><span class="sxs-lookup"><span data-stu-id="ae7a3-185">servers</span></span>|<span data-ttu-id="ae7a3-186">[коллекция vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-186">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="ae7a3-187">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-187">List of VPN Servers on the network.</span></span> <span data-ttu-id="ae7a3-188">Убедитесь, что конечные пользователи могут получить доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-188">Make sure end users can access these network locations.</span></span> <span data-ttu-id="ae7a3-189">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ae7a3-190">Унаследованный от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-190">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-191">customXml</span><span class="sxs-lookup"><span data-stu-id="ae7a3-191">customXml</span></span>|<span data-ttu-id="ae7a3-192">Binary</span><span class="sxs-lookup"><span data-stu-id="ae7a3-192">Binary</span></span>|<span data-ttu-id="ae7a3-193">Настраиваемые XML-команды, настраиваемые vpn-подключением.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-193">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="ae7a3-194">(массив byte, закодированный UTF8) Унаследованный от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-194">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-195">profileTarget</span><span class="sxs-lookup"><span data-stu-id="ae7a3-195">profileTarget</span></span>|[<span data-ttu-id="ae7a3-196">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="ae7a3-196">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="ae7a3-197">Тип целевого профиля.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-197">Profile target type.</span></span> <span data-ttu-id="ae7a3-198">Возможные значения: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-198">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="ae7a3-199">connectionType</span><span class="sxs-lookup"><span data-stu-id="ae7a3-199">connectionType</span></span>|[<span data-ttu-id="ae7a3-200">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="ae7a3-200">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="ae7a3-201">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-201">Connection type.</span></span> <span data-ttu-id="ae7a3-202">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`, `ciscoAnyConnect`.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-202">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`, `ciscoAnyConnect`.</span></span>|
|<span data-ttu-id="ae7a3-203">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="ae7a3-203">enableSplitTunneling</span></span>|<span data-ttu-id="ae7a3-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae7a3-204">Boolean</span></span>|<span data-ttu-id="ae7a3-205">Включить раздельный туннель.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-205">Enable split tunneling.</span></span>|
|<span data-ttu-id="ae7a3-206">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="ae7a3-206">enableAlwaysOn</span></span>|<span data-ttu-id="ae7a3-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae7a3-207">Boolean</span></span>|<span data-ttu-id="ae7a3-208">Включить режим Always On.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-208">Enable Always On mode.</span></span>|
|<span data-ttu-id="ae7a3-209">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="ae7a3-209">enableDeviceTunnel</span></span>|<span data-ttu-id="ae7a3-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae7a3-210">Boolean</span></span>|<span data-ttu-id="ae7a3-211">Включить туннель устройства.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-211">Enable device tunnel.</span></span>|
|<span data-ttu-id="ae7a3-212">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="ae7a3-212">enableDnsRegistration</span></span>|<span data-ttu-id="ae7a3-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae7a3-213">Boolean</span></span>|<span data-ttu-id="ae7a3-214">Включить регистрацию IP-адресов с помощью внутреннего DNS.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-214">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="ae7a3-215">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="ae7a3-215">dnsSuffixes</span></span>|<span data-ttu-id="ae7a3-216">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ae7a3-216">String collection</span></span>|<span data-ttu-id="ae7a3-217">Укажите суффиксы DNS, чтобы добавить их в список поиска DNS, чтобы правильно маршрутизировать короткие имена.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-217">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="ae7a3-218">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ae7a3-218">authenticationMethod</span></span>|[<span data-ttu-id="ae7a3-219">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ae7a3-219">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="ae7a3-220">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-220">Authentication method.</span></span> <span data-ttu-id="ae7a3-221">Возможные значения: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-221">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span></span>|
|<span data-ttu-id="ae7a3-222">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="ae7a3-222">rememberUserCredentials</span></span>|<span data-ttu-id="ae7a3-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae7a3-223">Boolean</span></span>|<span data-ttu-id="ae7a3-224">Помните учетные данные пользователей.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-224">Remember user credentials.</span></span>|
|<span data-ttu-id="ae7a3-225">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="ae7a3-225">enableConditionalAccess</span></span>|<span data-ttu-id="ae7a3-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae7a3-226">Boolean</span></span>|<span data-ttu-id="ae7a3-227">Включить условный доступ.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-227">Enable conditional access.</span></span>|
|<span data-ttu-id="ae7a3-228">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="ae7a3-228">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="ae7a3-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae7a3-229">Boolean</span></span>|<span data-ttu-id="ae7a3-230">Включить один вход (SSO) с помощью альтернативного сертификата.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-230">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="ae7a3-231">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="ae7a3-231">singleSignOnEku</span></span>|[<span data-ttu-id="ae7a3-232">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="ae7a3-232">extendedKeyUsage</span></span>](../resources/intune-shared-extendedkeyusage.md)|<span data-ttu-id="ae7a3-233">Использование расширенного ключа с одним входом (EKU).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-233">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="ae7a3-234">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="ae7a3-234">singleSignOnIssuerHash</span></span>|<span data-ttu-id="ae7a3-235">String</span><span class="sxs-lookup"><span data-stu-id="ae7a3-235">String</span></span>|<span data-ttu-id="ae7a3-236">Hash одного входного эмитента.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-236">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="ae7a3-237">eapXml</span><span class="sxs-lookup"><span data-stu-id="ae7a3-237">eapXml</span></span>|<span data-ttu-id="ae7a3-238">Binary</span><span class="sxs-lookup"><span data-stu-id="ae7a3-238">Binary</span></span>|<span data-ttu-id="ae7a3-239">XML-протокол экстратензивной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-239">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="ae7a3-240">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-240">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="ae7a3-241">proxyServer</span><span class="sxs-lookup"><span data-stu-id="ae7a3-241">proxyServer</span></span>|[<span data-ttu-id="ae7a3-242">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="ae7a3-242">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="ae7a3-243">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-243">Proxy Server.</span></span>|
|<span data-ttu-id="ae7a3-244">associatedApps</span><span class="sxs-lookup"><span data-stu-id="ae7a3-244">associatedApps</span></span>|<span data-ttu-id="ae7a3-245">[коллекция windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-245">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="ae7a3-246">Связанные приложения.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-246">Associated Apps.</span></span> <span data-ttu-id="ae7a3-247">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-247">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ae7a3-248">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="ae7a3-248">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="ae7a3-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae7a3-249">Boolean</span></span>|<span data-ttu-id="ae7a3-250">Только связанные приложения могут использовать подключение (VPN для каждого приложения).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-250">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="ae7a3-251">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="ae7a3-251">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="ae7a3-252">String</span><span class="sxs-lookup"><span data-stu-id="ae7a3-252">String</span></span>|<span data-ttu-id="ae7a3-253">Домен Windows Information Protection (WIP) для связи с этим подключением.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-253">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="ae7a3-254">trafficRules</span><span class="sxs-lookup"><span data-stu-id="ae7a3-254">trafficRules</span></span>|<span data-ttu-id="ae7a3-255">[коллекция vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-255">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="ae7a3-256">Правила дорожного движения.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-256">Traffic rules.</span></span> <span data-ttu-id="ae7a3-257">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-257">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="ae7a3-258">маршруты</span><span class="sxs-lookup"><span data-stu-id="ae7a3-258">routes</span></span>|<span data-ttu-id="ae7a3-259">[коллекция vpnRoute](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-259">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="ae7a3-260">Маршруты (необязательные для сторонних поставщиков).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-260">Routes (optional for third-party providers).</span></span> <span data-ttu-id="ae7a3-261">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-261">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="ae7a3-262">dnsRules</span><span class="sxs-lookup"><span data-stu-id="ae7a3-262">dnsRules</span></span>|<span data-ttu-id="ae7a3-263">[коллекция vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-263">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="ae7a3-264">Правила DNS.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-264">DNS rules.</span></span> <span data-ttu-id="ae7a3-265">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-265">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="ae7a3-266">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="ae7a3-266">trustedNetworkDomains</span></span>|<span data-ttu-id="ae7a3-267">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ae7a3-267">String collection</span></span>|<span data-ttu-id="ae7a3-268">Доверенные сетевые домены</span><span class="sxs-lookup"><span data-stu-id="ae7a3-268">Trusted Network Domains</span></span>|
|<span data-ttu-id="ae7a3-269">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="ae7a3-269">cryptographySuite</span></span>|[<span data-ttu-id="ae7a3-270">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="ae7a3-270">cryptographySuite</span></span>](../resources/intune-deviceconfig-cryptographysuite.md)|<span data-ttu-id="ae7a3-271">Параметры безопасности пакета шифрования для VPN IKEv2 в Windows10 и выше</span><span class="sxs-lookup"><span data-stu-id="ae7a3-271">Cryptography Suite security settings for IKEv2 VPN in Windows10 and above</span></span> |

## <a name="relationships"></a><span data-ttu-id="ae7a3-272">Связи</span><span class="sxs-lookup"><span data-stu-id="ae7a3-272">Relationships</span></span>
|<span data-ttu-id="ae7a3-273">Связь</span><span class="sxs-lookup"><span data-stu-id="ae7a3-273">Relationship</span></span>|<span data-ttu-id="ae7a3-274">Тип</span><span class="sxs-lookup"><span data-stu-id="ae7a3-274">Type</span></span>|<span data-ttu-id="ae7a3-275">Описание</span><span class="sxs-lookup"><span data-stu-id="ae7a3-275">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae7a3-276">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="ae7a3-276">groupAssignments</span></span>|<span data-ttu-id="ae7a3-277">[коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-277">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="ae7a3-278">Список назначений групп для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-278">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="ae7a3-279">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-279">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-280">assignments</span><span class="sxs-lookup"><span data-stu-id="ae7a3-280">assignments</span></span>|<span data-ttu-id="ae7a3-281">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-281">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ae7a3-282">Список назначений для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-282">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="ae7a3-283">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-283">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-284">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="ae7a3-284">deviceStatuses</span></span>|<span data-ttu-id="ae7a3-285">Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-285">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="ae7a3-286">Состояние установки конфигурации для каждого устройства.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-286">Device configuration installation status by device.</span></span> <span data-ttu-id="ae7a3-287">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-287">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-288">userStatuses</span><span class="sxs-lookup"><span data-stu-id="ae7a3-288">userStatuses</span></span>|<span data-ttu-id="ae7a3-289">Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-289">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="ae7a3-290">Состояние установки конфигурации устройства пользователем.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-290">Device configuration installation status by user.</span></span> <span data-ttu-id="ae7a3-291">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-291">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-292">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="ae7a3-292">deviceStatusOverview</span></span>|[<span data-ttu-id="ae7a3-293">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ae7a3-293">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="ae7a3-294">Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-294">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-295">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="ae7a3-295">userStatusOverview</span></span>|[<span data-ttu-id="ae7a3-296">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="ae7a3-296">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="ae7a3-297">Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-297">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-298">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="ae7a3-298">deviceSettingStateSummaries</span></span>|<span data-ttu-id="ae7a3-299">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="ae7a3-299">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="ae7a3-300">Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae7a3-300">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae7a3-301">identityCertificate</span><span class="sxs-lookup"><span data-stu-id="ae7a3-301">identityCertificate</span></span>|[<span data-ttu-id="ae7a3-302">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="ae7a3-302">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="ae7a3-303">Сертификат удостоверений для проверки подлинности клиента, когда метод проверки подлинности является сертификатом.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-303">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae7a3-304">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae7a3-304">JSON Representation</span></span>
<span data-ttu-id="ae7a3-305">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae7a3-305">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10VpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "connectionName": "String",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "String",
      "address": "String",
      "isDefaultServer": true
    }
  ],
  "customXml": "binary",
  "profileTarget": "String",
  "connectionType": "String",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "String"
  ],
  "authenticationMethod": "String",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "String",
    "objectIdentifier": "String"
  },
  "singleSignOnIssuerHash": "String",
  "eapXml": "binary",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "String",
      "identifier": "String"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "String",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "String",
      "protocols": 1024,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "appId": "String",
      "appType": "String",
      "routingPolicyType": "String",
      "claims": "String"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "String",
      "prefixSize": 1024
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "String",
      "servers": [
        "String"
      ],
      "proxyServerUri": "String",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "String"
  ],
  "cryptographySuite": {
    "@odata.type": "microsoft.graph.cryptographySuite",
    "encryptionMethod": "String",
    "integrityCheckMethod": "String",
    "dhGroup": "String",
    "cipherTransformConstants": "String",
    "authenticationTransformConstants": "String",
    "pfsGroup": "String"
  }
}
```




