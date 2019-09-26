---
title: Создание Макосвификонфигуратион
description: Создание нового объекта Макосвификонфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d3bfc88e56e68a04c6c3f78cb0d41e988bbe2620
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37183802"
---
# <a name="create-macoswificonfiguration"></a><span data-ttu-id="f431c-103">Создание Макосвификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="f431c-103">Create macOSWiFiConfiguration</span></span>

> <span data-ttu-id="f431c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f431c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f431c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f431c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f431c-106">Создание нового объекта [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f431c-106">Create a new [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f431c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f431c-107">Prerequisites</span></span>
<span data-ttu-id="f431c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f431c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f431c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f431c-110">Permission type</span></span>|<span data-ttu-id="f431c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f431c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f431c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f431c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f431c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f431c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f431c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f431c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f431c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f431c-115">Not supported.</span></span>|
|<span data-ttu-id="f431c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f431c-116">Application</span></span>|<span data-ttu-id="f431c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f431c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f431c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f431c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f431c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f431c-119">Request headers</span></span>
|<span data-ttu-id="f431c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f431c-120">Header</span></span>|<span data-ttu-id="f431c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f431c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f431c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f431c-122">Authorization</span></span>|<span data-ttu-id="f431c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f431c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f431c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f431c-124">Accept</span></span>|<span data-ttu-id="f431c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f431c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f431c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f431c-126">Request body</span></span>
<span data-ttu-id="f431c-127">В тексте запроса добавьте представление объекта Макосвификонфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f431c-127">In the request body, supply a JSON representation for the macOSWiFiConfiguration object.</span></span>

<span data-ttu-id="f431c-128">В следующей таблице приведены свойства, необходимые при создании Макосвификонфигуратион.</span><span class="sxs-lookup"><span data-stu-id="f431c-128">The following table shows the properties that are required when you create the macOSWiFiConfiguration.</span></span>

|<span data-ttu-id="f431c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f431c-129">Property</span></span>|<span data-ttu-id="f431c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f431c-130">Type</span></span>|<span data-ttu-id="f431c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f431c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f431c-132">id</span><span class="sxs-lookup"><span data-stu-id="f431c-132">id</span></span>|<span data-ttu-id="f431c-133">String</span><span class="sxs-lookup"><span data-stu-id="f431c-133">String</span></span>|<span data-ttu-id="f431c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f431c-134">Key of the entity.</span></span> <span data-ttu-id="f431c-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f431c-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f431c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f431c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f431c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f431c-137">DateTimeOffset</span></span>|<span data-ttu-id="f431c-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f431c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f431c-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f431c-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f431c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f431c-140">roleScopeTagIds</span></span>|<span data-ttu-id="f431c-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f431c-141">String collection</span></span>|<span data-ttu-id="f431c-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f431c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f431c-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f431c-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f431c-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f431c-144">supportsScopeTags</span></span>|<span data-ttu-id="f431c-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f431c-145">Boolean</span></span>|<span data-ttu-id="f431c-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f431c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f431c-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f431c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f431c-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f431c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f431c-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f431c-149">This property is read-only.</span></span> <span data-ttu-id="f431c-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f431c-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f431c-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f431c-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f431c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f431c-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f431c-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f431c-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f431c-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f431c-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f431c-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f431c-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f431c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f431c-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f431c-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f431c-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f431c-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f431c-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f431c-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="f431c-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f431c-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="f431c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f431c-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f431c-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f431c-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f431c-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f431c-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f431c-163">createdDateTime</span></span>|<span data-ttu-id="f431c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f431c-164">DateTimeOffset</span></span>|<span data-ttu-id="f431c-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f431c-165">DateTime the object was created.</span></span> <span data-ttu-id="f431c-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f431c-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f431c-167">description</span><span class="sxs-lookup"><span data-stu-id="f431c-167">description</span></span>|<span data-ttu-id="f431c-168">String</span><span class="sxs-lookup"><span data-stu-id="f431c-168">String</span></span>|<span data-ttu-id="f431c-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f431c-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f431c-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f431c-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f431c-171">displayName</span><span class="sxs-lookup"><span data-stu-id="f431c-171">displayName</span></span>|<span data-ttu-id="f431c-172">Строка</span><span class="sxs-lookup"><span data-stu-id="f431c-172">String</span></span>|<span data-ttu-id="f431c-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f431c-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f431c-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f431c-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f431c-175">version</span><span class="sxs-lookup"><span data-stu-id="f431c-175">version</span></span>|<span data-ttu-id="f431c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f431c-176">Int32</span></span>|<span data-ttu-id="f431c-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f431c-177">Version of the device configuration.</span></span> <span data-ttu-id="f431c-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f431c-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f431c-179">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="f431c-179">networkName</span></span>|<span data-ttu-id="f431c-180">String.</span><span class="sxs-lookup"><span data-stu-id="f431c-180">String</span></span>|<span data-ttu-id="f431c-181">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="f431c-181">Network Name</span></span>|
|<span data-ttu-id="f431c-182">SSID</span><span class="sxs-lookup"><span data-stu-id="f431c-182">ssid</span></span>|<span data-ttu-id="f431c-183">String.</span><span class="sxs-lookup"><span data-stu-id="f431c-183">String</span></span>|<span data-ttu-id="f431c-184">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="f431c-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="f431c-185">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="f431c-185">connectAutomatically</span></span>|<span data-ttu-id="f431c-186">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f431c-186">Boolean</span></span>|<span data-ttu-id="f431c-187">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="f431c-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="f431c-188">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="f431c-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="f431c-189">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="f431c-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="f431c-190">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f431c-190">Boolean</span></span>|<span data-ttu-id="f431c-191">Подключаться, если сеть не ведет вещание своего имени (SSID).</span><span class="sxs-lookup"><span data-stu-id="f431c-191">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="f431c-192">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="f431c-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="f431c-193">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="f431c-193">wiFiSecurityType</span></span>|[<span data-ttu-id="f431c-194">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="f431c-194">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="f431c-195">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="f431c-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="f431c-196">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="f431c-196">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="f431c-197">proxySettings</span><span class="sxs-lookup"><span data-stu-id="f431c-197">proxySettings</span></span>|[<span data-ttu-id="f431c-198">вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="f431c-198">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="f431c-199">Тип прокси-сервера для этого подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f431c-199">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="f431c-200">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="f431c-200">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="f431c-201">проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="f431c-201">proxyManualAddress</span></span>|<span data-ttu-id="f431c-202">String.</span><span class="sxs-lookup"><span data-stu-id="f431c-202">String</span></span>|<span data-ttu-id="f431c-203">IP-адрес или DNS-имя узла прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="f431c-203">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="f431c-204">проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="f431c-204">proxyManualPort</span></span>|<span data-ttu-id="f431c-205">Int32</span><span class="sxs-lookup"><span data-stu-id="f431c-205">Int32</span></span>|<span data-ttu-id="f431c-206">Порт прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="f431c-206">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="f431c-207">проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="f431c-207">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="f431c-208">String.</span><span class="sxs-lookup"><span data-stu-id="f431c-208">String</span></span>|<span data-ttu-id="f431c-209">URL-адрес скрипта автоматической настройки прокси-сервера при выборе параметра Автоматическая настройка.</span><span class="sxs-lookup"><span data-stu-id="f431c-209">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="f431c-210">Обычно это URL-адрес файла PAC (Автонастройка прокси-сервера).</span><span class="sxs-lookup"><span data-stu-id="f431c-210">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="f431c-211">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="f431c-211">preSharedKey</span></span>|<span data-ttu-id="f431c-212">String.</span><span class="sxs-lookup"><span data-stu-id="f431c-212">String</span></span>|<span data-ttu-id="f431c-213">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="f431c-213">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="f431c-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="f431c-214">Response</span></span>
<span data-ttu-id="f431c-215">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f431c-215">If successful, this method returns a `201 Created` response code and a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f431c-216">Пример</span><span class="sxs-lookup"><span data-stu-id="f431c-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="f431c-217">Запрос</span><span class="sxs-lookup"><span data-stu-id="f431c-217">Request</span></span>
<span data-ttu-id="f431c-218">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f431c-218">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1450

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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

### <a name="response"></a><span data-ttu-id="f431c-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="f431c-219">Response</span></span>
<span data-ttu-id="f431c-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f431c-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1622

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
  "id": "471203fb-03fb-4712-fb03-1247fb031247",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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




