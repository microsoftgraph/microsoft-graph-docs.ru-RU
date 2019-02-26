---
title: Создание windowsPhone81VpnConfiguration
description: Создание нового объекта windowsPhone81VpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5fa2c90a2cffaf9e33534e11c8a35a44d5197140
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140497"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="6ea21-103">Создание windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6ea21-103">Create windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="6ea21-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ea21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ea21-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ea21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ea21-106">Создание нового объекта [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6ea21-106">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ea21-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6ea21-107">Prerequisites</span></span>
<span data-ttu-id="6ea21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6ea21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6ea21-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ea21-110">Permission type</span></span>|<span data-ttu-id="6ea21-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ea21-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ea21-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ea21-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6ea21-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ea21-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ea21-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ea21-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ea21-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ea21-115">Not supported.</span></span>|
|<span data-ttu-id="6ea21-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ea21-116">Application</span></span>|<span data-ttu-id="6ea21-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ea21-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ea21-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ea21-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6ea21-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ea21-119">Request headers</span></span>
|<span data-ttu-id="6ea21-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ea21-120">Header</span></span>|<span data-ttu-id="6ea21-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6ea21-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ea21-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ea21-122">Authorization</span></span>|<span data-ttu-id="6ea21-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6ea21-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ea21-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6ea21-124">Accept</span></span>|<span data-ttu-id="6ea21-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6ea21-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ea21-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ea21-126">Request body</span></span>
<span data-ttu-id="6ea21-127">В тексте запроса добавьте представление объекта windowsPhone81VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ea21-127">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="6ea21-128">В следующей таблице приведены свойства, необходимые при создании windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6ea21-128">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="6ea21-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ea21-129">Property</span></span>|<span data-ttu-id="6ea21-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6ea21-130">Type</span></span>|<span data-ttu-id="6ea21-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6ea21-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ea21-132">id</span><span class="sxs-lookup"><span data-stu-id="6ea21-132">id</span></span>|<span data-ttu-id="6ea21-133">String</span><span class="sxs-lookup"><span data-stu-id="6ea21-133">String</span></span>|<span data-ttu-id="6ea21-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6ea21-134">Key of the entity.</span></span> <span data-ttu-id="6ea21-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ea21-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ea21-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ea21-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6ea21-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ea21-137">DateTimeOffset</span></span>|<span data-ttu-id="6ea21-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6ea21-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6ea21-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ea21-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ea21-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6ea21-140">roleScopeTagIds</span></span>|<span data-ttu-id="6ea21-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6ea21-141">String collection</span></span>|<span data-ttu-id="6ea21-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6ea21-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6ea21-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ea21-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ea21-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="6ea21-144">supportsScopeTags</span></span>|<span data-ttu-id="6ea21-145">Логический</span><span class="sxs-lookup"><span data-stu-id="6ea21-145">Boolean</span></span>|<span data-ttu-id="6ea21-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="6ea21-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6ea21-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="6ea21-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6ea21-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6ea21-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6ea21-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ea21-149">This property is read-only.</span></span> <span data-ttu-id="6ea21-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ea21-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ea21-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ea21-151">createdDateTime</span></span>|<span data-ttu-id="6ea21-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ea21-152">DateTimeOffset</span></span>|<span data-ttu-id="6ea21-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6ea21-153">DateTime the object was created.</span></span> <span data-ttu-id="6ea21-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ea21-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ea21-155">description</span><span class="sxs-lookup"><span data-stu-id="6ea21-155">description</span></span>|<span data-ttu-id="6ea21-156">String</span><span class="sxs-lookup"><span data-stu-id="6ea21-156">String</span></span>|<span data-ttu-id="6ea21-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6ea21-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6ea21-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ea21-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ea21-159">displayName</span><span class="sxs-lookup"><span data-stu-id="6ea21-159">displayName</span></span>|<span data-ttu-id="6ea21-160">String</span><span class="sxs-lookup"><span data-stu-id="6ea21-160">String</span></span>|<span data-ttu-id="6ea21-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6ea21-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6ea21-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ea21-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ea21-163">version</span><span class="sxs-lookup"><span data-stu-id="6ea21-163">version</span></span>|<span data-ttu-id="6ea21-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6ea21-164">Int32</span></span>|<span data-ttu-id="6ea21-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6ea21-165">Version of the device configuration.</span></span> <span data-ttu-id="6ea21-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ea21-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ea21-167">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="6ea21-167">connectionName</span></span>|<span data-ttu-id="6ea21-168">String</span><span class="sxs-lookup"><span data-stu-id="6ea21-168">String</span></span>|<span data-ttu-id="6ea21-169">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ea21-169">Connection name displayed to the user.</span></span> <span data-ttu-id="6ea21-170">НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ea21-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ea21-171">серверы</span><span class="sxs-lookup"><span data-stu-id="6ea21-171">servers</span></span>|<span data-ttu-id="6ea21-172">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="6ea21-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="6ea21-173">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="6ea21-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="6ea21-174">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="6ea21-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="6ea21-175">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6ea21-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6ea21-176">НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ea21-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ea21-177">customXml</span><span class="sxs-lookup"><span data-stu-id="6ea21-177">customXml</span></span>|<span data-ttu-id="6ea21-178">Binary</span><span class="sxs-lookup"><span data-stu-id="6ea21-178">Binary</span></span>|<span data-ttu-id="6ea21-179">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="6ea21-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="6ea21-180">(Массив байтов в кодировке UTF8) НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ea21-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ea21-181">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="6ea21-181">applyOnlyToWindows81</span></span>|<span data-ttu-id="6ea21-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ea21-182">Boolean</span></span>|<span data-ttu-id="6ea21-183">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="6ea21-183">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="6ea21-184">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ea21-184">This property is read-only.</span></span> <span data-ttu-id="6ea21-185">НаСледуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ea21-185">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ea21-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="6ea21-186">connectionType</span></span>|[<span data-ttu-id="6ea21-187">Виндовсвпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="6ea21-187">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="6ea21-188">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="6ea21-188">Connection type.</span></span> <span data-ttu-id="6ea21-189">НаСледуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ea21-189">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="6ea21-190">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="6ea21-190">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="6ea21-191">Логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="6ea21-191">loginGroupOrDomain</span></span>|<span data-ttu-id="6ea21-192">String</span><span class="sxs-lookup"><span data-stu-id="6ea21-192">String</span></span>|<span data-ttu-id="6ea21-193">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="6ea21-193">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="6ea21-194">НаСледуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ea21-194">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ea21-195">Енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="6ea21-195">enableSplitTunneling</span></span>|<span data-ttu-id="6ea21-196">Логический</span><span class="sxs-lookup"><span data-stu-id="6ea21-196">Boolean</span></span>|<span data-ttu-id="6ea21-197">Включение Расщепленного туннелирования для VPN.</span><span class="sxs-lookup"><span data-stu-id="6ea21-197">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="6ea21-198">НаСледуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ea21-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ea21-199">проксисервер</span><span class="sxs-lookup"><span data-stu-id="6ea21-199">proxyServer</span></span>|[<span data-ttu-id="6ea21-200">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="6ea21-200">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="6ea21-201">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="6ea21-201">Proxy Server.</span></span> <span data-ttu-id="6ea21-202">НаСледуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ea21-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="6ea21-203">Бипассвпнонкомпанивифи</span><span class="sxs-lookup"><span data-stu-id="6ea21-203">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="6ea21-204">Логический</span><span class="sxs-lookup"><span data-stu-id="6ea21-204">Boolean</span></span>|<span data-ttu-id="6ea21-205">Обход VPN в сети Wi-Fi компании.</span><span class="sxs-lookup"><span data-stu-id="6ea21-205">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="6ea21-206">Бипассвпнонхомевифи</span><span class="sxs-lookup"><span data-stu-id="6ea21-206">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="6ea21-207">Логический</span><span class="sxs-lookup"><span data-stu-id="6ea21-207">Boolean</span></span>|<span data-ttu-id="6ea21-208">Обход VPN для домашнего Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="6ea21-208">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="6ea21-209">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="6ea21-209">authenticationMethod</span></span>|[<span data-ttu-id="6ea21-210">Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="6ea21-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="6ea21-211">Метод проверки поДлинности.</span><span class="sxs-lookup"><span data-stu-id="6ea21-211">Authentication method.</span></span> <span data-ttu-id="6ea21-212">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="6ea21-212">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="6ea21-213">Ремемберусеркредентиалс</span><span class="sxs-lookup"><span data-stu-id="6ea21-213">rememberUserCredentials</span></span>|<span data-ttu-id="6ea21-214">Логический</span><span class="sxs-lookup"><span data-stu-id="6ea21-214">Boolean</span></span>|<span data-ttu-id="6ea21-215">Запомнить учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ea21-215">Remember user credentials.</span></span>|
|<span data-ttu-id="6ea21-216">Днссуффикссеарчлист</span><span class="sxs-lookup"><span data-stu-id="6ea21-216">dnsSuffixSearchList</span></span>|<span data-ttu-id="6ea21-217">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6ea21-217">String collection</span></span>|<span data-ttu-id="6ea21-218">Список поиска DNS-суффиксов.</span><span class="sxs-lookup"><span data-stu-id="6ea21-218">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="6ea21-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ea21-219">Response</span></span>
<span data-ttu-id="6ea21-220">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6ea21-220">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ea21-221">Пример</span><span class="sxs-lookup"><span data-stu-id="6ea21-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ea21-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ea21-222">Request</span></span>
<span data-ttu-id="6ea21-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ea21-223">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6ea21-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ea21-224">Response</span></span>
<span data-ttu-id="6ea21-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6ea21-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




