---
title: Обновление windowsWifiConfiguration
description: Обновление свойства объекта windowsWifiConfiguration.
author: tfitzmac
ms.openlocfilehash: 0cd1d8ba372daf63561bf94763994fedafb24f46
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310285"
---
# <a name="update-windowswificonfiguration"></a><span data-ttu-id="fe723-103">Обновление windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="fe723-103">Update windowsWifiConfiguration</span></span>

> <span data-ttu-id="fe723-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fe723-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe723-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe723-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe723-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fe723-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe723-107">Обновление свойства объекта [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fe723-107">Update the properties of a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe723-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fe723-108">Prerequisites</span></span>
<span data-ttu-id="fe723-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe723-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe723-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe723-111">Permission type</span></span>|<span data-ttu-id="fe723-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe723-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe723-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe723-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe723-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe723-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe723-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe723-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe723-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe723-116">Not supported.</span></span>|
|<span data-ttu-id="fe723-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe723-117">Application</span></span>|<span data-ttu-id="fe723-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe723-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe723-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe723-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fe723-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe723-120">Request headers</span></span>
|<span data-ttu-id="fe723-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe723-121">Header</span></span>|<span data-ttu-id="fe723-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fe723-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe723-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe723-123">Authorization</span></span>|<span data-ttu-id="fe723-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fe723-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe723-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fe723-125">Accept</span></span>|<span data-ttu-id="fe723-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe723-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe723-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe723-127">Request body</span></span>
<span data-ttu-id="fe723-128">В тексте запроса укажите представление JSON для объекта [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fe723-128">In the request body, supply a JSON representation for the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

<span data-ttu-id="fe723-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe723-129">The following table shows the properties that are required when you create the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span>

|<span data-ttu-id="fe723-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe723-130">Property</span></span>|<span data-ttu-id="fe723-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fe723-131">Type</span></span>|<span data-ttu-id="fe723-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fe723-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe723-133">id</span><span class="sxs-lookup"><span data-stu-id="fe723-133">id</span></span>|<span data-ttu-id="fe723-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fe723-134">String</span></span>|<span data-ttu-id="fe723-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fe723-135">Key of the entity.</span></span> <span data-ttu-id="fe723-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe723-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe723-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe723-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fe723-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe723-138">DateTimeOffset</span></span>|<span data-ttu-id="fe723-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fe723-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fe723-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe723-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe723-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fe723-141">roleScopeTagIds</span></span>|<span data-ttu-id="fe723-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fe723-142">String collection</span></span>|<span data-ttu-id="fe723-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fe723-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fe723-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe723-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe723-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fe723-145">supportsScopeTags</span></span>|<span data-ttu-id="fe723-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="fe723-146">Boolean</span></span>|<span data-ttu-id="fe723-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="fe723-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fe723-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="fe723-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fe723-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fe723-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fe723-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe723-150">This property is read-only.</span></span> <span data-ttu-id="fe723-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe723-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe723-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe723-152">createdDateTime</span></span>|<span data-ttu-id="fe723-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe723-153">DateTimeOffset</span></span>|<span data-ttu-id="fe723-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fe723-154">DateTime the object was created.</span></span> <span data-ttu-id="fe723-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe723-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe723-156">описание</span><span class="sxs-lookup"><span data-stu-id="fe723-156">description</span></span>|<span data-ttu-id="fe723-157">Строка</span><span class="sxs-lookup"><span data-stu-id="fe723-157">String</span></span>|<span data-ttu-id="fe723-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fe723-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fe723-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe723-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe723-160">displayName</span><span class="sxs-lookup"><span data-stu-id="fe723-160">displayName</span></span>|<span data-ttu-id="fe723-161">Строка</span><span class="sxs-lookup"><span data-stu-id="fe723-161">String</span></span>|<span data-ttu-id="fe723-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fe723-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fe723-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe723-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe723-164">version</span><span class="sxs-lookup"><span data-stu-id="fe723-164">version</span></span>|<span data-ttu-id="fe723-165">Int32</span><span class="sxs-lookup"><span data-stu-id="fe723-165">Int32</span></span>|<span data-ttu-id="fe723-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fe723-166">Version of the device configuration.</span></span> <span data-ttu-id="fe723-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe723-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe723-168">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="fe723-168">preSharedKey</span></span>|<span data-ttu-id="fe723-169">String.</span><span class="sxs-lookup"><span data-stu-id="fe723-169">String</span></span>|<span data-ttu-id="fe723-170">Это предварительный ключ для WPA личных Сеть Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="fe723-170">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="fe723-171">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="fe723-171">wifiSecurityType</span></span>|[<span data-ttu-id="fe723-172">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="fe723-172">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="fe723-173">Укажите тип безопасности Wifi.</span><span class="sxs-lookup"><span data-stu-id="fe723-173">Specify the Wifi Security Type.</span></span> <span data-ttu-id="fe723-174">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="fe723-174">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="fe723-175">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="fe723-175">meteredConnectionLimit</span></span>|[<span data-ttu-id="fe723-176">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="fe723-176">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="fe723-177">Задать тип ограничение лимитным тарифным планом подключения для Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="fe723-177">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="fe723-178">Возможные значения: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="fe723-178">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="fe723-179">SSID</span><span class="sxs-lookup"><span data-stu-id="fe723-179">ssid</span></span>|<span data-ttu-id="fe723-180">String.</span><span class="sxs-lookup"><span data-stu-id="fe723-180">String</span></span>|<span data-ttu-id="fe723-181">Укажите SSID Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="fe723-181">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="fe723-182">networkName</span><span class="sxs-lookup"><span data-stu-id="fe723-182">networkName</span></span>|<span data-ttu-id="fe723-183">String.</span><span class="sxs-lookup"><span data-stu-id="fe723-183">String</span></span>|<span data-ttu-id="fe723-184">Укажите имя конфигурации сети.</span><span class="sxs-lookup"><span data-stu-id="fe723-184">Specify the network configuration name.</span></span>|
|<span data-ttu-id="fe723-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="fe723-185">connectAutomatically</span></span>|<span data-ttu-id="fe723-186">Boolean.</span><span class="sxs-lookup"><span data-stu-id="fe723-186">Boolean</span></span>|<span data-ttu-id="fe723-187">Укажите, будет ли Wi-Fi следует автоматически подключаться при работе в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="fe723-187">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="fe723-188">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="fe723-188">connectToPreferredNetwork</span></span>|<span data-ttu-id="fe723-189">Boolean.</span><span class="sxs-lookup"><span data-stu-id="fe723-189">Boolean</span></span>|<span data-ttu-id="fe723-190">Укажите, должны ли Wi-Fi подключаться к более подходящей сети, если уже подключен этой.</span><span class="sxs-lookup"><span data-stu-id="fe723-190">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="fe723-191">Требуется ConnectAutomatically значение true.</span><span class="sxs-lookup"><span data-stu-id="fe723-191">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="fe723-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="fe723-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="fe723-193">Boolean.</span><span class="sxs-lookup"><span data-stu-id="fe723-193">Boolean</span></span>|<span data-ttu-id="fe723-194">Укажите, автоматически подключения Wi-Fi даже когда не передают SSID.</span><span class="sxs-lookup"><span data-stu-id="fe723-194">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="fe723-195">proxySetting</span><span class="sxs-lookup"><span data-stu-id="fe723-195">proxySetting</span></span>|[<span data-ttu-id="fe723-196">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="fe723-196">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="fe723-197">Укажите параметры для Wi-Fi конфигурации прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="fe723-197">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="fe723-198">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="fe723-198">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="fe723-199">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="fe723-199">proxyManualAddress</span></span>|<span data-ttu-id="fe723-200">String.</span><span class="sxs-lookup"><span data-stu-id="fe723-200">String</span></span>|<span data-ttu-id="fe723-201">Укажите IP-адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="fe723-201">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="fe723-202">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="fe723-202">proxyManualPort</span></span>|<span data-ttu-id="fe723-203">Int32</span><span class="sxs-lookup"><span data-stu-id="fe723-203">Int32</span></span>|<span data-ttu-id="fe723-204">Указание порта для прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="fe723-204">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="fe723-205">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="fe723-205">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="fe723-206">String.</span><span class="sxs-lookup"><span data-stu-id="fe723-206">String</span></span>|<span data-ttu-id="fe723-207">Укажите URL-адрес для сценария настройки сервера прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="fe723-207">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="fe723-208">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="fe723-208">forceFIPSCompliance</span></span>|<span data-ttu-id="fe723-209">Boolean.</span><span class="sxs-lookup"><span data-stu-id="fe723-209">Boolean</span></span>|<span data-ttu-id="fe723-210">Укажите необходимость проверки соответствия требованиям FIPS.</span><span class="sxs-lookup"><span data-stu-id="fe723-210">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="fe723-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe723-211">Response</span></span>
<span data-ttu-id="fe723-212">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fe723-212">If successful, this method returns a `200 OK` response code and an updated [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe723-213">Пример</span><span class="sxs-lookup"><span data-stu-id="fe723-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe723-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe723-214">Request</span></span>
<span data-ttu-id="fe723-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe723-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 787

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true
}
```

### <a name="response"></a><span data-ttu-id="fe723-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe723-216">Response</span></span>
<span data-ttu-id="fe723-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fe723-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 958

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
  "id": "8a9e790f-790f-8a9e-0f79-9e8a0f799e8a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true
}
```





