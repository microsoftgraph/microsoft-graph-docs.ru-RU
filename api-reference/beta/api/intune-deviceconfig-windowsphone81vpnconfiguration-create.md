---
title: Создание windowsPhone81VpnConfiguration
description: Создание нового объекта windowsPhone81VpnConfiguration.
author: tfitzmac
ms.openlocfilehash: 3880742f3c0ccafcf647b7747cba1d63d90def73
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352922"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="3843f-103">Создание windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3843f-103">Create windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="3843f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3843f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3843f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3843f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3843f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3843f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3843f-107">Создание нового объекта [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3843f-107">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3843f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3843f-108">Prerequisites</span></span>
<span data-ttu-id="3843f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3843f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3843f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3843f-111">Permission type</span></span>|<span data-ttu-id="3843f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3843f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3843f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3843f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3843f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3843f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3843f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3843f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3843f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3843f-116">Not supported.</span></span>|
|<span data-ttu-id="3843f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3843f-117">Application</span></span>|<span data-ttu-id="3843f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3843f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3843f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3843f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3843f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3843f-120">Request headers</span></span>
|<span data-ttu-id="3843f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3843f-121">Header</span></span>|<span data-ttu-id="3843f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3843f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3843f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3843f-123">Authorization</span></span>|<span data-ttu-id="3843f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3843f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3843f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3843f-125">Accept</span></span>|<span data-ttu-id="3843f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3843f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3843f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3843f-127">Request body</span></span>
<span data-ttu-id="3843f-128">В тексте запроса укажите представление JSON для объекта windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3843f-128">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="3843f-129">В следующей таблице показаны свойства, которые необходимы для создания windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3843f-129">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="3843f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3843f-130">Property</span></span>|<span data-ttu-id="3843f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3843f-131">Type</span></span>|<span data-ttu-id="3843f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3843f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3843f-133">id</span><span class="sxs-lookup"><span data-stu-id="3843f-133">id</span></span>|<span data-ttu-id="3843f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3843f-134">String</span></span>|<span data-ttu-id="3843f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3843f-135">Key of the entity.</span></span> <span data-ttu-id="3843f-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3843f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3843f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3843f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3843f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3843f-138">DateTimeOffset</span></span>|<span data-ttu-id="3843f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3843f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3843f-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3843f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3843f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3843f-141">roleScopeTagIds</span></span>|<span data-ttu-id="3843f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3843f-142">String collection</span></span>|<span data-ttu-id="3843f-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3843f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3843f-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3843f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3843f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3843f-145">supportsScopeTags</span></span>|<span data-ttu-id="3843f-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="3843f-146">Boolean</span></span>|<span data-ttu-id="3843f-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="3843f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3843f-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="3843f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3843f-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3843f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3843f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3843f-150">This property is read-only.</span></span> <span data-ttu-id="3843f-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3843f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3843f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3843f-152">createdDateTime</span></span>|<span data-ttu-id="3843f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3843f-153">DateTimeOffset</span></span>|<span data-ttu-id="3843f-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3843f-154">DateTime the object was created.</span></span> <span data-ttu-id="3843f-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3843f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3843f-156">описание</span><span class="sxs-lookup"><span data-stu-id="3843f-156">description</span></span>|<span data-ttu-id="3843f-157">Строка</span><span class="sxs-lookup"><span data-stu-id="3843f-157">String</span></span>|<span data-ttu-id="3843f-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3843f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3843f-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3843f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3843f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="3843f-160">displayName</span></span>|<span data-ttu-id="3843f-161">Строка</span><span class="sxs-lookup"><span data-stu-id="3843f-161">String</span></span>|<span data-ttu-id="3843f-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3843f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3843f-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3843f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3843f-164">version</span><span class="sxs-lookup"><span data-stu-id="3843f-164">version</span></span>|<span data-ttu-id="3843f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3843f-165">Int32</span></span>|<span data-ttu-id="3843f-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3843f-166">Version of the device configuration.</span></span> <span data-ttu-id="3843f-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3843f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3843f-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="3843f-168">connectionName</span></span>|<span data-ttu-id="3843f-169">String.</span><span class="sxs-lookup"><span data-stu-id="3843f-169">String</span></span>|<span data-ttu-id="3843f-170">Имя подключения отображается для пользователя.</span><span class="sxs-lookup"><span data-stu-id="3843f-170">Connection name displayed to the user.</span></span> <span data-ttu-id="3843f-171">Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3843f-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="3843f-172">серверы</span><span class="sxs-lookup"><span data-stu-id="3843f-172">servers</span></span>|<span data-ttu-id="3843f-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="3843f-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="3843f-174">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="3843f-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="3843f-175">Убедитесь, что конечные пользователи могут получить доступ к эти расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="3843f-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="3843f-176">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3843f-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="3843f-177">Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3843f-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="3843f-178">customXml</span><span class="sxs-lookup"><span data-stu-id="3843f-178">customXml</span></span>|<span data-ttu-id="3843f-179">Binary</span><span class="sxs-lookup"><span data-stu-id="3843f-179">Binary</span></span>|<span data-ttu-id="3843f-180">Настраиваемые команды XML, которые настраиваются VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="3843f-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="3843f-181">(UTF8 закодированный массив байтов) Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3843f-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="3843f-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="3843f-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="3843f-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="3843f-183">Boolean</span></span>|<span data-ttu-id="3843f-184">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="3843f-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="3843f-185">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3843f-185">This property is read-only.</span></span> <span data-ttu-id="3843f-186">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3843f-186">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="3843f-187">Тип подключения</span><span class="sxs-lookup"><span data-stu-id="3843f-187">connectionType</span></span>|[<span data-ttu-id="3843f-188">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="3843f-188">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="3843f-189">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="3843f-189">Connection type.</span></span> <span data-ttu-id="3843f-190">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3843f-190">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="3843f-191">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="3843f-191">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="3843f-192">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="3843f-192">loginGroupOrDomain</span></span>|<span data-ttu-id="3843f-193">String.</span><span class="sxs-lookup"><span data-stu-id="3843f-193">String</span></span>|<span data-ttu-id="3843f-194">Группа для входа или домена, если тип подключения задано значение Dell SonicWALL Mobile подключения.</span><span class="sxs-lookup"><span data-stu-id="3843f-194">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="3843f-195">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3843f-195">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="3843f-196">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="3843f-196">enableSplitTunneling</span></span>|<span data-ttu-id="3843f-197">Boolean.</span><span class="sxs-lookup"><span data-stu-id="3843f-197">Boolean</span></span>|<span data-ttu-id="3843f-198">Включение разделенное туннелирование сети VPN.</span><span class="sxs-lookup"><span data-stu-id="3843f-198">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="3843f-199">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3843f-199">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="3843f-200">прокси-серверу</span><span class="sxs-lookup"><span data-stu-id="3843f-200">proxyServer</span></span>|[<span data-ttu-id="3843f-201">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="3843f-201">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="3843f-202">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="3843f-202">Proxy Server.</span></span> <span data-ttu-id="3843f-203">Наследуется от [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3843f-203">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="3843f-204">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="3843f-204">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="3843f-205">Boolean.</span><span class="sxs-lookup"><span data-stu-id="3843f-205">Boolean</span></span>|<span data-ttu-id="3843f-206">Обход сервера-посредника VPN на компании Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="3843f-206">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="3843f-207">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="3843f-207">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="3843f-208">Boolean.</span><span class="sxs-lookup"><span data-stu-id="3843f-208">Boolean</span></span>|<span data-ttu-id="3843f-209">Обход сервера-посредника VPN на домашний Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="3843f-209">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="3843f-210">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3843f-210">authenticationMethod</span></span>|[<span data-ttu-id="3843f-211">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3843f-211">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="3843f-212">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="3843f-212">Authentication method.</span></span> <span data-ttu-id="3843f-213">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="3843f-213">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="3843f-214">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="3843f-214">rememberUserCredentials</span></span>|<span data-ttu-id="3843f-215">Boolean.</span><span class="sxs-lookup"><span data-stu-id="3843f-215">Boolean</span></span>|<span data-ttu-id="3843f-216">Не забудьте учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="3843f-216">Remember user credentials.</span></span>|
|<span data-ttu-id="3843f-217">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="3843f-217">dnsSuffixSearchList</span></span>|<span data-ttu-id="3843f-218">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3843f-218">String collection</span></span>|<span data-ttu-id="3843f-219">Список поиска суффиксов DNS.</span><span class="sxs-lookup"><span data-stu-id="3843f-219">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="3843f-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="3843f-220">Response</span></span>
<span data-ttu-id="3843f-221">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3843f-221">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3843f-222">Пример</span><span class="sxs-lookup"><span data-stu-id="3843f-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="3843f-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="3843f-223">Request</span></span>
<span data-ttu-id="3843f-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3843f-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3843f-225">Ответ</span><span class="sxs-lookup"><span data-stu-id="3843f-225">Response</span></span>
<span data-ttu-id="3843f-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3843f-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





