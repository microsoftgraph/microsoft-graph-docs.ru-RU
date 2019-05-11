---
title: Создание windowsPhone81VpnConfiguration
description: Создание нового объекта windowsPhone81VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 82e7dd4e3737ba39790554c62f9bb6829ce2d206
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917592"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="f99e1-103">Создание windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f99e1-103">Create windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="f99e1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f99e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f99e1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f99e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f99e1-106">Создание нового объекта [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f99e1-106">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f99e1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f99e1-107">Prerequisites</span></span>
<span data-ttu-id="f99e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f99e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f99e1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f99e1-110">Permission type</span></span>|<span data-ttu-id="f99e1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f99e1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f99e1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f99e1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f99e1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f99e1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f99e1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f99e1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f99e1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f99e1-115">Not supported.</span></span>|
|<span data-ttu-id="f99e1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f99e1-116">Application</span></span>|<span data-ttu-id="f99e1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f99e1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f99e1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f99e1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f99e1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f99e1-119">Request headers</span></span>
|<span data-ttu-id="f99e1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f99e1-120">Header</span></span>|<span data-ttu-id="f99e1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f99e1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f99e1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f99e1-122">Authorization</span></span>|<span data-ttu-id="f99e1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f99e1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f99e1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f99e1-124">Accept</span></span>|<span data-ttu-id="f99e1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f99e1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f99e1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f99e1-126">Request body</span></span>
<span data-ttu-id="f99e1-127">В тексте запроса добавьте представление объекта windowsPhone81VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f99e1-127">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="f99e1-128">В следующей таблице приведены свойства, необходимые при создании windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f99e1-128">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="f99e1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f99e1-129">Property</span></span>|<span data-ttu-id="f99e1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f99e1-130">Type</span></span>|<span data-ttu-id="f99e1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f99e1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f99e1-132">id</span><span class="sxs-lookup"><span data-stu-id="f99e1-132">id</span></span>|<span data-ttu-id="f99e1-133">String</span><span class="sxs-lookup"><span data-stu-id="f99e1-133">String</span></span>|<span data-ttu-id="f99e1-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f99e1-134">Key of the entity.</span></span> <span data-ttu-id="f99e1-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f99e1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f99e1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f99e1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f99e1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f99e1-137">DateTimeOffset</span></span>|<span data-ttu-id="f99e1-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f99e1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f99e1-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f99e1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f99e1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f99e1-140">roleScopeTagIds</span></span>|<span data-ttu-id="f99e1-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f99e1-141">String collection</span></span>|<span data-ttu-id="f99e1-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f99e1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f99e1-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f99e1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f99e1-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f99e1-144">supportsScopeTags</span></span>|<span data-ttu-id="f99e1-145">Логический</span><span class="sxs-lookup"><span data-stu-id="f99e1-145">Boolean</span></span>|<span data-ttu-id="f99e1-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f99e1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f99e1-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f99e1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f99e1-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f99e1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f99e1-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f99e1-149">This property is read-only.</span></span> <span data-ttu-id="f99e1-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f99e1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f99e1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f99e1-151">createdDateTime</span></span>|<span data-ttu-id="f99e1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f99e1-152">DateTimeOffset</span></span>|<span data-ttu-id="f99e1-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f99e1-153">DateTime the object was created.</span></span> <span data-ttu-id="f99e1-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f99e1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f99e1-155">description</span><span class="sxs-lookup"><span data-stu-id="f99e1-155">description</span></span>|<span data-ttu-id="f99e1-156">String</span><span class="sxs-lookup"><span data-stu-id="f99e1-156">String</span></span>|<span data-ttu-id="f99e1-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f99e1-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f99e1-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f99e1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f99e1-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f99e1-159">displayName</span></span>|<span data-ttu-id="f99e1-160">Строка</span><span class="sxs-lookup"><span data-stu-id="f99e1-160">String</span></span>|<span data-ttu-id="f99e1-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f99e1-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f99e1-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f99e1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f99e1-163">version</span><span class="sxs-lookup"><span data-stu-id="f99e1-163">version</span></span>|<span data-ttu-id="f99e1-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f99e1-164">Int32</span></span>|<span data-ttu-id="f99e1-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f99e1-165">Version of the device configuration.</span></span> <span data-ttu-id="f99e1-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f99e1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f99e1-167">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="f99e1-167">connectionName</span></span>|<span data-ttu-id="f99e1-168">Строка</span><span class="sxs-lookup"><span data-stu-id="f99e1-168">String</span></span>|<span data-ttu-id="f99e1-169">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f99e1-169">Connection name displayed to the user.</span></span> <span data-ttu-id="f99e1-170">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f99e1-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f99e1-171">серверами</span><span class="sxs-lookup"><span data-stu-id="f99e1-171">servers</span></span>|<span data-ttu-id="f99e1-172">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="f99e1-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="f99e1-173">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="f99e1-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="f99e1-174">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="f99e1-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="f99e1-175">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f99e1-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f99e1-176">Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f99e1-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f99e1-177">customXml</span><span class="sxs-lookup"><span data-stu-id="f99e1-177">customXml</span></span>|<span data-ttu-id="f99e1-178">Binary</span><span class="sxs-lookup"><span data-stu-id="f99e1-178">Binary</span></span>|<span data-ttu-id="f99e1-179">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="f99e1-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="f99e1-180">(Массив байтов в кодировке UTF8) Наследуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f99e1-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f99e1-181">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="f99e1-181">applyOnlyToWindows81</span></span>|<span data-ttu-id="f99e1-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="f99e1-182">Boolean</span></span>|<span data-ttu-id="f99e1-183">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="f99e1-183">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="f99e1-184">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f99e1-184">This property is read-only.</span></span> <span data-ttu-id="f99e1-185">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f99e1-185">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="f99e1-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="f99e1-186">connectionType</span></span>|[<span data-ttu-id="f99e1-187">Виндовсвпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="f99e1-187">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="f99e1-188">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="f99e1-188">Connection type.</span></span> <span data-ttu-id="f99e1-189">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f99e1-189">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="f99e1-190">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="f99e1-190">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="f99e1-191">Логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="f99e1-191">loginGroupOrDomain</span></span>|<span data-ttu-id="f99e1-192">Строка</span><span class="sxs-lookup"><span data-stu-id="f99e1-192">String</span></span>|<span data-ttu-id="f99e1-193">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="f99e1-193">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="f99e1-194">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f99e1-194">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="f99e1-195">Енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="f99e1-195">enableSplitTunneling</span></span>|<span data-ttu-id="f99e1-196">Логический</span><span class="sxs-lookup"><span data-stu-id="f99e1-196">Boolean</span></span>|<span data-ttu-id="f99e1-197">Включение Расщепленного туннелирования для VPN.</span><span class="sxs-lookup"><span data-stu-id="f99e1-197">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="f99e1-198">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f99e1-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="f99e1-199">проксисервер</span><span class="sxs-lookup"><span data-stu-id="f99e1-199">proxyServer</span></span>|[<span data-ttu-id="f99e1-200">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="f99e1-200">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="f99e1-201">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="f99e1-201">Proxy Server.</span></span> <span data-ttu-id="f99e1-202">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f99e1-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="f99e1-203">Бипассвпнонкомпанивифи</span><span class="sxs-lookup"><span data-stu-id="f99e1-203">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="f99e1-204">Логический</span><span class="sxs-lookup"><span data-stu-id="f99e1-204">Boolean</span></span>|<span data-ttu-id="f99e1-205">Обход VPN в сети Wi-Fi компании.</span><span class="sxs-lookup"><span data-stu-id="f99e1-205">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="f99e1-206">Бипассвпнонхомевифи</span><span class="sxs-lookup"><span data-stu-id="f99e1-206">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="f99e1-207">Логический</span><span class="sxs-lookup"><span data-stu-id="f99e1-207">Boolean</span></span>|<span data-ttu-id="f99e1-208">Обход VPN для домашнего Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f99e1-208">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="f99e1-209">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="f99e1-209">authenticationMethod</span></span>|[<span data-ttu-id="f99e1-210">Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="f99e1-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="f99e1-211">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="f99e1-211">Authentication method.</span></span> <span data-ttu-id="f99e1-212">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="f99e1-212">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="f99e1-213">Ремемберусеркредентиалс</span><span class="sxs-lookup"><span data-stu-id="f99e1-213">rememberUserCredentials</span></span>|<span data-ttu-id="f99e1-214">Логический</span><span class="sxs-lookup"><span data-stu-id="f99e1-214">Boolean</span></span>|<span data-ttu-id="f99e1-215">Запомнить учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="f99e1-215">Remember user credentials.</span></span>|
|<span data-ttu-id="f99e1-216">Днссуффикссеарчлист</span><span class="sxs-lookup"><span data-stu-id="f99e1-216">dnsSuffixSearchList</span></span>|<span data-ttu-id="f99e1-217">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f99e1-217">String collection</span></span>|<span data-ttu-id="f99e1-218">Список поиска DNS-суффиксов.</span><span class="sxs-lookup"><span data-stu-id="f99e1-218">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="f99e1-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="f99e1-219">Response</span></span>
<span data-ttu-id="f99e1-220">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f99e1-220">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f99e1-221">Пример</span><span class="sxs-lookup"><span data-stu-id="f99e1-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="f99e1-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="f99e1-222">Request</span></span>
<span data-ttu-id="f99e1-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f99e1-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1243

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="f99e1-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="f99e1-224">Response</span></span>
<span data-ttu-id="f99e1-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f99e1-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1415

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
  "id": "7cecc0db-c0db-7cec-dbc0-ec7cdbc0ec7c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




