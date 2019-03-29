---
title: Обновление androidEnterpriseWiFiConfiguration
description: Обновление свойств объекта androidEnterpriseWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b3ff22b96975001cde8cedcf79fe14c061401f54
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957831"
---
# <a name="update-androidenterprisewificonfiguration"></a><span data-ttu-id="06874-103">Обновление androidEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="06874-103">Update androidEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="06874-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06874-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06874-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06874-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06874-106">Обновление свойств объекта [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="06874-106">Update the properties of a [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06874-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="06874-107">Prerequisites</span></span>
<span data-ttu-id="06874-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06874-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06874-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06874-110">Permission type</span></span>|<span data-ttu-id="06874-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="06874-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06874-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06874-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06874-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06874-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06874-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06874-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06874-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06874-115">Not supported.</span></span>|
|<span data-ttu-id="06874-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06874-116">Application</span></span>|<span data-ttu-id="06874-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06874-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06874-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06874-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="06874-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06874-119">Request headers</span></span>
|<span data-ttu-id="06874-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06874-120">Header</span></span>|<span data-ttu-id="06874-121">Значение</span><span class="sxs-lookup"><span data-stu-id="06874-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06874-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06874-122">Authorization</span></span>|<span data-ttu-id="06874-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06874-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06874-124">Accept</span><span class="sxs-lookup"><span data-stu-id="06874-124">Accept</span></span>|<span data-ttu-id="06874-125">application/json</span><span class="sxs-lookup"><span data-stu-id="06874-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06874-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06874-126">Request body</span></span>
<span data-ttu-id="06874-127">В тексте запроса добавьте представление объекта [AndroidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06874-127">In the request body, supply a JSON representation for the [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="06874-128">В следующей таблице приведены свойства, необходимые при создании [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06874-128">The following table shows the properties that are required when you create the [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="06874-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="06874-129">Property</span></span>|<span data-ttu-id="06874-130">Тип</span><span class="sxs-lookup"><span data-stu-id="06874-130">Type</span></span>|<span data-ttu-id="06874-131">Описание</span><span class="sxs-lookup"><span data-stu-id="06874-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06874-132">id</span><span class="sxs-lookup"><span data-stu-id="06874-132">id</span></span>|<span data-ttu-id="06874-133">Строка</span><span class="sxs-lookup"><span data-stu-id="06874-133">String</span></span>|<span data-ttu-id="06874-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="06874-134">Key of the entity.</span></span> <span data-ttu-id="06874-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06874-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06874-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06874-136">lastModifiedDateTime</span></span>|<span data-ttu-id="06874-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06874-137">DateTimeOffset</span></span>|<span data-ttu-id="06874-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="06874-138">DateTime the object was last modified.</span></span> <span data-ttu-id="06874-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06874-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06874-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="06874-140">roleScopeTagIds</span></span>|<span data-ttu-id="06874-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="06874-141">String collection</span></span>|<span data-ttu-id="06874-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="06874-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="06874-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06874-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06874-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="06874-144">supportsScopeTags</span></span>|<span data-ttu-id="06874-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="06874-145">Boolean</span></span>|<span data-ttu-id="06874-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="06874-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="06874-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="06874-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="06874-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="06874-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="06874-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="06874-149">This property is read-only.</span></span> <span data-ttu-id="06874-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06874-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06874-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06874-151">createdDateTime</span></span>|<span data-ttu-id="06874-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06874-152">DateTimeOffset</span></span>|<span data-ttu-id="06874-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="06874-153">DateTime the object was created.</span></span> <span data-ttu-id="06874-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06874-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06874-155">description</span><span class="sxs-lookup"><span data-stu-id="06874-155">description</span></span>|<span data-ttu-id="06874-156">String</span><span class="sxs-lookup"><span data-stu-id="06874-156">String</span></span>|<span data-ttu-id="06874-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="06874-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="06874-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06874-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06874-159">displayName</span><span class="sxs-lookup"><span data-stu-id="06874-159">displayName</span></span>|<span data-ttu-id="06874-160">String</span><span class="sxs-lookup"><span data-stu-id="06874-160">String</span></span>|<span data-ttu-id="06874-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="06874-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="06874-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06874-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06874-163">version</span><span class="sxs-lookup"><span data-stu-id="06874-163">version</span></span>|<span data-ttu-id="06874-164">Int32</span><span class="sxs-lookup"><span data-stu-id="06874-164">Int32</span></span>|<span data-ttu-id="06874-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="06874-165">Version of the device configuration.</span></span> <span data-ttu-id="06874-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06874-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06874-167">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="06874-167">networkName</span></span>|<span data-ttu-id="06874-168">String</span><span class="sxs-lookup"><span data-stu-id="06874-168">String</span></span>|<span data-ttu-id="06874-169">Сетевое имя, унаследованное от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06874-169">Network Name Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="06874-170">SSID</span><span class="sxs-lookup"><span data-stu-id="06874-170">ssid</span></span>|<span data-ttu-id="06874-171">String</span><span class="sxs-lookup"><span data-stu-id="06874-171">String</span></span>|<span data-ttu-id="06874-172">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="06874-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="06874-173">НаСледуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06874-173">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="06874-174">Коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="06874-174">connectAutomatically</span></span>|<span data-ttu-id="06874-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="06874-175">Boolean</span></span>|<span data-ttu-id="06874-176">ПодКлючаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="06874-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="06874-177">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="06874-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="06874-178">НаСледуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06874-178">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="06874-179">Коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="06874-179">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="06874-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="06874-180">Boolean</span></span>|<span data-ttu-id="06874-181">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="06874-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="06874-182">НаСледуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06874-182">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="06874-183">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="06874-183">wiFiSecurityType</span></span>|[<span data-ttu-id="06874-184">Андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="06874-184">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="06874-185">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="06874-185">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="06874-186">НаСледуется от [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06874-186">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span> <span data-ttu-id="06874-187">Возможные значения: `open`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="06874-187">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="06874-188">Еаптипе</span><span class="sxs-lookup"><span data-stu-id="06874-188">eapType</span></span>|[<span data-ttu-id="06874-189">Андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="06874-189">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="06874-190">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="06874-190">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="06874-191">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="06874-191">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="06874-192">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="06874-192">authenticationMethod</span></span>|[<span data-ttu-id="06874-193">Вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="06874-193">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="06874-194">Указывает метод проверки поДлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="06874-194">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="06874-195">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="06874-195">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="06874-196">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="06874-196">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="06874-197">Нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="06874-197">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="06874-198">Метод проверки поДлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="06874-198">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="06874-199">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="06874-199">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="06874-200">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="06874-200">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="06874-201">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="06874-201">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="06874-202">Метод проверки поДлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="06874-202">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="06874-203">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="06874-203">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="06874-204">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="06874-204">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="06874-205">String</span><span class="sxs-lookup"><span data-stu-id="06874-205">String</span></span>|<span data-ttu-id="06874-206">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="06874-206">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="06874-207">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="06874-207">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="06874-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="06874-208">Response</span></span>
<span data-ttu-id="06874-209">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06874-209">If successful, this method returns a `200 OK` response code and an updated [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06874-210">Пример</span><span class="sxs-lookup"><span data-stu-id="06874-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="06874-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="06874-211">Request</span></span>
<span data-ttu-id="06874-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06874-212">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 765

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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="06874-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="06874-213">Response</span></span>
<span data-ttu-id="06874-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06874-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 937

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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




