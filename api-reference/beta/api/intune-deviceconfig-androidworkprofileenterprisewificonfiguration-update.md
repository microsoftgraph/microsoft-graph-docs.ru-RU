---
title: Обновление androidWorkProfileEnterpriseWiFiConfiguration
description: Обновление свойства объекта androidWorkProfileEnterpriseWiFiConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 05dd752507a402fb54d27dad40a4264617395b50
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406761"
---
# <a name="update-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="19b27-103">Обновление androidWorkProfileEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="19b27-103">Update androidWorkProfileEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="19b27-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="19b27-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="19b27-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19b27-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19b27-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19b27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19b27-107">Обновление свойства объекта [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="19b27-107">Update the properties of a [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19b27-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="19b27-108">Prerequisites</span></span>
<span data-ttu-id="19b27-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="19b27-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="19b27-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19b27-111">Permission type</span></span>|<span data-ttu-id="19b27-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19b27-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19b27-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19b27-113">Delegated (work or school account)</span></span>|<span data-ttu-id="19b27-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19b27-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="19b27-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19b27-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19b27-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19b27-116">Not supported.</span></span>|
|<span data-ttu-id="19b27-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19b27-117">Application</span></span>|<span data-ttu-id="19b27-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19b27-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19b27-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19b27-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="19b27-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19b27-120">Request headers</span></span>
|<span data-ttu-id="19b27-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19b27-121">Header</span></span>|<span data-ttu-id="19b27-122">Значение</span><span class="sxs-lookup"><span data-stu-id="19b27-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19b27-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19b27-123">Authorization</span></span>|<span data-ttu-id="19b27-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="19b27-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19b27-125">Accept</span><span class="sxs-lookup"><span data-stu-id="19b27-125">Accept</span></span>|<span data-ttu-id="19b27-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19b27-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19b27-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19b27-127">Request body</span></span>
<span data-ttu-id="19b27-128">В тексте запроса укажите представление JSON для объекта [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="19b27-128">In the request body, supply a JSON representation for the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="19b27-129">В следующей таблице показаны свойства, которые необходимы для создания [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19b27-129">The following table shows the properties that are required when you create the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="19b27-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="19b27-130">Property</span></span>|<span data-ttu-id="19b27-131">Тип</span><span class="sxs-lookup"><span data-stu-id="19b27-131">Type</span></span>|<span data-ttu-id="19b27-132">Описание</span><span class="sxs-lookup"><span data-stu-id="19b27-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19b27-133">id</span><span class="sxs-lookup"><span data-stu-id="19b27-133">id</span></span>|<span data-ttu-id="19b27-134">String</span><span class="sxs-lookup"><span data-stu-id="19b27-134">String</span></span>|<span data-ttu-id="19b27-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="19b27-135">Key of the entity.</span></span> <span data-ttu-id="19b27-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19b27-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19b27-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19b27-137">lastModifiedDateTime</span></span>|<span data-ttu-id="19b27-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19b27-138">DateTimeOffset</span></span>|<span data-ttu-id="19b27-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="19b27-139">DateTime the object was last modified.</span></span> <span data-ttu-id="19b27-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19b27-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19b27-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="19b27-141">roleScopeTagIds</span></span>|<span data-ttu-id="19b27-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="19b27-142">String collection</span></span>|<span data-ttu-id="19b27-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="19b27-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="19b27-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19b27-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19b27-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="19b27-145">supportsScopeTags</span></span>|<span data-ttu-id="19b27-146">Логический</span><span class="sxs-lookup"><span data-stu-id="19b27-146">Boolean</span></span>|<span data-ttu-id="19b27-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="19b27-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="19b27-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="19b27-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="19b27-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="19b27-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="19b27-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19b27-150">This property is read-only.</span></span> <span data-ttu-id="19b27-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19b27-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19b27-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19b27-152">createdDateTime</span></span>|<span data-ttu-id="19b27-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19b27-153">DateTimeOffset</span></span>|<span data-ttu-id="19b27-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="19b27-154">DateTime the object was created.</span></span> <span data-ttu-id="19b27-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19b27-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19b27-156">description</span><span class="sxs-lookup"><span data-stu-id="19b27-156">description</span></span>|<span data-ttu-id="19b27-157">String</span><span class="sxs-lookup"><span data-stu-id="19b27-157">String</span></span>|<span data-ttu-id="19b27-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="19b27-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="19b27-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19b27-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19b27-160">displayName</span><span class="sxs-lookup"><span data-stu-id="19b27-160">displayName</span></span>|<span data-ttu-id="19b27-161">String</span><span class="sxs-lookup"><span data-stu-id="19b27-161">String</span></span>|<span data-ttu-id="19b27-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="19b27-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="19b27-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19b27-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19b27-164">version</span><span class="sxs-lookup"><span data-stu-id="19b27-164">version</span></span>|<span data-ttu-id="19b27-165">Int32</span><span class="sxs-lookup"><span data-stu-id="19b27-165">Int32</span></span>|<span data-ttu-id="19b27-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="19b27-166">Version of the device configuration.</span></span> <span data-ttu-id="19b27-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19b27-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19b27-168">networkName</span><span class="sxs-lookup"><span data-stu-id="19b27-168">networkName</span></span>|<span data-ttu-id="19b27-169">String</span><span class="sxs-lookup"><span data-stu-id="19b27-169">String</span></span>|<span data-ttu-id="19b27-170">Сеть имя наследуется от [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19b27-170">Network Name Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="19b27-171">SSID</span><span class="sxs-lookup"><span data-stu-id="19b27-171">ssid</span></span>|<span data-ttu-id="19b27-172">String</span><span class="sxs-lookup"><span data-stu-id="19b27-172">String</span></span>|<span data-ttu-id="19b27-173">Это имя в сети Wi-Fi, который передается на все устройства.</span><span class="sxs-lookup"><span data-stu-id="19b27-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="19b27-174">Наследуется от [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19b27-174">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="19b27-175">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="19b27-175">connectAutomatically</span></span>|<span data-ttu-id="19b27-176">Логический</span><span class="sxs-lookup"><span data-stu-id="19b27-176">Boolean</span></span>|<span data-ttu-id="19b27-177">Автоматическое подключение, сети, если она в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="19b27-177">Connect automatically when this network is in range.</span></span> <span data-ttu-id="19b27-178">Установка значения true пропустите строке пользователя и автоматически подключаться к сети Wi-Fi устройства.</span><span class="sxs-lookup"><span data-stu-id="19b27-178">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="19b27-179">Наследуется от [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19b27-179">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="19b27-180">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="19b27-180">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="19b27-181">Логический</span><span class="sxs-lookup"><span data-stu-id="19b27-181">Boolean</span></span>|<span data-ttu-id="19b27-182">Когда установлено значение true, этот профиль принудительно устройства для подключения к сети, в которой не передает свое имя SSID для всех устройств.</span><span class="sxs-lookup"><span data-stu-id="19b27-182">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="19b27-183">Наследуется от [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19b27-183">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="19b27-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="19b27-184">wiFiSecurityType</span></span>|[<span data-ttu-id="19b27-185">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="19b27-185">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="19b27-186">Указывает, используется ли конечная точка Wi-Fi тип безопасности на основе внешних Приложений.</span><span class="sxs-lookup"><span data-stu-id="19b27-186">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="19b27-187">Наследуется от [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19b27-187">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span> <span data-ttu-id="19b27-188">Возможные значения: `open`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="19b27-188">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="19b27-189">eapType</span><span class="sxs-lookup"><span data-stu-id="19b27-189">eapType</span></span>|[<span data-ttu-id="19b27-190">androidEapType</span><span class="sxs-lookup"><span data-stu-id="19b27-190">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="19b27-191">Указывает тип протокола EAP на конечной точке Wi-Fi (маршрутизатор).</span><span class="sxs-lookup"><span data-stu-id="19b27-191">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="19b27-192">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="19b27-192">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="19b27-193">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="19b27-193">authenticationMethod</span></span>|[<span data-ttu-id="19b27-194">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="19b27-194">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="19b27-195">Указывает метод проверки подлинности клиента (устройств) необходимо использовать при настройке типа EAP PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="19b27-195">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="19b27-196">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="19b27-196">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="19b27-197">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="19b27-197">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="19b27-198">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="19b27-198">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="19b27-199">Метод EAP без проверки подлинности (внутреннее удостоверение) при тип EAP — EAP-TTLS и Authenticationmethod — это имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="19b27-199">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="19b27-200">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="19b27-200">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="19b27-201">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="19b27-201">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="19b27-202">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="19b27-202">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="19b27-203">Метод EAP без проверки подлинности (внутренний идентификатор) при PEAP — это тип EAP и Authenticationmethod — это имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="19b27-203">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="19b27-204">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="19b27-204">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="19b27-205">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="19b27-205">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="19b27-206">String</span><span class="sxs-lookup"><span data-stu-id="19b27-206">String</span></span>|<span data-ttu-id="19b27-207">Включите удостоверение конфиденциальности (учетную запись), если тип EAP настроено для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="19b27-207">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="19b27-208">Строка, представленные здесь используется для скрытие имя пользователя для отдельных пользователей, когда пользователь пытается подключиться к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="19b27-208">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="19b27-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="19b27-209">Response</span></span>
<span data-ttu-id="19b27-210">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="19b27-210">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19b27-211">Пример</span><span class="sxs-lookup"><span data-stu-id="19b27-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="19b27-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="19b27-212">Request</span></span>
<span data-ttu-id="19b27-213">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19b27-213">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="19b27-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="19b27-214">Response</span></span>
<span data-ttu-id="19b27-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="19b27-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




