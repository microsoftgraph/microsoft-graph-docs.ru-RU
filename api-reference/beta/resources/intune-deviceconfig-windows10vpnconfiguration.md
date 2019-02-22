---
title: Тип ресурса windows10VpnConfiguration
description: Предоставляя конфигурации в этом профиле, вы можете указать устройству Windows 10 (настольный или мобильный) подключаться к необходимой конечной точке VPN. Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, вы можете сделать VPN-подключение неполноценным для конечного пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4b1b906fc4a98895acc6e23a4b3e9a4d78ff28a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148715"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="08f1d-104">Тип ресурса windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="08f1d-104">windows10VpnConfiguration resource type</span></span>

> <span data-ttu-id="08f1d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08f1d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08f1d-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08f1d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08f1d-107">Предоставляя конфигурации в этом профиле, вы можете указать устройству Windows 10 (настольный или мобильный) подключаться к необходимой конечной точке VPN.</span><span class="sxs-lookup"><span data-stu-id="08f1d-107">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="08f1d-108">Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, вы можете сделать VPN-подключение неполноценным для конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="08f1d-108">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="08f1d-109">НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08f1d-109">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="08f1d-110">Методы</span><span class="sxs-lookup"><span data-stu-id="08f1d-110">Methods</span></span>
|<span data-ttu-id="08f1d-111">Метод</span><span class="sxs-lookup"><span data-stu-id="08f1d-111">Method</span></span>|<span data-ttu-id="08f1d-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="08f1d-112">Return Type</span></span>|<span data-ttu-id="08f1d-113">Описание</span><span class="sxs-lookup"><span data-stu-id="08f1d-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="08f1d-114">Список windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="08f1d-114">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="08f1d-115">Коллекция [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08f1d-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="08f1d-116">Список свойств и связей объектов [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="08f1d-116">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="08f1d-117">Получение windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="08f1d-117">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="08f1d-118">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="08f1d-118">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="08f1d-119">Чтение свойств и связей объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="08f1d-119">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="08f1d-120">Создание windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="08f1d-120">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="08f1d-121">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="08f1d-121">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="08f1d-122">Создание нового объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="08f1d-122">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="08f1d-123">Удаление windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="08f1d-123">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="08f1d-124">Нет</span><span class="sxs-lookup"><span data-stu-id="08f1d-124">None</span></span>|<span data-ttu-id="08f1d-125">Удаляет объект [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08f1d-125">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="08f1d-126">Обновление windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="08f1d-126">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="08f1d-127">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="08f1d-127">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="08f1d-128">Обновление свойств объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="08f1d-128">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="08f1d-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="08f1d-129">Properties</span></span>
|<span data-ttu-id="08f1d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="08f1d-130">Property</span></span>|<span data-ttu-id="08f1d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="08f1d-131">Type</span></span>|<span data-ttu-id="08f1d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="08f1d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08f1d-133">id</span><span class="sxs-lookup"><span data-stu-id="08f1d-133">id</span></span>|<span data-ttu-id="08f1d-134">String</span><span class="sxs-lookup"><span data-stu-id="08f1d-134">String</span></span>|<span data-ttu-id="08f1d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="08f1d-135">Key of the entity.</span></span> <span data-ttu-id="08f1d-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08f1d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f1d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08f1d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="08f1d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08f1d-138">DateTimeOffset</span></span>|<span data-ttu-id="08f1d-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="08f1d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="08f1d-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08f1d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f1d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="08f1d-141">roleScopeTagIds</span></span>|<span data-ttu-id="08f1d-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="08f1d-142">String collection</span></span>|<span data-ttu-id="08f1d-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="08f1d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="08f1d-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08f1d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f1d-145">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="08f1d-145">supportsScopeTags</span></span>|<span data-ttu-id="08f1d-146">Логический</span><span class="sxs-lookup"><span data-stu-id="08f1d-146">Boolean</span></span>|<span data-ttu-id="08f1d-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="08f1d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="08f1d-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="08f1d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="08f1d-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="08f1d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="08f1d-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08f1d-150">This property is read-only.</span></span> <span data-ttu-id="08f1d-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08f1d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f1d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08f1d-152">createdDateTime</span></span>|<span data-ttu-id="08f1d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08f1d-153">DateTimeOffset</span></span>|<span data-ttu-id="08f1d-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="08f1d-154">DateTime the object was created.</span></span> <span data-ttu-id="08f1d-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08f1d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f1d-156">description</span><span class="sxs-lookup"><span data-stu-id="08f1d-156">description</span></span>|<span data-ttu-id="08f1d-157">String</span><span class="sxs-lookup"><span data-stu-id="08f1d-157">String</span></span>|<span data-ttu-id="08f1d-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="08f1d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="08f1d-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08f1d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f1d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="08f1d-160">displayName</span></span>|<span data-ttu-id="08f1d-161">String</span><span class="sxs-lookup"><span data-stu-id="08f1d-161">String</span></span>|<span data-ttu-id="08f1d-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="08f1d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="08f1d-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08f1d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f1d-164">version</span><span class="sxs-lookup"><span data-stu-id="08f1d-164">version</span></span>|<span data-ttu-id="08f1d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="08f1d-165">Int32</span></span>|<span data-ttu-id="08f1d-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="08f1d-166">Version of the device configuration.</span></span> <span data-ttu-id="08f1d-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08f1d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f1d-168">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="08f1d-168">connectionName</span></span>|<span data-ttu-id="08f1d-169">String</span><span class="sxs-lookup"><span data-stu-id="08f1d-169">String</span></span>|<span data-ttu-id="08f1d-170">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="08f1d-170">Connection name displayed to the user.</span></span> <span data-ttu-id="08f1d-171">НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08f1d-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="08f1d-172">серверы</span><span class="sxs-lookup"><span data-stu-id="08f1d-172">servers</span></span>|<span data-ttu-id="08f1d-173">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="08f1d-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="08f1d-174">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="08f1d-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="08f1d-175">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="08f1d-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="08f1d-176">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="08f1d-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="08f1d-177">НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08f1d-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="08f1d-178">customXml</span><span class="sxs-lookup"><span data-stu-id="08f1d-178">customXml</span></span>|<span data-ttu-id="08f1d-179">Binary</span><span class="sxs-lookup"><span data-stu-id="08f1d-179">Binary</span></span>|<span data-ttu-id="08f1d-180">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="08f1d-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="08f1d-181">(Массив байтов в кодировке UTF8) НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08f1d-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="08f1d-182">Профилетаржет</span><span class="sxs-lookup"><span data-stu-id="08f1d-182">profileTarget</span></span>|[<span data-ttu-id="08f1d-183">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="08f1d-183">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="08f1d-184">Тип целевого объекта профиля.</span><span class="sxs-lookup"><span data-stu-id="08f1d-184">Profile target type.</span></span> <span data-ttu-id="08f1d-185">Возможные значения: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="08f1d-185">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="08f1d-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="08f1d-186">connectionType</span></span>|[<span data-ttu-id="08f1d-187">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="08f1d-187">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="08f1d-188">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="08f1d-188">Connection type.</span></span> <span data-ttu-id="08f1d-189">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="08f1d-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="08f1d-190">Енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="08f1d-190">enableSplitTunneling</span></span>|<span data-ttu-id="08f1d-191">Логический</span><span class="sxs-lookup"><span data-stu-id="08f1d-191">Boolean</span></span>|<span data-ttu-id="08f1d-192">Включение Расщепленного туннелирования.</span><span class="sxs-lookup"><span data-stu-id="08f1d-192">Enable split tunneling.</span></span>|
|<span data-ttu-id="08f1d-193">Енаблеалвайсон</span><span class="sxs-lookup"><span data-stu-id="08f1d-193">enableAlwaysOn</span></span>|<span data-ttu-id="08f1d-194">Логический</span><span class="sxs-lookup"><span data-stu-id="08f1d-194">Boolean</span></span>|<span data-ttu-id="08f1d-195">Включение режима "всегда включено".</span><span class="sxs-lookup"><span data-stu-id="08f1d-195">Enable Always On mode.</span></span>|
|<span data-ttu-id="08f1d-196">Енабледевицетуннел</span><span class="sxs-lookup"><span data-stu-id="08f1d-196">enableDeviceTunnel</span></span>|<span data-ttu-id="08f1d-197">Логический</span><span class="sxs-lookup"><span data-stu-id="08f1d-197">Boolean</span></span>|<span data-ttu-id="08f1d-198">Включите туннель устройства.</span><span class="sxs-lookup"><span data-stu-id="08f1d-198">Enable device tunnel.</span></span>|
|<span data-ttu-id="08f1d-199">Енабледнсрегистратион</span><span class="sxs-lookup"><span data-stu-id="08f1d-199">enableDnsRegistration</span></span>|<span data-ttu-id="08f1d-200">Логический</span><span class="sxs-lookup"><span data-stu-id="08f1d-200">Boolean</span></span>|<span data-ttu-id="08f1d-201">Включить регистрацию IP-адресов с использованием внутренней DNS.</span><span class="sxs-lookup"><span data-stu-id="08f1d-201">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="08f1d-202">Днссуффиксес</span><span class="sxs-lookup"><span data-stu-id="08f1d-202">dnsSuffixes</span></span>|<span data-ttu-id="08f1d-203">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="08f1d-203">String collection</span></span>|<span data-ttu-id="08f1d-204">Укажите DNS-суффиксы, которые необходимо добавить в список поиска DNS, чтобы правильно маршрутизировать короткие имена.</span><span class="sxs-lookup"><span data-stu-id="08f1d-204">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="08f1d-205">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="08f1d-205">authenticationMethod</span></span>|[<span data-ttu-id="08f1d-206">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="08f1d-206">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="08f1d-207">Метод проверки поДлинности.</span><span class="sxs-lookup"><span data-stu-id="08f1d-207">Authentication method.</span></span> <span data-ttu-id="08f1d-208">Возможные значения: `certificate`, `usernameAndPassword`, `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="08f1d-208">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="08f1d-209">Ремемберусеркредентиалс</span><span class="sxs-lookup"><span data-stu-id="08f1d-209">rememberUserCredentials</span></span>|<span data-ttu-id="08f1d-210">Логический</span><span class="sxs-lookup"><span data-stu-id="08f1d-210">Boolean</span></span>|<span data-ttu-id="08f1d-211">Запомнить учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="08f1d-211">Remember user credentials.</span></span>|
|<span data-ttu-id="08f1d-212">Енаблекондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="08f1d-212">enableConditionalAccess</span></span>|<span data-ttu-id="08f1d-213">Логический</span><span class="sxs-lookup"><span data-stu-id="08f1d-213">Boolean</span></span>|<span data-ttu-id="08f1d-214">Включение условного доступа.</span><span class="sxs-lookup"><span data-stu-id="08f1d-214">Enable conditional access.</span></span>|
|<span data-ttu-id="08f1d-215">Енаблесинглесигнонвисалтернатецертификате</span><span class="sxs-lookup"><span data-stu-id="08f1d-215">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="08f1d-216">Логический</span><span class="sxs-lookup"><span data-stu-id="08f1d-216">Boolean</span></span>|<span data-ttu-id="08f1d-217">Включите единый вход (SSO) с альтернативным сертификатом.</span><span class="sxs-lookup"><span data-stu-id="08f1d-217">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="08f1d-218">Синглесигнонеку</span><span class="sxs-lookup"><span data-stu-id="08f1d-218">singleSignOnEku</span></span>|[<span data-ttu-id="08f1d-219">Екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="08f1d-219">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="08f1d-220">Расширенное использование ключа (EKU) единого входа.</span><span class="sxs-lookup"><span data-stu-id="08f1d-220">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="08f1d-221">Синглесигнониссуерхаш</span><span class="sxs-lookup"><span data-stu-id="08f1d-221">singleSignOnIssuerHash</span></span>|<span data-ttu-id="08f1d-222">String</span><span class="sxs-lookup"><span data-stu-id="08f1d-222">String</span></span>|<span data-ttu-id="08f1d-223">Хэш поставщика единого входа.</span><span class="sxs-lookup"><span data-stu-id="08f1d-223">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="08f1d-224">Еапксмл</span><span class="sxs-lookup"><span data-stu-id="08f1d-224">eapXml</span></span>|<span data-ttu-id="08f1d-225">Binary</span><span class="sxs-lookup"><span data-stu-id="08f1d-225">Binary</span></span>|<span data-ttu-id="08f1d-226">XML-файл протокола расширенной проверки поДлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="08f1d-226">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="08f1d-227">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="08f1d-227">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="08f1d-228">проксисервер</span><span class="sxs-lookup"><span data-stu-id="08f1d-228">proxyServer</span></span>|[<span data-ttu-id="08f1d-229">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="08f1d-229">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="08f1d-230">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="08f1d-230">Proxy Server.</span></span>|
|<span data-ttu-id="08f1d-231">АссоЦиатедаппс</span><span class="sxs-lookup"><span data-stu-id="08f1d-231">associatedApps</span></span>|<span data-ttu-id="08f1d-232">Коллекция [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="08f1d-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="08f1d-233">Связанные приложения.</span><span class="sxs-lookup"><span data-stu-id="08f1d-233">Associated Apps.</span></span> <span data-ttu-id="08f1d-234">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="08f1d-234">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="08f1d-235">ОнляссоЦиатедаппсканусеконнектион</span><span class="sxs-lookup"><span data-stu-id="08f1d-235">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="08f1d-236">Логический</span><span class="sxs-lookup"><span data-stu-id="08f1d-236">Boolean</span></span>|<span data-ttu-id="08f1d-237">Подключение можно использовать только для связанных приложений (VPN для каждого приложения).</span><span class="sxs-lookup"><span data-stu-id="08f1d-237">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="08f1d-238">Виндовсинформатионпротектиондомаин</span><span class="sxs-lookup"><span data-stu-id="08f1d-238">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="08f1d-239">String</span><span class="sxs-lookup"><span data-stu-id="08f1d-239">String</span></span>|<span data-ttu-id="08f1d-240">Домен Windows Information Protection (WIP) для связи с этим подключением.</span><span class="sxs-lookup"><span data-stu-id="08f1d-240">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="08f1d-241">Траффикрулес</span><span class="sxs-lookup"><span data-stu-id="08f1d-241">trafficRules</span></span>|<span data-ttu-id="08f1d-242">Коллекция [впнтраффикруле](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="08f1d-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="08f1d-243">Правила трафика.</span><span class="sxs-lookup"><span data-stu-id="08f1d-243">Traffic rules.</span></span> <span data-ttu-id="08f1d-244">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="08f1d-244">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="08f1d-245">сылает</span><span class="sxs-lookup"><span data-stu-id="08f1d-245">routes</span></span>|<span data-ttu-id="08f1d-246">Коллекция [впнрауте](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="08f1d-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="08f1d-247">Маршруты (необязательно для сторонних поставщиков).</span><span class="sxs-lookup"><span data-stu-id="08f1d-247">Routes (optional for third-party providers).</span></span> <span data-ttu-id="08f1d-248">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="08f1d-248">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="08f1d-249">Днсрулес</span><span class="sxs-lookup"><span data-stu-id="08f1d-249">dnsRules</span></span>|<span data-ttu-id="08f1d-250">Коллекция [впнднсруле](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="08f1d-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="08f1d-251">Правила DNS.</span><span class="sxs-lookup"><span data-stu-id="08f1d-251">DNS rules.</span></span> <span data-ttu-id="08f1d-252">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="08f1d-252">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="08f1d-253">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="08f1d-253">trustedNetworkDomains</span></span>|<span data-ttu-id="08f1d-254">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="08f1d-254">String collection</span></span>|<span data-ttu-id="08f1d-255">Доверенные сетевые домены</span><span class="sxs-lookup"><span data-stu-id="08f1d-255">Trusted Network Domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="08f1d-256">Отношения</span><span class="sxs-lookup"><span data-stu-id="08f1d-256">Relationships</span></span>
|<span data-ttu-id="08f1d-257">Связь</span><span class="sxs-lookup"><span data-stu-id="08f1d-257">Relationship</span></span>|<span data-ttu-id="08f1d-258">Тип</span><span class="sxs-lookup"><span data-stu-id="08f1d-258">Type</span></span>|<span data-ttu-id="08f1d-259">Описание</span><span class="sxs-lookup"><span data-stu-id="08f1d-259">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08f1d-260">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="08f1d-260">groupAssignments</span></span>|<span data-ttu-id="08f1d-261">Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="08f1d-261">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="08f1d-262">Список назначений групп для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="08f1d-262">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="08f1d-263">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08f1d-263">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f1d-264">assignments</span><span class="sxs-lookup"><span data-stu-id="08f1d-264">assignments</span></span>|<span data-ttu-id="08f1d-265">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="08f1d-265">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="08f1d-266">Список назначений для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="08f1d-266">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="08f1d-267">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08f1d-267">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f1d-268">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="08f1d-268">deviceStatuses</span></span>|<span data-ttu-id="08f1d-269">Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="08f1d-269">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="08f1d-270">Состояние установки конфигурации для каждого устройства.</span><span class="sxs-lookup"><span data-stu-id="08f1d-270">Device configuration installation status by device.</span></span> <span data-ttu-id="08f1d-271">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08f1d-271">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f1d-272">userStatuses</span><span class="sxs-lookup"><span data-stu-id="08f1d-272">userStatuses</span></span>|<span data-ttu-id="08f1d-273">Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="08f1d-273">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="08f1d-274">Состояние установки конфигурации устройств пользователем.</span><span class="sxs-lookup"><span data-stu-id="08f1d-274">Device configuration installation status by user.</span></span> <span data-ttu-id="08f1d-275">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="08f1d-275">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f1d-276">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="08f1d-276">deviceStatusOverview</span></span>|[<span data-ttu-id="08f1d-277">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="08f1d-277">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="08f1d-278">Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08f1d-278">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f1d-279">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="08f1d-279">userStatusOverview</span></span>|[<span data-ttu-id="08f1d-280">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="08f1d-280">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="08f1d-281">Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08f1d-281">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f1d-282">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="08f1d-282">deviceSettingStateSummaries</span></span>|<span data-ttu-id="08f1d-283">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="08f1d-283">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="08f1d-284">Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08f1d-284">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f1d-285">Identitycertificate (</span><span class="sxs-lookup"><span data-stu-id="08f1d-285">identityCertificate</span></span>|[<span data-ttu-id="08f1d-286">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="08f1d-286">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="08f1d-287">Сертификат удостоверения для проверки подлинности клиента при использовании метода проверки подлинности Certificate.</span><span class="sxs-lookup"><span data-stu-id="08f1d-287">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08f1d-288">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08f1d-288">JSON Representation</span></span>
<span data-ttu-id="08f1d-289">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08f1d-289">Here is a JSON representation of the resource.</span></span>
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




