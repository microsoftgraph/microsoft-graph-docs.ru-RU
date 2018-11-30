---
title: Создание macOSWiFiConfiguration
description: Создание нового объекта macOSWiFiConfiguration.
ms.openlocfilehash: c0974fa16e89b514332303c1779663c5b7795619
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082482"
---
# <a name="create-macoswificonfiguration"></a><span data-ttu-id="810cc-103">Создание macOSWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="810cc-103">Create macOSWiFiConfiguration</span></span>

> <span data-ttu-id="810cc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="810cc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="810cc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="810cc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="810cc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="810cc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="810cc-107">Создание нового объекта [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="810cc-107">Create a new [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="810cc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="810cc-108">Prerequisites</span></span>
<span data-ttu-id="810cc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="810cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="810cc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="810cc-111">Permission type</span></span>|<span data-ttu-id="810cc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="810cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="810cc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="810cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="810cc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="810cc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="810cc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="810cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="810cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="810cc-116">Not supported.</span></span>|
|<span data-ttu-id="810cc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="810cc-117">Application</span></span>|<span data-ttu-id="810cc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="810cc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="810cc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="810cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="810cc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="810cc-120">Request headers</span></span>
|<span data-ttu-id="810cc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="810cc-121">Header</span></span>|<span data-ttu-id="810cc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="810cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="810cc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="810cc-123">Authorization</span></span>|<span data-ttu-id="810cc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="810cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="810cc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="810cc-125">Accept</span></span>|<span data-ttu-id="810cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="810cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="810cc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="810cc-127">Request body</span></span>
<span data-ttu-id="810cc-128">В тексте запроса укажите представление JSON для объекта macOSWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="810cc-128">In the request body, supply a JSON representation for the macOSWiFiConfiguration object.</span></span>

<span data-ttu-id="810cc-129">В следующей таблице показаны свойства, которые необходимы для создания macOSWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="810cc-129">The following table shows the properties that are required when you create the macOSWiFiConfiguration.</span></span>

|<span data-ttu-id="810cc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="810cc-130">Property</span></span>|<span data-ttu-id="810cc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="810cc-131">Type</span></span>|<span data-ttu-id="810cc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="810cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="810cc-133">id</span><span class="sxs-lookup"><span data-stu-id="810cc-133">id</span></span>|<span data-ttu-id="810cc-134">String</span><span class="sxs-lookup"><span data-stu-id="810cc-134">String</span></span>|<span data-ttu-id="810cc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="810cc-135">Key of the entity.</span></span> <span data-ttu-id="810cc-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="810cc-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="810cc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="810cc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="810cc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="810cc-138">DateTimeOffset</span></span>|<span data-ttu-id="810cc-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="810cc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="810cc-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="810cc-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="810cc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="810cc-141">roleScopeTagIds</span></span>|<span data-ttu-id="810cc-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="810cc-142">String collection</span></span>|<span data-ttu-id="810cc-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="810cc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="810cc-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="810cc-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="810cc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="810cc-145">supportsScopeTags</span></span>|<span data-ttu-id="810cc-146">Логический</span><span class="sxs-lookup"><span data-stu-id="810cc-146">Boolean</span></span>|<span data-ttu-id="810cc-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="810cc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="810cc-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="810cc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="810cc-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="810cc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="810cc-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="810cc-150">This property is read-only.</span></span> <span data-ttu-id="810cc-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="810cc-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="810cc-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="810cc-152">createdDateTime</span></span>|<span data-ttu-id="810cc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="810cc-153">DateTimeOffset</span></span>|<span data-ttu-id="810cc-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="810cc-154">DateTime the object was created.</span></span> <span data-ttu-id="810cc-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="810cc-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="810cc-156">описание</span><span class="sxs-lookup"><span data-stu-id="810cc-156">description</span></span>|<span data-ttu-id="810cc-157">String</span><span class="sxs-lookup"><span data-stu-id="810cc-157">String</span></span>|<span data-ttu-id="810cc-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="810cc-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="810cc-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="810cc-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="810cc-160">displayName</span><span class="sxs-lookup"><span data-stu-id="810cc-160">displayName</span></span>|<span data-ttu-id="810cc-161">String</span><span class="sxs-lookup"><span data-stu-id="810cc-161">String</span></span>|<span data-ttu-id="810cc-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="810cc-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="810cc-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="810cc-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="810cc-164">version</span><span class="sxs-lookup"><span data-stu-id="810cc-164">version</span></span>|<span data-ttu-id="810cc-165">Int32</span><span class="sxs-lookup"><span data-stu-id="810cc-165">Int32</span></span>|<span data-ttu-id="810cc-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="810cc-166">Version of the device configuration.</span></span> <span data-ttu-id="810cc-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="810cc-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="810cc-168">networkName</span><span class="sxs-lookup"><span data-stu-id="810cc-168">networkName</span></span>|<span data-ttu-id="810cc-169">String</span><span class="sxs-lookup"><span data-stu-id="810cc-169">String</span></span>|<span data-ttu-id="810cc-170">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="810cc-170">Network Name</span></span>|
|<span data-ttu-id="810cc-171">SSID</span><span class="sxs-lookup"><span data-stu-id="810cc-171">ssid</span></span>|<span data-ttu-id="810cc-172">String</span><span class="sxs-lookup"><span data-stu-id="810cc-172">String</span></span>|<span data-ttu-id="810cc-173">Это имя в сети Wi-Fi, который передается на все устройства.</span><span class="sxs-lookup"><span data-stu-id="810cc-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="810cc-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="810cc-174">connectAutomatically</span></span>|<span data-ttu-id="810cc-175">Логический</span><span class="sxs-lookup"><span data-stu-id="810cc-175">Boolean</span></span>|<span data-ttu-id="810cc-176">Автоматическое подключение, сети, если она в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="810cc-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="810cc-177">Установка значения true пропустите строке пользователя и автоматически подключаться к сети Wi-Fi устройства.</span><span class="sxs-lookup"><span data-stu-id="810cc-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="810cc-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="810cc-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="810cc-179">Логический</span><span class="sxs-lookup"><span data-stu-id="810cc-179">Boolean</span></span>|<span data-ttu-id="810cc-180">Если для сети не передают свое имя (SSID) подключиться.</span><span class="sxs-lookup"><span data-stu-id="810cc-180">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="810cc-181">Когда установлено значение true, этот профиль принудительно устройства для подключения к сети, в которой не передает свое имя SSID для всех устройств.</span><span class="sxs-lookup"><span data-stu-id="810cc-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="810cc-182">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="810cc-182">wiFiSecurityType</span></span>|[<span data-ttu-id="810cc-183">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="810cc-183">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="810cc-184">Указывает, используется ли конечная точка Wi-Fi тип безопасности на основе внешних Приложений.</span><span class="sxs-lookup"><span data-stu-id="810cc-184">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="810cc-185">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="810cc-185">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="810cc-186">proxySettings</span><span class="sxs-lookup"><span data-stu-id="810cc-186">proxySettings</span></span>|[<span data-ttu-id="810cc-187">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="810cc-187">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="810cc-188">Тип прокси-сервера для этого подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="810cc-188">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="810cc-189">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="810cc-189">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="810cc-190">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="810cc-190">proxyManualAddress</span></span>|<span data-ttu-id="810cc-191">String</span><span class="sxs-lookup"><span data-stu-id="810cc-191">String</span></span>|<span data-ttu-id="810cc-192">IP-адрес или DNS-имя узла прокси-сервера при выборе ручной настройки.</span><span class="sxs-lookup"><span data-stu-id="810cc-192">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="810cc-193">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="810cc-193">proxyManualPort</span></span>|<span data-ttu-id="810cc-194">Int32</span><span class="sxs-lookup"><span data-stu-id="810cc-194">Int32</span></span>|<span data-ttu-id="810cc-195">Порт прокси-сервера при выборе ручной настройки.</span><span class="sxs-lookup"><span data-stu-id="810cc-195">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="810cc-196">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="810cc-196">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="810cc-197">String</span><span class="sxs-lookup"><span data-stu-id="810cc-197">String</span></span>|<span data-ttu-id="810cc-198">URL-адрес прокси-сервера сценарий автоматической настройки сервера при выборе автоматической настройки.</span><span class="sxs-lookup"><span data-stu-id="810cc-198">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="810cc-199">Этот URL-адрес обычно имеет расположение файла PAC (автоматической конфигурации прокси-сервера).</span><span class="sxs-lookup"><span data-stu-id="810cc-199">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="810cc-200">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="810cc-200">preSharedKey</span></span>|<span data-ttu-id="810cc-201">String</span><span class="sxs-lookup"><span data-stu-id="810cc-201">String</span></span>|<span data-ttu-id="810cc-202">Это предварительный ключ для WPA личных Сеть Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="810cc-202">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="810cc-203">Ответ</span><span class="sxs-lookup"><span data-stu-id="810cc-203">Response</span></span>
<span data-ttu-id="810cc-204">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="810cc-204">If successful, this method returns a `201 Created` response code and a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="810cc-205">Пример</span><span class="sxs-lookup"><span data-stu-id="810cc-205">Example</span></span>
### <a name="request"></a><span data-ttu-id="810cc-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="810cc-206">Request</span></span>
<span data-ttu-id="810cc-207">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="810cc-207">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 741

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="810cc-208">Ответ</span><span class="sxs-lookup"><span data-stu-id="810cc-208">Response</span></span>
<span data-ttu-id="810cc-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="810cc-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 849

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
  "id": "471203fb-03fb-4712-fb03-1247fb031247",
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





