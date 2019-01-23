---
title: Обновление windows10VpnConfiguration
description: Обновление свойства объекта windows10VpnConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d2d6a7fda3dc357d91fbb56b7bd3e01e76152cd8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421608"
---
# <a name="update-windows10vpnconfiguration"></a><span data-ttu-id="0db54-103">Обновление windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0db54-103">Update windows10VpnConfiguration</span></span>

> <span data-ttu-id="0db54-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0db54-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0db54-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0db54-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0db54-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0db54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0db54-107">Обновление свойства объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0db54-107">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0db54-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="0db54-108">Prerequisites</span></span>
<span data-ttu-id="0db54-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0db54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0db54-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0db54-111">Permission type</span></span>|<span data-ttu-id="0db54-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0db54-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0db54-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0db54-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0db54-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0db54-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0db54-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0db54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0db54-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0db54-116">Not supported.</span></span>|
|<span data-ttu-id="0db54-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0db54-117">Application</span></span>|<span data-ttu-id="0db54-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0db54-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0db54-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0db54-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0db54-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0db54-120">Request headers</span></span>
|<span data-ttu-id="0db54-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0db54-121">Header</span></span>|<span data-ttu-id="0db54-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0db54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0db54-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0db54-123">Authorization</span></span>|<span data-ttu-id="0db54-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0db54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0db54-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0db54-125">Accept</span></span>|<span data-ttu-id="0db54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0db54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0db54-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0db54-127">Request body</span></span>
<span data-ttu-id="0db54-128">В тексте запроса укажите представление JSON для объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0db54-128">In the request body, supply a JSON representation for the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

<span data-ttu-id="0db54-129">В следующей таблице показаны свойства, которые необходимы для создания [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0db54-129">The following table shows the properties that are required when you create the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>

|<span data-ttu-id="0db54-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0db54-130">Property</span></span>|<span data-ttu-id="0db54-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0db54-131">Type</span></span>|<span data-ttu-id="0db54-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0db54-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0db54-133">id</span><span class="sxs-lookup"><span data-stu-id="0db54-133">id</span></span>|<span data-ttu-id="0db54-134">String</span><span class="sxs-lookup"><span data-stu-id="0db54-134">String</span></span>|<span data-ttu-id="0db54-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0db54-135">Key of the entity.</span></span> <span data-ttu-id="0db54-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0db54-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0db54-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0db54-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0db54-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0db54-138">DateTimeOffset</span></span>|<span data-ttu-id="0db54-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0db54-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0db54-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0db54-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0db54-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0db54-141">roleScopeTagIds</span></span>|<span data-ttu-id="0db54-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0db54-142">String collection</span></span>|<span data-ttu-id="0db54-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="0db54-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0db54-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0db54-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0db54-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0db54-145">supportsScopeTags</span></span>|<span data-ttu-id="0db54-146">Логический</span><span class="sxs-lookup"><span data-stu-id="0db54-146">Boolean</span></span>|<span data-ttu-id="0db54-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="0db54-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0db54-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="0db54-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0db54-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="0db54-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0db54-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0db54-150">This property is read-only.</span></span> <span data-ttu-id="0db54-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0db54-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0db54-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0db54-152">createdDateTime</span></span>|<span data-ttu-id="0db54-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0db54-153">DateTimeOffset</span></span>|<span data-ttu-id="0db54-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0db54-154">DateTime the object was created.</span></span> <span data-ttu-id="0db54-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0db54-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0db54-156">description</span><span class="sxs-lookup"><span data-stu-id="0db54-156">description</span></span>|<span data-ttu-id="0db54-157">String</span><span class="sxs-lookup"><span data-stu-id="0db54-157">String</span></span>|<span data-ttu-id="0db54-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0db54-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0db54-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0db54-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0db54-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0db54-160">displayName</span></span>|<span data-ttu-id="0db54-161">String</span><span class="sxs-lookup"><span data-stu-id="0db54-161">String</span></span>|<span data-ttu-id="0db54-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0db54-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0db54-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0db54-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0db54-164">version</span><span class="sxs-lookup"><span data-stu-id="0db54-164">version</span></span>|<span data-ttu-id="0db54-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0db54-165">Int32</span></span>|<span data-ttu-id="0db54-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0db54-166">Version of the device configuration.</span></span> <span data-ttu-id="0db54-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0db54-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0db54-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="0db54-168">connectionName</span></span>|<span data-ttu-id="0db54-169">String</span><span class="sxs-lookup"><span data-stu-id="0db54-169">String</span></span>|<span data-ttu-id="0db54-170">Имя подключения отображается для пользователя.</span><span class="sxs-lookup"><span data-stu-id="0db54-170">Connection name displayed to the user.</span></span> <span data-ttu-id="0db54-171">Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0db54-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0db54-172">серверы</span><span class="sxs-lookup"><span data-stu-id="0db54-172">servers</span></span>|<span data-ttu-id="0db54-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0db54-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="0db54-174">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="0db54-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="0db54-175">Убедитесь, что конечные пользователи могут получить доступ к эти расположения в сети.</span><span class="sxs-lookup"><span data-stu-id="0db54-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="0db54-176">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="0db54-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0db54-177">Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0db54-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0db54-178">customXml</span><span class="sxs-lookup"><span data-stu-id="0db54-178">customXml</span></span>|<span data-ttu-id="0db54-179">Binary</span><span class="sxs-lookup"><span data-stu-id="0db54-179">Binary</span></span>|<span data-ttu-id="0db54-180">Настраиваемые команды XML, которые настраиваются VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="0db54-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="0db54-181">(UTF8 закодированный массив байтов) Наследуется от [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0db54-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0db54-182">profileTarget</span><span class="sxs-lookup"><span data-stu-id="0db54-182">profileTarget</span></span>|[<span data-ttu-id="0db54-183">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="0db54-183">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="0db54-184">Тип конечного профиля.</span><span class="sxs-lookup"><span data-stu-id="0db54-184">Profile target type.</span></span> <span data-ttu-id="0db54-185">Возможные значения: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="0db54-185">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="0db54-186">Тип подключения</span><span class="sxs-lookup"><span data-stu-id="0db54-186">connectionType</span></span>|[<span data-ttu-id="0db54-187">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="0db54-187">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="0db54-188">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="0db54-188">Connection type.</span></span> <span data-ttu-id="0db54-189">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="0db54-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="0db54-190">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="0db54-190">enableSplitTunneling</span></span>|<span data-ttu-id="0db54-191">Логический</span><span class="sxs-lookup"><span data-stu-id="0db54-191">Boolean</span></span>|<span data-ttu-id="0db54-192">Включение разделенное туннелирование.</span><span class="sxs-lookup"><span data-stu-id="0db54-192">Enable split tunneling.</span></span>|
|<span data-ttu-id="0db54-193">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="0db54-193">enableAlwaysOn</span></span>|<span data-ttu-id="0db54-194">Логический</span><span class="sxs-lookup"><span data-stu-id="0db54-194">Boolean</span></span>|<span data-ttu-id="0db54-195">Включение режима всегда на.</span><span class="sxs-lookup"><span data-stu-id="0db54-195">Enable Always On mode.</span></span>|
|<span data-ttu-id="0db54-196">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="0db54-196">enableDeviceTunnel</span></span>|<span data-ttu-id="0db54-197">Логический</span><span class="sxs-lookup"><span data-stu-id="0db54-197">Boolean</span></span>|<span data-ttu-id="0db54-198">Включение туннель устройства.</span><span class="sxs-lookup"><span data-stu-id="0db54-198">Enable device tunnel.</span></span>|
|<span data-ttu-id="0db54-199">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="0db54-199">enableDnsRegistration</span></span>|<span data-ttu-id="0db54-200">Логический</span><span class="sxs-lookup"><span data-stu-id="0db54-200">Boolean</span></span>|<span data-ttu-id="0db54-201">Включение регистрации IP-адреса с внутренней DNS.</span><span class="sxs-lookup"><span data-stu-id="0db54-201">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="0db54-202">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="0db54-202">dnsSuffixes</span></span>|<span data-ttu-id="0db54-203">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0db54-203">String collection</span></span>|<span data-ttu-id="0db54-204">Укажите DNS-суффиксы для добавления в список поиска DNS маршрутизацию короткие имена.</span><span class="sxs-lookup"><span data-stu-id="0db54-204">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="0db54-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0db54-205">authenticationMethod</span></span>|[<span data-ttu-id="0db54-206">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0db54-206">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="0db54-207">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="0db54-207">Authentication method.</span></span> <span data-ttu-id="0db54-208">Возможные значения: `certificate`, `usernameAndPassword`, `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="0db54-208">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="0db54-209">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="0db54-209">rememberUserCredentials</span></span>|<span data-ttu-id="0db54-210">Логический</span><span class="sxs-lookup"><span data-stu-id="0db54-210">Boolean</span></span>|<span data-ttu-id="0db54-211">Не забудьте учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="0db54-211">Remember user credentials.</span></span>|
|<span data-ttu-id="0db54-212">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="0db54-212">enableConditionalAccess</span></span>|<span data-ttu-id="0db54-213">Логический</span><span class="sxs-lookup"><span data-stu-id="0db54-213">Boolean</span></span>|<span data-ttu-id="0db54-214">Включение условного доступа.</span><span class="sxs-lookup"><span data-stu-id="0db54-214">Enable conditional access.</span></span>|
|<span data-ttu-id="0db54-215">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="0db54-215">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="0db54-216">Логический</span><span class="sxs-lookup"><span data-stu-id="0db54-216">Boolean</span></span>|<span data-ttu-id="0db54-217">Включение единого входа (SSO) с помощью альтернативного сертификата.</span><span class="sxs-lookup"><span data-stu-id="0db54-217">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="0db54-218">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="0db54-218">singleSignOnEku</span></span>|[<span data-ttu-id="0db54-219">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="0db54-219">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="0db54-220">Единого входа расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="0db54-220">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="0db54-221">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="0db54-221">singleSignOnIssuerHash</span></span>|<span data-ttu-id="0db54-222">String</span><span class="sxs-lookup"><span data-stu-id="0db54-222">String</span></span>|<span data-ttu-id="0db54-223">Хэш-функции поставщика единого входа.</span><span class="sxs-lookup"><span data-stu-id="0db54-223">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="0db54-224">eapXml</span><span class="sxs-lookup"><span data-stu-id="0db54-224">eapXml</span></span>|<span data-ttu-id="0db54-225">Binary</span><span class="sxs-lookup"><span data-stu-id="0db54-225">Binary</span></span>|<span data-ttu-id="0db54-226">Протокол расширенной проверки подлинности (EAP) XML.</span><span class="sxs-lookup"><span data-stu-id="0db54-226">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="0db54-227">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="0db54-227">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="0db54-228">прокси-серверу</span><span class="sxs-lookup"><span data-stu-id="0db54-228">proxyServer</span></span>|[<span data-ttu-id="0db54-229">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="0db54-229">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="0db54-230">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="0db54-230">Proxy Server.</span></span>|
|<span data-ttu-id="0db54-231">associatedApps</span><span class="sxs-lookup"><span data-stu-id="0db54-231">associatedApps</span></span>|<span data-ttu-id="0db54-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0db54-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="0db54-233">Связанные приложения.</span><span class="sxs-lookup"><span data-stu-id="0db54-233">Associated Apps.</span></span> <span data-ttu-id="0db54-234">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="0db54-234">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="0db54-235">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="0db54-235">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="0db54-236">Логический</span><span class="sxs-lookup"><span data-stu-id="0db54-236">Boolean</span></span>|<span data-ttu-id="0db54-237">Только связанного приложения могут использовать подключения (VPN-app).</span><span class="sxs-lookup"><span data-stu-id="0db54-237">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="0db54-238">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="0db54-238">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="0db54-239">String</span><span class="sxs-lookup"><span data-stu-id="0db54-239">String</span></span>|<span data-ttu-id="0db54-240">Сведения о защите Windows (НЗП) домена, связанного с этим подключением.</span><span class="sxs-lookup"><span data-stu-id="0db54-240">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="0db54-241">trafficRules</span><span class="sxs-lookup"><span data-stu-id="0db54-241">trafficRules</span></span>|<span data-ttu-id="0db54-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0db54-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="0db54-243">Правила трафика.</span><span class="sxs-lookup"><span data-stu-id="0db54-243">Traffic rules.</span></span> <span data-ttu-id="0db54-244">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="0db54-244">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="0db54-245">маршруты</span><span class="sxs-lookup"><span data-stu-id="0db54-245">routes</span></span>|<span data-ttu-id="0db54-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0db54-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="0db54-247">Маршрутизация (не обязательно для сторонних поставщиков).</span><span class="sxs-lookup"><span data-stu-id="0db54-247">Routes (optional for third-party providers).</span></span> <span data-ttu-id="0db54-248">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="0db54-248">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="0db54-249">dnsRules</span><span class="sxs-lookup"><span data-stu-id="0db54-249">dnsRules</span></span>|<span data-ttu-id="0db54-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0db54-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="0db54-251">Правила DNS.</span><span class="sxs-lookup"><span data-stu-id="0db54-251">DNS rules.</span></span> <span data-ttu-id="0db54-252">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="0db54-252">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="0db54-253">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="0db54-253">trustedNetworkDomains</span></span>|<span data-ttu-id="0db54-254">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0db54-254">String collection</span></span>|<span data-ttu-id="0db54-255">Надежные сетевыми доменами</span><span class="sxs-lookup"><span data-stu-id="0db54-255">Trusted Network Domains</span></span>|



## <a name="response"></a><span data-ttu-id="0db54-256">Отклик</span><span class="sxs-lookup"><span data-stu-id="0db54-256">Response</span></span>
<span data-ttu-id="0db54-257">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0db54-257">If successful, this method returns a `200 OK` response code and an updated [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0db54-258">Пример</span><span class="sxs-lookup"><span data-stu-id="0db54-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="0db54-259">Запрос</span><span class="sxs-lookup"><span data-stu-id="0db54-259">Request</span></span>
<span data-ttu-id="0db54-260">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0db54-260">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3387

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
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
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="0db54-261">Отклик</span><span class="sxs-lookup"><span data-stu-id="0db54-261">Response</span></span>
<span data-ttu-id="0db54-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0db54-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3559

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
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ]
}
```




