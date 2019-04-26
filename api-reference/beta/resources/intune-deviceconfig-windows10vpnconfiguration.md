---
title: Тип ресурса windows10VpnConfiguration
description: Предоставляя конфигурации в этом профиле, вы можете указать устройству Windows 10 (настольный или мобильный) подключаться к необходимой конечной точке VPN. Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, вы можете сделать VPN-подключение неполноценным для конечного пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88d32aedb16516f7659ff6e8094172e4a59f6345
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572019"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="f1889-104">Тип ресурса windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1889-104">windows10VpnConfiguration resource type</span></span>

> <span data-ttu-id="f1889-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1889-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1889-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1889-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1889-107">Предоставляя конфигурации в этом профиле, вы можете указать устройству Windows 10 (настольный или мобильный) подключаться к необходимой конечной точке VPN.</span><span class="sxs-lookup"><span data-stu-id="f1889-107">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="f1889-108">Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, вы можете сделать VPN-подключение неполноценным для конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1889-108">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="f1889-109">НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1889-109">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="f1889-110">Методы</span><span class="sxs-lookup"><span data-stu-id="f1889-110">Methods</span></span>
|<span data-ttu-id="f1889-111">Метод</span><span class="sxs-lookup"><span data-stu-id="f1889-111">Method</span></span>|<span data-ttu-id="f1889-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f1889-112">Return Type</span></span>|<span data-ttu-id="f1889-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f1889-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f1889-114">Список windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="f1889-114">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="f1889-115">Коллекция [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1889-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="f1889-116">Список свойств и связей объектов [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f1889-116">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="f1889-117">Получение windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1889-117">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="f1889-118">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1889-118">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="f1889-119">Чтение свойств и связей объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f1889-119">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="f1889-120">Создание windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1889-120">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="f1889-121">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1889-121">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="f1889-122">Создание нового объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f1889-122">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="f1889-123">Удаление windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1889-123">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="f1889-124">Нет</span><span class="sxs-lookup"><span data-stu-id="f1889-124">None</span></span>|<span data-ttu-id="f1889-125">Удаляет объект [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1889-125">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="f1889-126">Обновление windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1889-126">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="f1889-127">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1889-127">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="f1889-128">Обновление свойств объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f1889-128">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f1889-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1889-129">Properties</span></span>
|<span data-ttu-id="f1889-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1889-130">Property</span></span>|<span data-ttu-id="f1889-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f1889-131">Type</span></span>|<span data-ttu-id="f1889-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f1889-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1889-133">id</span><span class="sxs-lookup"><span data-stu-id="f1889-133">id</span></span>|<span data-ttu-id="f1889-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f1889-134">String</span></span>|<span data-ttu-id="f1889-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f1889-135">Key of the entity.</span></span> <span data-ttu-id="f1889-136">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1889-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1889-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1889-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f1889-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1889-138">DateTimeOffset</span></span>|<span data-ttu-id="f1889-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f1889-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f1889-140">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1889-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1889-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f1889-141">roleScopeTagIds</span></span>|<span data-ttu-id="f1889-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f1889-142">String collection</span></span>|<span data-ttu-id="f1889-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f1889-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f1889-144">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1889-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1889-145">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f1889-145">supportsScopeTags</span></span>|<span data-ttu-id="f1889-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1889-146">Boolean</span></span>|<span data-ttu-id="f1889-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f1889-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f1889-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f1889-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f1889-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f1889-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f1889-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f1889-150">This property is read-only.</span></span> <span data-ttu-id="f1889-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1889-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1889-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1889-152">createdDateTime</span></span>|<span data-ttu-id="f1889-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1889-153">DateTimeOffset</span></span>|<span data-ttu-id="f1889-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f1889-154">DateTime the object was created.</span></span> <span data-ttu-id="f1889-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1889-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1889-156">description</span><span class="sxs-lookup"><span data-stu-id="f1889-156">description</span></span>|<span data-ttu-id="f1889-157">String</span><span class="sxs-lookup"><span data-stu-id="f1889-157">String</span></span>|<span data-ttu-id="f1889-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f1889-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f1889-159">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1889-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1889-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f1889-160">displayName</span></span>|<span data-ttu-id="f1889-161">String</span><span class="sxs-lookup"><span data-stu-id="f1889-161">String</span></span>|<span data-ttu-id="f1889-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f1889-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f1889-163">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1889-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1889-164">version</span><span class="sxs-lookup"><span data-stu-id="f1889-164">version</span></span>|<span data-ttu-id="f1889-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f1889-165">Int32</span></span>|<span data-ttu-id="f1889-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f1889-166">Version of the device configuration.</span></span> <span data-ttu-id="f1889-167">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1889-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1889-168">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="f1889-168">connectionName</span></span>|<span data-ttu-id="f1889-169">String</span><span class="sxs-lookup"><span data-stu-id="f1889-169">String</span></span>|<span data-ttu-id="f1889-170">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1889-170">Connection name displayed to the user.</span></span> <span data-ttu-id="f1889-171">НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1889-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f1889-172">серверами</span><span class="sxs-lookup"><span data-stu-id="f1889-172">servers</span></span>|<span data-ttu-id="f1889-173">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="f1889-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="f1889-174">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="f1889-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="f1889-175">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="f1889-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="f1889-176">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f1889-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f1889-177">НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1889-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f1889-178">customXml</span><span class="sxs-lookup"><span data-stu-id="f1889-178">customXml</span></span>|<span data-ttu-id="f1889-179">Двоичный</span><span class="sxs-lookup"><span data-stu-id="f1889-179">Binary</span></span>|<span data-ttu-id="f1889-180">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="f1889-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="f1889-181">(Массив байтов в кодировке UTF8) НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1889-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f1889-182">Профилетаржет</span><span class="sxs-lookup"><span data-stu-id="f1889-182">profileTarget</span></span>|[<span data-ttu-id="f1889-183">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="f1889-183">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="f1889-184">Тип целевого объекта профиля.</span><span class="sxs-lookup"><span data-stu-id="f1889-184">Profile target type.</span></span> <span data-ttu-id="f1889-185">Возможные значения: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="f1889-185">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="f1889-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="f1889-186">connectionType</span></span>|[<span data-ttu-id="f1889-187">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="f1889-187">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="f1889-188">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="f1889-188">Connection type.</span></span> <span data-ttu-id="f1889-189">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="f1889-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="f1889-190">Енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="f1889-190">enableSplitTunneling</span></span>|<span data-ttu-id="f1889-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1889-191">Boolean</span></span>|<span data-ttu-id="f1889-192">Включение Расщепленного туннелирования.</span><span class="sxs-lookup"><span data-stu-id="f1889-192">Enable split tunneling.</span></span>|
|<span data-ttu-id="f1889-193">Енаблеалвайсон</span><span class="sxs-lookup"><span data-stu-id="f1889-193">enableAlwaysOn</span></span>|<span data-ttu-id="f1889-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1889-194">Boolean</span></span>|<span data-ttu-id="f1889-195">Включение режима "всегда включено".</span><span class="sxs-lookup"><span data-stu-id="f1889-195">Enable Always On mode.</span></span>|
|<span data-ttu-id="f1889-196">Енабледевицетуннел</span><span class="sxs-lookup"><span data-stu-id="f1889-196">enableDeviceTunnel</span></span>|<span data-ttu-id="f1889-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1889-197">Boolean</span></span>|<span data-ttu-id="f1889-198">Включите туннель устройства.</span><span class="sxs-lookup"><span data-stu-id="f1889-198">Enable device tunnel.</span></span>|
|<span data-ttu-id="f1889-199">Енабледнсрегистратион</span><span class="sxs-lookup"><span data-stu-id="f1889-199">enableDnsRegistration</span></span>|<span data-ttu-id="f1889-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1889-200">Boolean</span></span>|<span data-ttu-id="f1889-201">Включить регистрацию IP-адресов с использованием внутренней DNS.</span><span class="sxs-lookup"><span data-stu-id="f1889-201">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="f1889-202">Днссуффиксес</span><span class="sxs-lookup"><span data-stu-id="f1889-202">dnsSuffixes</span></span>|<span data-ttu-id="f1889-203">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f1889-203">String collection</span></span>|<span data-ttu-id="f1889-204">Укажите DNS-суффиксы, которые необходимо добавить в список поиска DNS, чтобы правильно маршрутизировать короткие имена.</span><span class="sxs-lookup"><span data-stu-id="f1889-204">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="f1889-205">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="f1889-205">authenticationMethod</span></span>|[<span data-ttu-id="f1889-206">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f1889-206">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="f1889-207">Метод проверки поДлинности.</span><span class="sxs-lookup"><span data-stu-id="f1889-207">Authentication method.</span></span> <span data-ttu-id="f1889-208">Возможные значения: `certificate`, `usernameAndPassword`, `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="f1889-208">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="f1889-209">Ремемберусеркредентиалс</span><span class="sxs-lookup"><span data-stu-id="f1889-209">rememberUserCredentials</span></span>|<span data-ttu-id="f1889-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1889-210">Boolean</span></span>|<span data-ttu-id="f1889-211">Запомнить учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1889-211">Remember user credentials.</span></span>|
|<span data-ttu-id="f1889-212">Енаблекондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="f1889-212">enableConditionalAccess</span></span>|<span data-ttu-id="f1889-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1889-213">Boolean</span></span>|<span data-ttu-id="f1889-214">Включение условного доступа.</span><span class="sxs-lookup"><span data-stu-id="f1889-214">Enable conditional access.</span></span>|
|<span data-ttu-id="f1889-215">Енаблесинглесигнонвисалтернатецертификате</span><span class="sxs-lookup"><span data-stu-id="f1889-215">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="f1889-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1889-216">Boolean</span></span>|<span data-ttu-id="f1889-217">Включите единый вход (SSO) с альтернативным сертификатом.</span><span class="sxs-lookup"><span data-stu-id="f1889-217">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="f1889-218">Синглесигнонеку</span><span class="sxs-lookup"><span data-stu-id="f1889-218">singleSignOnEku</span></span>|[<span data-ttu-id="f1889-219">Екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="f1889-219">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="f1889-220">Расширенное использование ключа (EKU) единого входа.</span><span class="sxs-lookup"><span data-stu-id="f1889-220">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="f1889-221">Синглесигнониссуерхаш</span><span class="sxs-lookup"><span data-stu-id="f1889-221">singleSignOnIssuerHash</span></span>|<span data-ttu-id="f1889-222">String</span><span class="sxs-lookup"><span data-stu-id="f1889-222">String</span></span>|<span data-ttu-id="f1889-223">Хэш поставщика единого входа.</span><span class="sxs-lookup"><span data-stu-id="f1889-223">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="f1889-224">Еапксмл</span><span class="sxs-lookup"><span data-stu-id="f1889-224">eapXml</span></span>|<span data-ttu-id="f1889-225">Двоичный</span><span class="sxs-lookup"><span data-stu-id="f1889-225">Binary</span></span>|<span data-ttu-id="f1889-226">XML-файл протокола расширенной проверки поДлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="f1889-226">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="f1889-227">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="f1889-227">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="f1889-228">проксисервер</span><span class="sxs-lookup"><span data-stu-id="f1889-228">proxyServer</span></span>|[<span data-ttu-id="f1889-229">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="f1889-229">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="f1889-230">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="f1889-230">Proxy Server.</span></span>|
|<span data-ttu-id="f1889-231">АссоЦиатедаппс</span><span class="sxs-lookup"><span data-stu-id="f1889-231">associatedApps</span></span>|<span data-ttu-id="f1889-232">Коллекция [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="f1889-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="f1889-233">Связанные приложения.</span><span class="sxs-lookup"><span data-stu-id="f1889-233">Associated Apps.</span></span> <span data-ttu-id="f1889-234">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="f1889-234">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="f1889-235">ОнляссоЦиатедаппсканусеконнектион</span><span class="sxs-lookup"><span data-stu-id="f1889-235">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="f1889-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1889-236">Boolean</span></span>|<span data-ttu-id="f1889-237">Подключение можно использовать только для связанных приложений (VPN для каждого приложения).</span><span class="sxs-lookup"><span data-stu-id="f1889-237">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="f1889-238">Виндовсинформатионпротектиондомаин</span><span class="sxs-lookup"><span data-stu-id="f1889-238">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="f1889-239">String</span><span class="sxs-lookup"><span data-stu-id="f1889-239">String</span></span>|<span data-ttu-id="f1889-240">Домен Windows Information Protection (WIP) для связи с этим подключением.</span><span class="sxs-lookup"><span data-stu-id="f1889-240">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="f1889-241">Траффикрулес</span><span class="sxs-lookup"><span data-stu-id="f1889-241">trafficRules</span></span>|<span data-ttu-id="f1889-242">Коллекция [впнтраффикруле](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="f1889-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="f1889-243">Правила трафика.</span><span class="sxs-lookup"><span data-stu-id="f1889-243">Traffic rules.</span></span> <span data-ttu-id="f1889-244">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="f1889-244">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="f1889-245">сылает</span><span class="sxs-lookup"><span data-stu-id="f1889-245">routes</span></span>|<span data-ttu-id="f1889-246">Коллекция [впнрауте](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="f1889-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="f1889-247">Маршруты (необязательно для сторонних поставщиков).</span><span class="sxs-lookup"><span data-stu-id="f1889-247">Routes (optional for third-party providers).</span></span> <span data-ttu-id="f1889-248">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="f1889-248">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="f1889-249">Днсрулес</span><span class="sxs-lookup"><span data-stu-id="f1889-249">dnsRules</span></span>|<span data-ttu-id="f1889-250">Коллекция [впнднсруле](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="f1889-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="f1889-251">Правила DNS.</span><span class="sxs-lookup"><span data-stu-id="f1889-251">DNS rules.</span></span> <span data-ttu-id="f1889-252">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="f1889-252">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="f1889-253">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="f1889-253">trustedNetworkDomains</span></span>|<span data-ttu-id="f1889-254">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f1889-254">String collection</span></span>|<span data-ttu-id="f1889-255">Доверенные сетевые домены</span><span class="sxs-lookup"><span data-stu-id="f1889-255">Trusted Network Domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1889-256">Связи</span><span class="sxs-lookup"><span data-stu-id="f1889-256">Relationships</span></span>
|<span data-ttu-id="f1889-257">Отношение</span><span class="sxs-lookup"><span data-stu-id="f1889-257">Relationship</span></span>|<span data-ttu-id="f1889-258">Тип</span><span class="sxs-lookup"><span data-stu-id="f1889-258">Type</span></span>|<span data-ttu-id="f1889-259">Описание</span><span class="sxs-lookup"><span data-stu-id="f1889-259">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1889-260">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="f1889-260">groupAssignments</span></span>|<span data-ttu-id="f1889-261">Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f1889-261">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="f1889-262">Список назначений групп для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f1889-262">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="f1889-263">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1889-263">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1889-264">assignments</span><span class="sxs-lookup"><span data-stu-id="f1889-264">assignments</span></span>|<span data-ttu-id="f1889-265">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f1889-265">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f1889-266">Список назначений для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f1889-266">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="f1889-267">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1889-267">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1889-268">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="f1889-268">deviceStatuses</span></span>|<span data-ttu-id="f1889-269">Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="f1889-269">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="f1889-270">Состояние установки конфигурации для каждого устройства.</span><span class="sxs-lookup"><span data-stu-id="f1889-270">Device configuration installation status by device.</span></span> <span data-ttu-id="f1889-271">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1889-271">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1889-272">userStatuses</span><span class="sxs-lookup"><span data-stu-id="f1889-272">userStatuses</span></span>|<span data-ttu-id="f1889-273">Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="f1889-273">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="f1889-274">Состояние установки конфигурации устройств пользователем.</span><span class="sxs-lookup"><span data-stu-id="f1889-274">Device configuration installation status by user.</span></span> <span data-ttu-id="f1889-275">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1889-275">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1889-276">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="f1889-276">deviceStatusOverview</span></span>|[<span data-ttu-id="f1889-277">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f1889-277">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="f1889-278">Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1889-278">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1889-279">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="f1889-279">userStatusOverview</span></span>|[<span data-ttu-id="f1889-280">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="f1889-280">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="f1889-281">Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1889-281">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1889-282">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="f1889-282">deviceSettingStateSummaries</span></span>|<span data-ttu-id="f1889-283">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="f1889-283">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="f1889-284">Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1889-284">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1889-285">Identitycertificate (</span><span class="sxs-lookup"><span data-stu-id="f1889-285">identityCertificate</span></span>|[<span data-ttu-id="f1889-286">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="f1889-286">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="f1889-287">Сертификат удостоверения для проверки подлинности клиента при использовании метода проверки подлинности Certificate.</span><span class="sxs-lookup"><span data-stu-id="f1889-287">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1889-288">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1889-288">JSON Representation</span></span>
<span data-ttu-id="f1889-289">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1889-289">Here is a JSON representation of the resource.</span></span>
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





