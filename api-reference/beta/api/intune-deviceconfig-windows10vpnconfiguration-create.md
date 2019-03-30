---
title: Создание windows10VpnConfiguration
description: Создание нового объекта windows10VpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa05bee08f30936ca496499090f8bdf9ee1877c5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988660"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="58609-103">Создание windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="58609-103">Create windows10VpnConfiguration</span></span>

> <span data-ttu-id="58609-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58609-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58609-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58609-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58609-106">Создание нового объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="58609-106">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58609-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="58609-107">Prerequisites</span></span>
<span data-ttu-id="58609-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58609-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58609-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58609-110">Permission type</span></span>|<span data-ttu-id="58609-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="58609-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58609-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58609-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58609-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58609-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="58609-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58609-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58609-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58609-115">Not supported.</span></span>|
|<span data-ttu-id="58609-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58609-116">Application</span></span>|<span data-ttu-id="58609-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58609-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58609-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58609-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="58609-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58609-119">Request headers</span></span>
|<span data-ttu-id="58609-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58609-120">Header</span></span>|<span data-ttu-id="58609-121">Значение</span><span class="sxs-lookup"><span data-stu-id="58609-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58609-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58609-122">Authorization</span></span>|<span data-ttu-id="58609-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58609-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58609-124">Accept</span><span class="sxs-lookup"><span data-stu-id="58609-124">Accept</span></span>|<span data-ttu-id="58609-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58609-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58609-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="58609-126">Request body</span></span>
<span data-ttu-id="58609-127">В тексте запроса добавьте представление объекта windows10VpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58609-127">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="58609-128">В следующей таблице приведены свойства, необходимые при создании windows10VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="58609-128">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="58609-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="58609-129">Property</span></span>|<span data-ttu-id="58609-130">Тип</span><span class="sxs-lookup"><span data-stu-id="58609-130">Type</span></span>|<span data-ttu-id="58609-131">Описание</span><span class="sxs-lookup"><span data-stu-id="58609-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58609-132">id</span><span class="sxs-lookup"><span data-stu-id="58609-132">id</span></span>|<span data-ttu-id="58609-133">Строка</span><span class="sxs-lookup"><span data-stu-id="58609-133">String</span></span>|<span data-ttu-id="58609-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="58609-134">Key of the entity.</span></span> <span data-ttu-id="58609-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58609-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58609-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58609-136">lastModifiedDateTime</span></span>|<span data-ttu-id="58609-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58609-137">DateTimeOffset</span></span>|<span data-ttu-id="58609-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="58609-138">DateTime the object was last modified.</span></span> <span data-ttu-id="58609-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58609-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58609-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="58609-140">roleScopeTagIds</span></span>|<span data-ttu-id="58609-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="58609-141">String collection</span></span>|<span data-ttu-id="58609-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="58609-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="58609-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58609-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58609-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="58609-144">supportsScopeTags</span></span>|<span data-ttu-id="58609-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="58609-145">Boolean</span></span>|<span data-ttu-id="58609-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="58609-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="58609-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="58609-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="58609-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="58609-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="58609-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="58609-149">This property is read-only.</span></span> <span data-ttu-id="58609-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58609-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58609-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58609-151">createdDateTime</span></span>|<span data-ttu-id="58609-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58609-152">DateTimeOffset</span></span>|<span data-ttu-id="58609-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="58609-153">DateTime the object was created.</span></span> <span data-ttu-id="58609-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58609-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58609-155">description</span><span class="sxs-lookup"><span data-stu-id="58609-155">description</span></span>|<span data-ttu-id="58609-156">String</span><span class="sxs-lookup"><span data-stu-id="58609-156">String</span></span>|<span data-ttu-id="58609-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="58609-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="58609-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58609-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58609-159">displayName</span><span class="sxs-lookup"><span data-stu-id="58609-159">displayName</span></span>|<span data-ttu-id="58609-160">String</span><span class="sxs-lookup"><span data-stu-id="58609-160">String</span></span>|<span data-ttu-id="58609-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="58609-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="58609-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58609-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58609-163">version</span><span class="sxs-lookup"><span data-stu-id="58609-163">version</span></span>|<span data-ttu-id="58609-164">Int32</span><span class="sxs-lookup"><span data-stu-id="58609-164">Int32</span></span>|<span data-ttu-id="58609-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="58609-165">Version of the device configuration.</span></span> <span data-ttu-id="58609-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58609-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58609-167">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="58609-167">connectionName</span></span>|<span data-ttu-id="58609-168">String</span><span class="sxs-lookup"><span data-stu-id="58609-168">String</span></span>|<span data-ttu-id="58609-169">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="58609-169">Connection name displayed to the user.</span></span> <span data-ttu-id="58609-170">НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58609-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="58609-171">серверами</span><span class="sxs-lookup"><span data-stu-id="58609-171">servers</span></span>|<span data-ttu-id="58609-172">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="58609-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="58609-173">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="58609-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="58609-174">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="58609-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="58609-175">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="58609-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="58609-176">НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58609-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="58609-177">customXml</span><span class="sxs-lookup"><span data-stu-id="58609-177">customXml</span></span>|<span data-ttu-id="58609-178">Binary</span><span class="sxs-lookup"><span data-stu-id="58609-178">Binary</span></span>|<span data-ttu-id="58609-179">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="58609-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="58609-180">(Массив байтов в кодировке UTF8) НаСледуется от [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58609-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="58609-181">Профилетаржет</span><span class="sxs-lookup"><span data-stu-id="58609-181">profileTarget</span></span>|[<span data-ttu-id="58609-182">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="58609-182">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="58609-183">Тип целевого объекта профиля.</span><span class="sxs-lookup"><span data-stu-id="58609-183">Profile target type.</span></span> <span data-ttu-id="58609-184">Возможные значения: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="58609-184">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="58609-185">connectionType</span><span class="sxs-lookup"><span data-stu-id="58609-185">connectionType</span></span>|[<span data-ttu-id="58609-186">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="58609-186">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="58609-187">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="58609-187">Connection type.</span></span> <span data-ttu-id="58609-188">Возможные значения: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="58609-188">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="58609-189">Енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="58609-189">enableSplitTunneling</span></span>|<span data-ttu-id="58609-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="58609-190">Boolean</span></span>|<span data-ttu-id="58609-191">Включение Расщепленного туннелирования.</span><span class="sxs-lookup"><span data-stu-id="58609-191">Enable split tunneling.</span></span>|
|<span data-ttu-id="58609-192">Енаблеалвайсон</span><span class="sxs-lookup"><span data-stu-id="58609-192">enableAlwaysOn</span></span>|<span data-ttu-id="58609-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="58609-193">Boolean</span></span>|<span data-ttu-id="58609-194">Включение режима "всегда включено".</span><span class="sxs-lookup"><span data-stu-id="58609-194">Enable Always On mode.</span></span>|
|<span data-ttu-id="58609-195">Енабледевицетуннел</span><span class="sxs-lookup"><span data-stu-id="58609-195">enableDeviceTunnel</span></span>|<span data-ttu-id="58609-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="58609-196">Boolean</span></span>|<span data-ttu-id="58609-197">Включите туннель устройства.</span><span class="sxs-lookup"><span data-stu-id="58609-197">Enable device tunnel.</span></span>|
|<span data-ttu-id="58609-198">Енабледнсрегистратион</span><span class="sxs-lookup"><span data-stu-id="58609-198">enableDnsRegistration</span></span>|<span data-ttu-id="58609-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="58609-199">Boolean</span></span>|<span data-ttu-id="58609-200">Включить регистрацию IP-адресов с использованием внутренней DNS.</span><span class="sxs-lookup"><span data-stu-id="58609-200">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="58609-201">Днссуффиксес</span><span class="sxs-lookup"><span data-stu-id="58609-201">dnsSuffixes</span></span>|<span data-ttu-id="58609-202">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="58609-202">String collection</span></span>|<span data-ttu-id="58609-203">Укажите DNS-суффиксы, которые необходимо добавить в список поиска DNS, чтобы правильно маршрутизировать короткие имена.</span><span class="sxs-lookup"><span data-stu-id="58609-203">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="58609-204">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="58609-204">authenticationMethod</span></span>|[<span data-ttu-id="58609-205">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="58609-205">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="58609-206">Метод проверки поДлинности.</span><span class="sxs-lookup"><span data-stu-id="58609-206">Authentication method.</span></span> <span data-ttu-id="58609-207">Возможные значения: `certificate`, `usernameAndPassword`, `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="58609-207">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="58609-208">Ремемберусеркредентиалс</span><span class="sxs-lookup"><span data-stu-id="58609-208">rememberUserCredentials</span></span>|<span data-ttu-id="58609-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="58609-209">Boolean</span></span>|<span data-ttu-id="58609-210">Запомнить учетные данные пользователя.</span><span class="sxs-lookup"><span data-stu-id="58609-210">Remember user credentials.</span></span>|
|<span data-ttu-id="58609-211">Енаблекондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="58609-211">enableConditionalAccess</span></span>|<span data-ttu-id="58609-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="58609-212">Boolean</span></span>|<span data-ttu-id="58609-213">Включение условного доступа.</span><span class="sxs-lookup"><span data-stu-id="58609-213">Enable conditional access.</span></span>|
|<span data-ttu-id="58609-214">Енаблесинглесигнонвисалтернатецертификате</span><span class="sxs-lookup"><span data-stu-id="58609-214">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="58609-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="58609-215">Boolean</span></span>|<span data-ttu-id="58609-216">Включите единый вход (SSO) с альтернативным сертификатом.</span><span class="sxs-lookup"><span data-stu-id="58609-216">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="58609-217">Синглесигнонеку</span><span class="sxs-lookup"><span data-stu-id="58609-217">singleSignOnEku</span></span>|[<span data-ttu-id="58609-218">Екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="58609-218">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="58609-219">Расширенное использование ключа (EKU) единого входа.</span><span class="sxs-lookup"><span data-stu-id="58609-219">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="58609-220">Синглесигнониссуерхаш</span><span class="sxs-lookup"><span data-stu-id="58609-220">singleSignOnIssuerHash</span></span>|<span data-ttu-id="58609-221">String</span><span class="sxs-lookup"><span data-stu-id="58609-221">String</span></span>|<span data-ttu-id="58609-222">Хэш поставщика единого входа.</span><span class="sxs-lookup"><span data-stu-id="58609-222">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="58609-223">Еапксмл</span><span class="sxs-lookup"><span data-stu-id="58609-223">eapXml</span></span>|<span data-ttu-id="58609-224">Binary</span><span class="sxs-lookup"><span data-stu-id="58609-224">Binary</span></span>|<span data-ttu-id="58609-225">XML-файл протокола расширенной проверки поДлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="58609-225">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="58609-226">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="58609-226">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="58609-227">проксисервер</span><span class="sxs-lookup"><span data-stu-id="58609-227">proxyServer</span></span>|[<span data-ttu-id="58609-228">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="58609-228">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="58609-229">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="58609-229">Proxy Server.</span></span>|
|<span data-ttu-id="58609-230">АссоЦиатедаппс</span><span class="sxs-lookup"><span data-stu-id="58609-230">associatedApps</span></span>|<span data-ttu-id="58609-231">Коллекция [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="58609-231">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="58609-232">Связанные приложения.</span><span class="sxs-lookup"><span data-stu-id="58609-232">Associated Apps.</span></span> <span data-ttu-id="58609-233">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="58609-233">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="58609-234">ОнляссоЦиатедаппсканусеконнектион</span><span class="sxs-lookup"><span data-stu-id="58609-234">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="58609-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="58609-235">Boolean</span></span>|<span data-ttu-id="58609-236">Подключение можно использовать только для связанных приложений (VPN для каждого приложения).</span><span class="sxs-lookup"><span data-stu-id="58609-236">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="58609-237">Виндовсинформатионпротектиондомаин</span><span class="sxs-lookup"><span data-stu-id="58609-237">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="58609-238">String</span><span class="sxs-lookup"><span data-stu-id="58609-238">String</span></span>|<span data-ttu-id="58609-239">Домен Windows Information Protection (WIP) для связи с этим подключением.</span><span class="sxs-lookup"><span data-stu-id="58609-239">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="58609-240">Траффикрулес</span><span class="sxs-lookup"><span data-stu-id="58609-240">trafficRules</span></span>|<span data-ttu-id="58609-241">Коллекция [впнтраффикруле](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="58609-241">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="58609-242">Правила трафика.</span><span class="sxs-lookup"><span data-stu-id="58609-242">Traffic rules.</span></span> <span data-ttu-id="58609-243">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="58609-243">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="58609-244">сылает</span><span class="sxs-lookup"><span data-stu-id="58609-244">routes</span></span>|<span data-ttu-id="58609-245">Коллекция [впнрауте](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="58609-245">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="58609-246">Маршруты (необязательно для сторонних поставщиков).</span><span class="sxs-lookup"><span data-stu-id="58609-246">Routes (optional for third-party providers).</span></span> <span data-ttu-id="58609-247">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="58609-247">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="58609-248">Днсрулес</span><span class="sxs-lookup"><span data-stu-id="58609-248">dnsRules</span></span>|<span data-ttu-id="58609-249">Коллекция [впнднсруле](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="58609-249">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="58609-250">Правила DNS.</span><span class="sxs-lookup"><span data-stu-id="58609-250">DNS rules.</span></span> <span data-ttu-id="58609-251">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="58609-251">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="58609-252">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="58609-252">trustedNetworkDomains</span></span>|<span data-ttu-id="58609-253">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="58609-253">String collection</span></span>|<span data-ttu-id="58609-254">Доверенные сетевые домены</span><span class="sxs-lookup"><span data-stu-id="58609-254">Trusted Network Domains</span></span>|



## <a name="response"></a><span data-ttu-id="58609-255">Отклик</span><span class="sxs-lookup"><span data-stu-id="58609-255">Response</span></span>
<span data-ttu-id="58609-256">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58609-256">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58609-257">Пример</span><span class="sxs-lookup"><span data-stu-id="58609-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="58609-258">Запрос</span><span class="sxs-lookup"><span data-stu-id="58609-258">Request</span></span>
<span data-ttu-id="58609-259">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58609-259">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="58609-260">Отклик</span><span class="sxs-lookup"><span data-stu-id="58609-260">Response</span></span>
<span data-ttu-id="58609-p121">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58609-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




