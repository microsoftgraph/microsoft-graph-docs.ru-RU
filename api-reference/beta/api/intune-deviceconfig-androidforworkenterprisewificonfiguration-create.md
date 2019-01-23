---
title: Создание androidForWorkEnterpriseWiFiConfiguration
description: Создание нового объекта androidForWorkEnterpriseWiFiConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8eac56d5ae95b9d1ae991241cd762ebfa763fb0a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414902"
---
# <a name="create-androidforworkenterprisewificonfiguration"></a><span data-ttu-id="c2857-103">Создание androidForWorkEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="c2857-103">Create androidForWorkEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="c2857-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c2857-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c2857-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2857-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2857-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2857-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2857-107">Создание нового объекта [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c2857-107">Create a new [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2857-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="c2857-108">Prerequisites</span></span>
<span data-ttu-id="c2857-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c2857-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c2857-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2857-111">Permission type</span></span>|<span data-ttu-id="c2857-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2857-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2857-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2857-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2857-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2857-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c2857-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2857-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2857-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2857-116">Not supported.</span></span>|
|<span data-ttu-id="c2857-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2857-117">Application</span></span>|<span data-ttu-id="c2857-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2857-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2857-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2857-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c2857-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2857-120">Request headers</span></span>
|<span data-ttu-id="c2857-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2857-121">Header</span></span>|<span data-ttu-id="c2857-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c2857-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2857-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2857-123">Authorization</span></span>|<span data-ttu-id="c2857-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c2857-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2857-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c2857-125">Accept</span></span>|<span data-ttu-id="c2857-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2857-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2857-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2857-127">Request body</span></span>
<span data-ttu-id="c2857-128">В тексте запроса укажите представление JSON для объекта androidForWorkEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c2857-128">In the request body, supply a JSON representation for the androidForWorkEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="c2857-129">В следующей таблице показаны свойства, которые необходимы для создания androidForWorkEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c2857-129">The following table shows the properties that are required when you create the androidForWorkEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="c2857-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2857-130">Property</span></span>|<span data-ttu-id="c2857-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c2857-131">Type</span></span>|<span data-ttu-id="c2857-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c2857-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2857-133">id</span><span class="sxs-lookup"><span data-stu-id="c2857-133">id</span></span>|<span data-ttu-id="c2857-134">String</span><span class="sxs-lookup"><span data-stu-id="c2857-134">String</span></span>|<span data-ttu-id="c2857-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c2857-135">Key of the entity.</span></span> <span data-ttu-id="c2857-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2857-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2857-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2857-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c2857-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2857-138">DateTimeOffset</span></span>|<span data-ttu-id="c2857-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c2857-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c2857-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2857-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2857-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c2857-141">roleScopeTagIds</span></span>|<span data-ttu-id="c2857-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c2857-142">String collection</span></span>|<span data-ttu-id="c2857-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c2857-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c2857-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2857-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2857-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c2857-145">supportsScopeTags</span></span>|<span data-ttu-id="c2857-146">Логический</span><span class="sxs-lookup"><span data-stu-id="c2857-146">Boolean</span></span>|<span data-ttu-id="c2857-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="c2857-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c2857-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="c2857-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c2857-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c2857-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c2857-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2857-150">This property is read-only.</span></span> <span data-ttu-id="c2857-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2857-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2857-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c2857-152">createdDateTime</span></span>|<span data-ttu-id="c2857-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2857-153">DateTimeOffset</span></span>|<span data-ttu-id="c2857-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c2857-154">DateTime the object was created.</span></span> <span data-ttu-id="c2857-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2857-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2857-156">description</span><span class="sxs-lookup"><span data-stu-id="c2857-156">description</span></span>|<span data-ttu-id="c2857-157">String</span><span class="sxs-lookup"><span data-stu-id="c2857-157">String</span></span>|<span data-ttu-id="c2857-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c2857-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c2857-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2857-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2857-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c2857-160">displayName</span></span>|<span data-ttu-id="c2857-161">String</span><span class="sxs-lookup"><span data-stu-id="c2857-161">String</span></span>|<span data-ttu-id="c2857-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c2857-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c2857-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2857-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2857-164">version</span><span class="sxs-lookup"><span data-stu-id="c2857-164">version</span></span>|<span data-ttu-id="c2857-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c2857-165">Int32</span></span>|<span data-ttu-id="c2857-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c2857-166">Version of the device configuration.</span></span> <span data-ttu-id="c2857-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2857-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2857-168">networkName</span><span class="sxs-lookup"><span data-stu-id="c2857-168">networkName</span></span>|<span data-ttu-id="c2857-169">String</span><span class="sxs-lookup"><span data-stu-id="c2857-169">String</span></span>|<span data-ttu-id="c2857-170">Сеть имя наследуется от [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2857-170">Network Name Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="c2857-171">SSID</span><span class="sxs-lookup"><span data-stu-id="c2857-171">ssid</span></span>|<span data-ttu-id="c2857-172">String</span><span class="sxs-lookup"><span data-stu-id="c2857-172">String</span></span>|<span data-ttu-id="c2857-173">Это имя в сети Wi-Fi, который передается на все устройства.</span><span class="sxs-lookup"><span data-stu-id="c2857-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="c2857-174">Наследуется от [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2857-174">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="c2857-175">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="c2857-175">connectAutomatically</span></span>|<span data-ttu-id="c2857-176">Логический</span><span class="sxs-lookup"><span data-stu-id="c2857-176">Boolean</span></span>|<span data-ttu-id="c2857-177">Автоматическое подключение, сети, если она в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="c2857-177">Connect automatically when this network is in range.</span></span> <span data-ttu-id="c2857-178">Установка значения true пропустите строке пользователя и автоматически подключаться к сети Wi-Fi устройства.</span><span class="sxs-lookup"><span data-stu-id="c2857-178">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="c2857-179">Наследуется от [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2857-179">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="c2857-180">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="c2857-180">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="c2857-181">Логический</span><span class="sxs-lookup"><span data-stu-id="c2857-181">Boolean</span></span>|<span data-ttu-id="c2857-182">Когда установлено значение true, этот профиль принудительно устройства для подключения к сети, в которой не передает свое имя SSID для всех устройств.</span><span class="sxs-lookup"><span data-stu-id="c2857-182">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="c2857-183">Наследуется от [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2857-183">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="c2857-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="c2857-184">wiFiSecurityType</span></span>|[<span data-ttu-id="c2857-185">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="c2857-185">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="c2857-186">Указывает, используется ли конечная точка Wi-Fi тип безопасности на основе внешних Приложений.</span><span class="sxs-lookup"><span data-stu-id="c2857-186">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="c2857-187">Наследуется от [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2857-187">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span> <span data-ttu-id="c2857-188">Возможные значения: `open`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="c2857-188">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="c2857-189">eapType</span><span class="sxs-lookup"><span data-stu-id="c2857-189">eapType</span></span>|[<span data-ttu-id="c2857-190">androidEapType</span><span class="sxs-lookup"><span data-stu-id="c2857-190">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="c2857-191">Указывает тип протокола EAP на конечной точке Wi-Fi (маршрутизатор).</span><span class="sxs-lookup"><span data-stu-id="c2857-191">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="c2857-192">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="c2857-192">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="c2857-193">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c2857-193">authenticationMethod</span></span>|[<span data-ttu-id="c2857-194">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c2857-194">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="c2857-195">Указывает метод проверки подлинности клиента (устройств) необходимо использовать при настройке типа EAP PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="c2857-195">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="c2857-196">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="c2857-196">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="c2857-197">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="c2857-197">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="c2857-198">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="c2857-198">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="c2857-199">Метод EAP без проверки подлинности (внутреннее удостоверение) при тип EAP — EAP-TTLS и Authenticationmethod — это имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="c2857-199">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="c2857-200">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="c2857-200">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="c2857-201">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="c2857-201">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="c2857-202">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="c2857-202">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="c2857-203">Метод EAP без проверки подлинности (внутренний идентификатор) при PEAP — это тип EAP и Authenticationmethod — это имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="c2857-203">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="c2857-204">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="c2857-204">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="c2857-205">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="c2857-205">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="c2857-206">String</span><span class="sxs-lookup"><span data-stu-id="c2857-206">String</span></span>|<span data-ttu-id="c2857-207">Включите удостоверение конфиденциальности (учетную запись), если тип EAP настроено для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="c2857-207">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="c2857-208">Строка, представленные здесь используется для скрытие имя пользователя для отдельных пользователей, когда пользователь пытается подключиться к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="c2857-208">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="c2857-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2857-209">Response</span></span>
<span data-ttu-id="c2857-210">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c2857-210">If successful, this method returns a `201 Created` response code and a [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2857-211">Пример</span><span class="sxs-lookup"><span data-stu-id="c2857-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2857-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2857-212">Request</span></span>
<span data-ttu-id="c2857-213">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2857-213">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c2857-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2857-214">Response</span></span>
<span data-ttu-id="c2857-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c2857-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




