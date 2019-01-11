---
title: Тип ресурса windows10VpnConfiguration
description: С указанием конфигураций в этот профиль может проинструктировать устройства Windows 10 (настольного компьютера или мобильного) для подключения к требуемой конечной точки VPN. Путем указания типов безопасности и метод проверки подлинности ожидаемого конечной точкой виртуальной частной сети VPN-подключение можно сделать полностью для конечных пользователей.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 72617e1d91a6a9ce180e63733a209bcee7e204bc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816068"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="81d0a-104">Тип ресурса windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="81d0a-104">windows10VpnConfiguration resource type</span></span>

> <span data-ttu-id="81d0a-105">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="81d0a-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81d0a-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81d0a-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81d0a-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="81d0a-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81d0a-108">С указанием конфигураций в этот профиль может проинструктировать устройства Windows 10 (настольного компьютера или мобильного) для подключения к требуемой конечной точки VPN.</span><span class="sxs-lookup"><span data-stu-id="81d0a-108">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="81d0a-109">Путем указания типов безопасности и метод проверки подлинности ожидаемого конечной точкой виртуальной частной сети VPN-подключение можно сделать полностью для конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="81d0a-109">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>

<span data-ttu-id="81d0a-110">Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81d0a-110">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="81d0a-111">Методы</span><span class="sxs-lookup"><span data-stu-id="81d0a-111">Methods</span></span>
|<span data-ttu-id="81d0a-112">Метод</span><span class="sxs-lookup"><span data-stu-id="81d0a-112">Method</span></span>|<span data-ttu-id="81d0a-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="81d0a-113">Return Type</span></span>|<span data-ttu-id="81d0a-114">Описание</span><span class="sxs-lookup"><span data-stu-id="81d0a-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="81d0a-115">Список windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="81d0a-115">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="81d0a-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="81d0a-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="81d0a-117">Свойства списка и связей объектов [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="81d0a-117">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="81d0a-118">Получение windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="81d0a-118">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="81d0a-119">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="81d0a-119">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="81d0a-120">Чтение свойства и связи объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="81d0a-120">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="81d0a-121">Создание windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="81d0a-121">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="81d0a-122">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="81d0a-122">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="81d0a-123">Создание нового объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="81d0a-123">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="81d0a-124">Удаление windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="81d0a-124">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="81d0a-125">Нет</span><span class="sxs-lookup"><span data-stu-id="81d0a-125">None</span></span>|<span data-ttu-id="81d0a-126">Удаляет [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81d0a-126">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="81d0a-127">Обновление windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="81d0a-127">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="81d0a-128">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="81d0a-128">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="81d0a-129">Обновление свойства объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="81d0a-129">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="81d0a-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="81d0a-130">Properties</span></span>
|<span data-ttu-id="81d0a-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="81d0a-131">Property</span></span>|<span data-ttu-id="81d0a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="81d0a-132">Type</span></span>|<span data-ttu-id="81d0a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="81d0a-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81d0a-134">id</span><span class="sxs-lookup"><span data-stu-id="81d0a-134">id</span></span>|<span data-ttu-id="81d0a-135">Строка</span><span class="sxs-lookup"><span data-stu-id="81d0a-135">String</span></span>|<span data-ttu-id="81d0a-136">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="81d0a-136">Key of the entity.</span></span> <span data-ttu-id="81d0a-137">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81d0a-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81d0a-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81d0a-138">lastModifiedDateTime</span></span>|<span data-ttu-id="81d0a-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81d0a-139">DateTimeOffset</span></span>|<span data-ttu-id="81d0a-140">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="81d0a-140">DateTime the object was last modified.</span></span> <span data-ttu-id="81d0a-141">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81d0a-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81d0a-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="81d0a-142">roleScopeTagIds</span></span>|<span data-ttu-id="81d0a-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="81d0a-143">String collection</span></span>|<span data-ttu-id="81d0a-144">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="81d0a-144">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="81d0a-145">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81d0a-145">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81d0a-146">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="81d0a-146">supportsScopeTags</span></span>|<span data-ttu-id="81d0a-147">Логический</span><span class="sxs-lookup"><span data-stu-id="81d0a-147">Boolean</span></span>|<span data-ttu-id="81d0a-148">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="81d0a-148">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="81d0a-149">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="81d0a-149">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="81d0a-150">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="81d0a-150">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="81d0a-151">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81d0a-151">This property is read-only.</span></span> <span data-ttu-id="81d0a-152">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81d0a-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81d0a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81d0a-153">createdDateTime</span></span>|<span data-ttu-id="81d0a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81d0a-154">DateTimeOffset</span></span>|<span data-ttu-id="81d0a-155">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="81d0a-155">DateTime the object was created.</span></span> <span data-ttu-id="81d0a-156">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81d0a-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81d0a-157">описание</span><span class="sxs-lookup"><span data-stu-id="81d0a-157">description</span></span>|<span data-ttu-id="81d0a-158">Строка</span><span class="sxs-lookup"><span data-stu-id="81d0a-158">String</span></span>|<span data-ttu-id="81d0a-159">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="81d0a-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="81d0a-160">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81d0a-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81d0a-161">displayName</span><span class="sxs-lookup"><span data-stu-id="81d0a-161">displayName</span></span>|<span data-ttu-id="81d0a-162">Строка</span><span class="sxs-lookup"><span data-stu-id="81d0a-162">String</span></span>|<span data-ttu-id="81d0a-163">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="81d0a-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="81d0a-164">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81d0a-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81d0a-165">version</span><span class="sxs-lookup"><span data-stu-id="81d0a-165">version</span></span>|<span data-ttu-id="81d0a-166">Int32</span><span class="sxs-lookup"><span data-stu-id="81d0a-166">Int32</span></span>|<span data-ttu-id="81d0a-167">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="81d0a-167">Version of the device configuration.</span></span> <span data-ttu-id="81d0a-168">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81d0a-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81d0a-169">connectionName</span><span class="sxs-lookup"><span data-stu-id="81d0a-169">connectionName</span></span>|<span data-ttu-id="81d0a-170">Строка</span><span class="sxs-lookup"><span data-stu-id="81d0a-170">String</span></span>|<span data-ttu-id="81d0a-171">Имя подключения отображается для пользователя.</span><span class="sxs-lookup"><span data-stu-id="81d0a-171">Connection name displayed to the user.</span></span> <span data-ttu-id="81d0a-172">Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81d0a-172">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="81d0a-173">серверы</span><span class="sxs-lookup"><span data-stu-id="81d0a-173">servers</span></span>|<span data-ttu-id="81d0a-174">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="81d0a-174">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="81d0a-175">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="81d0a-175">List of VPN Servers on the network.</span></span> <span data-ttu-id="81d0a-176">Убедитесь, что конечные пользователи могут получить доступ к эти расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="81d0a-176">Make sure end users can access these network locations.</span></span> <span data-ttu-id="81d0a-177">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="81d0a-177">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="81d0a-178">Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81d0a-178">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="81d0a-179">customXml</span><span class="sxs-lookup"><span data-stu-id="81d0a-179">customXml</span></span>|<span data-ttu-id="81d0a-180">Binary</span><span class="sxs-lookup"><span data-stu-id="81d0a-180">Binary</span></span>|<span data-ttu-id="81d0a-181">Настраиваемые команды XML, которые настраиваются VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="81d0a-181">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="81d0a-182">(UTF8 закодированный массив байтов) Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81d0a-182">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="81d0a-183">profileTarget</span><span class="sxs-lookup"><span data-stu-id="81d0a-183">profileTarget</span></span>|[<span data-ttu-id="81d0a-184">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="81d0a-184">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="81d0a-185">Тип конечного профиля.</span><span class="sxs-lookup"><span data-stu-id="81d0a-185">Profile target type.</span></span> <span data-ttu-id="81d0a-186">Возможные значения: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="81d0a-186">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="81d0a-187">Тип подключения</span><span class="sxs-lookup"><span data-stu-id="81d0a-187">connectionType</span></span>|[<span data-ttu-id="81d0a-188">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="81d0a-188">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="81d0a-189">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="81d0a-189">Connection type.</span></span> <span data-ttu-id="81d0a-190">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="81d0a-190">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="81d0a-191">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="81d0a-191">enableSplitTunneling</span></span>|<span data-ttu-id="81d0a-192">Логический</span><span class="sxs-lookup"><span data-stu-id="81d0a-192">Boolean</span></span>|<span data-ttu-id="81d0a-193">Включение разделенное туннелирование.</span><span class="sxs-lookup"><span data-stu-id="81d0a-193">Enable split tunneling.</span></span>|
|<span data-ttu-id="81d0a-194">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="81d0a-194">enableAlwaysOn</span></span>|<span data-ttu-id="81d0a-195">Логический</span><span class="sxs-lookup"><span data-stu-id="81d0a-195">Boolean</span></span>|<span data-ttu-id="81d0a-196">Включение режима всегда на.</span><span class="sxs-lookup"><span data-stu-id="81d0a-196">Enable Always On mode.</span></span>|
|<span data-ttu-id="81d0a-197">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="81d0a-197">enableDeviceTunnel</span></span>|<span data-ttu-id="81d0a-198">Логический</span><span class="sxs-lookup"><span data-stu-id="81d0a-198">Boolean</span></span>|<span data-ttu-id="81d0a-199">Включение туннель устройства.</span><span class="sxs-lookup"><span data-stu-id="81d0a-199">Enable device tunnel.</span></span>|
|<span data-ttu-id="81d0a-200">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="81d0a-200">enableDnsRegistration</span></span>|<span data-ttu-id="81d0a-201">Логический</span><span class="sxs-lookup"><span data-stu-id="81d0a-201">Boolean</span></span>|<span data-ttu-id="81d0a-202">Включение регистрации IP-адреса с внутренней DNS.</span><span class="sxs-lookup"><span data-stu-id="81d0a-202">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="81d0a-203">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="81d0a-203">dnsSuffixes</span></span>|<span data-ttu-id="81d0a-204">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="81d0a-204">String collection</span></span>|<span data-ttu-id="81d0a-205">Укажите DNS-суффиксы для добавления в список поиска DNS маршрутизацию короткие имена.</span><span class="sxs-lookup"><span data-stu-id="81d0a-205">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="81d0a-206">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="81d0a-206">authenticationMethod</span></span>|[<span data-ttu-id="81d0a-207">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="81d0a-207">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="81d0a-208">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="81d0a-208">Authentication method.</span></span> <span data-ttu-id="81d0a-209">Возможные значения: `certificate`, `usernameAndPassword`, `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="81d0a-209">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="81d0a-210">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="81d0a-210">rememberUserCredentials</span></span>|<span data-ttu-id="81d0a-211">Логический</span><span class="sxs-lookup"><span data-stu-id="81d0a-211">Boolean</span></span>|<span data-ttu-id="81d0a-212">Не забудьте учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="81d0a-212">Remember user credentials.</span></span>|
|<span data-ttu-id="81d0a-213">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="81d0a-213">enableConditionalAccess</span></span>|<span data-ttu-id="81d0a-214">Логический</span><span class="sxs-lookup"><span data-stu-id="81d0a-214">Boolean</span></span>|<span data-ttu-id="81d0a-215">Включение условного доступа.</span><span class="sxs-lookup"><span data-stu-id="81d0a-215">Enable conditional access.</span></span>|
|<span data-ttu-id="81d0a-216">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="81d0a-216">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="81d0a-217">Логический</span><span class="sxs-lookup"><span data-stu-id="81d0a-217">Boolean</span></span>|<span data-ttu-id="81d0a-218">Включение единого входа (SSO) с помощью альтернативного сертификата.</span><span class="sxs-lookup"><span data-stu-id="81d0a-218">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="81d0a-219">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="81d0a-219">singleSignOnEku</span></span>|[<span data-ttu-id="81d0a-220">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="81d0a-220">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="81d0a-221">Единого входа расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="81d0a-221">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="81d0a-222">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="81d0a-222">singleSignOnIssuerHash</span></span>|<span data-ttu-id="81d0a-223">Строка</span><span class="sxs-lookup"><span data-stu-id="81d0a-223">String</span></span>|<span data-ttu-id="81d0a-224">Хэш-функции поставщика единого входа.</span><span class="sxs-lookup"><span data-stu-id="81d0a-224">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="81d0a-225">eapXml</span><span class="sxs-lookup"><span data-stu-id="81d0a-225">eapXml</span></span>|<span data-ttu-id="81d0a-226">Binary</span><span class="sxs-lookup"><span data-stu-id="81d0a-226">Binary</span></span>|<span data-ttu-id="81d0a-227">Протокол расширенной проверки подлинности (EAP) XML.</span><span class="sxs-lookup"><span data-stu-id="81d0a-227">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="81d0a-228">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="81d0a-228">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="81d0a-229">прокси-серверу</span><span class="sxs-lookup"><span data-stu-id="81d0a-229">proxyServer</span></span>|[<span data-ttu-id="81d0a-230">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="81d0a-230">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="81d0a-231">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="81d0a-231">Proxy Server.</span></span>|
|<span data-ttu-id="81d0a-232">associatedApps</span><span class="sxs-lookup"><span data-stu-id="81d0a-232">associatedApps</span></span>|<span data-ttu-id="81d0a-233">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="81d0a-233">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="81d0a-234">Связанные приложения.</span><span class="sxs-lookup"><span data-stu-id="81d0a-234">Associated Apps.</span></span> <span data-ttu-id="81d0a-235">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="81d0a-235">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="81d0a-236">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="81d0a-236">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="81d0a-237">Логический</span><span class="sxs-lookup"><span data-stu-id="81d0a-237">Boolean</span></span>|<span data-ttu-id="81d0a-238">Только связанного приложения могут использовать подключения (VPN-app).</span><span class="sxs-lookup"><span data-stu-id="81d0a-238">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="81d0a-239">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="81d0a-239">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="81d0a-240">Строка</span><span class="sxs-lookup"><span data-stu-id="81d0a-240">String</span></span>|<span data-ttu-id="81d0a-241">Сведения о защите Windows (НЗП) домена, связанного с этим подключением.</span><span class="sxs-lookup"><span data-stu-id="81d0a-241">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="81d0a-242">trafficRules</span><span class="sxs-lookup"><span data-stu-id="81d0a-242">trafficRules</span></span>|<span data-ttu-id="81d0a-243">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="81d0a-243">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="81d0a-244">Правила трафика.</span><span class="sxs-lookup"><span data-stu-id="81d0a-244">Traffic rules.</span></span> <span data-ttu-id="81d0a-245">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="81d0a-245">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="81d0a-246">маршруты</span><span class="sxs-lookup"><span data-stu-id="81d0a-246">routes</span></span>|<span data-ttu-id="81d0a-247">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="81d0a-247">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="81d0a-248">Маршрутизация (не обязательно для сторонних поставщиков).</span><span class="sxs-lookup"><span data-stu-id="81d0a-248">Routes (optional for third-party providers).</span></span> <span data-ttu-id="81d0a-249">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="81d0a-249">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="81d0a-250">dnsRules</span><span class="sxs-lookup"><span data-stu-id="81d0a-250">dnsRules</span></span>|<span data-ttu-id="81d0a-251">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="81d0a-251">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="81d0a-252">Правила DNS.</span><span class="sxs-lookup"><span data-stu-id="81d0a-252">DNS rules.</span></span> <span data-ttu-id="81d0a-253">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="81d0a-253">This collection can contain a maximum of 1000 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81d0a-254">Связи</span><span class="sxs-lookup"><span data-stu-id="81d0a-254">Relationships</span></span>
|<span data-ttu-id="81d0a-255">Связь</span><span class="sxs-lookup"><span data-stu-id="81d0a-255">Relationship</span></span>|<span data-ttu-id="81d0a-256">Тип</span><span class="sxs-lookup"><span data-stu-id="81d0a-256">Type</span></span>|<span data-ttu-id="81d0a-257">Описание</span><span class="sxs-lookup"><span data-stu-id="81d0a-257">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81d0a-258">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="81d0a-258">groupAssignments</span></span>|<span data-ttu-id="81d0a-259">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="81d0a-259">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="81d0a-260">Список назначений групп для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="81d0a-260">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="81d0a-261">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81d0a-261">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81d0a-262">assignments</span><span class="sxs-lookup"><span data-stu-id="81d0a-262">assignments</span></span>|<span data-ttu-id="81d0a-263">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="81d0a-263">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="81d0a-264">Список назначений для профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="81d0a-264">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="81d0a-265">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81d0a-265">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81d0a-266">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="81d0a-266">deviceStatuses</span></span>|<span data-ttu-id="81d0a-267">Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="81d0a-267">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="81d0a-268">Состояние установки конфигурации для каждого устройства.</span><span class="sxs-lookup"><span data-stu-id="81d0a-268">Device configuration installation status by device.</span></span> <span data-ttu-id="81d0a-269">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81d0a-269">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81d0a-270">userStatuses</span><span class="sxs-lookup"><span data-stu-id="81d0a-270">userStatuses</span></span>|<span data-ttu-id="81d0a-271">Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="81d0a-271">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="81d0a-272">Состояние установки конфигурации устройства пользователем.</span><span class="sxs-lookup"><span data-stu-id="81d0a-272">Device configuration installation status by user.</span></span> <span data-ttu-id="81d0a-273">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81d0a-273">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81d0a-274">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="81d0a-274">deviceStatusOverview</span></span>|[<span data-ttu-id="81d0a-275">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="81d0a-275">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="81d0a-276">Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81d0a-276">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81d0a-277">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="81d0a-277">userStatusOverview</span></span>|[<span data-ttu-id="81d0a-278">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="81d0a-278">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="81d0a-279">Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81d0a-279">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81d0a-280">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="81d0a-280">deviceSettingStateSummaries</span></span>|<span data-ttu-id="81d0a-281">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="81d0a-281">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="81d0a-282">Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="81d0a-282">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81d0a-283">identityCertificate</span><span class="sxs-lookup"><span data-stu-id="81d0a-283">identityCertificate</span></span>|[<span data-ttu-id="81d0a-284">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="81d0a-284">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="81d0a-285">Сертификат удостоверения для проверки подлинности клиентов, если метод проверки подлинности сертификата.</span><span class="sxs-lookup"><span data-stu-id="81d0a-285">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81d0a-286">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81d0a-286">JSON Representation</span></span>
<span data-ttu-id="81d0a-287">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81d0a-287">Here is a JSON representation of the resource.</span></span>
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
      "proxyServerUri": "String"
    }
  ]
}
```





