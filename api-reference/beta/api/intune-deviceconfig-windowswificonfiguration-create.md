---
title: Создание windowsWifiConfiguration
description: Создание нового объекта windowsWifiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1dcb2254c5f73f3e223d2d36d6911ab33f07bb3b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826420"
---
# <a name="create-windowswificonfiguration"></a><span data-ttu-id="464c7-103">Создание windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="464c7-103">Create windowsWifiConfiguration</span></span>

> <span data-ttu-id="464c7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="464c7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="464c7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="464c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="464c7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="464c7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="464c7-107">Создание нового объекта [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="464c7-107">Create a new [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="464c7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="464c7-108">Prerequisites</span></span>
<span data-ttu-id="464c7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="464c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="464c7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="464c7-111">Permission type</span></span>|<span data-ttu-id="464c7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="464c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="464c7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="464c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="464c7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="464c7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="464c7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="464c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="464c7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="464c7-116">Not supported.</span></span>|
|<span data-ttu-id="464c7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="464c7-117">Application</span></span>|<span data-ttu-id="464c7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="464c7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="464c7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="464c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="464c7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="464c7-120">Request headers</span></span>
|<span data-ttu-id="464c7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="464c7-121">Header</span></span>|<span data-ttu-id="464c7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="464c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="464c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="464c7-123">Authorization</span></span>|<span data-ttu-id="464c7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="464c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="464c7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="464c7-125">Accept</span></span>|<span data-ttu-id="464c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="464c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="464c7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="464c7-127">Request body</span></span>
<span data-ttu-id="464c7-128">В тексте запроса укажите представление JSON для объекта windowsWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="464c7-128">In the request body, supply a JSON representation for the windowsWifiConfiguration object.</span></span>

<span data-ttu-id="464c7-129">В следующей таблице показаны свойства, которые необходимы для создания windowsWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="464c7-129">The following table shows the properties that are required when you create the windowsWifiConfiguration.</span></span>

|<span data-ttu-id="464c7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="464c7-130">Property</span></span>|<span data-ttu-id="464c7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="464c7-131">Type</span></span>|<span data-ttu-id="464c7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="464c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="464c7-133">id</span><span class="sxs-lookup"><span data-stu-id="464c7-133">id</span></span>|<span data-ttu-id="464c7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="464c7-134">String</span></span>|<span data-ttu-id="464c7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="464c7-135">Key of the entity.</span></span> <span data-ttu-id="464c7-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="464c7-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="464c7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="464c7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="464c7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="464c7-138">DateTimeOffset</span></span>|<span data-ttu-id="464c7-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="464c7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="464c7-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="464c7-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="464c7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="464c7-141">roleScopeTagIds</span></span>|<span data-ttu-id="464c7-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="464c7-142">String collection</span></span>|<span data-ttu-id="464c7-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="464c7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="464c7-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="464c7-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="464c7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="464c7-145">supportsScopeTags</span></span>|<span data-ttu-id="464c7-146">Логический</span><span class="sxs-lookup"><span data-stu-id="464c7-146">Boolean</span></span>|<span data-ttu-id="464c7-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="464c7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="464c7-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="464c7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="464c7-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="464c7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="464c7-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="464c7-150">This property is read-only.</span></span> <span data-ttu-id="464c7-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="464c7-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="464c7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="464c7-152">createdDateTime</span></span>|<span data-ttu-id="464c7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="464c7-153">DateTimeOffset</span></span>|<span data-ttu-id="464c7-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="464c7-154">DateTime the object was created.</span></span> <span data-ttu-id="464c7-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="464c7-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="464c7-156">описание</span><span class="sxs-lookup"><span data-stu-id="464c7-156">description</span></span>|<span data-ttu-id="464c7-157">Строка</span><span class="sxs-lookup"><span data-stu-id="464c7-157">String</span></span>|<span data-ttu-id="464c7-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="464c7-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="464c7-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="464c7-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="464c7-160">displayName</span><span class="sxs-lookup"><span data-stu-id="464c7-160">displayName</span></span>|<span data-ttu-id="464c7-161">Строка</span><span class="sxs-lookup"><span data-stu-id="464c7-161">String</span></span>|<span data-ttu-id="464c7-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="464c7-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="464c7-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="464c7-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="464c7-164">version</span><span class="sxs-lookup"><span data-stu-id="464c7-164">version</span></span>|<span data-ttu-id="464c7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="464c7-165">Int32</span></span>|<span data-ttu-id="464c7-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="464c7-166">Version of the device configuration.</span></span> <span data-ttu-id="464c7-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="464c7-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="464c7-168">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="464c7-168">preSharedKey</span></span>|<span data-ttu-id="464c7-169">Строка</span><span class="sxs-lookup"><span data-stu-id="464c7-169">String</span></span>|<span data-ttu-id="464c7-170">Это предварительный ключ для WPA личных Сеть Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="464c7-170">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="464c7-171">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="464c7-171">wifiSecurityType</span></span>|[<span data-ttu-id="464c7-172">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="464c7-172">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="464c7-173">Укажите тип безопасности Wifi.</span><span class="sxs-lookup"><span data-stu-id="464c7-173">Specify the Wifi Security Type.</span></span> <span data-ttu-id="464c7-174">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="464c7-174">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="464c7-175">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="464c7-175">meteredConnectionLimit</span></span>|[<span data-ttu-id="464c7-176">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="464c7-176">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="464c7-177">Задать тип ограничение лимитным тарифным планом подключения для Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="464c7-177">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="464c7-178">Возможные значения: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="464c7-178">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="464c7-179">SSID</span><span class="sxs-lookup"><span data-stu-id="464c7-179">ssid</span></span>|<span data-ttu-id="464c7-180">Строка</span><span class="sxs-lookup"><span data-stu-id="464c7-180">String</span></span>|<span data-ttu-id="464c7-181">Укажите SSID Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="464c7-181">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="464c7-182">networkName</span><span class="sxs-lookup"><span data-stu-id="464c7-182">networkName</span></span>|<span data-ttu-id="464c7-183">Строка</span><span class="sxs-lookup"><span data-stu-id="464c7-183">String</span></span>|<span data-ttu-id="464c7-184">Укажите имя конфигурации сети.</span><span class="sxs-lookup"><span data-stu-id="464c7-184">Specify the network configuration name.</span></span>|
|<span data-ttu-id="464c7-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="464c7-185">connectAutomatically</span></span>|<span data-ttu-id="464c7-186">Логический</span><span class="sxs-lookup"><span data-stu-id="464c7-186">Boolean</span></span>|<span data-ttu-id="464c7-187">Укажите, будет ли Wi-Fi следует автоматически подключаться при работе в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="464c7-187">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="464c7-188">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="464c7-188">connectToPreferredNetwork</span></span>|<span data-ttu-id="464c7-189">Логический</span><span class="sxs-lookup"><span data-stu-id="464c7-189">Boolean</span></span>|<span data-ttu-id="464c7-190">Укажите, должны ли Wi-Fi подключаться к более подходящей сети, если уже подключен этой.</span><span class="sxs-lookup"><span data-stu-id="464c7-190">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="464c7-191">Требуется ConnectAutomatically значение true.</span><span class="sxs-lookup"><span data-stu-id="464c7-191">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="464c7-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="464c7-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="464c7-193">Логический</span><span class="sxs-lookup"><span data-stu-id="464c7-193">Boolean</span></span>|<span data-ttu-id="464c7-194">Укажите, автоматически подключения Wi-Fi даже когда не передают SSID.</span><span class="sxs-lookup"><span data-stu-id="464c7-194">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="464c7-195">proxySetting</span><span class="sxs-lookup"><span data-stu-id="464c7-195">proxySetting</span></span>|[<span data-ttu-id="464c7-196">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="464c7-196">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="464c7-197">Укажите параметры для Wi-Fi конфигурации прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="464c7-197">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="464c7-198">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="464c7-198">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="464c7-199">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="464c7-199">proxyManualAddress</span></span>|<span data-ttu-id="464c7-200">Строка</span><span class="sxs-lookup"><span data-stu-id="464c7-200">String</span></span>|<span data-ttu-id="464c7-201">Укажите IP-адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="464c7-201">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="464c7-202">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="464c7-202">proxyManualPort</span></span>|<span data-ttu-id="464c7-203">Int32</span><span class="sxs-lookup"><span data-stu-id="464c7-203">Int32</span></span>|<span data-ttu-id="464c7-204">Указание порта для прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="464c7-204">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="464c7-205">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="464c7-205">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="464c7-206">Строка</span><span class="sxs-lookup"><span data-stu-id="464c7-206">String</span></span>|<span data-ttu-id="464c7-207">Укажите URL-адрес для сценария настройки сервера прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="464c7-207">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="464c7-208">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="464c7-208">forceFIPSCompliance</span></span>|<span data-ttu-id="464c7-209">Логический</span><span class="sxs-lookup"><span data-stu-id="464c7-209">Boolean</span></span>|<span data-ttu-id="464c7-210">Укажите необходимость проверки соответствия требованиям FIPS.</span><span class="sxs-lookup"><span data-stu-id="464c7-210">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="464c7-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="464c7-211">Response</span></span>
<span data-ttu-id="464c7-212">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="464c7-212">If successful, this method returns a `201 Created` response code and a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="464c7-213">Пример</span><span class="sxs-lookup"><span data-stu-id="464c7-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="464c7-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="464c7-214">Request</span></span>
<span data-ttu-id="464c7-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="464c7-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 850

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
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

### <a name="response"></a><span data-ttu-id="464c7-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="464c7-216">Response</span></span>
<span data-ttu-id="464c7-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="464c7-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





