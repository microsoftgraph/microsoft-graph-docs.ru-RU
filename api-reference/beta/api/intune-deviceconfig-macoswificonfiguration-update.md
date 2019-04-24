---
title: Обновление Макосвификонфигуратион
description: Обновление свойств объекта Макосвификонфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba82df6f6f709fa5066e57f5fb107f0f45c4a0c0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518235"
---
# <a name="update-macoswificonfiguration"></a><span data-ttu-id="43743-103">Обновление Макосвификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="43743-103">Update macOSWiFiConfiguration</span></span>

> <span data-ttu-id="43743-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43743-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43743-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43743-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43743-106">Обновление свойств объекта [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="43743-106">Update the properties of a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43743-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="43743-107">Prerequisites</span></span>
<span data-ttu-id="43743-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43743-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43743-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43743-110">Permission type</span></span>|<span data-ttu-id="43743-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="43743-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43743-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43743-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43743-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43743-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43743-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43743-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43743-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43743-115">Not supported.</span></span>|
|<span data-ttu-id="43743-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43743-116">Application</span></span>|<span data-ttu-id="43743-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43743-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43743-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43743-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="43743-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43743-119">Request headers</span></span>
|<span data-ttu-id="43743-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43743-120">Header</span></span>|<span data-ttu-id="43743-121">Значение</span><span class="sxs-lookup"><span data-stu-id="43743-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43743-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43743-122">Authorization</span></span>|<span data-ttu-id="43743-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43743-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43743-124">Accept</span><span class="sxs-lookup"><span data-stu-id="43743-124">Accept</span></span>|<span data-ttu-id="43743-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43743-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43743-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43743-126">Request body</span></span>
<span data-ttu-id="43743-127">В тексте запроса добавьте представление объекта [Макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43743-127">In the request body, supply a JSON representation for the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

<span data-ttu-id="43743-128">В следующей таблице приведены свойства, необходимые при создании [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="43743-128">The following table shows the properties that are required when you create the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span>

|<span data-ttu-id="43743-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="43743-129">Property</span></span>|<span data-ttu-id="43743-130">Тип</span><span class="sxs-lookup"><span data-stu-id="43743-130">Type</span></span>|<span data-ttu-id="43743-131">Описание</span><span class="sxs-lookup"><span data-stu-id="43743-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43743-132">id</span><span class="sxs-lookup"><span data-stu-id="43743-132">id</span></span>|<span data-ttu-id="43743-133">Строка</span><span class="sxs-lookup"><span data-stu-id="43743-133">String</span></span>|<span data-ttu-id="43743-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="43743-134">Key of the entity.</span></span> <span data-ttu-id="43743-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="43743-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43743-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43743-136">lastModifiedDateTime</span></span>|<span data-ttu-id="43743-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43743-137">DateTimeOffset</span></span>|<span data-ttu-id="43743-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="43743-138">DateTime the object was last modified.</span></span> <span data-ttu-id="43743-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="43743-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43743-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="43743-140">roleScopeTagIds</span></span>|<span data-ttu-id="43743-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="43743-141">String collection</span></span>|<span data-ttu-id="43743-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="43743-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="43743-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="43743-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43743-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="43743-144">supportsScopeTags</span></span>|<span data-ttu-id="43743-145">Логический</span><span class="sxs-lookup"><span data-stu-id="43743-145">Boolean</span></span>|<span data-ttu-id="43743-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="43743-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="43743-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="43743-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="43743-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="43743-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="43743-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43743-149">This property is read-only.</span></span> <span data-ttu-id="43743-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="43743-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43743-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43743-151">createdDateTime</span></span>|<span data-ttu-id="43743-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43743-152">DateTimeOffset</span></span>|<span data-ttu-id="43743-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="43743-153">DateTime the object was created.</span></span> <span data-ttu-id="43743-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="43743-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43743-155">description</span><span class="sxs-lookup"><span data-stu-id="43743-155">description</span></span>|<span data-ttu-id="43743-156">String</span><span class="sxs-lookup"><span data-stu-id="43743-156">String</span></span>|<span data-ttu-id="43743-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="43743-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="43743-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="43743-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43743-159">displayName</span><span class="sxs-lookup"><span data-stu-id="43743-159">displayName</span></span>|<span data-ttu-id="43743-160">String</span><span class="sxs-lookup"><span data-stu-id="43743-160">String</span></span>|<span data-ttu-id="43743-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="43743-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="43743-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="43743-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43743-163">version</span><span class="sxs-lookup"><span data-stu-id="43743-163">version</span></span>|<span data-ttu-id="43743-164">Int32</span><span class="sxs-lookup"><span data-stu-id="43743-164">Int32</span></span>|<span data-ttu-id="43743-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="43743-165">Version of the device configuration.</span></span> <span data-ttu-id="43743-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="43743-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43743-167">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="43743-167">networkName</span></span>|<span data-ttu-id="43743-168">String</span><span class="sxs-lookup"><span data-stu-id="43743-168">String</span></span>|<span data-ttu-id="43743-169">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="43743-169">Network Name</span></span>|
|<span data-ttu-id="43743-170">SSID</span><span class="sxs-lookup"><span data-stu-id="43743-170">ssid</span></span>|<span data-ttu-id="43743-171">String</span><span class="sxs-lookup"><span data-stu-id="43743-171">String</span></span>|<span data-ttu-id="43743-172">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="43743-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="43743-173">Коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="43743-173">connectAutomatically</span></span>|<span data-ttu-id="43743-174">Логический</span><span class="sxs-lookup"><span data-stu-id="43743-174">Boolean</span></span>|<span data-ttu-id="43743-175">ПодКлючаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="43743-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="43743-176">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="43743-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="43743-177">Коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="43743-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="43743-178">Логический</span><span class="sxs-lookup"><span data-stu-id="43743-178">Boolean</span></span>|<span data-ttu-id="43743-179">ПодКлючаться, если сеть не ведет вещание своего имени (SSID).</span><span class="sxs-lookup"><span data-stu-id="43743-179">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="43743-180">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="43743-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="43743-181">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="43743-181">wiFiSecurityType</span></span>|[<span data-ttu-id="43743-182">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="43743-182">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="43743-183">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="43743-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="43743-184">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="43743-184">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="43743-185">proxySettings</span><span class="sxs-lookup"><span data-stu-id="43743-185">proxySettings</span></span>|[<span data-ttu-id="43743-186">Вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="43743-186">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="43743-187">Тип прокси-сервера для этого подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="43743-187">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="43743-188">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="43743-188">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="43743-189">Проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="43743-189">proxyManualAddress</span></span>|<span data-ttu-id="43743-190">String</span><span class="sxs-lookup"><span data-stu-id="43743-190">String</span></span>|<span data-ttu-id="43743-191">IP-адрес или DNS-имя узла прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="43743-191">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="43743-192">Проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="43743-192">proxyManualPort</span></span>|<span data-ttu-id="43743-193">Int32</span><span class="sxs-lookup"><span data-stu-id="43743-193">Int32</span></span>|<span data-ttu-id="43743-194">Порт прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="43743-194">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="43743-195">Проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="43743-195">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="43743-196">String</span><span class="sxs-lookup"><span data-stu-id="43743-196">String</span></span>|<span data-ttu-id="43743-197">URL-адрес скрипта автоматической настройки прокси-сервера при выборе параметра Автоматическая настройка.</span><span class="sxs-lookup"><span data-stu-id="43743-197">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="43743-198">Обычно это URL-адрес файла PAC (автоНастройка прокси-сервера).</span><span class="sxs-lookup"><span data-stu-id="43743-198">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="43743-199">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="43743-199">preSharedKey</span></span>|<span data-ttu-id="43743-200">String</span><span class="sxs-lookup"><span data-stu-id="43743-200">String</span></span>|<span data-ttu-id="43743-201">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="43743-201">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="43743-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="43743-202">Response</span></span>
<span data-ttu-id="43743-203">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="43743-203">If successful, this method returns a `200 OK` response code and an updated [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43743-204">Пример</span><span class="sxs-lookup"><span data-stu-id="43743-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="43743-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="43743-205">Request</span></span>
<span data-ttu-id="43743-206">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43743-206">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="43743-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="43743-207">Response</span></span>
<span data-ttu-id="43743-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43743-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





