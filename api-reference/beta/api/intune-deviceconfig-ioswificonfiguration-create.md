---
title: Создание iosWiFiConfiguration
description: Создание нового объекта iosWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f93477c0ee570fec3005fb6290d1fbe9f637dbdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853663"
---
# <a name="create-ioswificonfiguration"></a><span data-ttu-id="a7906-103">Создание iosWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7906-103">Create iosWiFiConfiguration</span></span>

> <span data-ttu-id="a7906-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a7906-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7906-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7906-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7906-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a7906-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7906-107">Создание нового объекта [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a7906-107">Create a new [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a7906-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a7906-108">Prerequisites</span></span>
<span data-ttu-id="a7906-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7906-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7906-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7906-111">Permission type</span></span>|<span data-ttu-id="a7906-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7906-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7906-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7906-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7906-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7906-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7906-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7906-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7906-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7906-116">Not supported.</span></span>|
|<span data-ttu-id="a7906-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7906-117">Application</span></span>|<span data-ttu-id="a7906-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7906-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7906-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7906-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a7906-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7906-120">Request headers</span></span>
|<span data-ttu-id="a7906-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7906-121">Header</span></span>|<span data-ttu-id="a7906-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a7906-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7906-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7906-123">Authorization</span></span>|<span data-ttu-id="a7906-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a7906-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7906-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a7906-125">Accept</span></span>|<span data-ttu-id="a7906-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7906-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7906-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a7906-127">Request body</span></span>
<span data-ttu-id="a7906-128">В тексте запроса укажите представление JSON для объекта iosWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a7906-128">In the request body, supply a JSON representation for the iosWiFiConfiguration object.</span></span>

<span data-ttu-id="a7906-129">В следующей таблице показаны свойства, которые необходимы для создания iosWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a7906-129">The following table shows the properties that are required when you create the iosWiFiConfiguration.</span></span>

|<span data-ttu-id="a7906-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7906-130">Property</span></span>|<span data-ttu-id="a7906-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a7906-131">Type</span></span>|<span data-ttu-id="a7906-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a7906-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7906-133">id</span><span class="sxs-lookup"><span data-stu-id="a7906-133">id</span></span>|<span data-ttu-id="a7906-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a7906-134">String</span></span>|<span data-ttu-id="a7906-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a7906-135">Key of the entity.</span></span> <span data-ttu-id="a7906-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7906-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7906-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7906-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a7906-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7906-138">DateTimeOffset</span></span>|<span data-ttu-id="a7906-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a7906-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a7906-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7906-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7906-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a7906-141">roleScopeTagIds</span></span>|<span data-ttu-id="a7906-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a7906-142">String collection</span></span>|<span data-ttu-id="a7906-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a7906-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a7906-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7906-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7906-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a7906-145">supportsScopeTags</span></span>|<span data-ttu-id="a7906-146">Логический</span><span class="sxs-lookup"><span data-stu-id="a7906-146">Boolean</span></span>|<span data-ttu-id="a7906-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="a7906-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a7906-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="a7906-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a7906-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a7906-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a7906-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a7906-150">This property is read-only.</span></span> <span data-ttu-id="a7906-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7906-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7906-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7906-152">createdDateTime</span></span>|<span data-ttu-id="a7906-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7906-153">DateTimeOffset</span></span>|<span data-ttu-id="a7906-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a7906-154">DateTime the object was created.</span></span> <span data-ttu-id="a7906-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7906-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7906-156">описание</span><span class="sxs-lookup"><span data-stu-id="a7906-156">description</span></span>|<span data-ttu-id="a7906-157">Строка</span><span class="sxs-lookup"><span data-stu-id="a7906-157">String</span></span>|<span data-ttu-id="a7906-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a7906-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a7906-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7906-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7906-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a7906-160">displayName</span></span>|<span data-ttu-id="a7906-161">Строка</span><span class="sxs-lookup"><span data-stu-id="a7906-161">String</span></span>|<span data-ttu-id="a7906-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a7906-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a7906-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7906-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7906-164">version</span><span class="sxs-lookup"><span data-stu-id="a7906-164">version</span></span>|<span data-ttu-id="a7906-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a7906-165">Int32</span></span>|<span data-ttu-id="a7906-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a7906-166">Version of the device configuration.</span></span> <span data-ttu-id="a7906-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7906-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7906-168">networkName</span><span class="sxs-lookup"><span data-stu-id="a7906-168">networkName</span></span>|<span data-ttu-id="a7906-169">Строка</span><span class="sxs-lookup"><span data-stu-id="a7906-169">String</span></span>|<span data-ttu-id="a7906-170">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="a7906-170">Network Name</span></span>|
|<span data-ttu-id="a7906-171">SSID</span><span class="sxs-lookup"><span data-stu-id="a7906-171">ssid</span></span>|<span data-ttu-id="a7906-172">Строка</span><span class="sxs-lookup"><span data-stu-id="a7906-172">String</span></span>|<span data-ttu-id="a7906-173">Это имя в сети Wi-Fi, который передается на все устройства.</span><span class="sxs-lookup"><span data-stu-id="a7906-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="a7906-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="a7906-174">connectAutomatically</span></span>|<span data-ttu-id="a7906-175">Логический</span><span class="sxs-lookup"><span data-stu-id="a7906-175">Boolean</span></span>|<span data-ttu-id="a7906-176">Автоматическое подключение, сети, если она в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="a7906-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="a7906-177">Установка значения true пропустите строке пользователя и автоматически подключаться к сети Wi-Fi устройства.</span><span class="sxs-lookup"><span data-stu-id="a7906-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="a7906-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="a7906-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="a7906-179">Логический</span><span class="sxs-lookup"><span data-stu-id="a7906-179">Boolean</span></span>|<span data-ttu-id="a7906-180">Если для сети не передают свое имя (SSID) подключиться.</span><span class="sxs-lookup"><span data-stu-id="a7906-180">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="a7906-181">Когда установлено значение true, этот профиль принудительно устройства для подключения к сети, в которой не передает свое имя SSID для всех устройств.</span><span class="sxs-lookup"><span data-stu-id="a7906-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="a7906-182">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="a7906-182">wiFiSecurityType</span></span>|[<span data-ttu-id="a7906-183">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="a7906-183">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="a7906-184">Указывает, используется ли конечная точка Wi-Fi тип безопасности на основе внешних Приложений.</span><span class="sxs-lookup"><span data-stu-id="a7906-184">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="a7906-185">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="a7906-185">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="a7906-186">proxySettings</span><span class="sxs-lookup"><span data-stu-id="a7906-186">proxySettings</span></span>|[<span data-ttu-id="a7906-187">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="a7906-187">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="a7906-188">Тип прокси-сервера для этого подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="a7906-188">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="a7906-189">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="a7906-189">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="a7906-190">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="a7906-190">proxyManualAddress</span></span>|<span data-ttu-id="a7906-191">Строка</span><span class="sxs-lookup"><span data-stu-id="a7906-191">String</span></span>|<span data-ttu-id="a7906-192">IP-адрес или DNS-имя узла прокси-сервера при выборе ручной настройки.</span><span class="sxs-lookup"><span data-stu-id="a7906-192">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="a7906-193">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="a7906-193">proxyManualPort</span></span>|<span data-ttu-id="a7906-194">Int32</span><span class="sxs-lookup"><span data-stu-id="a7906-194">Int32</span></span>|<span data-ttu-id="a7906-195">Порт прокси-сервера при выборе ручной настройки.</span><span class="sxs-lookup"><span data-stu-id="a7906-195">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="a7906-196">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="a7906-196">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="a7906-197">Строка</span><span class="sxs-lookup"><span data-stu-id="a7906-197">String</span></span>|<span data-ttu-id="a7906-198">URL-адрес прокси-сервера сценарий автоматической настройки сервера при выборе автоматической настройки.</span><span class="sxs-lookup"><span data-stu-id="a7906-198">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="a7906-199">Этот URL-адрес обычно имеет расположение файла PAC (автоматической конфигурации прокси-сервера).</span><span class="sxs-lookup"><span data-stu-id="a7906-199">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="a7906-200">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="a7906-200">preSharedKey</span></span>|<span data-ttu-id="a7906-201">Строка</span><span class="sxs-lookup"><span data-stu-id="a7906-201">String</span></span>|<span data-ttu-id="a7906-202">Это предварительный ключ для WPA личных Сеть Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="a7906-202">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="a7906-203">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7906-203">Response</span></span>
<span data-ttu-id="a7906-204">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a7906-204">If successful, this method returns a `201 Created` response code and a [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7906-205">Пример</span><span class="sxs-lookup"><span data-stu-id="a7906-205">Example</span></span>
### <a name="request"></a><span data-ttu-id="a7906-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7906-206">Request</span></span>
<span data-ttu-id="a7906-207">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7906-207">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 739

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
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
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="a7906-208">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7906-208">Response</span></span>
<span data-ttu-id="a7906-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a7906-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 847

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
  "id": "516f9ef9-9ef9-516f-f99e-6f51f99e6f51",
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
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value"
}
```





