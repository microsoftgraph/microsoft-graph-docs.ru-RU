---
title: Обновление Андроидворкпрофилинтерприсевификонфигуратион
description: Обновление свойств объекта Андроидворкпрофилинтерприсевификонфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5def1cb85d57c3d4a90fa573444b646f54d31117
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152334"
---
# <a name="update-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="c5366-103">Обновление Андроидворкпрофилинтерприсевификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="c5366-103">Update androidWorkProfileEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="c5366-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5366-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5366-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5366-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5366-106">Обновление свойств объекта [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c5366-106">Update the properties of a [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5366-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c5366-107">Prerequisites</span></span>
<span data-ttu-id="c5366-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5366-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c5366-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5366-110">Permission type</span></span>|<span data-ttu-id="c5366-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5366-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5366-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5366-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5366-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5366-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c5366-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5366-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5366-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5366-115">Not supported.</span></span>|
|<span data-ttu-id="c5366-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5366-116">Application</span></span>|<span data-ttu-id="c5366-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5366-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5366-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5366-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c5366-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5366-119">Request headers</span></span>
|<span data-ttu-id="c5366-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5366-120">Header</span></span>|<span data-ttu-id="c5366-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c5366-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5366-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5366-122">Authorization</span></span>|<span data-ttu-id="c5366-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c5366-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5366-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c5366-124">Accept</span></span>|<span data-ttu-id="c5366-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c5366-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5366-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5366-126">Request body</span></span>
<span data-ttu-id="c5366-127">В тексте запроса добавьте представление объекта [Андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5366-127">In the request body, supply a JSON representation for the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="c5366-128">В следующей таблице приведены свойства, необходимые при создании [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5366-128">The following table shows the properties that are required when you create the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="c5366-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5366-129">Property</span></span>|<span data-ttu-id="c5366-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c5366-130">Type</span></span>|<span data-ttu-id="c5366-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c5366-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5366-132">id</span><span class="sxs-lookup"><span data-stu-id="c5366-132">id</span></span>|<span data-ttu-id="c5366-133">String</span><span class="sxs-lookup"><span data-stu-id="c5366-133">String</span></span>|<span data-ttu-id="c5366-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c5366-134">Key of the entity.</span></span> <span data-ttu-id="c5366-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5366-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5366-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5366-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c5366-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5366-137">DateTimeOffset</span></span>|<span data-ttu-id="c5366-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c5366-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c5366-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5366-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5366-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c5366-140">roleScopeTagIds</span></span>|<span data-ttu-id="c5366-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c5366-141">String collection</span></span>|<span data-ttu-id="c5366-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c5366-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c5366-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5366-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5366-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c5366-144">supportsScopeTags</span></span>|<span data-ttu-id="c5366-145">Логический</span><span class="sxs-lookup"><span data-stu-id="c5366-145">Boolean</span></span>|<span data-ttu-id="c5366-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c5366-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c5366-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c5366-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c5366-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c5366-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c5366-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c5366-149">This property is read-only.</span></span> <span data-ttu-id="c5366-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5366-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5366-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5366-151">createdDateTime</span></span>|<span data-ttu-id="c5366-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5366-152">DateTimeOffset</span></span>|<span data-ttu-id="c5366-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c5366-153">DateTime the object was created.</span></span> <span data-ttu-id="c5366-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5366-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5366-155">description</span><span class="sxs-lookup"><span data-stu-id="c5366-155">description</span></span>|<span data-ttu-id="c5366-156">String</span><span class="sxs-lookup"><span data-stu-id="c5366-156">String</span></span>|<span data-ttu-id="c5366-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c5366-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c5366-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5366-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5366-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c5366-159">displayName</span></span>|<span data-ttu-id="c5366-160">String</span><span class="sxs-lookup"><span data-stu-id="c5366-160">String</span></span>|<span data-ttu-id="c5366-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c5366-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c5366-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5366-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5366-163">version</span><span class="sxs-lookup"><span data-stu-id="c5366-163">version</span></span>|<span data-ttu-id="c5366-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c5366-164">Int32</span></span>|<span data-ttu-id="c5366-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c5366-165">Version of the device configuration.</span></span> <span data-ttu-id="c5366-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5366-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5366-167">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="c5366-167">networkName</span></span>|<span data-ttu-id="c5366-168">String</span><span class="sxs-lookup"><span data-stu-id="c5366-168">String</span></span>|<span data-ttu-id="c5366-169">Сетевое имя, унаследованное от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5366-169">Network Name Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="c5366-170">SSID</span><span class="sxs-lookup"><span data-stu-id="c5366-170">ssid</span></span>|<span data-ttu-id="c5366-171">String</span><span class="sxs-lookup"><span data-stu-id="c5366-171">String</span></span>|<span data-ttu-id="c5366-172">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="c5366-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="c5366-173">НаСледуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5366-173">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="c5366-174">Коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="c5366-174">connectAutomatically</span></span>|<span data-ttu-id="c5366-175">Логический</span><span class="sxs-lookup"><span data-stu-id="c5366-175">Boolean</span></span>|<span data-ttu-id="c5366-176">ПодКлючаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="c5366-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="c5366-177">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="c5366-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="c5366-178">НаСледуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5366-178">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="c5366-179">Коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="c5366-179">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="c5366-180">Логический</span><span class="sxs-lookup"><span data-stu-id="c5366-180">Boolean</span></span>|<span data-ttu-id="c5366-181">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="c5366-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="c5366-182">НаСледуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5366-182">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="c5366-183">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="c5366-183">wiFiSecurityType</span></span>|[<span data-ttu-id="c5366-184">Андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="c5366-184">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="c5366-185">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="c5366-185">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="c5366-186">НаСледуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c5366-186">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span> <span data-ttu-id="c5366-187">Возможные значения: `open`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="c5366-187">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="c5366-188">Еаптипе</span><span class="sxs-lookup"><span data-stu-id="c5366-188">eapType</span></span>|[<span data-ttu-id="c5366-189">Андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="c5366-189">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="c5366-190">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="c5366-190">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="c5366-191">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="c5366-191">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="c5366-192">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="c5366-192">authenticationMethod</span></span>|[<span data-ttu-id="c5366-193">Вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="c5366-193">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="c5366-194">Указывает метод проверки поДлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="c5366-194">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="c5366-195">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="c5366-195">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="c5366-196">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="c5366-196">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="c5366-197">Нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="c5366-197">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="c5366-198">Метод проверки поДлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="c5366-198">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="c5366-199">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="c5366-199">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="c5366-200">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="c5366-200">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="c5366-201">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="c5366-201">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="c5366-202">Метод проверки поДлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="c5366-202">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="c5366-203">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="c5366-203">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="c5366-204">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="c5366-204">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="c5366-205">String</span><span class="sxs-lookup"><span data-stu-id="c5366-205">String</span></span>|<span data-ttu-id="c5366-206">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="c5366-206">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="c5366-207">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="c5366-207">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="c5366-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5366-208">Response</span></span>
<span data-ttu-id="c5366-209">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5366-209">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5366-210">Пример</span><span class="sxs-lookup"><span data-stu-id="c5366-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5366-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5366-211">Request</span></span>
<span data-ttu-id="c5366-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5366-212">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="c5366-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5366-213">Response</span></span>
<span data-ttu-id="c5366-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c5366-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




