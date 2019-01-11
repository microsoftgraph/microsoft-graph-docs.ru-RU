---
title: Обновление windowsWifiConfiguration
description: Обновление свойства объекта windowsWifiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c58ede51940c1d913632668919532ba6d61ad201
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847112"
---
# <a name="update-windowswificonfiguration"></a><span data-ttu-id="d50a2-103">Обновление windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="d50a2-103">Update windowsWifiConfiguration</span></span>

> <span data-ttu-id="d50a2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d50a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d50a2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d50a2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d50a2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d50a2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d50a2-107">Обновление свойства объекта [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d50a2-107">Update the properties of a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d50a2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d50a2-108">Prerequisites</span></span>
<span data-ttu-id="d50a2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d50a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d50a2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d50a2-111">Permission type</span></span>|<span data-ttu-id="d50a2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d50a2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d50a2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d50a2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d50a2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d50a2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d50a2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d50a2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d50a2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d50a2-116">Not supported.</span></span>|
|<span data-ttu-id="d50a2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d50a2-117">Application</span></span>|<span data-ttu-id="d50a2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d50a2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d50a2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d50a2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d50a2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d50a2-120">Request headers</span></span>
|<span data-ttu-id="d50a2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d50a2-121">Header</span></span>|<span data-ttu-id="d50a2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d50a2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d50a2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d50a2-123">Authorization</span></span>|<span data-ttu-id="d50a2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d50a2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d50a2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d50a2-125">Accept</span></span>|<span data-ttu-id="d50a2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d50a2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d50a2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d50a2-127">Request body</span></span>
<span data-ttu-id="d50a2-128">В тексте запроса укажите представление JSON для объекта [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d50a2-128">In the request body, supply a JSON representation for the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

<span data-ttu-id="d50a2-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d50a2-129">The following table shows the properties that are required when you create the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span>

|<span data-ttu-id="d50a2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d50a2-130">Property</span></span>|<span data-ttu-id="d50a2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d50a2-131">Type</span></span>|<span data-ttu-id="d50a2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d50a2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d50a2-133">id</span><span class="sxs-lookup"><span data-stu-id="d50a2-133">id</span></span>|<span data-ttu-id="d50a2-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d50a2-134">String</span></span>|<span data-ttu-id="d50a2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d50a2-135">Key of the entity.</span></span> <span data-ttu-id="d50a2-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d50a2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d50a2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d50a2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d50a2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d50a2-138">DateTimeOffset</span></span>|<span data-ttu-id="d50a2-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d50a2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d50a2-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d50a2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d50a2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d50a2-141">roleScopeTagIds</span></span>|<span data-ttu-id="d50a2-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d50a2-142">String collection</span></span>|<span data-ttu-id="d50a2-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d50a2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d50a2-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d50a2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d50a2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d50a2-145">supportsScopeTags</span></span>|<span data-ttu-id="d50a2-146">Логический</span><span class="sxs-lookup"><span data-stu-id="d50a2-146">Boolean</span></span>|<span data-ttu-id="d50a2-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="d50a2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d50a2-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="d50a2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d50a2-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d50a2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d50a2-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d50a2-150">This property is read-only.</span></span> <span data-ttu-id="d50a2-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d50a2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d50a2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d50a2-152">createdDateTime</span></span>|<span data-ttu-id="d50a2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d50a2-153">DateTimeOffset</span></span>|<span data-ttu-id="d50a2-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d50a2-154">DateTime the object was created.</span></span> <span data-ttu-id="d50a2-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d50a2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d50a2-156">описание</span><span class="sxs-lookup"><span data-stu-id="d50a2-156">description</span></span>|<span data-ttu-id="d50a2-157">Строка</span><span class="sxs-lookup"><span data-stu-id="d50a2-157">String</span></span>|<span data-ttu-id="d50a2-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d50a2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d50a2-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d50a2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d50a2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d50a2-160">displayName</span></span>|<span data-ttu-id="d50a2-161">Строка</span><span class="sxs-lookup"><span data-stu-id="d50a2-161">String</span></span>|<span data-ttu-id="d50a2-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d50a2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d50a2-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d50a2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d50a2-164">version</span><span class="sxs-lookup"><span data-stu-id="d50a2-164">version</span></span>|<span data-ttu-id="d50a2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d50a2-165">Int32</span></span>|<span data-ttu-id="d50a2-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d50a2-166">Version of the device configuration.</span></span> <span data-ttu-id="d50a2-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d50a2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d50a2-168">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="d50a2-168">preSharedKey</span></span>|<span data-ttu-id="d50a2-169">Строка</span><span class="sxs-lookup"><span data-stu-id="d50a2-169">String</span></span>|<span data-ttu-id="d50a2-170">Это предварительный ключ для WPA личных Сеть Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="d50a2-170">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="d50a2-171">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="d50a2-171">wifiSecurityType</span></span>|[<span data-ttu-id="d50a2-172">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="d50a2-172">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="d50a2-173">Укажите тип безопасности Wifi.</span><span class="sxs-lookup"><span data-stu-id="d50a2-173">Specify the Wifi Security Type.</span></span> <span data-ttu-id="d50a2-174">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="d50a2-174">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="d50a2-175">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="d50a2-175">meteredConnectionLimit</span></span>|[<span data-ttu-id="d50a2-176">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="d50a2-176">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="d50a2-177">Задать тип ограничение лимитным тарифным планом подключения для Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="d50a2-177">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="d50a2-178">Возможные значения: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="d50a2-178">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="d50a2-179">SSID</span><span class="sxs-lookup"><span data-stu-id="d50a2-179">ssid</span></span>|<span data-ttu-id="d50a2-180">Строка</span><span class="sxs-lookup"><span data-stu-id="d50a2-180">String</span></span>|<span data-ttu-id="d50a2-181">Укажите SSID Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="d50a2-181">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="d50a2-182">networkName</span><span class="sxs-lookup"><span data-stu-id="d50a2-182">networkName</span></span>|<span data-ttu-id="d50a2-183">Строка</span><span class="sxs-lookup"><span data-stu-id="d50a2-183">String</span></span>|<span data-ttu-id="d50a2-184">Укажите имя конфигурации сети.</span><span class="sxs-lookup"><span data-stu-id="d50a2-184">Specify the network configuration name.</span></span>|
|<span data-ttu-id="d50a2-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="d50a2-185">connectAutomatically</span></span>|<span data-ttu-id="d50a2-186">Логический</span><span class="sxs-lookup"><span data-stu-id="d50a2-186">Boolean</span></span>|<span data-ttu-id="d50a2-187">Укажите, будет ли Wi-Fi следует автоматически подключаться при работе в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="d50a2-187">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="d50a2-188">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="d50a2-188">connectToPreferredNetwork</span></span>|<span data-ttu-id="d50a2-189">Логический</span><span class="sxs-lookup"><span data-stu-id="d50a2-189">Boolean</span></span>|<span data-ttu-id="d50a2-190">Укажите, должны ли Wi-Fi подключаться к более подходящей сети, если уже подключен этой.</span><span class="sxs-lookup"><span data-stu-id="d50a2-190">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="d50a2-191">Требуется ConnectAutomatically значение true.</span><span class="sxs-lookup"><span data-stu-id="d50a2-191">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="d50a2-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="d50a2-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="d50a2-193">Логический</span><span class="sxs-lookup"><span data-stu-id="d50a2-193">Boolean</span></span>|<span data-ttu-id="d50a2-194">Укажите, автоматически подключения Wi-Fi даже когда не передают SSID.</span><span class="sxs-lookup"><span data-stu-id="d50a2-194">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="d50a2-195">proxySetting</span><span class="sxs-lookup"><span data-stu-id="d50a2-195">proxySetting</span></span>|[<span data-ttu-id="d50a2-196">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="d50a2-196">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="d50a2-197">Укажите параметры для Wi-Fi конфигурации прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="d50a2-197">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="d50a2-198">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="d50a2-198">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="d50a2-199">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="d50a2-199">proxyManualAddress</span></span>|<span data-ttu-id="d50a2-200">Строка</span><span class="sxs-lookup"><span data-stu-id="d50a2-200">String</span></span>|<span data-ttu-id="d50a2-201">Укажите IP-адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="d50a2-201">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="d50a2-202">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="d50a2-202">proxyManualPort</span></span>|<span data-ttu-id="d50a2-203">Int32</span><span class="sxs-lookup"><span data-stu-id="d50a2-203">Int32</span></span>|<span data-ttu-id="d50a2-204">Указание порта для прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="d50a2-204">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="d50a2-205">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="d50a2-205">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="d50a2-206">Строка</span><span class="sxs-lookup"><span data-stu-id="d50a2-206">String</span></span>|<span data-ttu-id="d50a2-207">Укажите URL-адрес для сценария настройки сервера прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="d50a2-207">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="d50a2-208">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="d50a2-208">forceFIPSCompliance</span></span>|<span data-ttu-id="d50a2-209">Логический</span><span class="sxs-lookup"><span data-stu-id="d50a2-209">Boolean</span></span>|<span data-ttu-id="d50a2-210">Укажите необходимость проверки соответствия требованиям FIPS.</span><span class="sxs-lookup"><span data-stu-id="d50a2-210">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="d50a2-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="d50a2-211">Response</span></span>
<span data-ttu-id="d50a2-212">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d50a2-212">If successful, this method returns a `200 OK` response code and an updated [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d50a2-213">Пример</span><span class="sxs-lookup"><span data-stu-id="d50a2-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="d50a2-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="d50a2-214">Request</span></span>
<span data-ttu-id="d50a2-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d50a2-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d50a2-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="d50a2-216">Response</span></span>
<span data-ttu-id="d50a2-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d50a2-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





