---
title: Создание Виндовсвификонфигуратион
description: Создание нового объекта Виндовсвификонфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39b5cf192fbb294818d2fb9fb23b49ed0c866739
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163779"
---
# <a name="create-windowswificonfiguration"></a><span data-ttu-id="1c616-103">Создание Виндовсвификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="1c616-103">Create windowsWifiConfiguration</span></span>

> <span data-ttu-id="1c616-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c616-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c616-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c616-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c616-106">Создание нового объекта [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1c616-106">Create a new [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c616-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1c616-107">Prerequisites</span></span>
<span data-ttu-id="1c616-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1c616-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1c616-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c616-110">Permission type</span></span>|<span data-ttu-id="1c616-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c616-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c616-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c616-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1c616-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c616-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c616-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c616-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c616-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c616-115">Not supported.</span></span>|
|<span data-ttu-id="1c616-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c616-116">Application</span></span>|<span data-ttu-id="1c616-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c616-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c616-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c616-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1c616-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c616-119">Request headers</span></span>
|<span data-ttu-id="1c616-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c616-120">Header</span></span>|<span data-ttu-id="1c616-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1c616-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c616-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c616-122">Authorization</span></span>|<span data-ttu-id="1c616-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1c616-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c616-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1c616-124">Accept</span></span>|<span data-ttu-id="1c616-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1c616-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c616-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c616-126">Request body</span></span>
<span data-ttu-id="1c616-127">В тексте запроса добавьте представление объекта Виндовсвификонфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c616-127">In the request body, supply a JSON representation for the windowsWifiConfiguration object.</span></span>

<span data-ttu-id="1c616-128">В следующей таблице приведены свойства, необходимые при создании Виндовсвификонфигуратион.</span><span class="sxs-lookup"><span data-stu-id="1c616-128">The following table shows the properties that are required when you create the windowsWifiConfiguration.</span></span>

|<span data-ttu-id="1c616-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c616-129">Property</span></span>|<span data-ttu-id="1c616-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1c616-130">Type</span></span>|<span data-ttu-id="1c616-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1c616-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c616-132">id</span><span class="sxs-lookup"><span data-stu-id="1c616-132">id</span></span>|<span data-ttu-id="1c616-133">String</span><span class="sxs-lookup"><span data-stu-id="1c616-133">String</span></span>|<span data-ttu-id="1c616-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1c616-134">Key of the entity.</span></span> <span data-ttu-id="1c616-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c616-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c616-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c616-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1c616-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c616-137">DateTimeOffset</span></span>|<span data-ttu-id="1c616-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1c616-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1c616-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c616-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c616-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1c616-140">roleScopeTagIds</span></span>|<span data-ttu-id="1c616-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1c616-141">String collection</span></span>|<span data-ttu-id="1c616-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1c616-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1c616-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c616-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c616-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="1c616-144">supportsScopeTags</span></span>|<span data-ttu-id="1c616-145">Логический</span><span class="sxs-lookup"><span data-stu-id="1c616-145">Boolean</span></span>|<span data-ttu-id="1c616-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1c616-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1c616-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="1c616-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1c616-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1c616-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1c616-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1c616-149">This property is read-only.</span></span> <span data-ttu-id="1c616-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c616-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c616-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c616-151">createdDateTime</span></span>|<span data-ttu-id="1c616-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c616-152">DateTimeOffset</span></span>|<span data-ttu-id="1c616-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1c616-153">DateTime the object was created.</span></span> <span data-ttu-id="1c616-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c616-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c616-155">description</span><span class="sxs-lookup"><span data-stu-id="1c616-155">description</span></span>|<span data-ttu-id="1c616-156">String</span><span class="sxs-lookup"><span data-stu-id="1c616-156">String</span></span>|<span data-ttu-id="1c616-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1c616-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1c616-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c616-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c616-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1c616-159">displayName</span></span>|<span data-ttu-id="1c616-160">String</span><span class="sxs-lookup"><span data-stu-id="1c616-160">String</span></span>|<span data-ttu-id="1c616-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1c616-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1c616-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c616-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c616-163">version</span><span class="sxs-lookup"><span data-stu-id="1c616-163">version</span></span>|<span data-ttu-id="1c616-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1c616-164">Int32</span></span>|<span data-ttu-id="1c616-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1c616-165">Version of the device configuration.</span></span> <span data-ttu-id="1c616-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c616-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c616-167">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="1c616-167">preSharedKey</span></span>|<span data-ttu-id="1c616-168">String</span><span class="sxs-lookup"><span data-stu-id="1c616-168">String</span></span>|<span data-ttu-id="1c616-169">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="1c616-169">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="1c616-170">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="1c616-170">wifiSecurityType</span></span>|[<span data-ttu-id="1c616-171">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="1c616-171">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="1c616-172">Укажите тип безопасности Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="1c616-172">Specify the Wifi Security Type.</span></span> <span data-ttu-id="1c616-173">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="1c616-173">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="1c616-174">Метередконнектионлимит</span><span class="sxs-lookup"><span data-stu-id="1c616-174">meteredConnectionLimit</span></span>|[<span data-ttu-id="1c616-175">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="1c616-175">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="1c616-176">Указать тип лимита межлимитного подключения для подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="1c616-176">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="1c616-177">Возможные значения: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="1c616-177">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="1c616-178">SSID</span><span class="sxs-lookup"><span data-stu-id="1c616-178">ssid</span></span>|<span data-ttu-id="1c616-179">String</span><span class="sxs-lookup"><span data-stu-id="1c616-179">String</span></span>|<span data-ttu-id="1c616-180">Укажите идентификатор SSID подключения WiFi.</span><span class="sxs-lookup"><span data-stu-id="1c616-180">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="1c616-181">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="1c616-181">networkName</span></span>|<span data-ttu-id="1c616-182">String</span><span class="sxs-lookup"><span data-stu-id="1c616-182">String</span></span>|<span data-ttu-id="1c616-183">Укажите имя конфигурации сети.</span><span class="sxs-lookup"><span data-stu-id="1c616-183">Specify the network configuration name.</span></span>|
|<span data-ttu-id="1c616-184">Коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="1c616-184">connectAutomatically</span></span>|<span data-ttu-id="1c616-185">Логический</span><span class="sxs-lookup"><span data-stu-id="1c616-185">Boolean</span></span>|<span data-ttu-id="1c616-186">Указывает, должно ли подключение WiFi автоматически подключаться к сети в пределах диапазона.</span><span class="sxs-lookup"><span data-stu-id="1c616-186">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="1c616-187">Коннекттопреферреднетворк</span><span class="sxs-lookup"><span data-stu-id="1c616-187">connectToPreferredNetwork</span></span>|<span data-ttu-id="1c616-188">Логический</span><span class="sxs-lookup"><span data-stu-id="1c616-188">Boolean</span></span>|<span data-ttu-id="1c616-189">Укажите, должно ли подключение WiFi подключаться к более предпочтительным сетям, если оно уже подключено к этому.</span><span class="sxs-lookup"><span data-stu-id="1c616-189">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="1c616-190">Необходимо, чтобы Коннектаутоматикалли был true.</span><span class="sxs-lookup"><span data-stu-id="1c616-190">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="1c616-191">Коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="1c616-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="1c616-192">Логический</span><span class="sxs-lookup"><span data-stu-id="1c616-192">Boolean</span></span>|<span data-ttu-id="1c616-193">Укажите, должно ли подключение WiFi автоматически подключаться, даже если идентификатор SSID не является широковещательным.</span><span class="sxs-lookup"><span data-stu-id="1c616-193">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="1c616-194">Проксисеттинг</span><span class="sxs-lookup"><span data-stu-id="1c616-194">proxySetting</span></span>|[<span data-ttu-id="1c616-195">Вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="1c616-195">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="1c616-196">Укажите параметры прокси-сервера для конфигурации Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="1c616-196">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="1c616-197">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="1c616-197">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="1c616-198">Проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="1c616-198">proxyManualAddress</span></span>|<span data-ttu-id="1c616-199">String</span><span class="sxs-lookup"><span data-stu-id="1c616-199">String</span></span>|<span data-ttu-id="1c616-200">Укажите IP-адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="1c616-200">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="1c616-201">Проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="1c616-201">proxyManualPort</span></span>|<span data-ttu-id="1c616-202">Int32</span><span class="sxs-lookup"><span data-stu-id="1c616-202">Int32</span></span>|<span data-ttu-id="1c616-203">Укажите порт прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="1c616-203">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="1c616-204">Проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="1c616-204">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="1c616-205">String</span><span class="sxs-lookup"><span data-stu-id="1c616-205">String</span></span>|<span data-ttu-id="1c616-206">Укажите URL-адрес скрипта настройки прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="1c616-206">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="1c616-207">Форцефипскомплианце</span><span class="sxs-lookup"><span data-stu-id="1c616-207">forceFIPSCompliance</span></span>|<span data-ttu-id="1c616-208">Логический</span><span class="sxs-lookup"><span data-stu-id="1c616-208">Boolean</span></span>|<span data-ttu-id="1c616-209">Укажите, следует ли применять соответствие требованиям FIPS.</span><span class="sxs-lookup"><span data-stu-id="1c616-209">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="1c616-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c616-210">Response</span></span>
<span data-ttu-id="1c616-211">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1c616-211">If successful, this method returns a `201 Created` response code and a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c616-212">Пример</span><span class="sxs-lookup"><span data-stu-id="1c616-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c616-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c616-213">Request</span></span>
<span data-ttu-id="1c616-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c616-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 786

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
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

### <a name="response"></a><span data-ttu-id="1c616-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c616-215">Response</span></span>
<span data-ttu-id="1c616-p114">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c616-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




