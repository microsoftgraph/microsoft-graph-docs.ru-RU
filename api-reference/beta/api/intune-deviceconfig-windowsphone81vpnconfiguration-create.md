---
title: Создание windowsPhone81VpnConfiguration
description: Создание нового объекта windowsPhone81VpnConfiguration.
ms.openlocfilehash: 8b4fb7ad9118ae91712cfd74ca78e7654e5db601
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082052"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="17248-103">Создание windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="17248-103">Create windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="17248-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="17248-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17248-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17248-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17248-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="17248-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17248-107">Создание нового объекта [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="17248-107">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="17248-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="17248-108">Prerequisites</span></span>
<span data-ttu-id="17248-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17248-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17248-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17248-111">Permission type</span></span>|<span data-ttu-id="17248-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="17248-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17248-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17248-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17248-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17248-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17248-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17248-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17248-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17248-116">Not supported.</span></span>|
|<span data-ttu-id="17248-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17248-117">Application</span></span>|<span data-ttu-id="17248-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17248-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17248-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17248-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="17248-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17248-120">Request headers</span></span>
|<span data-ttu-id="17248-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17248-121">Header</span></span>|<span data-ttu-id="17248-122">Значение</span><span class="sxs-lookup"><span data-stu-id="17248-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17248-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="17248-123">Authorization</span></span>|<span data-ttu-id="17248-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="17248-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17248-125">Accept</span><span class="sxs-lookup"><span data-stu-id="17248-125">Accept</span></span>|<span data-ttu-id="17248-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17248-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17248-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17248-127">Request body</span></span>
<span data-ttu-id="17248-128">В тексте запроса укажите представление JSON для объекта windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="17248-128">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="17248-129">В следующей таблице показаны свойства, которые необходимы для создания windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="17248-129">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="17248-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="17248-130">Property</span></span>|<span data-ttu-id="17248-131">Тип</span><span class="sxs-lookup"><span data-stu-id="17248-131">Type</span></span>|<span data-ttu-id="17248-132">Описание</span><span class="sxs-lookup"><span data-stu-id="17248-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17248-133">id</span><span class="sxs-lookup"><span data-stu-id="17248-133">id</span></span>|<span data-ttu-id="17248-134">String</span><span class="sxs-lookup"><span data-stu-id="17248-134">String</span></span>|<span data-ttu-id="17248-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="17248-135">Key of the entity.</span></span> <span data-ttu-id="17248-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17248-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17248-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17248-137">lastModifiedDateTime</span></span>|<span data-ttu-id="17248-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17248-138">DateTimeOffset</span></span>|<span data-ttu-id="17248-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="17248-139">DateTime the object was last modified.</span></span> <span data-ttu-id="17248-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17248-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17248-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="17248-141">roleScopeTagIds</span></span>|<span data-ttu-id="17248-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="17248-142">String collection</span></span>|<span data-ttu-id="17248-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="17248-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="17248-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17248-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17248-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="17248-145">supportsScopeTags</span></span>|<span data-ttu-id="17248-146">Логический</span><span class="sxs-lookup"><span data-stu-id="17248-146">Boolean</span></span>|<span data-ttu-id="17248-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="17248-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="17248-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="17248-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="17248-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="17248-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="17248-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17248-150">This property is read-only.</span></span> <span data-ttu-id="17248-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17248-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17248-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17248-152">createdDateTime</span></span>|<span data-ttu-id="17248-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17248-153">DateTimeOffset</span></span>|<span data-ttu-id="17248-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="17248-154">DateTime the object was created.</span></span> <span data-ttu-id="17248-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17248-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17248-156">описание</span><span class="sxs-lookup"><span data-stu-id="17248-156">description</span></span>|<span data-ttu-id="17248-157">String</span><span class="sxs-lookup"><span data-stu-id="17248-157">String</span></span>|<span data-ttu-id="17248-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="17248-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="17248-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17248-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17248-160">displayName</span><span class="sxs-lookup"><span data-stu-id="17248-160">displayName</span></span>|<span data-ttu-id="17248-161">String</span><span class="sxs-lookup"><span data-stu-id="17248-161">String</span></span>|<span data-ttu-id="17248-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="17248-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="17248-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17248-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17248-164">version</span><span class="sxs-lookup"><span data-stu-id="17248-164">version</span></span>|<span data-ttu-id="17248-165">Int32</span><span class="sxs-lookup"><span data-stu-id="17248-165">Int32</span></span>|<span data-ttu-id="17248-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="17248-166">Version of the device configuration.</span></span> <span data-ttu-id="17248-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17248-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17248-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="17248-168">connectionName</span></span>|<span data-ttu-id="17248-169">String</span><span class="sxs-lookup"><span data-stu-id="17248-169">String</span></span>|<span data-ttu-id="17248-170">Имя подключения отображается для пользователя.</span><span class="sxs-lookup"><span data-stu-id="17248-170">Connection name displayed to the user.</span></span> <span data-ttu-id="17248-171">Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17248-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="17248-172">серверы</span><span class="sxs-lookup"><span data-stu-id="17248-172">servers</span></span>|<span data-ttu-id="17248-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="17248-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="17248-174">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="17248-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="17248-175">Убедитесь, что конечные пользователи могут получить доступ к эти расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="17248-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="17248-176">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="17248-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="17248-177">Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17248-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="17248-178">customXml</span><span class="sxs-lookup"><span data-stu-id="17248-178">customXml</span></span>|<span data-ttu-id="17248-179">Двоичный</span><span class="sxs-lookup"><span data-stu-id="17248-179">Binary</span></span>|<span data-ttu-id="17248-180">Настраиваемые команды XML, которые настраиваются VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="17248-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="17248-181">(UTF8 закодированный массив байтов) Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17248-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="17248-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="17248-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="17248-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="17248-183">Boolean</span></span>|<span data-ttu-id="17248-184">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="17248-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="17248-185">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17248-185">This property is read-only.</span></span> <span data-ttu-id="17248-186">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17248-186">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="17248-187">Тип подключения</span><span class="sxs-lookup"><span data-stu-id="17248-187">connectionType</span></span>|[<span data-ttu-id="17248-188">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="17248-188">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="17248-189">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="17248-189">Connection type.</span></span> <span data-ttu-id="17248-190">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="17248-190">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="17248-191">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="17248-191">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="17248-192">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="17248-192">loginGroupOrDomain</span></span>|<span data-ttu-id="17248-193">String</span><span class="sxs-lookup"><span data-stu-id="17248-193">String</span></span>|<span data-ttu-id="17248-194">Группа для входа или домена, если тип подключения задано значение Dell SonicWALL Mobile подключения.</span><span class="sxs-lookup"><span data-stu-id="17248-194">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="17248-195">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17248-195">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="17248-196">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="17248-196">enableSplitTunneling</span></span>|<span data-ttu-id="17248-197">Логический</span><span class="sxs-lookup"><span data-stu-id="17248-197">Boolean</span></span>|<span data-ttu-id="17248-198">Включение разделенное туннелирование сети VPN.</span><span class="sxs-lookup"><span data-stu-id="17248-198">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="17248-199">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17248-199">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="17248-200">прокси-серверу</span><span class="sxs-lookup"><span data-stu-id="17248-200">proxyServer</span></span>|[<span data-ttu-id="17248-201">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="17248-201">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="17248-202">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="17248-202">Proxy Server.</span></span> <span data-ttu-id="17248-203">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17248-203">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="17248-204">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="17248-204">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="17248-205">Логический</span><span class="sxs-lookup"><span data-stu-id="17248-205">Boolean</span></span>|<span data-ttu-id="17248-206">Обход сервера-посредника VPN на компании Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="17248-206">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="17248-207">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="17248-207">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="17248-208">Логический</span><span class="sxs-lookup"><span data-stu-id="17248-208">Boolean</span></span>|<span data-ttu-id="17248-209">Обход сервера-посредника VPN на домашний Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="17248-209">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="17248-210">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="17248-210">authenticationMethod</span></span>|[<span data-ttu-id="17248-211">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="17248-211">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="17248-212">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="17248-212">Authentication method.</span></span> <span data-ttu-id="17248-213">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="17248-213">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="17248-214">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="17248-214">rememberUserCredentials</span></span>|<span data-ttu-id="17248-215">Логический</span><span class="sxs-lookup"><span data-stu-id="17248-215">Boolean</span></span>|<span data-ttu-id="17248-216">Не забудьте учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="17248-216">Remember user credentials.</span></span>|
|<span data-ttu-id="17248-217">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="17248-217">dnsSuffixSearchList</span></span>|<span data-ttu-id="17248-218">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="17248-218">String collection</span></span>|<span data-ttu-id="17248-219">Список поиска суффиксов DNS.</span><span class="sxs-lookup"><span data-stu-id="17248-219">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="17248-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="17248-220">Response</span></span>
<span data-ttu-id="17248-221">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="17248-221">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17248-222">Пример</span><span class="sxs-lookup"><span data-stu-id="17248-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="17248-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="17248-223">Request</span></span>
<span data-ttu-id="17248-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17248-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1307

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="17248-225">Ответ</span><span class="sxs-lookup"><span data-stu-id="17248-225">Response</span></span>
<span data-ttu-id="17248-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="17248-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





