---
title: Создание androidForWorkEnterpriseWiFiConfiguration
description: Создание нового объекта androidForWorkEnterpriseWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b5fbadc2841b6583987394cc8ca7921ca0f9c725
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32479311"
---
# <a name="create-androidforworkenterprisewificonfiguration"></a><span data-ttu-id="ce9af-103">Создание androidForWorkEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="ce9af-103">Create androidForWorkEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="ce9af-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce9af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce9af-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce9af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce9af-106">Создание нового объекта [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ce9af-106">Create a new [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce9af-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ce9af-107">Prerequisites</span></span>
<span data-ttu-id="ce9af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce9af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce9af-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce9af-110">Permission type</span></span>|<span data-ttu-id="ce9af-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce9af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce9af-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce9af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ce9af-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce9af-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ce9af-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce9af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce9af-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce9af-115">Not supported.</span></span>|
|<span data-ttu-id="ce9af-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce9af-116">Application</span></span>|<span data-ttu-id="ce9af-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce9af-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce9af-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce9af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ce9af-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce9af-119">Request headers</span></span>
|<span data-ttu-id="ce9af-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce9af-120">Header</span></span>|<span data-ttu-id="ce9af-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ce9af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce9af-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce9af-122">Authorization</span></span>|<span data-ttu-id="ce9af-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce9af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce9af-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ce9af-124">Accept</span></span>|<span data-ttu-id="ce9af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ce9af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce9af-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce9af-126">Request body</span></span>
<span data-ttu-id="ce9af-127">В тексте запроса добавьте представление объекта androidForWorkEnterpriseWiFiConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce9af-127">In the request body, supply a JSON representation for the androidForWorkEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="ce9af-128">В следующей таблице приведены свойства, необходимые при создании androidForWorkEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ce9af-128">The following table shows the properties that are required when you create the androidForWorkEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="ce9af-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce9af-129">Property</span></span>|<span data-ttu-id="ce9af-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ce9af-130">Type</span></span>|<span data-ttu-id="ce9af-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ce9af-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce9af-132">id</span><span class="sxs-lookup"><span data-stu-id="ce9af-132">id</span></span>|<span data-ttu-id="ce9af-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ce9af-133">String</span></span>|<span data-ttu-id="ce9af-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ce9af-134">Key of the entity.</span></span> <span data-ttu-id="ce9af-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce9af-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce9af-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce9af-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ce9af-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce9af-137">DateTimeOffset</span></span>|<span data-ttu-id="ce9af-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ce9af-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ce9af-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce9af-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce9af-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ce9af-140">roleScopeTagIds</span></span>|<span data-ttu-id="ce9af-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ce9af-141">String collection</span></span>|<span data-ttu-id="ce9af-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ce9af-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ce9af-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce9af-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce9af-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="ce9af-144">supportsScopeTags</span></span>|<span data-ttu-id="ce9af-145">Логический</span><span class="sxs-lookup"><span data-stu-id="ce9af-145">Boolean</span></span>|<span data-ttu-id="ce9af-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ce9af-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ce9af-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="ce9af-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ce9af-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ce9af-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ce9af-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce9af-149">This property is read-only.</span></span> <span data-ttu-id="ce9af-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce9af-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce9af-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce9af-151">createdDateTime</span></span>|<span data-ttu-id="ce9af-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce9af-152">DateTimeOffset</span></span>|<span data-ttu-id="ce9af-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ce9af-153">DateTime the object was created.</span></span> <span data-ttu-id="ce9af-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce9af-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce9af-155">description</span><span class="sxs-lookup"><span data-stu-id="ce9af-155">description</span></span>|<span data-ttu-id="ce9af-156">String</span><span class="sxs-lookup"><span data-stu-id="ce9af-156">String</span></span>|<span data-ttu-id="ce9af-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ce9af-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ce9af-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce9af-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce9af-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ce9af-159">displayName</span></span>|<span data-ttu-id="ce9af-160">String</span><span class="sxs-lookup"><span data-stu-id="ce9af-160">String</span></span>|<span data-ttu-id="ce9af-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ce9af-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ce9af-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce9af-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce9af-163">version</span><span class="sxs-lookup"><span data-stu-id="ce9af-163">version</span></span>|<span data-ttu-id="ce9af-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ce9af-164">Int32</span></span>|<span data-ttu-id="ce9af-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ce9af-165">Version of the device configuration.</span></span> <span data-ttu-id="ce9af-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce9af-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce9af-167">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="ce9af-167">networkName</span></span>|<span data-ttu-id="ce9af-168">String</span><span class="sxs-lookup"><span data-stu-id="ce9af-168">String</span></span>|<span data-ttu-id="ce9af-169">Сетевое имя, унаследованное от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce9af-169">Network Name Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="ce9af-170">SSID</span><span class="sxs-lookup"><span data-stu-id="ce9af-170">ssid</span></span>|<span data-ttu-id="ce9af-171">String</span><span class="sxs-lookup"><span data-stu-id="ce9af-171">String</span></span>|<span data-ttu-id="ce9af-172">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="ce9af-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="ce9af-173">НаСледуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce9af-173">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="ce9af-174">Коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="ce9af-174">connectAutomatically</span></span>|<span data-ttu-id="ce9af-175">Логический</span><span class="sxs-lookup"><span data-stu-id="ce9af-175">Boolean</span></span>|<span data-ttu-id="ce9af-176">ПодКлючаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="ce9af-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="ce9af-177">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="ce9af-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="ce9af-178">НаСледуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce9af-178">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="ce9af-179">Коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="ce9af-179">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="ce9af-180">Логический</span><span class="sxs-lookup"><span data-stu-id="ce9af-180">Boolean</span></span>|<span data-ttu-id="ce9af-181">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="ce9af-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="ce9af-182">НаСледуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce9af-182">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="ce9af-183">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="ce9af-183">wiFiSecurityType</span></span>|[<span data-ttu-id="ce9af-184">Андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="ce9af-184">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="ce9af-185">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="ce9af-185">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="ce9af-186">НаСледуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce9af-186">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span> <span data-ttu-id="ce9af-187">Возможные значения: `open`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="ce9af-187">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="ce9af-188">Еаптипе</span><span class="sxs-lookup"><span data-stu-id="ce9af-188">eapType</span></span>|[<span data-ttu-id="ce9af-189">Андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="ce9af-189">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="ce9af-190">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="ce9af-190">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="ce9af-191">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="ce9af-191">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="ce9af-192">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="ce9af-192">authenticationMethod</span></span>|[<span data-ttu-id="ce9af-193">Вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="ce9af-193">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="ce9af-194">Указывает метод проверки поДлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="ce9af-194">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="ce9af-195">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="ce9af-195">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="ce9af-196">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="ce9af-196">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="ce9af-197">Нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="ce9af-197">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="ce9af-198">Метод проверки поДлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="ce9af-198">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="ce9af-199">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="ce9af-199">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="ce9af-200">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="ce9af-200">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="ce9af-201">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="ce9af-201">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="ce9af-202">Метод проверки поДлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="ce9af-202">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="ce9af-203">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="ce9af-203">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="ce9af-204">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="ce9af-204">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="ce9af-205">String</span><span class="sxs-lookup"><span data-stu-id="ce9af-205">String</span></span>|<span data-ttu-id="ce9af-206">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="ce9af-206">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="ce9af-207">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="ce9af-207">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="ce9af-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce9af-208">Response</span></span>
<span data-ttu-id="ce9af-209">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ce9af-209">If successful, this method returns a `201 Created` response code and a [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce9af-210">Пример</span><span class="sxs-lookup"><span data-stu-id="ce9af-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce9af-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce9af-211">Request</span></span>
<span data-ttu-id="ce9af-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce9af-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 772

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="ce9af-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce9af-213">Response</span></span>
<span data-ttu-id="ce9af-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce9af-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 944

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
  "id": "742d953a-953a-742d-3a95-2d743a952d74",
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





