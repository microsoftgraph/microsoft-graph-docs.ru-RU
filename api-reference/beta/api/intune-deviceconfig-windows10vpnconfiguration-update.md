---
title: Обновление windows10VpnConfiguration
description: Обновление свойства объекта windows10VpnConfiguration.
author: tfitzmac
ms.openlocfilehash: 24112120dd414bc7929d9223094b528b32ad818a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305070"
---
# <a name="update-windows10vpnconfiguration"></a><span data-ttu-id="f08c9-103">Обновление windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f08c9-103">Update windows10VpnConfiguration</span></span>

> <span data-ttu-id="f08c9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f08c9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f08c9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f08c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f08c9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f08c9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f08c9-107">Обновление свойства объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f08c9-107">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f08c9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f08c9-108">Prerequisites</span></span>
<span data-ttu-id="f08c9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f08c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f08c9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f08c9-111">Permission type</span></span>|<span data-ttu-id="f08c9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f08c9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f08c9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f08c9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f08c9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f08c9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f08c9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f08c9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f08c9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f08c9-116">Not supported.</span></span>|
|<span data-ttu-id="f08c9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f08c9-117">Application</span></span>|<span data-ttu-id="f08c9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f08c9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f08c9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f08c9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f08c9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f08c9-120">Request headers</span></span>
|<span data-ttu-id="f08c9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f08c9-121">Header</span></span>|<span data-ttu-id="f08c9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f08c9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f08c9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f08c9-123">Authorization</span></span>|<span data-ttu-id="f08c9-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f08c9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f08c9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f08c9-125">Accept</span></span>|<span data-ttu-id="f08c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f08c9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f08c9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f08c9-127">Request body</span></span>
<span data-ttu-id="f08c9-128">В тексте запроса укажите представление JSON для объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f08c9-128">In the request body, supply a JSON representation for the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

<span data-ttu-id="f08c9-129">В следующей таблице показаны свойства, которые необходимы для создания [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08c9-129">The following table shows the properties that are required when you create the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>

|<span data-ttu-id="f08c9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f08c9-130">Property</span></span>|<span data-ttu-id="f08c9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f08c9-131">Type</span></span>|<span data-ttu-id="f08c9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f08c9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f08c9-133">id</span><span class="sxs-lookup"><span data-stu-id="f08c9-133">id</span></span>|<span data-ttu-id="f08c9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f08c9-134">String</span></span>|<span data-ttu-id="f08c9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f08c9-135">Key of the entity.</span></span> <span data-ttu-id="f08c9-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08c9-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f08c9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f08c9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f08c9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f08c9-138">DateTimeOffset</span></span>|<span data-ttu-id="f08c9-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f08c9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f08c9-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08c9-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f08c9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f08c9-141">roleScopeTagIds</span></span>|<span data-ttu-id="f08c9-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f08c9-142">String collection</span></span>|<span data-ttu-id="f08c9-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f08c9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f08c9-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08c9-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f08c9-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f08c9-145">supportsScopeTags</span></span>|<span data-ttu-id="f08c9-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f08c9-146">Boolean</span></span>|<span data-ttu-id="f08c9-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="f08c9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f08c9-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="f08c9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f08c9-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f08c9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f08c9-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f08c9-150">This property is read-only.</span></span> <span data-ttu-id="f08c9-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08c9-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f08c9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f08c9-152">createdDateTime</span></span>|<span data-ttu-id="f08c9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f08c9-153">DateTimeOffset</span></span>|<span data-ttu-id="f08c9-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f08c9-154">DateTime the object was created.</span></span> <span data-ttu-id="f08c9-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08c9-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f08c9-156">описание</span><span class="sxs-lookup"><span data-stu-id="f08c9-156">description</span></span>|<span data-ttu-id="f08c9-157">Строка</span><span class="sxs-lookup"><span data-stu-id="f08c9-157">String</span></span>|<span data-ttu-id="f08c9-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f08c9-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f08c9-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08c9-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f08c9-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f08c9-160">displayName</span></span>|<span data-ttu-id="f08c9-161">Строка</span><span class="sxs-lookup"><span data-stu-id="f08c9-161">String</span></span>|<span data-ttu-id="f08c9-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f08c9-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f08c9-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08c9-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f08c9-164">version</span><span class="sxs-lookup"><span data-stu-id="f08c9-164">version</span></span>|<span data-ttu-id="f08c9-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f08c9-165">Int32</span></span>|<span data-ttu-id="f08c9-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f08c9-166">Version of the device configuration.</span></span> <span data-ttu-id="f08c9-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f08c9-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f08c9-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="f08c9-168">connectionName</span></span>|<span data-ttu-id="f08c9-169">String.</span><span class="sxs-lookup"><span data-stu-id="f08c9-169">String</span></span>|<span data-ttu-id="f08c9-170">Имя подключения отображается для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f08c9-170">Connection name displayed to the user.</span></span> <span data-ttu-id="f08c9-171">Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f08c9-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f08c9-172">серверы</span><span class="sxs-lookup"><span data-stu-id="f08c9-172">servers</span></span>|<span data-ttu-id="f08c9-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f08c9-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="f08c9-174">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="f08c9-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="f08c9-175">Убедитесь, что конечные пользователи могут получить доступ к эти расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="f08c9-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="f08c9-176">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f08c9-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f08c9-177">Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f08c9-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f08c9-178">customXml</span><span class="sxs-lookup"><span data-stu-id="f08c9-178">customXml</span></span>|<span data-ttu-id="f08c9-179">Binary</span><span class="sxs-lookup"><span data-stu-id="f08c9-179">Binary</span></span>|<span data-ttu-id="f08c9-180">Настраиваемые команды XML, которые настраиваются VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="f08c9-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="f08c9-181">(UTF8 закодированный массив байтов) Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f08c9-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f08c9-182">profileTarget</span><span class="sxs-lookup"><span data-stu-id="f08c9-182">profileTarget</span></span>|[<span data-ttu-id="f08c9-183">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="f08c9-183">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="f08c9-184">Тип конечного профиля.</span><span class="sxs-lookup"><span data-stu-id="f08c9-184">Profile target type.</span></span> <span data-ttu-id="f08c9-185">Возможные значения: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="f08c9-185">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="f08c9-186">Тип подключения</span><span class="sxs-lookup"><span data-stu-id="f08c9-186">connectionType</span></span>|[<span data-ttu-id="f08c9-187">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="f08c9-187">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="f08c9-188">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="f08c9-188">Connection type.</span></span> <span data-ttu-id="f08c9-189">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="f08c9-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="f08c9-190">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="f08c9-190">enableSplitTunneling</span></span>|<span data-ttu-id="f08c9-191">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f08c9-191">Boolean</span></span>|<span data-ttu-id="f08c9-192">Включение разделенное туннелирование.</span><span class="sxs-lookup"><span data-stu-id="f08c9-192">Enable split tunneling.</span></span>|
|<span data-ttu-id="f08c9-193">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="f08c9-193">enableAlwaysOn</span></span>|<span data-ttu-id="f08c9-194">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f08c9-194">Boolean</span></span>|<span data-ttu-id="f08c9-195">Включение режима всегда на.</span><span class="sxs-lookup"><span data-stu-id="f08c9-195">Enable Always On mode.</span></span>|
|<span data-ttu-id="f08c9-196">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="f08c9-196">enableDeviceTunnel</span></span>|<span data-ttu-id="f08c9-197">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f08c9-197">Boolean</span></span>|<span data-ttu-id="f08c9-198">Включение туннель устройства.</span><span class="sxs-lookup"><span data-stu-id="f08c9-198">Enable device tunnel.</span></span>|
|<span data-ttu-id="f08c9-199">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="f08c9-199">enableDnsRegistration</span></span>|<span data-ttu-id="f08c9-200">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f08c9-200">Boolean</span></span>|<span data-ttu-id="f08c9-201">Включение регистрации IP-адреса с внутренней DNS.</span><span class="sxs-lookup"><span data-stu-id="f08c9-201">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="f08c9-202">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="f08c9-202">dnsSuffixes</span></span>|<span data-ttu-id="f08c9-203">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f08c9-203">String collection</span></span>|<span data-ttu-id="f08c9-204">Укажите DNS-суффиксы для добавления в список поиска DNS маршрутизацию короткие имена.</span><span class="sxs-lookup"><span data-stu-id="f08c9-204">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="f08c9-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f08c9-205">authenticationMethod</span></span>|[<span data-ttu-id="f08c9-206">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f08c9-206">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="f08c9-207">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="f08c9-207">Authentication method.</span></span> <span data-ttu-id="f08c9-208">Возможные значения: `certificate`, `usernameAndPassword`, `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="f08c9-208">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="f08c9-209">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="f08c9-209">rememberUserCredentials</span></span>|<span data-ttu-id="f08c9-210">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f08c9-210">Boolean</span></span>|<span data-ttu-id="f08c9-211">Не забудьте учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="f08c9-211">Remember user credentials.</span></span>|
|<span data-ttu-id="f08c9-212">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="f08c9-212">enableConditionalAccess</span></span>|<span data-ttu-id="f08c9-213">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f08c9-213">Boolean</span></span>|<span data-ttu-id="f08c9-214">Включение условного доступа.</span><span class="sxs-lookup"><span data-stu-id="f08c9-214">Enable conditional access.</span></span>|
|<span data-ttu-id="f08c9-215">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="f08c9-215">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="f08c9-216">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f08c9-216">Boolean</span></span>|<span data-ttu-id="f08c9-217">Включение единого входа (SSO) с помощью альтернативного сертификата.</span><span class="sxs-lookup"><span data-stu-id="f08c9-217">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="f08c9-218">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="f08c9-218">singleSignOnEku</span></span>|[<span data-ttu-id="f08c9-219">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="f08c9-219">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="f08c9-220">Единого входа расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="f08c9-220">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="f08c9-221">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="f08c9-221">singleSignOnIssuerHash</span></span>|<span data-ttu-id="f08c9-222">String.</span><span class="sxs-lookup"><span data-stu-id="f08c9-222">String</span></span>|<span data-ttu-id="f08c9-223">Хэш-функции поставщика единого входа.</span><span class="sxs-lookup"><span data-stu-id="f08c9-223">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="f08c9-224">eapXml</span><span class="sxs-lookup"><span data-stu-id="f08c9-224">eapXml</span></span>|<span data-ttu-id="f08c9-225">Binary</span><span class="sxs-lookup"><span data-stu-id="f08c9-225">Binary</span></span>|<span data-ttu-id="f08c9-226">Протокол расширенной проверки подлинности (EAP) XML.</span><span class="sxs-lookup"><span data-stu-id="f08c9-226">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="f08c9-227">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="f08c9-227">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="f08c9-228">прокси-серверу</span><span class="sxs-lookup"><span data-stu-id="f08c9-228">proxyServer</span></span>|[<span data-ttu-id="f08c9-229">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="f08c9-229">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="f08c9-230">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="f08c9-230">Proxy Server.</span></span>|
|<span data-ttu-id="f08c9-231">associatedApps</span><span class="sxs-lookup"><span data-stu-id="f08c9-231">associatedApps</span></span>|<span data-ttu-id="f08c9-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f08c9-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="f08c9-233">Связанные приложения.</span><span class="sxs-lookup"><span data-stu-id="f08c9-233">Associated Apps.</span></span> <span data-ttu-id="f08c9-234">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="f08c9-234">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="f08c9-235">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="f08c9-235">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="f08c9-236">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f08c9-236">Boolean</span></span>|<span data-ttu-id="f08c9-237">Только связанного приложения могут использовать подключения (VPN-app).</span><span class="sxs-lookup"><span data-stu-id="f08c9-237">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="f08c9-238">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="f08c9-238">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="f08c9-239">String.</span><span class="sxs-lookup"><span data-stu-id="f08c9-239">String</span></span>|<span data-ttu-id="f08c9-240">Сведения о защите Windows (НЗП) домена, связанного с этим подключением.</span><span class="sxs-lookup"><span data-stu-id="f08c9-240">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="f08c9-241">trafficRules</span><span class="sxs-lookup"><span data-stu-id="f08c9-241">trafficRules</span></span>|<span data-ttu-id="f08c9-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f08c9-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="f08c9-243">Правила трафика.</span><span class="sxs-lookup"><span data-stu-id="f08c9-243">Traffic rules.</span></span> <span data-ttu-id="f08c9-244">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="f08c9-244">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="f08c9-245">маршруты</span><span class="sxs-lookup"><span data-stu-id="f08c9-245">routes</span></span>|<span data-ttu-id="f08c9-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f08c9-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="f08c9-247">Маршрутизация (не обязательно для сторонних поставщиков).</span><span class="sxs-lookup"><span data-stu-id="f08c9-247">Routes (optional for third-party providers).</span></span> <span data-ttu-id="f08c9-248">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="f08c9-248">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="f08c9-249">dnsRules</span><span class="sxs-lookup"><span data-stu-id="f08c9-249">dnsRules</span></span>|<span data-ttu-id="f08c9-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f08c9-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="f08c9-251">Правила DNS.</span><span class="sxs-lookup"><span data-stu-id="f08c9-251">DNS rules.</span></span> <span data-ttu-id="f08c9-252">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="f08c9-252">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f08c9-253">Ответ</span><span class="sxs-lookup"><span data-stu-id="f08c9-253">Response</span></span>
<span data-ttu-id="f08c9-254">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f08c9-254">If successful, this method returns a `200 OK` response code and an updated [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f08c9-255">Пример</span><span class="sxs-lookup"><span data-stu-id="f08c9-255">Example</span></span>
### <a name="request"></a><span data-ttu-id="f08c9-256">Запрос</span><span class="sxs-lookup"><span data-stu-id="f08c9-256">Request</span></span>
<span data-ttu-id="f08c9-257">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f08c9-257">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3259

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
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f08c9-258">Ответ</span><span class="sxs-lookup"><span data-stu-id="f08c9-258">Response</span></span>
<span data-ttu-id="f08c9-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f08c9-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3431

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
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
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value"
    }
  ]
}
```





