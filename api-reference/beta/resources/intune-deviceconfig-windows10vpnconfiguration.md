---
title: Тип ресурса windows10VpnConfiguration
description: Предоставляя конфигурации в этом профиле, вы можете указать устройству Windows 10 (настольный или мобильный) подключаться к необходимой конечной точке VPN. Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, вы можете сделать VPN-подключение неполноценным для конечного пользователя.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b51d85a894a07ab62f31ceab51bc222e42fa7b50
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122513"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="8175f-104">Тип ресурса windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8175f-104">windows10VpnConfiguration resource type</span></span>

<span data-ttu-id="8175f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8175f-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8175f-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8175f-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8175f-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8175f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8175f-108">Предоставляя конфигурации в этом профиле, вы можете указать устройству Windows 10 (настольный или мобильный) подключаться к необходимой конечной точке VPN.</span><span class="sxs-lookup"><span data-stu-id="8175f-108">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="8175f-109">Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, вы можете сделать VPN-подключение неполноценным для конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="8175f-109">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="8175f-110">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8175f-110">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="8175f-111">Методы</span><span class="sxs-lookup"><span data-stu-id="8175f-111">Methods</span></span>
|<span data-ttu-id="8175f-112">Метод</span><span class="sxs-lookup"><span data-stu-id="8175f-112">Method</span></span>|<span data-ttu-id="8175f-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8175f-113">Return Type</span></span>|<span data-ttu-id="8175f-114">Описание</span><span class="sxs-lookup"><span data-stu-id="8175f-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8175f-115">Список windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="8175f-115">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="8175f-116">Коллекция [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8175f-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="8175f-117">Список свойств и связей объектов [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8175f-117">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="8175f-118">Получение windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8175f-118">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="8175f-119">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8175f-119">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="8175f-120">Чтение свойств и связей объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8175f-120">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="8175f-121">Создание windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8175f-121">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="8175f-122">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8175f-122">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="8175f-123">Создание нового объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8175f-123">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="8175f-124">Удаление windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8175f-124">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="8175f-125">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="8175f-125">None</span></span>|<span data-ttu-id="8175f-126">Удаляет объект [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-126">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="8175f-127">Обновление windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8175f-127">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="8175f-128">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8175f-128">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="8175f-129">Обновление свойств объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8175f-129">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8175f-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="8175f-130">Properties</span></span>
|<span data-ttu-id="8175f-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="8175f-131">Property</span></span>|<span data-ttu-id="8175f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8175f-132">Type</span></span>|<span data-ttu-id="8175f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8175f-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8175f-134">id</span><span class="sxs-lookup"><span data-stu-id="8175f-134">id</span></span>|<span data-ttu-id="8175f-135">String</span><span class="sxs-lookup"><span data-stu-id="8175f-135">String</span></span>|<span data-ttu-id="8175f-136">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8175f-136">Key of the entity.</span></span> <span data-ttu-id="8175f-137">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-137">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8175f-138">lastModifiedDateTime</span></span>|<span data-ttu-id="8175f-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8175f-139">DateTimeOffset</span></span>|<span data-ttu-id="8175f-140">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8175f-140">DateTime the object was last modified.</span></span> <span data-ttu-id="8175f-141">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-141">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8175f-142">roleScopeTagIds</span></span>|<span data-ttu-id="8175f-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8175f-143">String collection</span></span>|<span data-ttu-id="8175f-144">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8175f-144">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8175f-145">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-146">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="8175f-146">supportsScopeTags</span></span>|<span data-ttu-id="8175f-147">Логический</span><span class="sxs-lookup"><span data-stu-id="8175f-147">Boolean</span></span>|<span data-ttu-id="8175f-148">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8175f-148">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8175f-149">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="8175f-149">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8175f-150">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8175f-150">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8175f-151">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8175f-151">This property is read-only.</span></span> <span data-ttu-id="8175f-152">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-152">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8175f-153">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8175f-154">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8175f-154">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8175f-155">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8175f-155">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8175f-156">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-156">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8175f-157">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8175f-158">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8175f-158">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8175f-159">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8175f-159">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8175f-160">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-160">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8175f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8175f-162">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8175f-162">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8175f-163">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8175f-163">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8175f-164">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-164">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-165">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8175f-165">createdDateTime</span></span>|<span data-ttu-id="8175f-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8175f-166">DateTimeOffset</span></span>|<span data-ttu-id="8175f-167">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8175f-167">DateTime the object was created.</span></span> <span data-ttu-id="8175f-168">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-168">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-169">description</span><span class="sxs-lookup"><span data-stu-id="8175f-169">description</span></span>|<span data-ttu-id="8175f-170">String</span><span class="sxs-lookup"><span data-stu-id="8175f-170">String</span></span>|<span data-ttu-id="8175f-171">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8175f-171">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8175f-172">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-172">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-173">displayName</span><span class="sxs-lookup"><span data-stu-id="8175f-173">displayName</span></span>|<span data-ttu-id="8175f-174">Строка</span><span class="sxs-lookup"><span data-stu-id="8175f-174">String</span></span>|<span data-ttu-id="8175f-175">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8175f-175">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8175f-176">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-176">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-177">version</span><span class="sxs-lookup"><span data-stu-id="8175f-177">version</span></span>|<span data-ttu-id="8175f-178">Int32</span><span class="sxs-lookup"><span data-stu-id="8175f-178">Int32</span></span>|<span data-ttu-id="8175f-179">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8175f-179">Version of the device configuration.</span></span> <span data-ttu-id="8175f-180">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-180">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-181">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="8175f-181">connectionName</span></span>|<span data-ttu-id="8175f-182">String</span><span class="sxs-lookup"><span data-stu-id="8175f-182">String</span></span>|<span data-ttu-id="8175f-183">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8175f-183">Connection name displayed to the user.</span></span> <span data-ttu-id="8175f-184">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8175f-184">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-185">серверами</span><span class="sxs-lookup"><span data-stu-id="8175f-185">servers</span></span>|<span data-ttu-id="8175f-186">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="8175f-186">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="8175f-187">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="8175f-187">List of VPN Servers on the network.</span></span> <span data-ttu-id="8175f-188">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="8175f-188">Make sure end users can access these network locations.</span></span> <span data-ttu-id="8175f-189">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="8175f-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="8175f-190">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8175f-190">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-191">customXml</span><span class="sxs-lookup"><span data-stu-id="8175f-191">customXml</span></span>|<span data-ttu-id="8175f-192">Binary</span><span class="sxs-lookup"><span data-stu-id="8175f-192">Binary</span></span>|<span data-ttu-id="8175f-193">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="8175f-193">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="8175f-194">(Массив байтов в кодировке UTF8) Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8175f-194">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-195">профилетаржет</span><span class="sxs-lookup"><span data-stu-id="8175f-195">profileTarget</span></span>|[<span data-ttu-id="8175f-196">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="8175f-196">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="8175f-197">Тип целевого объекта профиля.</span><span class="sxs-lookup"><span data-stu-id="8175f-197">Profile target type.</span></span> <span data-ttu-id="8175f-198">Возможные значения: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="8175f-198">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="8175f-199">connectionType</span><span class="sxs-lookup"><span data-stu-id="8175f-199">connectionType</span></span>|[<span data-ttu-id="8175f-200">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="8175f-200">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="8175f-201">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="8175f-201">Connection type.</span></span> <span data-ttu-id="8175f-202">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="8175f-202">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="8175f-203">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="8175f-203">enableSplitTunneling</span></span>|<span data-ttu-id="8175f-204">Логический</span><span class="sxs-lookup"><span data-stu-id="8175f-204">Boolean</span></span>|<span data-ttu-id="8175f-205">Включение Расщепленного туннелирования.</span><span class="sxs-lookup"><span data-stu-id="8175f-205">Enable split tunneling.</span></span>|
|<span data-ttu-id="8175f-206">енаблеалвайсон</span><span class="sxs-lookup"><span data-stu-id="8175f-206">enableAlwaysOn</span></span>|<span data-ttu-id="8175f-207">Логический</span><span class="sxs-lookup"><span data-stu-id="8175f-207">Boolean</span></span>|<span data-ttu-id="8175f-208">Включение режима "всегда включено".</span><span class="sxs-lookup"><span data-stu-id="8175f-208">Enable Always On mode.</span></span>|
|<span data-ttu-id="8175f-209">енабледевицетуннел</span><span class="sxs-lookup"><span data-stu-id="8175f-209">enableDeviceTunnel</span></span>|<span data-ttu-id="8175f-210">Логический</span><span class="sxs-lookup"><span data-stu-id="8175f-210">Boolean</span></span>|<span data-ttu-id="8175f-211">Включите туннель устройства.</span><span class="sxs-lookup"><span data-stu-id="8175f-211">Enable device tunnel.</span></span>|
|<span data-ttu-id="8175f-212">енабледнсрегистратион</span><span class="sxs-lookup"><span data-stu-id="8175f-212">enableDnsRegistration</span></span>|<span data-ttu-id="8175f-213">Логический</span><span class="sxs-lookup"><span data-stu-id="8175f-213">Boolean</span></span>|<span data-ttu-id="8175f-214">Включить регистрацию IP-адресов с использованием внутренней DNS.</span><span class="sxs-lookup"><span data-stu-id="8175f-214">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="8175f-215">днссуффиксес</span><span class="sxs-lookup"><span data-stu-id="8175f-215">dnsSuffixes</span></span>|<span data-ttu-id="8175f-216">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8175f-216">String collection</span></span>|<span data-ttu-id="8175f-217">Укажите DNS-суффиксы, которые необходимо добавить в список поиска DNS, чтобы правильно маршрутизировать короткие имена.</span><span class="sxs-lookup"><span data-stu-id="8175f-217">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="8175f-218">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="8175f-218">authenticationMethod</span></span>|[<span data-ttu-id="8175f-219">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8175f-219">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="8175f-220">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="8175f-220">Authentication method.</span></span> <span data-ttu-id="8175f-221">Возможные значения: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="8175f-221">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span></span>|
|<span data-ttu-id="8175f-222">ремемберусеркредентиалс</span><span class="sxs-lookup"><span data-stu-id="8175f-222">rememberUserCredentials</span></span>|<span data-ttu-id="8175f-223">Логический</span><span class="sxs-lookup"><span data-stu-id="8175f-223">Boolean</span></span>|<span data-ttu-id="8175f-224">Запомнить учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="8175f-224">Remember user credentials.</span></span>|
|<span data-ttu-id="8175f-225">енаблекондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="8175f-225">enableConditionalAccess</span></span>|<span data-ttu-id="8175f-226">Логический</span><span class="sxs-lookup"><span data-stu-id="8175f-226">Boolean</span></span>|<span data-ttu-id="8175f-227">Включение условного доступа.</span><span class="sxs-lookup"><span data-stu-id="8175f-227">Enable conditional access.</span></span>|
|<span data-ttu-id="8175f-228">енаблесинглесигнонвисалтернатецертификате</span><span class="sxs-lookup"><span data-stu-id="8175f-228">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="8175f-229">Логический</span><span class="sxs-lookup"><span data-stu-id="8175f-229">Boolean</span></span>|<span data-ttu-id="8175f-230">Включите единый вход (SSO) с альтернативным сертификатом.</span><span class="sxs-lookup"><span data-stu-id="8175f-230">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="8175f-231">синглесигнонеку</span><span class="sxs-lookup"><span data-stu-id="8175f-231">singleSignOnEku</span></span>|[<span data-ttu-id="8175f-232">екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="8175f-232">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="8175f-233">Расширенное использование ключа (EKU) единого входа.</span><span class="sxs-lookup"><span data-stu-id="8175f-233">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="8175f-234">синглесигнониссуерхаш</span><span class="sxs-lookup"><span data-stu-id="8175f-234">singleSignOnIssuerHash</span></span>|<span data-ttu-id="8175f-235">String</span><span class="sxs-lookup"><span data-stu-id="8175f-235">String</span></span>|<span data-ttu-id="8175f-236">Хэш поставщика единого входа.</span><span class="sxs-lookup"><span data-stu-id="8175f-236">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="8175f-237">еапксмл</span><span class="sxs-lookup"><span data-stu-id="8175f-237">eapXml</span></span>|<span data-ttu-id="8175f-238">Binary</span><span class="sxs-lookup"><span data-stu-id="8175f-238">Binary</span></span>|<span data-ttu-id="8175f-239">XML-файл протокола расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="8175f-239">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="8175f-240">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="8175f-240">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="8175f-241">проксисервер</span><span class="sxs-lookup"><span data-stu-id="8175f-241">proxyServer</span></span>|[<span data-ttu-id="8175f-242">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="8175f-242">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="8175f-243">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="8175f-243">Proxy Server.</span></span>|
|<span data-ttu-id="8175f-244">ассоЦиатедаппс</span><span class="sxs-lookup"><span data-stu-id="8175f-244">associatedApps</span></span>|<span data-ttu-id="8175f-245">Коллекция [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="8175f-245">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="8175f-246">Связанные приложения.</span><span class="sxs-lookup"><span data-stu-id="8175f-246">Associated Apps.</span></span> <span data-ttu-id="8175f-247">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="8175f-247">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="8175f-248">онляссоЦиатедаппсканусеконнектион</span><span class="sxs-lookup"><span data-stu-id="8175f-248">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="8175f-249">Логический</span><span class="sxs-lookup"><span data-stu-id="8175f-249">Boolean</span></span>|<span data-ttu-id="8175f-250">Подключение можно использовать только для связанных приложений (VPN для каждого приложения).</span><span class="sxs-lookup"><span data-stu-id="8175f-250">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="8175f-251">виндовсинформатионпротектиондомаин</span><span class="sxs-lookup"><span data-stu-id="8175f-251">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="8175f-252">String</span><span class="sxs-lookup"><span data-stu-id="8175f-252">String</span></span>|<span data-ttu-id="8175f-253">Домен Windows Information Protection (WIP) для связи с этим подключением.</span><span class="sxs-lookup"><span data-stu-id="8175f-253">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="8175f-254">траффикрулес</span><span class="sxs-lookup"><span data-stu-id="8175f-254">trafficRules</span></span>|<span data-ttu-id="8175f-255">Коллекция [впнтраффикруле](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="8175f-255">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="8175f-256">Правила трафика.</span><span class="sxs-lookup"><span data-stu-id="8175f-256">Traffic rules.</span></span> <span data-ttu-id="8175f-257">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="8175f-257">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="8175f-258">сылает</span><span class="sxs-lookup"><span data-stu-id="8175f-258">routes</span></span>|<span data-ttu-id="8175f-259">Коллекция [впнрауте](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="8175f-259">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="8175f-260">Маршруты (необязательно для сторонних поставщиков).</span><span class="sxs-lookup"><span data-stu-id="8175f-260">Routes (optional for third-party providers).</span></span> <span data-ttu-id="8175f-261">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="8175f-261">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="8175f-262">днсрулес</span><span class="sxs-lookup"><span data-stu-id="8175f-262">dnsRules</span></span>|<span data-ttu-id="8175f-263">Коллекция [впнднсруле](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="8175f-263">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="8175f-264">Правила DNS.</span><span class="sxs-lookup"><span data-stu-id="8175f-264">DNS rules.</span></span> <span data-ttu-id="8175f-265">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="8175f-265">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="8175f-266">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="8175f-266">trustedNetworkDomains</span></span>|<span data-ttu-id="8175f-267">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8175f-267">String collection</span></span>|<span data-ttu-id="8175f-268">Доверенные сетевые домены</span><span class="sxs-lookup"><span data-stu-id="8175f-268">Trusted Network Domains</span></span>|
|<span data-ttu-id="8175f-269">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="8175f-269">cryptographySuite</span></span>|[<span data-ttu-id="8175f-270">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="8175f-270">cryptographySuite</span></span>](../resources/intune-deviceconfig-cryptographysuite.md)|<span data-ttu-id="8175f-271">Параметры безопасности комплекта шифрования для VPN-подключения по протоколу IKEv2 в Windows10 и более поздних версий</span><span class="sxs-lookup"><span data-stu-id="8175f-271">Cryptography Suite security settings for IKEv2 VPN in Windows10 and above</span></span> |

## <a name="relationships"></a><span data-ttu-id="8175f-272">Связи</span><span class="sxs-lookup"><span data-stu-id="8175f-272">Relationships</span></span>
|<span data-ttu-id="8175f-273">Связь</span><span class="sxs-lookup"><span data-stu-id="8175f-273">Relationship</span></span>|<span data-ttu-id="8175f-274">Тип</span><span class="sxs-lookup"><span data-stu-id="8175f-274">Type</span></span>|<span data-ttu-id="8175f-275">Описание</span><span class="sxs-lookup"><span data-stu-id="8175f-275">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8175f-276">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="8175f-276">groupAssignments</span></span>|<span data-ttu-id="8175f-277">Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8175f-277">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="8175f-278">Список назначений групп для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8175f-278">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="8175f-279">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-279">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-280">assignments</span><span class="sxs-lookup"><span data-stu-id="8175f-280">assignments</span></span>|<span data-ttu-id="8175f-281">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8175f-281">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8175f-282">Список назначений для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8175f-282">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="8175f-283">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-283">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-284">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="8175f-284">deviceStatuses</span></span>|<span data-ttu-id="8175f-285">Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="8175f-285">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="8175f-286">Состояние установки конфигурации для каждого устройства.</span><span class="sxs-lookup"><span data-stu-id="8175f-286">Device configuration installation status by device.</span></span> <span data-ttu-id="8175f-287">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-287">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-288">userStatuses</span><span class="sxs-lookup"><span data-stu-id="8175f-288">userStatuses</span></span>|<span data-ttu-id="8175f-289">Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="8175f-289">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="8175f-290">Состояние установки конфигурации устройств пользователем.</span><span class="sxs-lookup"><span data-stu-id="8175f-290">Device configuration installation status by user.</span></span> <span data-ttu-id="8175f-291">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-291">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-292">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="8175f-292">deviceStatusOverview</span></span>|[<span data-ttu-id="8175f-293">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="8175f-293">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="8175f-294">Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-294">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-295">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="8175f-295">userStatusOverview</span></span>|[<span data-ttu-id="8175f-296">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="8175f-296">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="8175f-297">Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-297">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-298">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="8175f-298">deviceSettingStateSummaries</span></span>|<span data-ttu-id="8175f-299">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="8175f-299">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="8175f-300">Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8175f-300">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8175f-301">Identitycertificate (</span><span class="sxs-lookup"><span data-stu-id="8175f-301">identityCertificate</span></span>|[<span data-ttu-id="8175f-302">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="8175f-302">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="8175f-303">Сертификат удостоверения для проверки подлинности клиента при использовании метода проверки подлинности Certificate.</span><span class="sxs-lookup"><span data-stu-id="8175f-303">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8175f-304">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8175f-304">JSON Representation</span></span>
<span data-ttu-id="8175f-305">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8175f-305">Here is a JSON representation of the resource.</span></span>
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



