---
title: Создание Макосвификонфигуратион
description: Создание нового объекта Макосвификонфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 28b72ed5e99bd6aa3779e433c7976a4ad4b0d142
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967267"
---
# <a name="create-macoswificonfiguration"></a><span data-ttu-id="46763-103">Создание Макосвификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="46763-103">Create macOSWiFiConfiguration</span></span>

> <span data-ttu-id="46763-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46763-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46763-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46763-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46763-106">Создание нового объекта [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="46763-106">Create a new [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46763-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="46763-107">Prerequisites</span></span>
<span data-ttu-id="46763-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46763-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46763-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46763-110">Permission type</span></span>|<span data-ttu-id="46763-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46763-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46763-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46763-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46763-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46763-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="46763-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46763-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46763-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46763-115">Not supported.</span></span>|
|<span data-ttu-id="46763-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46763-116">Application</span></span>|<span data-ttu-id="46763-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46763-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46763-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46763-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="46763-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46763-119">Request headers</span></span>
|<span data-ttu-id="46763-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46763-120">Header</span></span>|<span data-ttu-id="46763-121">Значение</span><span class="sxs-lookup"><span data-stu-id="46763-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46763-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46763-122">Authorization</span></span>|<span data-ttu-id="46763-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46763-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46763-124">Accept</span><span class="sxs-lookup"><span data-stu-id="46763-124">Accept</span></span>|<span data-ttu-id="46763-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46763-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46763-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46763-126">Request body</span></span>
<span data-ttu-id="46763-127">В тексте запроса добавьте представление объекта Макосвификонфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46763-127">In the request body, supply a JSON representation for the macOSWiFiConfiguration object.</span></span>

<span data-ttu-id="46763-128">В следующей таблице приведены свойства, необходимые при создании Макосвификонфигуратион.</span><span class="sxs-lookup"><span data-stu-id="46763-128">The following table shows the properties that are required when you create the macOSWiFiConfiguration.</span></span>

|<span data-ttu-id="46763-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="46763-129">Property</span></span>|<span data-ttu-id="46763-130">Тип</span><span class="sxs-lookup"><span data-stu-id="46763-130">Type</span></span>|<span data-ttu-id="46763-131">Описание</span><span class="sxs-lookup"><span data-stu-id="46763-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46763-132">id</span><span class="sxs-lookup"><span data-stu-id="46763-132">id</span></span>|<span data-ttu-id="46763-133">Строка</span><span class="sxs-lookup"><span data-stu-id="46763-133">String</span></span>|<span data-ttu-id="46763-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="46763-134">Key of the entity.</span></span> <span data-ttu-id="46763-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46763-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46763-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="46763-136">lastModifiedDateTime</span></span>|<span data-ttu-id="46763-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46763-137">DateTimeOffset</span></span>|<span data-ttu-id="46763-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="46763-138">DateTime the object was last modified.</span></span> <span data-ttu-id="46763-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46763-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46763-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="46763-140">roleScopeTagIds</span></span>|<span data-ttu-id="46763-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="46763-141">String collection</span></span>|<span data-ttu-id="46763-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="46763-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="46763-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46763-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46763-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="46763-144">supportsScopeTags</span></span>|<span data-ttu-id="46763-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="46763-145">Boolean</span></span>|<span data-ttu-id="46763-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="46763-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="46763-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="46763-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="46763-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="46763-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="46763-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46763-149">This property is read-only.</span></span> <span data-ttu-id="46763-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46763-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46763-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="46763-151">createdDateTime</span></span>|<span data-ttu-id="46763-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46763-152">DateTimeOffset</span></span>|<span data-ttu-id="46763-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="46763-153">DateTime the object was created.</span></span> <span data-ttu-id="46763-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46763-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46763-155">description</span><span class="sxs-lookup"><span data-stu-id="46763-155">description</span></span>|<span data-ttu-id="46763-156">String</span><span class="sxs-lookup"><span data-stu-id="46763-156">String</span></span>|<span data-ttu-id="46763-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="46763-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="46763-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46763-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46763-159">displayName</span><span class="sxs-lookup"><span data-stu-id="46763-159">displayName</span></span>|<span data-ttu-id="46763-160">String</span><span class="sxs-lookup"><span data-stu-id="46763-160">String</span></span>|<span data-ttu-id="46763-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="46763-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="46763-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46763-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46763-163">version</span><span class="sxs-lookup"><span data-stu-id="46763-163">version</span></span>|<span data-ttu-id="46763-164">Int32</span><span class="sxs-lookup"><span data-stu-id="46763-164">Int32</span></span>|<span data-ttu-id="46763-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="46763-165">Version of the device configuration.</span></span> <span data-ttu-id="46763-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46763-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="46763-167">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="46763-167">networkName</span></span>|<span data-ttu-id="46763-168">String</span><span class="sxs-lookup"><span data-stu-id="46763-168">String</span></span>|<span data-ttu-id="46763-169">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="46763-169">Network Name</span></span>|
|<span data-ttu-id="46763-170">SSID</span><span class="sxs-lookup"><span data-stu-id="46763-170">ssid</span></span>|<span data-ttu-id="46763-171">String</span><span class="sxs-lookup"><span data-stu-id="46763-171">String</span></span>|<span data-ttu-id="46763-172">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="46763-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="46763-173">Коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="46763-173">connectAutomatically</span></span>|<span data-ttu-id="46763-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="46763-174">Boolean</span></span>|<span data-ttu-id="46763-175">ПодКлючаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="46763-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="46763-176">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="46763-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="46763-177">Коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="46763-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="46763-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="46763-178">Boolean</span></span>|<span data-ttu-id="46763-179">ПодКлючаться, если сеть не ведет вещание своего имени (SSID).</span><span class="sxs-lookup"><span data-stu-id="46763-179">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="46763-180">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="46763-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="46763-181">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="46763-181">wiFiSecurityType</span></span>|[<span data-ttu-id="46763-182">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="46763-182">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="46763-183">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="46763-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="46763-184">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="46763-184">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="46763-185">proxySettings</span><span class="sxs-lookup"><span data-stu-id="46763-185">proxySettings</span></span>|[<span data-ttu-id="46763-186">Вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="46763-186">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="46763-187">Тип прокси-сервера для этого подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="46763-187">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="46763-188">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="46763-188">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="46763-189">Проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="46763-189">proxyManualAddress</span></span>|<span data-ttu-id="46763-190">String</span><span class="sxs-lookup"><span data-stu-id="46763-190">String</span></span>|<span data-ttu-id="46763-191">IP-адрес или DNS-имя узла прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="46763-191">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="46763-192">Проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="46763-192">proxyManualPort</span></span>|<span data-ttu-id="46763-193">Int32</span><span class="sxs-lookup"><span data-stu-id="46763-193">Int32</span></span>|<span data-ttu-id="46763-194">Порт прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="46763-194">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="46763-195">Проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="46763-195">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="46763-196">String</span><span class="sxs-lookup"><span data-stu-id="46763-196">String</span></span>|<span data-ttu-id="46763-197">URL-адрес скрипта автоматической настройки прокси-сервера при выборе параметра Автоматическая настройка.</span><span class="sxs-lookup"><span data-stu-id="46763-197">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="46763-198">Обычно это URL-адрес файла PAC (автоНастройка прокси-сервера).</span><span class="sxs-lookup"><span data-stu-id="46763-198">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="46763-199">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="46763-199">preSharedKey</span></span>|<span data-ttu-id="46763-200">String</span><span class="sxs-lookup"><span data-stu-id="46763-200">String</span></span>|<span data-ttu-id="46763-201">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="46763-201">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="46763-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="46763-202">Response</span></span>
<span data-ttu-id="46763-203">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="46763-203">If successful, this method returns a `201 Created` response code and a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46763-204">Пример</span><span class="sxs-lookup"><span data-stu-id="46763-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="46763-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="46763-205">Request</span></span>
<span data-ttu-id="46763-206">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46763-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 677

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="46763-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="46763-207">Response</span></span>
<span data-ttu-id="46763-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46763-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




