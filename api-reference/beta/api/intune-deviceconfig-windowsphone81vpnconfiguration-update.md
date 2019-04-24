---
title: Обновление windowsPhone81VpnConfiguration
description: Обновление свойств объекта windowsPhone81VpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1e5f8726dc820ec352326f61e73aa77e725ccefa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32512623"
---
# <a name="update-windowsphone81vpnconfiguration"></a><span data-ttu-id="f4d06-103">Обновление windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4d06-103">Update windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="f4d06-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4d06-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4d06-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4d06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4d06-106">Обновление свойств объекта [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f4d06-106">Update the properties of a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4d06-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f4d06-107">Prerequisites</span></span>
<span data-ttu-id="f4d06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4d06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4d06-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4d06-110">Permission type</span></span>|<span data-ttu-id="f4d06-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4d06-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4d06-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4d06-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4d06-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4d06-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4d06-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4d06-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4d06-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4d06-115">Not supported.</span></span>|
|<span data-ttu-id="f4d06-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4d06-116">Application</span></span>|<span data-ttu-id="f4d06-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4d06-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4d06-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4d06-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f4d06-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4d06-119">Request headers</span></span>
|<span data-ttu-id="f4d06-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4d06-120">Header</span></span>|<span data-ttu-id="f4d06-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f4d06-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4d06-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4d06-122">Authorization</span></span>|<span data-ttu-id="f4d06-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4d06-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4d06-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f4d06-124">Accept</span></span>|<span data-ttu-id="f4d06-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4d06-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4d06-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4d06-126">Request body</span></span>
<span data-ttu-id="f4d06-127">В тексте запроса добавьте представление объекта [WindowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4d06-127">In the request body, supply a JSON representation for the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="f4d06-128">В следующей таблице приведены свойства, необходимые при создании [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4d06-128">The following table shows the properties that are required when you create the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span></span>

|<span data-ttu-id="f4d06-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4d06-129">Property</span></span>|<span data-ttu-id="f4d06-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f4d06-130">Type</span></span>|<span data-ttu-id="f4d06-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f4d06-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4d06-132">id</span><span class="sxs-lookup"><span data-stu-id="f4d06-132">id</span></span>|<span data-ttu-id="f4d06-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f4d06-133">String</span></span>|<span data-ttu-id="f4d06-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f4d06-134">Key of the entity.</span></span> <span data-ttu-id="f4d06-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4d06-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4d06-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4d06-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f4d06-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4d06-137">DateTimeOffset</span></span>|<span data-ttu-id="f4d06-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f4d06-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f4d06-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4d06-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4d06-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f4d06-140">roleScopeTagIds</span></span>|<span data-ttu-id="f4d06-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f4d06-141">String collection</span></span>|<span data-ttu-id="f4d06-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f4d06-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f4d06-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4d06-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4d06-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f4d06-144">supportsScopeTags</span></span>|<span data-ttu-id="f4d06-145">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d06-145">Boolean</span></span>|<span data-ttu-id="f4d06-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f4d06-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f4d06-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f4d06-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f4d06-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f4d06-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f4d06-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4d06-149">This property is read-only.</span></span> <span data-ttu-id="f4d06-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4d06-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4d06-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4d06-151">createdDateTime</span></span>|<span data-ttu-id="f4d06-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4d06-152">DateTimeOffset</span></span>|<span data-ttu-id="f4d06-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f4d06-153">DateTime the object was created.</span></span> <span data-ttu-id="f4d06-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4d06-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4d06-155">description</span><span class="sxs-lookup"><span data-stu-id="f4d06-155">description</span></span>|<span data-ttu-id="f4d06-156">String</span><span class="sxs-lookup"><span data-stu-id="f4d06-156">String</span></span>|<span data-ttu-id="f4d06-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f4d06-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f4d06-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4d06-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4d06-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f4d06-159">displayName</span></span>|<span data-ttu-id="f4d06-160">String</span><span class="sxs-lookup"><span data-stu-id="f4d06-160">String</span></span>|<span data-ttu-id="f4d06-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f4d06-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f4d06-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4d06-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4d06-163">version</span><span class="sxs-lookup"><span data-stu-id="f4d06-163">version</span></span>|<span data-ttu-id="f4d06-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f4d06-164">Int32</span></span>|<span data-ttu-id="f4d06-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f4d06-165">Version of the device configuration.</span></span> <span data-ttu-id="f4d06-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4d06-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4d06-167">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="f4d06-167">connectionName</span></span>|<span data-ttu-id="f4d06-168">String</span><span class="sxs-lookup"><span data-stu-id="f4d06-168">String</span></span>|<span data-ttu-id="f4d06-169">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4d06-169">Connection name displayed to the user.</span></span> <span data-ttu-id="f4d06-170">НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4d06-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4d06-171">серверами</span><span class="sxs-lookup"><span data-stu-id="f4d06-171">servers</span></span>|<span data-ttu-id="f4d06-172">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="f4d06-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="f4d06-173">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="f4d06-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="f4d06-174">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="f4d06-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="f4d06-175">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f4d06-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f4d06-176">НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4d06-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4d06-177">customXml</span><span class="sxs-lookup"><span data-stu-id="f4d06-177">customXml</span></span>|<span data-ttu-id="f4d06-178">Binary</span><span class="sxs-lookup"><span data-stu-id="f4d06-178">Binary</span></span>|<span data-ttu-id="f4d06-179">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="f4d06-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="f4d06-180">(Массив байтов в кодировке UTF8) НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4d06-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4d06-181">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="f4d06-181">applyOnlyToWindows81</span></span>|<span data-ttu-id="f4d06-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4d06-182">Boolean</span></span>|<span data-ttu-id="f4d06-183">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="f4d06-183">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="f4d06-184">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4d06-184">This property is read-only.</span></span> <span data-ttu-id="f4d06-185">НаСледуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4d06-185">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4d06-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="f4d06-186">connectionType</span></span>|[<span data-ttu-id="f4d06-187">Виндовсвпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="f4d06-187">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="f4d06-188">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="f4d06-188">Connection type.</span></span> <span data-ttu-id="f4d06-189">НаСледуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4d06-189">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="f4d06-190">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="f4d06-190">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="f4d06-191">Логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="f4d06-191">loginGroupOrDomain</span></span>|<span data-ttu-id="f4d06-192">String</span><span class="sxs-lookup"><span data-stu-id="f4d06-192">String</span></span>|<span data-ttu-id="f4d06-193">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="f4d06-193">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="f4d06-194">НаСледуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4d06-194">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4d06-195">Енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="f4d06-195">enableSplitTunneling</span></span>|<span data-ttu-id="f4d06-196">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d06-196">Boolean</span></span>|<span data-ttu-id="f4d06-197">Включение Расщепленного туннелирования для VPN.</span><span class="sxs-lookup"><span data-stu-id="f4d06-197">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="f4d06-198">НаСледуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4d06-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4d06-199">проксисервер</span><span class="sxs-lookup"><span data-stu-id="f4d06-199">proxyServer</span></span>|[<span data-ttu-id="f4d06-200">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="f4d06-200">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="f4d06-201">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="f4d06-201">Proxy Server.</span></span> <span data-ttu-id="f4d06-202">НаСледуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f4d06-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="f4d06-203">Бипассвпнонкомпанивифи</span><span class="sxs-lookup"><span data-stu-id="f4d06-203">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="f4d06-204">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d06-204">Boolean</span></span>|<span data-ttu-id="f4d06-205">Обход VPN в сети Wi-Fi компании.</span><span class="sxs-lookup"><span data-stu-id="f4d06-205">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="f4d06-206">Бипассвпнонхомевифи</span><span class="sxs-lookup"><span data-stu-id="f4d06-206">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="f4d06-207">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d06-207">Boolean</span></span>|<span data-ttu-id="f4d06-208">Обход VPN для домашнего Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f4d06-208">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="f4d06-209">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="f4d06-209">authenticationMethod</span></span>|[<span data-ttu-id="f4d06-210">Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="f4d06-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="f4d06-211">Метод проверки поДлинности.</span><span class="sxs-lookup"><span data-stu-id="f4d06-211">Authentication method.</span></span> <span data-ttu-id="f4d06-212">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="f4d06-212">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="f4d06-213">Ремемберусеркредентиалс</span><span class="sxs-lookup"><span data-stu-id="f4d06-213">rememberUserCredentials</span></span>|<span data-ttu-id="f4d06-214">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d06-214">Boolean</span></span>|<span data-ttu-id="f4d06-215">Запомнить учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4d06-215">Remember user credentials.</span></span>|
|<span data-ttu-id="f4d06-216">Днссуффикссеарчлист</span><span class="sxs-lookup"><span data-stu-id="f4d06-216">dnsSuffixSearchList</span></span>|<span data-ttu-id="f4d06-217">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f4d06-217">String collection</span></span>|<span data-ttu-id="f4d06-218">Список поиска DNS-суффиксов.</span><span class="sxs-lookup"><span data-stu-id="f4d06-218">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="f4d06-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4d06-219">Response</span></span>
<span data-ttu-id="f4d06-220">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f4d06-220">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4d06-221">Пример</span><span class="sxs-lookup"><span data-stu-id="f4d06-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4d06-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4d06-222">Request</span></span>
<span data-ttu-id="f4d06-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4d06-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="f4d06-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4d06-224">Response</span></span>
<span data-ttu-id="f4d06-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4d06-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





