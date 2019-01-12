---
title: Создание androidWorkProfileEnterpriseWiFiConfiguration
description: Создание нового объекта androidWorkProfileEnterpriseWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 200055c11b41f437a7bcfad332a104887697848c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929216"
---
# <a name="create-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="6de40-103">Создание androidWorkProfileEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="6de40-103">Create androidWorkProfileEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="6de40-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6de40-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6de40-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6de40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6de40-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6de40-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6de40-107">Создание нового объекта [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6de40-107">Create a new [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6de40-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6de40-108">Prerequisites</span></span>
<span data-ttu-id="6de40-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6de40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6de40-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6de40-111">Permission type</span></span>|<span data-ttu-id="6de40-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6de40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6de40-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6de40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6de40-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6de40-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6de40-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6de40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6de40-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6de40-116">Not supported.</span></span>|
|<span data-ttu-id="6de40-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6de40-117">Application</span></span>|<span data-ttu-id="6de40-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6de40-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6de40-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6de40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6de40-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6de40-120">Request headers</span></span>
|<span data-ttu-id="6de40-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6de40-121">Header</span></span>|<span data-ttu-id="6de40-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6de40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6de40-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6de40-123">Authorization</span></span>|<span data-ttu-id="6de40-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6de40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6de40-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6de40-125">Accept</span></span>|<span data-ttu-id="6de40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6de40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6de40-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6de40-127">Request body</span></span>
<span data-ttu-id="6de40-128">В тексте запроса укажите представление JSON для объекта androidWorkProfileEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6de40-128">In the request body, supply a JSON representation for the androidWorkProfileEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="6de40-129">В следующей таблице показаны свойства, которые необходимы для создания androidWorkProfileEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6de40-129">The following table shows the properties that are required when you create the androidWorkProfileEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="6de40-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6de40-130">Property</span></span>|<span data-ttu-id="6de40-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6de40-131">Type</span></span>|<span data-ttu-id="6de40-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6de40-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6de40-133">id</span><span class="sxs-lookup"><span data-stu-id="6de40-133">id</span></span>|<span data-ttu-id="6de40-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6de40-134">String</span></span>|<span data-ttu-id="6de40-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6de40-135">Key of the entity.</span></span> <span data-ttu-id="6de40-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6de40-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6de40-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6de40-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6de40-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6de40-138">DateTimeOffset</span></span>|<span data-ttu-id="6de40-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6de40-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6de40-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6de40-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6de40-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6de40-141">roleScopeTagIds</span></span>|<span data-ttu-id="6de40-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6de40-142">String collection</span></span>|<span data-ttu-id="6de40-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6de40-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6de40-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6de40-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6de40-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6de40-145">supportsScopeTags</span></span>|<span data-ttu-id="6de40-146">Логический</span><span class="sxs-lookup"><span data-stu-id="6de40-146">Boolean</span></span>|<span data-ttu-id="6de40-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="6de40-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6de40-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="6de40-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6de40-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6de40-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6de40-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6de40-150">This property is read-only.</span></span> <span data-ttu-id="6de40-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6de40-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6de40-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6de40-152">createdDateTime</span></span>|<span data-ttu-id="6de40-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6de40-153">DateTimeOffset</span></span>|<span data-ttu-id="6de40-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6de40-154">DateTime the object was created.</span></span> <span data-ttu-id="6de40-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6de40-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6de40-156">описание</span><span class="sxs-lookup"><span data-stu-id="6de40-156">description</span></span>|<span data-ttu-id="6de40-157">Строка</span><span class="sxs-lookup"><span data-stu-id="6de40-157">String</span></span>|<span data-ttu-id="6de40-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6de40-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6de40-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6de40-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6de40-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6de40-160">displayName</span></span>|<span data-ttu-id="6de40-161">Строка</span><span class="sxs-lookup"><span data-stu-id="6de40-161">String</span></span>|<span data-ttu-id="6de40-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6de40-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6de40-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6de40-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6de40-164">version</span><span class="sxs-lookup"><span data-stu-id="6de40-164">version</span></span>|<span data-ttu-id="6de40-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6de40-165">Int32</span></span>|<span data-ttu-id="6de40-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6de40-166">Version of the device configuration.</span></span> <span data-ttu-id="6de40-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6de40-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6de40-168">networkName</span><span class="sxs-lookup"><span data-stu-id="6de40-168">networkName</span></span>|<span data-ttu-id="6de40-169">Строка</span><span class="sxs-lookup"><span data-stu-id="6de40-169">String</span></span>|<span data-ttu-id="6de40-170">Сеть имя наследуется от [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6de40-170">Network Name Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="6de40-171">SSID</span><span class="sxs-lookup"><span data-stu-id="6de40-171">ssid</span></span>|<span data-ttu-id="6de40-172">Строка</span><span class="sxs-lookup"><span data-stu-id="6de40-172">String</span></span>|<span data-ttu-id="6de40-173">Это имя в сети Wi-Fi, который передается на все устройства.</span><span class="sxs-lookup"><span data-stu-id="6de40-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="6de40-174">Наследуется от [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6de40-174">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="6de40-175">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="6de40-175">connectAutomatically</span></span>|<span data-ttu-id="6de40-176">Логический</span><span class="sxs-lookup"><span data-stu-id="6de40-176">Boolean</span></span>|<span data-ttu-id="6de40-177">Автоматическое подключение, сети, если она в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="6de40-177">Connect automatically when this network is in range.</span></span> <span data-ttu-id="6de40-178">Установка значения true пропустите строке пользователя и автоматически подключаться к сети Wi-Fi устройства.</span><span class="sxs-lookup"><span data-stu-id="6de40-178">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="6de40-179">Наследуется от [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6de40-179">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="6de40-180">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="6de40-180">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="6de40-181">Логический</span><span class="sxs-lookup"><span data-stu-id="6de40-181">Boolean</span></span>|<span data-ttu-id="6de40-182">Когда установлено значение true, этот профиль принудительно устройства для подключения к сети, в которой не передает свое имя SSID для всех устройств.</span><span class="sxs-lookup"><span data-stu-id="6de40-182">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="6de40-183">Наследуется от [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6de40-183">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="6de40-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="6de40-184">wiFiSecurityType</span></span>|[<span data-ttu-id="6de40-185">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="6de40-185">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="6de40-186">Указывает, используется ли конечная точка Wi-Fi тип безопасности на основе внешних Приложений.</span><span class="sxs-lookup"><span data-stu-id="6de40-186">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="6de40-187">Наследуется от [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6de40-187">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span> <span data-ttu-id="6de40-188">Возможные значения: `open`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="6de40-188">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="6de40-189">eapType</span><span class="sxs-lookup"><span data-stu-id="6de40-189">eapType</span></span>|[<span data-ttu-id="6de40-190">androidEapType</span><span class="sxs-lookup"><span data-stu-id="6de40-190">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="6de40-191">Указывает тип протокола EAP на конечной точке Wi-Fi (маршрутизатор).</span><span class="sxs-lookup"><span data-stu-id="6de40-191">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="6de40-192">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="6de40-192">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="6de40-193">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6de40-193">authenticationMethod</span></span>|[<span data-ttu-id="6de40-194">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6de40-194">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="6de40-195">Указывает метод проверки подлинности клиента (устройств) необходимо использовать при настройке типа EAP PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="6de40-195">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="6de40-196">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="6de40-196">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="6de40-197">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="6de40-197">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="6de40-198">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="6de40-198">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="6de40-199">Метод EAP без проверки подлинности (внутреннее удостоверение) при тип EAP — EAP-TTLS и Authenticationmethod — это имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="6de40-199">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="6de40-200">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="6de40-200">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="6de40-201">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="6de40-201">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="6de40-202">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="6de40-202">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="6de40-203">Метод EAP без проверки подлинности (внутренний идентификатор) при PEAP — это тип EAP и Authenticationmethod — это имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="6de40-203">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="6de40-204">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="6de40-204">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="6de40-205">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="6de40-205">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="6de40-206">Строка</span><span class="sxs-lookup"><span data-stu-id="6de40-206">String</span></span>|<span data-ttu-id="6de40-207">Включите удостоверение конфиденциальности (учетную запись), если тип EAP настроено для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="6de40-207">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="6de40-208">Строка, представленные здесь используется для скрытие имя пользователя для отдельных пользователей, когда пользователь пытается подключиться к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="6de40-208">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="6de40-209">Ответ</span><span class="sxs-lookup"><span data-stu-id="6de40-209">Response</span></span>
<span data-ttu-id="6de40-210">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6de40-210">If successful, this method returns a `201 Created` response code and a [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6de40-211">Пример</span><span class="sxs-lookup"><span data-stu-id="6de40-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="6de40-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="6de40-212">Request</span></span>
<span data-ttu-id="6de40-213">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6de40-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 840

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="6de40-214">Ответ</span><span class="sxs-lookup"><span data-stu-id="6de40-214">Response</span></span>
<span data-ttu-id="6de40-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6de40-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





