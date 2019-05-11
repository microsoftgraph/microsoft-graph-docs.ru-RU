---
title: Обновление androidEnterpriseWiFiConfiguration
description: Обновление свойств объекта androidEnterpriseWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: daa945b2f6919ea75e9730edc393b8fd57182c93
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33932915"
---
# <a name="update-androidenterprisewificonfiguration"></a><span data-ttu-id="61133-103">Обновление androidEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="61133-103">Update androidEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="61133-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61133-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61133-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="61133-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61133-106">Обновление свойств объекта [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="61133-106">Update the properties of a [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61133-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="61133-107">Prerequisites</span></span>
<span data-ttu-id="61133-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61133-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61133-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61133-110">Permission type</span></span>|<span data-ttu-id="61133-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="61133-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61133-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61133-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61133-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61133-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="61133-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61133-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61133-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61133-115">Not supported.</span></span>|
|<span data-ttu-id="61133-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61133-116">Application</span></span>|<span data-ttu-id="61133-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61133-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61133-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61133-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="61133-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61133-119">Request headers</span></span>
|<span data-ttu-id="61133-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="61133-120">Header</span></span>|<span data-ttu-id="61133-121">Значение</span><span class="sxs-lookup"><span data-stu-id="61133-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61133-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="61133-122">Authorization</span></span>|<span data-ttu-id="61133-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61133-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61133-124">Accept</span><span class="sxs-lookup"><span data-stu-id="61133-124">Accept</span></span>|<span data-ttu-id="61133-125">application/json</span><span class="sxs-lookup"><span data-stu-id="61133-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61133-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="61133-126">Request body</span></span>
<span data-ttu-id="61133-127">В тексте запроса добавьте представление объекта [AndroidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61133-127">In the request body, supply a JSON representation for the [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="61133-128">В следующей таблице приведены свойства, необходимые при создании [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="61133-128">The following table shows the properties that are required when you create the [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="61133-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="61133-129">Property</span></span>|<span data-ttu-id="61133-130">Тип</span><span class="sxs-lookup"><span data-stu-id="61133-130">Type</span></span>|<span data-ttu-id="61133-131">Описание</span><span class="sxs-lookup"><span data-stu-id="61133-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61133-132">id</span><span class="sxs-lookup"><span data-stu-id="61133-132">id</span></span>|<span data-ttu-id="61133-133">String</span><span class="sxs-lookup"><span data-stu-id="61133-133">String</span></span>|<span data-ttu-id="61133-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="61133-134">Key of the entity.</span></span> <span data-ttu-id="61133-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="61133-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61133-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61133-136">lastModifiedDateTime</span></span>|<span data-ttu-id="61133-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61133-137">DateTimeOffset</span></span>|<span data-ttu-id="61133-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="61133-138">DateTime the object was last modified.</span></span> <span data-ttu-id="61133-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="61133-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61133-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="61133-140">roleScopeTagIds</span></span>|<span data-ttu-id="61133-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="61133-141">String collection</span></span>|<span data-ttu-id="61133-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="61133-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="61133-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="61133-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61133-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="61133-144">supportsScopeTags</span></span>|<span data-ttu-id="61133-145">Логический</span><span class="sxs-lookup"><span data-stu-id="61133-145">Boolean</span></span>|<span data-ttu-id="61133-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="61133-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="61133-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="61133-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="61133-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="61133-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="61133-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61133-149">This property is read-only.</span></span> <span data-ttu-id="61133-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="61133-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61133-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61133-151">createdDateTime</span></span>|<span data-ttu-id="61133-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61133-152">DateTimeOffset</span></span>|<span data-ttu-id="61133-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="61133-153">DateTime the object was created.</span></span> <span data-ttu-id="61133-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="61133-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61133-155">description</span><span class="sxs-lookup"><span data-stu-id="61133-155">description</span></span>|<span data-ttu-id="61133-156">String</span><span class="sxs-lookup"><span data-stu-id="61133-156">String</span></span>|<span data-ttu-id="61133-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="61133-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="61133-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="61133-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61133-159">displayName</span><span class="sxs-lookup"><span data-stu-id="61133-159">displayName</span></span>|<span data-ttu-id="61133-160">Строка</span><span class="sxs-lookup"><span data-stu-id="61133-160">String</span></span>|<span data-ttu-id="61133-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="61133-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="61133-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="61133-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61133-163">version</span><span class="sxs-lookup"><span data-stu-id="61133-163">version</span></span>|<span data-ttu-id="61133-164">Int32</span><span class="sxs-lookup"><span data-stu-id="61133-164">Int32</span></span>|<span data-ttu-id="61133-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="61133-165">Version of the device configuration.</span></span> <span data-ttu-id="61133-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="61133-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61133-167">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="61133-167">networkName</span></span>|<span data-ttu-id="61133-168">Строка</span><span class="sxs-lookup"><span data-stu-id="61133-168">String</span></span>|<span data-ttu-id="61133-169">Сетевое имя, унаследованное от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61133-169">Network Name Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="61133-170">SSID</span><span class="sxs-lookup"><span data-stu-id="61133-170">ssid</span></span>|<span data-ttu-id="61133-171">Строка</span><span class="sxs-lookup"><span data-stu-id="61133-171">String</span></span>|<span data-ttu-id="61133-172">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="61133-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="61133-173">Наследуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61133-173">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="61133-174">Коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="61133-174">connectAutomatically</span></span>|<span data-ttu-id="61133-175">Логический</span><span class="sxs-lookup"><span data-stu-id="61133-175">Boolean</span></span>|<span data-ttu-id="61133-176">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="61133-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="61133-177">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="61133-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="61133-178">Наследуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61133-178">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="61133-179">Коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="61133-179">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="61133-180">Логический</span><span class="sxs-lookup"><span data-stu-id="61133-180">Boolean</span></span>|<span data-ttu-id="61133-181">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="61133-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="61133-182">Наследуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61133-182">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="61133-183">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="61133-183">wiFiSecurityType</span></span>|[<span data-ttu-id="61133-184">Андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="61133-184">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="61133-185">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="61133-185">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="61133-186">Наследуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="61133-186">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span> <span data-ttu-id="61133-187">Возможные значения: `open`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="61133-187">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="61133-188">Еаптипе</span><span class="sxs-lookup"><span data-stu-id="61133-188">eapType</span></span>|[<span data-ttu-id="61133-189">Андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="61133-189">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="61133-190">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="61133-190">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="61133-191">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="61133-191">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="61133-192">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="61133-192">authenticationMethod</span></span>|[<span data-ttu-id="61133-193">Вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="61133-193">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="61133-194">Указывает метод проверки подлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="61133-194">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="61133-195">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="61133-195">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="61133-196">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="61133-196">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="61133-197">Нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="61133-197">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="61133-198">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="61133-198">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="61133-199">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="61133-199">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="61133-200">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="61133-200">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="61133-201">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="61133-201">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="61133-202">Метод проверки подлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="61133-202">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="61133-203">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="61133-203">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="61133-204">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="61133-204">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="61133-205">Строка</span><span class="sxs-lookup"><span data-stu-id="61133-205">String</span></span>|<span data-ttu-id="61133-206">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="61133-206">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="61133-207">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="61133-207">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|
|<span data-ttu-id="61133-208">Усернамеформатстринг</span><span class="sxs-lookup"><span data-stu-id="61133-208">usernameFormatString</span></span>|<span data-ttu-id="61133-209">Строка</span><span class="sxs-lookup"><span data-stu-id="61133-209">String</span></span>|<span data-ttu-id="61133-210">Строка формата имени пользователя, используемая для построения имени пользователя для подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="61133-210">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="61133-211">Пассвордформатстринг</span><span class="sxs-lookup"><span data-stu-id="61133-211">passwordFormatString</span></span>|<span data-ttu-id="61133-212">Строка</span><span class="sxs-lookup"><span data-stu-id="61133-212">String</span></span>|<span data-ttu-id="61133-213">Строка формата пароля, используемая для создания пароля подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="61133-213">Password format string used to build the password to connect to wifi</span></span>|
|<span data-ttu-id="61133-214">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="61133-214">preSharedKey</span></span>|<span data-ttu-id="61133-215">Строка</span><span class="sxs-lookup"><span data-stu-id="61133-215">String</span></span>|<span data-ttu-id="61133-216">PreSharedKey, используемый для создания пароля подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="61133-216">PreSharedKey used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="61133-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="61133-217">Response</span></span>
<span data-ttu-id="61133-218">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="61133-218">If successful, this method returns a `200 OK` response code and an updated [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61133-219">Пример</span><span class="sxs-lookup"><span data-stu-id="61133-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="61133-220">Запрос</span><span class="sxs-lookup"><span data-stu-id="61133-220">Request</span></span>
<span data-ttu-id="61133-221">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61133-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="61133-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="61133-222">Response</span></span>
<span data-ttu-id="61133-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="61133-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




