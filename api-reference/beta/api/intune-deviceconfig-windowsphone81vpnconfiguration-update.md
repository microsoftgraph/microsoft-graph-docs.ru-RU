---
title: Обновление windowsPhone81VpnConfiguration
description: Обновление свойства объекта windowsPhone81VpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b8bab7e2c0f6e5ba4e358de03cadc396593fc04b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836479"
---
# <a name="update-windowsphone81vpnconfiguration"></a><span data-ttu-id="67cf6-103">Обновление windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="67cf6-103">Update windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="67cf6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="67cf6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67cf6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67cf6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67cf6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="67cf6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67cf6-107">Обновление свойства объекта [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="67cf6-107">Update the properties of a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="67cf6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="67cf6-108">Prerequisites</span></span>
<span data-ttu-id="67cf6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67cf6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67cf6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67cf6-111">Permission type</span></span>|<span data-ttu-id="67cf6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="67cf6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67cf6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67cf6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67cf6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67cf6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="67cf6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67cf6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67cf6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67cf6-116">Not supported.</span></span>|
|<span data-ttu-id="67cf6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67cf6-117">Application</span></span>|<span data-ttu-id="67cf6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67cf6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67cf6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67cf6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="67cf6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67cf6-120">Request headers</span></span>
|<span data-ttu-id="67cf6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="67cf6-121">Header</span></span>|<span data-ttu-id="67cf6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="67cf6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67cf6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="67cf6-123">Authorization</span></span>|<span data-ttu-id="67cf6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="67cf6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67cf6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="67cf6-125">Accept</span></span>|<span data-ttu-id="67cf6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="67cf6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67cf6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="67cf6-127">Request body</span></span>
<span data-ttu-id="67cf6-128">В тексте запроса укажите представление JSON для объекта [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="67cf6-128">In the request body, supply a JSON representation for the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="67cf6-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67cf6-129">The following table shows the properties that are required when you create the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span></span>

|<span data-ttu-id="67cf6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="67cf6-130">Property</span></span>|<span data-ttu-id="67cf6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="67cf6-131">Type</span></span>|<span data-ttu-id="67cf6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="67cf6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67cf6-133">id</span><span class="sxs-lookup"><span data-stu-id="67cf6-133">id</span></span>|<span data-ttu-id="67cf6-134">Строка</span><span class="sxs-lookup"><span data-stu-id="67cf6-134">String</span></span>|<span data-ttu-id="67cf6-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="67cf6-135">Key of the entity.</span></span> <span data-ttu-id="67cf6-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67cf6-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67cf6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67cf6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="67cf6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67cf6-138">DateTimeOffset</span></span>|<span data-ttu-id="67cf6-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="67cf6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="67cf6-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67cf6-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67cf6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="67cf6-141">roleScopeTagIds</span></span>|<span data-ttu-id="67cf6-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="67cf6-142">String collection</span></span>|<span data-ttu-id="67cf6-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="67cf6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="67cf6-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67cf6-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67cf6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="67cf6-145">supportsScopeTags</span></span>|<span data-ttu-id="67cf6-146">Логический</span><span class="sxs-lookup"><span data-stu-id="67cf6-146">Boolean</span></span>|<span data-ttu-id="67cf6-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="67cf6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="67cf6-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="67cf6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="67cf6-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="67cf6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="67cf6-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="67cf6-150">This property is read-only.</span></span> <span data-ttu-id="67cf6-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67cf6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67cf6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67cf6-152">createdDateTime</span></span>|<span data-ttu-id="67cf6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67cf6-153">DateTimeOffset</span></span>|<span data-ttu-id="67cf6-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="67cf6-154">DateTime the object was created.</span></span> <span data-ttu-id="67cf6-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67cf6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67cf6-156">описание</span><span class="sxs-lookup"><span data-stu-id="67cf6-156">description</span></span>|<span data-ttu-id="67cf6-157">Строка</span><span class="sxs-lookup"><span data-stu-id="67cf6-157">String</span></span>|<span data-ttu-id="67cf6-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="67cf6-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="67cf6-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67cf6-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67cf6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="67cf6-160">displayName</span></span>|<span data-ttu-id="67cf6-161">Строка</span><span class="sxs-lookup"><span data-stu-id="67cf6-161">String</span></span>|<span data-ttu-id="67cf6-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="67cf6-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="67cf6-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67cf6-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67cf6-164">version</span><span class="sxs-lookup"><span data-stu-id="67cf6-164">version</span></span>|<span data-ttu-id="67cf6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="67cf6-165">Int32</span></span>|<span data-ttu-id="67cf6-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="67cf6-166">Version of the device configuration.</span></span> <span data-ttu-id="67cf6-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67cf6-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67cf6-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="67cf6-168">connectionName</span></span>|<span data-ttu-id="67cf6-169">Строка</span><span class="sxs-lookup"><span data-stu-id="67cf6-169">String</span></span>|<span data-ttu-id="67cf6-170">Имя подключения отображается для пользователя.</span><span class="sxs-lookup"><span data-stu-id="67cf6-170">Connection name displayed to the user.</span></span> <span data-ttu-id="67cf6-171">Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67cf6-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="67cf6-172">серверы</span><span class="sxs-lookup"><span data-stu-id="67cf6-172">servers</span></span>|<span data-ttu-id="67cf6-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="67cf6-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="67cf6-174">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="67cf6-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="67cf6-175">Убедитесь, что конечные пользователи могут получить доступ к эти расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="67cf6-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="67cf6-176">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="67cf6-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="67cf6-177">Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67cf6-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="67cf6-178">customXml</span><span class="sxs-lookup"><span data-stu-id="67cf6-178">customXml</span></span>|<span data-ttu-id="67cf6-179">Binary</span><span class="sxs-lookup"><span data-stu-id="67cf6-179">Binary</span></span>|<span data-ttu-id="67cf6-180">Настраиваемые команды XML, которые настраиваются VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="67cf6-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="67cf6-181">(UTF8 закодированный массив байтов) Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67cf6-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="67cf6-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="67cf6-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="67cf6-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="67cf6-183">Boolean</span></span>|<span data-ttu-id="67cf6-184">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="67cf6-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="67cf6-185">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="67cf6-185">This property is read-only.</span></span> <span data-ttu-id="67cf6-186">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67cf6-186">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="67cf6-187">Тип подключения</span><span class="sxs-lookup"><span data-stu-id="67cf6-187">connectionType</span></span>|[<span data-ttu-id="67cf6-188">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="67cf6-188">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="67cf6-189">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="67cf6-189">Connection type.</span></span> <span data-ttu-id="67cf6-190">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67cf6-190">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="67cf6-191">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="67cf6-191">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="67cf6-192">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="67cf6-192">loginGroupOrDomain</span></span>|<span data-ttu-id="67cf6-193">Строка</span><span class="sxs-lookup"><span data-stu-id="67cf6-193">String</span></span>|<span data-ttu-id="67cf6-194">Группа для входа или домена, если тип подключения задано значение Dell SonicWALL Mobile подключения.</span><span class="sxs-lookup"><span data-stu-id="67cf6-194">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="67cf6-195">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67cf6-195">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="67cf6-196">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="67cf6-196">enableSplitTunneling</span></span>|<span data-ttu-id="67cf6-197">Логический</span><span class="sxs-lookup"><span data-stu-id="67cf6-197">Boolean</span></span>|<span data-ttu-id="67cf6-198">Включение разделенное туннелирование сети VPN.</span><span class="sxs-lookup"><span data-stu-id="67cf6-198">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="67cf6-199">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67cf6-199">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="67cf6-200">прокси-серверу</span><span class="sxs-lookup"><span data-stu-id="67cf6-200">proxyServer</span></span>|[<span data-ttu-id="67cf6-201">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="67cf6-201">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="67cf6-202">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="67cf6-202">Proxy Server.</span></span> <span data-ttu-id="67cf6-203">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67cf6-203">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="67cf6-204">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="67cf6-204">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="67cf6-205">Логический</span><span class="sxs-lookup"><span data-stu-id="67cf6-205">Boolean</span></span>|<span data-ttu-id="67cf6-206">Обход сервера-посредника VPN на компании Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="67cf6-206">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="67cf6-207">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="67cf6-207">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="67cf6-208">Логический</span><span class="sxs-lookup"><span data-stu-id="67cf6-208">Boolean</span></span>|<span data-ttu-id="67cf6-209">Обход сервера-посредника VPN на домашний Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="67cf6-209">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="67cf6-210">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="67cf6-210">authenticationMethod</span></span>|[<span data-ttu-id="67cf6-211">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="67cf6-211">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="67cf6-212">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="67cf6-212">Authentication method.</span></span> <span data-ttu-id="67cf6-213">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="67cf6-213">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="67cf6-214">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="67cf6-214">rememberUserCredentials</span></span>|<span data-ttu-id="67cf6-215">Логический</span><span class="sxs-lookup"><span data-stu-id="67cf6-215">Boolean</span></span>|<span data-ttu-id="67cf6-216">Не забудьте учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="67cf6-216">Remember user credentials.</span></span>|
|<span data-ttu-id="67cf6-217">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="67cf6-217">dnsSuffixSearchList</span></span>|<span data-ttu-id="67cf6-218">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="67cf6-218">String collection</span></span>|<span data-ttu-id="67cf6-219">Список поиска суффиксов DNS.</span><span class="sxs-lookup"><span data-stu-id="67cf6-219">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="67cf6-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="67cf6-220">Response</span></span>
<span data-ttu-id="67cf6-221">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="67cf6-221">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67cf6-222">Пример</span><span class="sxs-lookup"><span data-stu-id="67cf6-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="67cf6-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="67cf6-223">Request</span></span>
<span data-ttu-id="67cf6-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67cf6-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1238

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="67cf6-225">Ответ</span><span class="sxs-lookup"><span data-stu-id="67cf6-225">Response</span></span>
<span data-ttu-id="67cf6-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="67cf6-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





