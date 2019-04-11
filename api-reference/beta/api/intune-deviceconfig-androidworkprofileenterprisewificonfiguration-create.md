---
title: Создание Андроидворкпрофилинтерприсевификонфигуратион
description: Создание нового объекта Андроидворкпрофилинтерприсевификонфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94ea0481b8be51569c789d87664758bb05a0e6d0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773016"
---
# <a name="create-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="ffd0f-103">Создание Андроидворкпрофилинтерприсевификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="ffd0f-103">Create androidWorkProfileEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="ffd0f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffd0f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffd0f-106">Создание нового объекта [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ffd0f-106">Create a new [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffd0f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ffd0f-107">Prerequisites</span></span>
<span data-ttu-id="ffd0f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffd0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffd0f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffd0f-110">Permission type</span></span>|<span data-ttu-id="ffd0f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffd0f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffd0f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffd0f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ffd0f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffd0f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ffd0f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffd0f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffd0f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-115">Not supported.</span></span>|
|<span data-ttu-id="ffd0f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffd0f-116">Application</span></span>|<span data-ttu-id="ffd0f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffd0f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffd0f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ffd0f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffd0f-119">Request headers</span></span>
|<span data-ttu-id="ffd0f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffd0f-120">Header</span></span>|<span data-ttu-id="ffd0f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ffd0f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffd0f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ffd0f-122">Authorization</span></span>|<span data-ttu-id="ffd0f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffd0f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ffd0f-124">Accept</span></span>|<span data-ttu-id="ffd0f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ffd0f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffd0f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ffd0f-126">Request body</span></span>
<span data-ttu-id="ffd0f-127">В тексте запроса добавьте представление объекта Андроидворкпрофилинтерприсевификонфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-127">In the request body, supply a JSON representation for the androidWorkProfileEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="ffd0f-128">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилинтерприсевификонфигуратион.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-128">The following table shows the properties that are required when you create the androidWorkProfileEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="ffd0f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ffd0f-129">Property</span></span>|<span data-ttu-id="ffd0f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ffd0f-130">Type</span></span>|<span data-ttu-id="ffd0f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ffd0f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffd0f-132">id</span><span class="sxs-lookup"><span data-stu-id="ffd0f-132">id</span></span>|<span data-ttu-id="ffd0f-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ffd0f-133">String</span></span>|<span data-ttu-id="ffd0f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-134">Key of the entity.</span></span> <span data-ttu-id="ffd0f-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffd0f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffd0f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ffd0f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ffd0f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffd0f-137">DateTimeOffset</span></span>|<span data-ttu-id="ffd0f-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ffd0f-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffd0f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffd0f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ffd0f-140">roleScopeTagIds</span></span>|<span data-ttu-id="ffd0f-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ffd0f-141">String collection</span></span>|<span data-ttu-id="ffd0f-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ffd0f-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffd0f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffd0f-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="ffd0f-144">supportsScopeTags</span></span>|<span data-ttu-id="ffd0f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffd0f-145">Boolean</span></span>|<span data-ttu-id="ffd0f-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ffd0f-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ffd0f-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ffd0f-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-149">This property is read-only.</span></span> <span data-ttu-id="ffd0f-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffd0f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffd0f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ffd0f-151">createdDateTime</span></span>|<span data-ttu-id="ffd0f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffd0f-152">DateTimeOffset</span></span>|<span data-ttu-id="ffd0f-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-153">DateTime the object was created.</span></span> <span data-ttu-id="ffd0f-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffd0f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffd0f-155">description</span><span class="sxs-lookup"><span data-stu-id="ffd0f-155">description</span></span>|<span data-ttu-id="ffd0f-156">String</span><span class="sxs-lookup"><span data-stu-id="ffd0f-156">String</span></span>|<span data-ttu-id="ffd0f-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ffd0f-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffd0f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffd0f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ffd0f-159">displayName</span></span>|<span data-ttu-id="ffd0f-160">String</span><span class="sxs-lookup"><span data-stu-id="ffd0f-160">String</span></span>|<span data-ttu-id="ffd0f-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ffd0f-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffd0f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffd0f-163">version</span><span class="sxs-lookup"><span data-stu-id="ffd0f-163">version</span></span>|<span data-ttu-id="ffd0f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ffd0f-164">Int32</span></span>|<span data-ttu-id="ffd0f-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-165">Version of the device configuration.</span></span> <span data-ttu-id="ffd0f-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffd0f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffd0f-167">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="ffd0f-167">networkName</span></span>|<span data-ttu-id="ffd0f-168">String</span><span class="sxs-lookup"><span data-stu-id="ffd0f-168">String</span></span>|<span data-ttu-id="ffd0f-169">Сетевое имя, унаследованное от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffd0f-169">Network Name Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="ffd0f-170">SSID</span><span class="sxs-lookup"><span data-stu-id="ffd0f-170">ssid</span></span>|<span data-ttu-id="ffd0f-171">String</span><span class="sxs-lookup"><span data-stu-id="ffd0f-171">String</span></span>|<span data-ttu-id="ffd0f-172">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="ffd0f-173">НаСледуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffd0f-173">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="ffd0f-174">Коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="ffd0f-174">connectAutomatically</span></span>|<span data-ttu-id="ffd0f-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffd0f-175">Boolean</span></span>|<span data-ttu-id="ffd0f-176">ПодКлючаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="ffd0f-177">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="ffd0f-178">НаСледуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffd0f-178">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="ffd0f-179">Коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="ffd0f-179">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="ffd0f-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffd0f-180">Boolean</span></span>|<span data-ttu-id="ffd0f-181">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="ffd0f-182">НаСледуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffd0f-182">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="ffd0f-183">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="ffd0f-183">wiFiSecurityType</span></span>|[<span data-ttu-id="ffd0f-184">Андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="ffd0f-184">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="ffd0f-185">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-185">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="ffd0f-186">НаСледуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffd0f-186">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span> <span data-ttu-id="ffd0f-187">Возможные значения: `open`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-187">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="ffd0f-188">Еаптипе</span><span class="sxs-lookup"><span data-stu-id="ffd0f-188">eapType</span></span>|[<span data-ttu-id="ffd0f-189">Андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="ffd0f-189">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="ffd0f-190">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="ffd0f-190">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="ffd0f-191">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-191">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="ffd0f-192">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="ffd0f-192">authenticationMethod</span></span>|[<span data-ttu-id="ffd0f-193">Вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="ffd0f-193">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="ffd0f-194">Указывает метод проверки поДлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-194">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="ffd0f-195">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-195">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="ffd0f-196">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="ffd0f-196">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="ffd0f-197">Нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="ffd0f-197">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="ffd0f-198">Метод проверки поДлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-198">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="ffd0f-199">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-199">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="ffd0f-200">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="ffd0f-200">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="ffd0f-201">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="ffd0f-201">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="ffd0f-202">Метод проверки поДлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-202">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="ffd0f-203">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-203">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="ffd0f-204">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="ffd0f-204">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="ffd0f-205">String</span><span class="sxs-lookup"><span data-stu-id="ffd0f-205">String</span></span>|<span data-ttu-id="ffd0f-206">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-206">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="ffd0f-207">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-207">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="ffd0f-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffd0f-208">Response</span></span>
<span data-ttu-id="ffd0f-209">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-209">If successful, this method returns a `201 Created` response code and a [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffd0f-210">Пример</span><span class="sxs-lookup"><span data-stu-id="ffd0f-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffd0f-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffd0f-211">Request</span></span>
<span data-ttu-id="ffd0f-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 776

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="ffd0f-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffd0f-213">Response</span></span>
<span data-ttu-id="ffd0f-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ffd0f-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 948

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
  "id": "c48cd726-d726-c48c-26d7-8cc426d78cc4",
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





