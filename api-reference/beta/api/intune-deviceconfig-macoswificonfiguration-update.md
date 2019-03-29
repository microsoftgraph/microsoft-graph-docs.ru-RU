---
title: Обновление Макосвификонфигуратион
description: Обновление свойств объекта Макосвификонфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7d74445159fa14bd23ba928eb2b2a1461b8c5eeb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967120"
---
# <a name="update-macoswificonfiguration"></a><span data-ttu-id="33785-103">Обновление Макосвификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="33785-103">Update macOSWiFiConfiguration</span></span>

> <span data-ttu-id="33785-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33785-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33785-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33785-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33785-106">Обновление свойств объекта [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="33785-106">Update the properties of a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33785-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="33785-107">Prerequisites</span></span>
<span data-ttu-id="33785-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33785-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33785-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33785-110">Permission type</span></span>|<span data-ttu-id="33785-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33785-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33785-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33785-112">Delegated (work or school account)</span></span>|<span data-ttu-id="33785-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33785-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="33785-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33785-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33785-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33785-115">Not supported.</span></span>|
|<span data-ttu-id="33785-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33785-116">Application</span></span>|<span data-ttu-id="33785-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33785-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33785-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33785-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="33785-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33785-119">Request headers</span></span>
|<span data-ttu-id="33785-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33785-120">Header</span></span>|<span data-ttu-id="33785-121">Значение</span><span class="sxs-lookup"><span data-stu-id="33785-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33785-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33785-122">Authorization</span></span>|<span data-ttu-id="33785-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33785-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33785-124">Accept</span><span class="sxs-lookup"><span data-stu-id="33785-124">Accept</span></span>|<span data-ttu-id="33785-125">application/json</span><span class="sxs-lookup"><span data-stu-id="33785-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33785-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33785-126">Request body</span></span>
<span data-ttu-id="33785-127">В тексте запроса добавьте представление объекта [Макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33785-127">In the request body, supply a JSON representation for the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

<span data-ttu-id="33785-128">В следующей таблице приведены свойства, необходимые при создании [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33785-128">The following table shows the properties that are required when you create the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span>

|<span data-ttu-id="33785-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="33785-129">Property</span></span>|<span data-ttu-id="33785-130">Тип</span><span class="sxs-lookup"><span data-stu-id="33785-130">Type</span></span>|<span data-ttu-id="33785-131">Описание</span><span class="sxs-lookup"><span data-stu-id="33785-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33785-132">id</span><span class="sxs-lookup"><span data-stu-id="33785-132">id</span></span>|<span data-ttu-id="33785-133">Строка</span><span class="sxs-lookup"><span data-stu-id="33785-133">String</span></span>|<span data-ttu-id="33785-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="33785-134">Key of the entity.</span></span> <span data-ttu-id="33785-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33785-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33785-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33785-136">lastModifiedDateTime</span></span>|<span data-ttu-id="33785-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33785-137">DateTimeOffset</span></span>|<span data-ttu-id="33785-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="33785-138">DateTime the object was last modified.</span></span> <span data-ttu-id="33785-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33785-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33785-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="33785-140">roleScopeTagIds</span></span>|<span data-ttu-id="33785-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="33785-141">String collection</span></span>|<span data-ttu-id="33785-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="33785-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="33785-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33785-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33785-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="33785-144">supportsScopeTags</span></span>|<span data-ttu-id="33785-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="33785-145">Boolean</span></span>|<span data-ttu-id="33785-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="33785-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="33785-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="33785-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="33785-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="33785-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="33785-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33785-149">This property is read-only.</span></span> <span data-ttu-id="33785-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33785-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33785-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33785-151">createdDateTime</span></span>|<span data-ttu-id="33785-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33785-152">DateTimeOffset</span></span>|<span data-ttu-id="33785-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="33785-153">DateTime the object was created.</span></span> <span data-ttu-id="33785-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33785-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33785-155">description</span><span class="sxs-lookup"><span data-stu-id="33785-155">description</span></span>|<span data-ttu-id="33785-156">String</span><span class="sxs-lookup"><span data-stu-id="33785-156">String</span></span>|<span data-ttu-id="33785-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="33785-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="33785-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33785-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33785-159">displayName</span><span class="sxs-lookup"><span data-stu-id="33785-159">displayName</span></span>|<span data-ttu-id="33785-160">String</span><span class="sxs-lookup"><span data-stu-id="33785-160">String</span></span>|<span data-ttu-id="33785-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="33785-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="33785-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33785-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33785-163">version</span><span class="sxs-lookup"><span data-stu-id="33785-163">version</span></span>|<span data-ttu-id="33785-164">Int32</span><span class="sxs-lookup"><span data-stu-id="33785-164">Int32</span></span>|<span data-ttu-id="33785-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="33785-165">Version of the device configuration.</span></span> <span data-ttu-id="33785-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33785-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33785-167">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="33785-167">networkName</span></span>|<span data-ttu-id="33785-168">String</span><span class="sxs-lookup"><span data-stu-id="33785-168">String</span></span>|<span data-ttu-id="33785-169">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="33785-169">Network Name</span></span>|
|<span data-ttu-id="33785-170">SSID</span><span class="sxs-lookup"><span data-stu-id="33785-170">ssid</span></span>|<span data-ttu-id="33785-171">String</span><span class="sxs-lookup"><span data-stu-id="33785-171">String</span></span>|<span data-ttu-id="33785-172">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="33785-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="33785-173">Коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="33785-173">connectAutomatically</span></span>|<span data-ttu-id="33785-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="33785-174">Boolean</span></span>|<span data-ttu-id="33785-175">ПодКлючаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="33785-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="33785-176">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="33785-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="33785-177">Коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="33785-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="33785-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="33785-178">Boolean</span></span>|<span data-ttu-id="33785-179">ПодКлючаться, если сеть не ведет вещание своего имени (SSID).</span><span class="sxs-lookup"><span data-stu-id="33785-179">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="33785-180">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="33785-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="33785-181">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="33785-181">wiFiSecurityType</span></span>|[<span data-ttu-id="33785-182">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="33785-182">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="33785-183">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="33785-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="33785-184">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="33785-184">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="33785-185">proxySettings</span><span class="sxs-lookup"><span data-stu-id="33785-185">proxySettings</span></span>|[<span data-ttu-id="33785-186">Вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="33785-186">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="33785-187">Тип прокси-сервера для этого подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="33785-187">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="33785-188">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="33785-188">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="33785-189">Проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="33785-189">proxyManualAddress</span></span>|<span data-ttu-id="33785-190">String</span><span class="sxs-lookup"><span data-stu-id="33785-190">String</span></span>|<span data-ttu-id="33785-191">IP-адрес или DNS-имя узла прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="33785-191">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="33785-192">Проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="33785-192">proxyManualPort</span></span>|<span data-ttu-id="33785-193">Int32</span><span class="sxs-lookup"><span data-stu-id="33785-193">Int32</span></span>|<span data-ttu-id="33785-194">Порт прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="33785-194">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="33785-195">Проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="33785-195">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="33785-196">String</span><span class="sxs-lookup"><span data-stu-id="33785-196">String</span></span>|<span data-ttu-id="33785-197">URL-адрес скрипта автоматической настройки прокси-сервера при выборе параметра Автоматическая настройка.</span><span class="sxs-lookup"><span data-stu-id="33785-197">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="33785-198">Обычно это URL-адрес файла PAC (автоНастройка прокси-сервера).</span><span class="sxs-lookup"><span data-stu-id="33785-198">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="33785-199">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="33785-199">preSharedKey</span></span>|<span data-ttu-id="33785-200">String</span><span class="sxs-lookup"><span data-stu-id="33785-200">String</span></span>|<span data-ttu-id="33785-201">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="33785-201">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="33785-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="33785-202">Response</span></span>
<span data-ttu-id="33785-203">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="33785-203">If successful, this method returns a `200 OK` response code and an updated [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33785-204">Пример</span><span class="sxs-lookup"><span data-stu-id="33785-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="33785-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="33785-205">Request</span></span>
<span data-ttu-id="33785-206">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33785-206">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="33785-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="33785-207">Response</span></span>
<span data-ttu-id="33785-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33785-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




