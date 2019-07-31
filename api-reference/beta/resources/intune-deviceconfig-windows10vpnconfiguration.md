---
title: Тип ресурса windows10VpnConfiguration
description: Предоставляя конфигурации в этом профиле, вы можете указать устройству Windows 10 (настольный или мобильный) подключаться к необходимой конечной точке VPN. Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, вы можете сделать VPN-подключение неполноценным для конечного пользователя.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dc72a3b0b8934b5056bad261cc2f11121293f6e7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000370"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="365fd-104">Тип ресурса windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="365fd-104">windows10VpnConfiguration resource type</span></span>

> <span data-ttu-id="365fd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="365fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="365fd-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="365fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="365fd-107">Предоставляя конфигурации в этом профиле, вы можете указать устройству Windows 10 (настольный или мобильный) подключаться к необходимой конечной точке VPN.</span><span class="sxs-lookup"><span data-stu-id="365fd-107">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="365fd-108">Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, вы можете сделать VPN-подключение неполноценным для конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="365fd-108">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="365fd-109">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="365fd-109">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="365fd-110">Методы</span><span class="sxs-lookup"><span data-stu-id="365fd-110">Methods</span></span>
|<span data-ttu-id="365fd-111">Метод</span><span class="sxs-lookup"><span data-stu-id="365fd-111">Method</span></span>|<span data-ttu-id="365fd-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="365fd-112">Return Type</span></span>|<span data-ttu-id="365fd-113">Описание</span><span class="sxs-lookup"><span data-stu-id="365fd-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="365fd-114">Список windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="365fd-114">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="365fd-115">Коллекция [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="365fd-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="365fd-116">Список свойств и связей объектов [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="365fd-116">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="365fd-117">Получение windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="365fd-117">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="365fd-118">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="365fd-118">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="365fd-119">Чтение свойств и связей объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="365fd-119">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="365fd-120">Создание windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="365fd-120">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="365fd-121">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="365fd-121">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="365fd-122">Создание нового объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="365fd-122">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="365fd-123">Удаление windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="365fd-123">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="365fd-124">Нет</span><span class="sxs-lookup"><span data-stu-id="365fd-124">None</span></span>|<span data-ttu-id="365fd-125">Удаляет объект [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-125">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="365fd-126">Обновление windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="365fd-126">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="365fd-127">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="365fd-127">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="365fd-128">Обновление свойств объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="365fd-128">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="365fd-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="365fd-129">Properties</span></span>
|<span data-ttu-id="365fd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="365fd-130">Property</span></span>|<span data-ttu-id="365fd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="365fd-131">Type</span></span>|<span data-ttu-id="365fd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="365fd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="365fd-133">id</span><span class="sxs-lookup"><span data-stu-id="365fd-133">id</span></span>|<span data-ttu-id="365fd-134">String</span><span class="sxs-lookup"><span data-stu-id="365fd-134">String</span></span>|<span data-ttu-id="365fd-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="365fd-135">Key of the entity.</span></span> <span data-ttu-id="365fd-136">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="365fd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="365fd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="365fd-138">DateTimeOffset</span></span>|<span data-ttu-id="365fd-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="365fd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="365fd-140">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="365fd-141">roleScopeTagIds</span></span>|<span data-ttu-id="365fd-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="365fd-142">String collection</span></span>|<span data-ttu-id="365fd-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="365fd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="365fd-144">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-145">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="365fd-145">supportsScopeTags</span></span>|<span data-ttu-id="365fd-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="365fd-146">Boolean</span></span>|<span data-ttu-id="365fd-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="365fd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="365fd-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="365fd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="365fd-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="365fd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="365fd-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="365fd-150">This property is read-only.</span></span> <span data-ttu-id="365fd-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="365fd-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="365fd-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="365fd-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="365fd-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="365fd-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="365fd-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="365fd-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="365fd-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="365fd-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="365fd-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="365fd-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="365fd-159">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="365fd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="365fd-161">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="365fd-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="365fd-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="365fd-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="365fd-163">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="365fd-164">createdDateTime</span></span>|<span data-ttu-id="365fd-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="365fd-165">DateTimeOffset</span></span>|<span data-ttu-id="365fd-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="365fd-166">DateTime the object was created.</span></span> <span data-ttu-id="365fd-167">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-168">description</span><span class="sxs-lookup"><span data-stu-id="365fd-168">description</span></span>|<span data-ttu-id="365fd-169">String</span><span class="sxs-lookup"><span data-stu-id="365fd-169">String</span></span>|<span data-ttu-id="365fd-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="365fd-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="365fd-171">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-171">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-172">displayName</span><span class="sxs-lookup"><span data-stu-id="365fd-172">displayName</span></span>|<span data-ttu-id="365fd-173">Строка</span><span class="sxs-lookup"><span data-stu-id="365fd-173">String</span></span>|<span data-ttu-id="365fd-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="365fd-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="365fd-175">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-175">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-176">version</span><span class="sxs-lookup"><span data-stu-id="365fd-176">version</span></span>|<span data-ttu-id="365fd-177">Int32</span><span class="sxs-lookup"><span data-stu-id="365fd-177">Int32</span></span>|<span data-ttu-id="365fd-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="365fd-178">Version of the device configuration.</span></span> <span data-ttu-id="365fd-179">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-179">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-180">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="365fd-180">connectionName</span></span>|<span data-ttu-id="365fd-181">String</span><span class="sxs-lookup"><span data-stu-id="365fd-181">String</span></span>|<span data-ttu-id="365fd-182">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="365fd-182">Connection name displayed to the user.</span></span> <span data-ttu-id="365fd-183">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="365fd-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-184">серверами</span><span class="sxs-lookup"><span data-stu-id="365fd-184">servers</span></span>|<span data-ttu-id="365fd-185">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="365fd-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="365fd-186">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="365fd-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="365fd-187">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="365fd-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="365fd-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="365fd-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="365fd-189">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="365fd-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-190">customXml</span><span class="sxs-lookup"><span data-stu-id="365fd-190">customXml</span></span>|<span data-ttu-id="365fd-191">Binary</span><span class="sxs-lookup"><span data-stu-id="365fd-191">Binary</span></span>|<span data-ttu-id="365fd-192">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="365fd-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="365fd-193">(Массив байтов в кодировке UTF8) Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="365fd-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-194">Профилетаржет</span><span class="sxs-lookup"><span data-stu-id="365fd-194">profileTarget</span></span>|[<span data-ttu-id="365fd-195">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="365fd-195">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="365fd-196">Тип целевого объекта профиля.</span><span class="sxs-lookup"><span data-stu-id="365fd-196">Profile target type.</span></span> <span data-ttu-id="365fd-197">Возможные значения: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="365fd-197">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="365fd-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="365fd-198">connectionType</span></span>|[<span data-ttu-id="365fd-199">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="365fd-199">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="365fd-200">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="365fd-200">Connection type.</span></span> <span data-ttu-id="365fd-201">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="365fd-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="365fd-202">Енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="365fd-202">enableSplitTunneling</span></span>|<span data-ttu-id="365fd-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="365fd-203">Boolean</span></span>|<span data-ttu-id="365fd-204">Включение Расщепленного туннелирования.</span><span class="sxs-lookup"><span data-stu-id="365fd-204">Enable split tunneling.</span></span>|
|<span data-ttu-id="365fd-205">Енаблеалвайсон</span><span class="sxs-lookup"><span data-stu-id="365fd-205">enableAlwaysOn</span></span>|<span data-ttu-id="365fd-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="365fd-206">Boolean</span></span>|<span data-ttu-id="365fd-207">Включение режима "всегда включено".</span><span class="sxs-lookup"><span data-stu-id="365fd-207">Enable Always On mode.</span></span>|
|<span data-ttu-id="365fd-208">Енабледевицетуннел</span><span class="sxs-lookup"><span data-stu-id="365fd-208">enableDeviceTunnel</span></span>|<span data-ttu-id="365fd-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="365fd-209">Boolean</span></span>|<span data-ttu-id="365fd-210">Включите туннель устройства.</span><span class="sxs-lookup"><span data-stu-id="365fd-210">Enable device tunnel.</span></span>|
|<span data-ttu-id="365fd-211">Енабледнсрегистратион</span><span class="sxs-lookup"><span data-stu-id="365fd-211">enableDnsRegistration</span></span>|<span data-ttu-id="365fd-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="365fd-212">Boolean</span></span>|<span data-ttu-id="365fd-213">Включить регистрацию IP-адресов с использованием внутренней DNS.</span><span class="sxs-lookup"><span data-stu-id="365fd-213">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="365fd-214">Днссуффиксес</span><span class="sxs-lookup"><span data-stu-id="365fd-214">dnsSuffixes</span></span>|<span data-ttu-id="365fd-215">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="365fd-215">String collection</span></span>|<span data-ttu-id="365fd-216">Укажите DNS-суффиксы, которые необходимо добавить в список поиска DNS, чтобы правильно маршрутизировать короткие имена.</span><span class="sxs-lookup"><span data-stu-id="365fd-216">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="365fd-217">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="365fd-217">authenticationMethod</span></span>|[<span data-ttu-id="365fd-218">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="365fd-218">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="365fd-219">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="365fd-219">Authentication method.</span></span> <span data-ttu-id="365fd-220">Возможные значения: `certificate`, `usernameAndPassword`, `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="365fd-220">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="365fd-221">Ремемберусеркредентиалс</span><span class="sxs-lookup"><span data-stu-id="365fd-221">rememberUserCredentials</span></span>|<span data-ttu-id="365fd-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="365fd-222">Boolean</span></span>|<span data-ttu-id="365fd-223">Запомнить учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="365fd-223">Remember user credentials.</span></span>|
|<span data-ttu-id="365fd-224">Енаблекондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="365fd-224">enableConditionalAccess</span></span>|<span data-ttu-id="365fd-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="365fd-225">Boolean</span></span>|<span data-ttu-id="365fd-226">Включение условного доступа.</span><span class="sxs-lookup"><span data-stu-id="365fd-226">Enable conditional access.</span></span>|
|<span data-ttu-id="365fd-227">Енаблесинглесигнонвисалтернатецертификате</span><span class="sxs-lookup"><span data-stu-id="365fd-227">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="365fd-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="365fd-228">Boolean</span></span>|<span data-ttu-id="365fd-229">Включите единый вход (SSO) с альтернативным сертификатом.</span><span class="sxs-lookup"><span data-stu-id="365fd-229">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="365fd-230">Синглесигнонеку</span><span class="sxs-lookup"><span data-stu-id="365fd-230">singleSignOnEku</span></span>|[<span data-ttu-id="365fd-231">Екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="365fd-231">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="365fd-232">Расширенное использование ключа (EKU) единого входа.</span><span class="sxs-lookup"><span data-stu-id="365fd-232">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="365fd-233">Синглесигнониссуерхаш</span><span class="sxs-lookup"><span data-stu-id="365fd-233">singleSignOnIssuerHash</span></span>|<span data-ttu-id="365fd-234">String</span><span class="sxs-lookup"><span data-stu-id="365fd-234">String</span></span>|<span data-ttu-id="365fd-235">Хэш поставщика единого входа.</span><span class="sxs-lookup"><span data-stu-id="365fd-235">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="365fd-236">Еапксмл</span><span class="sxs-lookup"><span data-stu-id="365fd-236">eapXml</span></span>|<span data-ttu-id="365fd-237">Binary</span><span class="sxs-lookup"><span data-stu-id="365fd-237">Binary</span></span>|<span data-ttu-id="365fd-238">XML-файл протокола расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="365fd-238">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="365fd-239">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="365fd-239">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="365fd-240">проксисервер</span><span class="sxs-lookup"><span data-stu-id="365fd-240">proxyServer</span></span>|[<span data-ttu-id="365fd-241">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="365fd-241">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="365fd-242">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="365fd-242">Proxy Server.</span></span>|
|<span data-ttu-id="365fd-243">АссоЦиатедаппс</span><span class="sxs-lookup"><span data-stu-id="365fd-243">associatedApps</span></span>|<span data-ttu-id="365fd-244">Коллекция [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="365fd-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="365fd-245">Связанные приложения.</span><span class="sxs-lookup"><span data-stu-id="365fd-245">Associated Apps.</span></span> <span data-ttu-id="365fd-246">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="365fd-246">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="365fd-247">ОнляссоЦиатедаппсканусеконнектион</span><span class="sxs-lookup"><span data-stu-id="365fd-247">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="365fd-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="365fd-248">Boolean</span></span>|<span data-ttu-id="365fd-249">Подключение можно использовать только для связанных приложений (VPN для каждого приложения).</span><span class="sxs-lookup"><span data-stu-id="365fd-249">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="365fd-250">Виндовсинформатионпротектиондомаин</span><span class="sxs-lookup"><span data-stu-id="365fd-250">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="365fd-251">String</span><span class="sxs-lookup"><span data-stu-id="365fd-251">String</span></span>|<span data-ttu-id="365fd-252">Домен Windows Information Protection (WIP) для связи с этим подключением.</span><span class="sxs-lookup"><span data-stu-id="365fd-252">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="365fd-253">Траффикрулес</span><span class="sxs-lookup"><span data-stu-id="365fd-253">trafficRules</span></span>|<span data-ttu-id="365fd-254">Коллекция [впнтраффикруле](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="365fd-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="365fd-255">Правила трафика.</span><span class="sxs-lookup"><span data-stu-id="365fd-255">Traffic rules.</span></span> <span data-ttu-id="365fd-256">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="365fd-256">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="365fd-257">сылает</span><span class="sxs-lookup"><span data-stu-id="365fd-257">routes</span></span>|<span data-ttu-id="365fd-258">Коллекция [впнрауте](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="365fd-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="365fd-259">Маршруты (необязательно для сторонних поставщиков).</span><span class="sxs-lookup"><span data-stu-id="365fd-259">Routes (optional for third-party providers).</span></span> <span data-ttu-id="365fd-260">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="365fd-260">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="365fd-261">Днсрулес</span><span class="sxs-lookup"><span data-stu-id="365fd-261">dnsRules</span></span>|<span data-ttu-id="365fd-262">Коллекция [впнднсруле](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="365fd-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="365fd-263">Правила DNS.</span><span class="sxs-lookup"><span data-stu-id="365fd-263">DNS rules.</span></span> <span data-ttu-id="365fd-264">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="365fd-264">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="365fd-265">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="365fd-265">trustedNetworkDomains</span></span>|<span data-ttu-id="365fd-266">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="365fd-266">String collection</span></span>|<span data-ttu-id="365fd-267">Доверенные сетевые домены</span><span class="sxs-lookup"><span data-stu-id="365fd-267">Trusted Network Domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="365fd-268">Отношения</span><span class="sxs-lookup"><span data-stu-id="365fd-268">Relationships</span></span>
|<span data-ttu-id="365fd-269">Отношение</span><span class="sxs-lookup"><span data-stu-id="365fd-269">Relationship</span></span>|<span data-ttu-id="365fd-270">Тип</span><span class="sxs-lookup"><span data-stu-id="365fd-270">Type</span></span>|<span data-ttu-id="365fd-271">Описание</span><span class="sxs-lookup"><span data-stu-id="365fd-271">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="365fd-272">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="365fd-272">groupAssignments</span></span>|<span data-ttu-id="365fd-273">Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="365fd-273">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="365fd-274">Список назначений групп для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="365fd-274">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="365fd-275">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-275">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-276">assignments</span><span class="sxs-lookup"><span data-stu-id="365fd-276">assignments</span></span>|<span data-ttu-id="365fd-277">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="365fd-277">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="365fd-278">Список назначений для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="365fd-278">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="365fd-279">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-279">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-280">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="365fd-280">deviceStatuses</span></span>|<span data-ttu-id="365fd-281">Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="365fd-281">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="365fd-282">Состояние установки конфигурации для каждого устройства.</span><span class="sxs-lookup"><span data-stu-id="365fd-282">Device configuration installation status by device.</span></span> <span data-ttu-id="365fd-283">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-283">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-284">userStatuses</span><span class="sxs-lookup"><span data-stu-id="365fd-284">userStatuses</span></span>|<span data-ttu-id="365fd-285">Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="365fd-285">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="365fd-286">Состояние установки конфигурации устройств пользователем.</span><span class="sxs-lookup"><span data-stu-id="365fd-286">Device configuration installation status by user.</span></span> <span data-ttu-id="365fd-287">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-287">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-288">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="365fd-288">deviceStatusOverview</span></span>|[<span data-ttu-id="365fd-289">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="365fd-289">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="365fd-290">Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-290">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-291">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="365fd-291">userStatusOverview</span></span>|[<span data-ttu-id="365fd-292">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="365fd-292">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="365fd-293">Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-293">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-294">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="365fd-294">deviceSettingStateSummaries</span></span>|<span data-ttu-id="365fd-295">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="365fd-295">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="365fd-296">Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="365fd-296">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="365fd-297">Identitycertificate (</span><span class="sxs-lookup"><span data-stu-id="365fd-297">identityCertificate</span></span>|[<span data-ttu-id="365fd-298">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="365fd-298">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="365fd-299">Сертификат удостоверения для проверки подлинности клиента при использовании метода проверки подлинности Certificate.</span><span class="sxs-lookup"><span data-stu-id="365fd-299">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="365fd-300">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="365fd-300">JSON Representation</span></span>
<span data-ttu-id="365fd-301">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="365fd-301">Here is a JSON representation of the resource.</span></span>
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
  ]
}
```





