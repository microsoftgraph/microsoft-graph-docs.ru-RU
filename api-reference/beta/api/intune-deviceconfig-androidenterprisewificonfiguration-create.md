---
title: Создание androidEnterpriseWiFiConfiguration
description: Создание нового объекта androidEnterpriseWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12a06abcf8def4780f7f64d0f8a65d164938188f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933083"
---
# <a name="create-androidenterprisewificonfiguration"></a><span data-ttu-id="ca337-103">Создание androidEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca337-103">Create androidEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="ca337-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca337-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca337-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca337-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca337-106">Создание нового объекта [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ca337-106">Create a new [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca337-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ca337-107">Prerequisites</span></span>
<span data-ttu-id="ca337-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca337-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca337-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca337-110">Permission type</span></span>|<span data-ttu-id="ca337-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca337-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca337-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca337-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca337-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca337-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca337-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca337-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca337-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca337-115">Not supported.</span></span>|
|<span data-ttu-id="ca337-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca337-116">Application</span></span>|<span data-ttu-id="ca337-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca337-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca337-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca337-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ca337-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca337-119">Request headers</span></span>
|<span data-ttu-id="ca337-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca337-120">Header</span></span>|<span data-ttu-id="ca337-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ca337-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca337-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca337-122">Authorization</span></span>|<span data-ttu-id="ca337-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca337-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca337-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ca337-124">Accept</span></span>|<span data-ttu-id="ca337-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca337-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca337-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ca337-126">Request body</span></span>
<span data-ttu-id="ca337-127">В тексте запроса добавьте представление объекта androidEnterpriseWiFiConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca337-127">In the request body, supply a JSON representation for the androidEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="ca337-128">В следующей таблице приведены свойства, необходимые при создании androidEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ca337-128">The following table shows the properties that are required when you create the androidEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="ca337-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca337-129">Property</span></span>|<span data-ttu-id="ca337-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ca337-130">Type</span></span>|<span data-ttu-id="ca337-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ca337-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca337-132">id</span><span class="sxs-lookup"><span data-stu-id="ca337-132">id</span></span>|<span data-ttu-id="ca337-133">String</span><span class="sxs-lookup"><span data-stu-id="ca337-133">String</span></span>|<span data-ttu-id="ca337-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ca337-134">Key of the entity.</span></span> <span data-ttu-id="ca337-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca337-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca337-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca337-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ca337-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca337-137">DateTimeOffset</span></span>|<span data-ttu-id="ca337-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ca337-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ca337-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca337-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca337-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ca337-140">roleScopeTagIds</span></span>|<span data-ttu-id="ca337-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ca337-141">String collection</span></span>|<span data-ttu-id="ca337-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ca337-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ca337-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca337-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca337-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="ca337-144">supportsScopeTags</span></span>|<span data-ttu-id="ca337-145">Логический</span><span class="sxs-lookup"><span data-stu-id="ca337-145">Boolean</span></span>|<span data-ttu-id="ca337-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ca337-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ca337-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="ca337-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ca337-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ca337-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ca337-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca337-149">This property is read-only.</span></span> <span data-ttu-id="ca337-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca337-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca337-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca337-151">createdDateTime</span></span>|<span data-ttu-id="ca337-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca337-152">DateTimeOffset</span></span>|<span data-ttu-id="ca337-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ca337-153">DateTime the object was created.</span></span> <span data-ttu-id="ca337-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca337-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca337-155">description</span><span class="sxs-lookup"><span data-stu-id="ca337-155">description</span></span>|<span data-ttu-id="ca337-156">String</span><span class="sxs-lookup"><span data-stu-id="ca337-156">String</span></span>|<span data-ttu-id="ca337-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ca337-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ca337-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca337-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca337-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ca337-159">displayName</span></span>|<span data-ttu-id="ca337-160">Строка</span><span class="sxs-lookup"><span data-stu-id="ca337-160">String</span></span>|<span data-ttu-id="ca337-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ca337-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ca337-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca337-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca337-163">version</span><span class="sxs-lookup"><span data-stu-id="ca337-163">version</span></span>|<span data-ttu-id="ca337-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ca337-164">Int32</span></span>|<span data-ttu-id="ca337-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ca337-165">Version of the device configuration.</span></span> <span data-ttu-id="ca337-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca337-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca337-167">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="ca337-167">networkName</span></span>|<span data-ttu-id="ca337-168">Строка</span><span class="sxs-lookup"><span data-stu-id="ca337-168">String</span></span>|<span data-ttu-id="ca337-169">Сетевое имя, унаследованное от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca337-169">Network Name Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="ca337-170">SSID</span><span class="sxs-lookup"><span data-stu-id="ca337-170">ssid</span></span>|<span data-ttu-id="ca337-171">Строка</span><span class="sxs-lookup"><span data-stu-id="ca337-171">String</span></span>|<span data-ttu-id="ca337-172">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="ca337-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="ca337-173">Наследуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca337-173">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="ca337-174">Коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="ca337-174">connectAutomatically</span></span>|<span data-ttu-id="ca337-175">Логический</span><span class="sxs-lookup"><span data-stu-id="ca337-175">Boolean</span></span>|<span data-ttu-id="ca337-176">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="ca337-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="ca337-177">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="ca337-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="ca337-178">Наследуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca337-178">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="ca337-179">Коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="ca337-179">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="ca337-180">Логический</span><span class="sxs-lookup"><span data-stu-id="ca337-180">Boolean</span></span>|<span data-ttu-id="ca337-181">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="ca337-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="ca337-182">Наследуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca337-182">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="ca337-183">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="ca337-183">wiFiSecurityType</span></span>|[<span data-ttu-id="ca337-184">Андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="ca337-184">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="ca337-185">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="ca337-185">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="ca337-186">Наследуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca337-186">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span> <span data-ttu-id="ca337-187">Возможные значения: `open`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="ca337-187">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="ca337-188">Еаптипе</span><span class="sxs-lookup"><span data-stu-id="ca337-188">eapType</span></span>|[<span data-ttu-id="ca337-189">Андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="ca337-189">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="ca337-190">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="ca337-190">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="ca337-191">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="ca337-191">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="ca337-192">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="ca337-192">authenticationMethod</span></span>|[<span data-ttu-id="ca337-193">Вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="ca337-193">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="ca337-194">Указывает метод проверки подлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="ca337-194">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="ca337-195">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="ca337-195">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="ca337-196">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="ca337-196">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="ca337-197">Нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="ca337-197">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="ca337-198">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="ca337-198">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="ca337-199">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="ca337-199">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="ca337-200">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="ca337-200">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="ca337-201">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="ca337-201">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="ca337-202">Метод проверки подлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="ca337-202">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="ca337-203">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="ca337-203">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="ca337-204">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="ca337-204">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="ca337-205">Строка</span><span class="sxs-lookup"><span data-stu-id="ca337-205">String</span></span>|<span data-ttu-id="ca337-206">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="ca337-206">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="ca337-207">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="ca337-207">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|
|<span data-ttu-id="ca337-208">Усернамеформатстринг</span><span class="sxs-lookup"><span data-stu-id="ca337-208">usernameFormatString</span></span>|<span data-ttu-id="ca337-209">Строка</span><span class="sxs-lookup"><span data-stu-id="ca337-209">String</span></span>|<span data-ttu-id="ca337-210">Строка формата имени пользователя, используемая для построения имени пользователя для подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="ca337-210">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="ca337-211">Пассвордформатстринг</span><span class="sxs-lookup"><span data-stu-id="ca337-211">passwordFormatString</span></span>|<span data-ttu-id="ca337-212">Строка</span><span class="sxs-lookup"><span data-stu-id="ca337-212">String</span></span>|<span data-ttu-id="ca337-213">Строка формата пароля, используемая для создания пароля подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="ca337-213">Password format string used to build the password to connect to wifi</span></span>|
|<span data-ttu-id="ca337-214">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="ca337-214">preSharedKey</span></span>|<span data-ttu-id="ca337-215">Строка</span><span class="sxs-lookup"><span data-stu-id="ca337-215">String</span></span>|<span data-ttu-id="ca337-216">PreSharedKey, используемый для создания пароля подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="ca337-216">PreSharedKey used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="ca337-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca337-217">Response</span></span>
<span data-ttu-id="ca337-218">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca337-218">If successful, this method returns a `201 Created` response code and a [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca337-219">Пример</span><span class="sxs-lookup"><span data-stu-id="ca337-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca337-220">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca337-220">Request</span></span>
<span data-ttu-id="ca337-221">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca337-221">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 926

{
  "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value",
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="ca337-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca337-222">Response</span></span>
<span data-ttu-id="ca337-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca337-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1098

{
  "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
  "id": "972edff4-dff4-972e-f4df-2e97f4df2e97",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value",
  "preSharedKey": "Pre Shared Key value"
}
```




