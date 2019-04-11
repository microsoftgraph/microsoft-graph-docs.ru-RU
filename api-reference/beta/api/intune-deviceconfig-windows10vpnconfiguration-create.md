---
title: Создание windows10VpnConfiguration
description: Создание нового объекта windows10VpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92b943968b389711a9c6e9e1ab0bf9d57dc29201
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794598"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="dd521-103">Создание windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="dd521-103">Create windows10VpnConfiguration</span></span>

> <span data-ttu-id="dd521-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd521-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd521-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd521-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd521-106">Создание нового объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="dd521-106">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd521-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dd521-107">Prerequisites</span></span>
<span data-ttu-id="dd521-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd521-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd521-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd521-110">Permission type</span></span>|<span data-ttu-id="dd521-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd521-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd521-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd521-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dd521-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd521-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd521-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd521-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd521-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd521-115">Not supported.</span></span>|
|<span data-ttu-id="dd521-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd521-116">Application</span></span>|<span data-ttu-id="dd521-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd521-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd521-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd521-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dd521-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd521-119">Request headers</span></span>
|<span data-ttu-id="dd521-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd521-120">Header</span></span>|<span data-ttu-id="dd521-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dd521-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd521-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd521-122">Authorization</span></span>|<span data-ttu-id="dd521-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd521-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd521-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dd521-124">Accept</span></span>|<span data-ttu-id="dd521-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dd521-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd521-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd521-126">Request body</span></span>
<span data-ttu-id="dd521-127">В тексте запроса добавьте представление объекта windows10VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd521-127">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="dd521-128">В следующей таблице приведены свойства, необходимые при создании windows10VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="dd521-128">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="dd521-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd521-129">Property</span></span>|<span data-ttu-id="dd521-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dd521-130">Type</span></span>|<span data-ttu-id="dd521-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dd521-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd521-132">id</span><span class="sxs-lookup"><span data-stu-id="dd521-132">id</span></span>|<span data-ttu-id="dd521-133">Строка</span><span class="sxs-lookup"><span data-stu-id="dd521-133">String</span></span>|<span data-ttu-id="dd521-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dd521-134">Key of the entity.</span></span> <span data-ttu-id="dd521-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd521-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd521-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd521-136">lastModifiedDateTime</span></span>|<span data-ttu-id="dd521-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd521-137">DateTimeOffset</span></span>|<span data-ttu-id="dd521-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="dd521-138">DateTime the object was last modified.</span></span> <span data-ttu-id="dd521-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd521-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd521-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dd521-140">roleScopeTagIds</span></span>|<span data-ttu-id="dd521-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dd521-141">String collection</span></span>|<span data-ttu-id="dd521-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="dd521-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dd521-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd521-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd521-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="dd521-144">supportsScopeTags</span></span>|<span data-ttu-id="dd521-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd521-145">Boolean</span></span>|<span data-ttu-id="dd521-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="dd521-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="dd521-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="dd521-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="dd521-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="dd521-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="dd521-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dd521-149">This property is read-only.</span></span> <span data-ttu-id="dd521-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd521-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd521-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd521-151">createdDateTime</span></span>|<span data-ttu-id="dd521-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd521-152">DateTimeOffset</span></span>|<span data-ttu-id="dd521-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="dd521-153">DateTime the object was created.</span></span> <span data-ttu-id="dd521-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd521-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd521-155">description</span><span class="sxs-lookup"><span data-stu-id="dd521-155">description</span></span>|<span data-ttu-id="dd521-156">String</span><span class="sxs-lookup"><span data-stu-id="dd521-156">String</span></span>|<span data-ttu-id="dd521-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dd521-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dd521-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd521-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd521-159">displayName</span><span class="sxs-lookup"><span data-stu-id="dd521-159">displayName</span></span>|<span data-ttu-id="dd521-160">String</span><span class="sxs-lookup"><span data-stu-id="dd521-160">String</span></span>|<span data-ttu-id="dd521-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dd521-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dd521-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd521-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd521-163">version</span><span class="sxs-lookup"><span data-stu-id="dd521-163">version</span></span>|<span data-ttu-id="dd521-164">Int32</span><span class="sxs-lookup"><span data-stu-id="dd521-164">Int32</span></span>|<span data-ttu-id="dd521-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dd521-165">Version of the device configuration.</span></span> <span data-ttu-id="dd521-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd521-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd521-167">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="dd521-167">connectionName</span></span>|<span data-ttu-id="dd521-168">String</span><span class="sxs-lookup"><span data-stu-id="dd521-168">String</span></span>|<span data-ttu-id="dd521-169">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="dd521-169">Connection name displayed to the user.</span></span> <span data-ttu-id="dd521-170">НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd521-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="dd521-171">серверами</span><span class="sxs-lookup"><span data-stu-id="dd521-171">servers</span></span>|<span data-ttu-id="dd521-172">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="dd521-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="dd521-173">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="dd521-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="dd521-174">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="dd521-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="dd521-175">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="dd521-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="dd521-176">НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd521-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="dd521-177">customXml</span><span class="sxs-lookup"><span data-stu-id="dd521-177">customXml</span></span>|<span data-ttu-id="dd521-178">Binary</span><span class="sxs-lookup"><span data-stu-id="dd521-178">Binary</span></span>|<span data-ttu-id="dd521-179">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="dd521-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="dd521-180">(Массив байтов в кодировке UTF8) НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd521-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="dd521-181">Профилетаржет</span><span class="sxs-lookup"><span data-stu-id="dd521-181">profileTarget</span></span>|[<span data-ttu-id="dd521-182">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="dd521-182">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="dd521-183">Тип целевого объекта профиля.</span><span class="sxs-lookup"><span data-stu-id="dd521-183">Profile target type.</span></span> <span data-ttu-id="dd521-184">Возможные значения: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="dd521-184">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="dd521-185">connectionType</span><span class="sxs-lookup"><span data-stu-id="dd521-185">connectionType</span></span>|[<span data-ttu-id="dd521-186">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="dd521-186">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="dd521-187">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="dd521-187">Connection type.</span></span> <span data-ttu-id="dd521-188">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="dd521-188">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="dd521-189">Енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="dd521-189">enableSplitTunneling</span></span>|<span data-ttu-id="dd521-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd521-190">Boolean</span></span>|<span data-ttu-id="dd521-191">Включение Расщепленного туннелирования.</span><span class="sxs-lookup"><span data-stu-id="dd521-191">Enable split tunneling.</span></span>|
|<span data-ttu-id="dd521-192">Енаблеалвайсон</span><span class="sxs-lookup"><span data-stu-id="dd521-192">enableAlwaysOn</span></span>|<span data-ttu-id="dd521-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd521-193">Boolean</span></span>|<span data-ttu-id="dd521-194">Включение режима "всегда включено".</span><span class="sxs-lookup"><span data-stu-id="dd521-194">Enable Always On mode.</span></span>|
|<span data-ttu-id="dd521-195">Енабледевицетуннел</span><span class="sxs-lookup"><span data-stu-id="dd521-195">enableDeviceTunnel</span></span>|<span data-ttu-id="dd521-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd521-196">Boolean</span></span>|<span data-ttu-id="dd521-197">Включите туннель устройства.</span><span class="sxs-lookup"><span data-stu-id="dd521-197">Enable device tunnel.</span></span>|
|<span data-ttu-id="dd521-198">Енабледнсрегистратион</span><span class="sxs-lookup"><span data-stu-id="dd521-198">enableDnsRegistration</span></span>|<span data-ttu-id="dd521-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd521-199">Boolean</span></span>|<span data-ttu-id="dd521-200">Включить регистрацию IP-адресов с использованием внутренней DNS.</span><span class="sxs-lookup"><span data-stu-id="dd521-200">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="dd521-201">Днссуффиксес</span><span class="sxs-lookup"><span data-stu-id="dd521-201">dnsSuffixes</span></span>|<span data-ttu-id="dd521-202">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dd521-202">String collection</span></span>|<span data-ttu-id="dd521-203">Укажите DNS-суффиксы, которые необходимо добавить в список поиска DNS, чтобы правильно маршрутизировать короткие имена.</span><span class="sxs-lookup"><span data-stu-id="dd521-203">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="dd521-204">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="dd521-204">authenticationMethod</span></span>|[<span data-ttu-id="dd521-205">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="dd521-205">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="dd521-206">Метод проверки поДлинности.</span><span class="sxs-lookup"><span data-stu-id="dd521-206">Authentication method.</span></span> <span data-ttu-id="dd521-207">Возможные значения: `certificate`, `usernameAndPassword`, `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="dd521-207">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="dd521-208">Ремемберусеркредентиалс</span><span class="sxs-lookup"><span data-stu-id="dd521-208">rememberUserCredentials</span></span>|<span data-ttu-id="dd521-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd521-209">Boolean</span></span>|<span data-ttu-id="dd521-210">Запомнить учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="dd521-210">Remember user credentials.</span></span>|
|<span data-ttu-id="dd521-211">Енаблекондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="dd521-211">enableConditionalAccess</span></span>|<span data-ttu-id="dd521-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd521-212">Boolean</span></span>|<span data-ttu-id="dd521-213">Включение условного доступа.</span><span class="sxs-lookup"><span data-stu-id="dd521-213">Enable conditional access.</span></span>|
|<span data-ttu-id="dd521-214">Енаблесинглесигнонвисалтернатецертификате</span><span class="sxs-lookup"><span data-stu-id="dd521-214">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="dd521-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd521-215">Boolean</span></span>|<span data-ttu-id="dd521-216">Включите единый вход (SSO) с альтернативным сертификатом.</span><span class="sxs-lookup"><span data-stu-id="dd521-216">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="dd521-217">Синглесигнонеку</span><span class="sxs-lookup"><span data-stu-id="dd521-217">singleSignOnEku</span></span>|[<span data-ttu-id="dd521-218">Екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="dd521-218">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="dd521-219">Расширенное использование ключа (EKU) единого входа.</span><span class="sxs-lookup"><span data-stu-id="dd521-219">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="dd521-220">Синглесигнониссуерхаш</span><span class="sxs-lookup"><span data-stu-id="dd521-220">singleSignOnIssuerHash</span></span>|<span data-ttu-id="dd521-221">String</span><span class="sxs-lookup"><span data-stu-id="dd521-221">String</span></span>|<span data-ttu-id="dd521-222">Хэш поставщика единого входа.</span><span class="sxs-lookup"><span data-stu-id="dd521-222">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="dd521-223">Еапксмл</span><span class="sxs-lookup"><span data-stu-id="dd521-223">eapXml</span></span>|<span data-ttu-id="dd521-224">Binary</span><span class="sxs-lookup"><span data-stu-id="dd521-224">Binary</span></span>|<span data-ttu-id="dd521-225">XML-файл протокола расширенной проверки поДлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="dd521-225">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="dd521-226">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="dd521-226">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="dd521-227">проксисервер</span><span class="sxs-lookup"><span data-stu-id="dd521-227">proxyServer</span></span>|[<span data-ttu-id="dd521-228">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="dd521-228">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="dd521-229">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="dd521-229">Proxy Server.</span></span>|
|<span data-ttu-id="dd521-230">АссоЦиатедаппс</span><span class="sxs-lookup"><span data-stu-id="dd521-230">associatedApps</span></span>|<span data-ttu-id="dd521-231">Коллекция [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="dd521-231">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="dd521-232">Связанные приложения.</span><span class="sxs-lookup"><span data-stu-id="dd521-232">Associated Apps.</span></span> <span data-ttu-id="dd521-233">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="dd521-233">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="dd521-234">ОнляссоЦиатедаппсканусеконнектион</span><span class="sxs-lookup"><span data-stu-id="dd521-234">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="dd521-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd521-235">Boolean</span></span>|<span data-ttu-id="dd521-236">Подключение можно использовать только для связанных приложений (VPN для каждого приложения).</span><span class="sxs-lookup"><span data-stu-id="dd521-236">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="dd521-237">Виндовсинформатионпротектиондомаин</span><span class="sxs-lookup"><span data-stu-id="dd521-237">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="dd521-238">String</span><span class="sxs-lookup"><span data-stu-id="dd521-238">String</span></span>|<span data-ttu-id="dd521-239">Домен Windows Information Protection (WIP) для связи с этим подключением.</span><span class="sxs-lookup"><span data-stu-id="dd521-239">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="dd521-240">Траффикрулес</span><span class="sxs-lookup"><span data-stu-id="dd521-240">trafficRules</span></span>|<span data-ttu-id="dd521-241">Коллекция [впнтраффикруле](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="dd521-241">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="dd521-242">Правила трафика.</span><span class="sxs-lookup"><span data-stu-id="dd521-242">Traffic rules.</span></span> <span data-ttu-id="dd521-243">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="dd521-243">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="dd521-244">сылает</span><span class="sxs-lookup"><span data-stu-id="dd521-244">routes</span></span>|<span data-ttu-id="dd521-245">Коллекция [впнрауте](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="dd521-245">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="dd521-246">Маршруты (необязательно для сторонних поставщиков).</span><span class="sxs-lookup"><span data-stu-id="dd521-246">Routes (optional for third-party providers).</span></span> <span data-ttu-id="dd521-247">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="dd521-247">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="dd521-248">Днсрулес</span><span class="sxs-lookup"><span data-stu-id="dd521-248">dnsRules</span></span>|<span data-ttu-id="dd521-249">Коллекция [впнднсруле](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="dd521-249">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="dd521-250">Правила DNS.</span><span class="sxs-lookup"><span data-stu-id="dd521-250">DNS rules.</span></span> <span data-ttu-id="dd521-251">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="dd521-251">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="dd521-252">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="dd521-252">trustedNetworkDomains</span></span>|<span data-ttu-id="dd521-253">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dd521-253">String collection</span></span>|<span data-ttu-id="dd521-254">Доверенные сетевые домены</span><span class="sxs-lookup"><span data-stu-id="dd521-254">Trusted Network Domains</span></span>|



## <a name="response"></a><span data-ttu-id="dd521-255">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd521-255">Response</span></span>
<span data-ttu-id="dd521-256">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd521-256">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd521-257">Пример</span><span class="sxs-lookup"><span data-stu-id="dd521-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd521-258">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd521-258">Request</span></span>
<span data-ttu-id="dd521-259">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd521-259">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="dd521-260">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd521-260">Response</span></span>
<span data-ttu-id="dd521-p121">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd521-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





