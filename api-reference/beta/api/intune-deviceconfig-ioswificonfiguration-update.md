---
title: Обновление iosWiFiConfiguration
description: Обновление свойств объекта iosWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f5321854cccc6b0bcb7a7f0eb2b0f108931ae506
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37178951"
---
# <a name="update-ioswificonfiguration"></a><span data-ttu-id="83d4e-103">Обновление iosWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="83d4e-103">Update iosWiFiConfiguration</span></span>

> <span data-ttu-id="83d4e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83d4e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83d4e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83d4e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83d4e-106">Обновление свойств объекта [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="83d4e-106">Update the properties of a [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83d4e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="83d4e-107">Prerequisites</span></span>
<span data-ttu-id="83d4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83d4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83d4e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83d4e-110">Permission type</span></span>|<span data-ttu-id="83d4e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="83d4e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83d4e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83d4e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="83d4e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83d4e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83d4e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83d4e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83d4e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83d4e-115">Not supported.</span></span>|
|<span data-ttu-id="83d4e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83d4e-116">Application</span></span>|<span data-ttu-id="83d4e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83d4e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83d4e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83d4e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="83d4e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83d4e-119">Request headers</span></span>
|<span data-ttu-id="83d4e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="83d4e-120">Header</span></span>|<span data-ttu-id="83d4e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="83d4e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83d4e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83d4e-122">Authorization</span></span>|<span data-ttu-id="83d4e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83d4e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83d4e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="83d4e-124">Accept</span></span>|<span data-ttu-id="83d4e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="83d4e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83d4e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="83d4e-126">Request body</span></span>
<span data-ttu-id="83d4e-127">В тексте запроса добавьте представление объекта [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83d4e-127">In the request body, supply a JSON representation for the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

<span data-ttu-id="83d4e-128">В следующей таблице приведены свойства, необходимые при создании [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83d4e-128">The following table shows the properties that are required when you create the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span>

|<span data-ttu-id="83d4e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="83d4e-129">Property</span></span>|<span data-ttu-id="83d4e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="83d4e-130">Type</span></span>|<span data-ttu-id="83d4e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="83d4e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83d4e-132">id</span><span class="sxs-lookup"><span data-stu-id="83d4e-132">id</span></span>|<span data-ttu-id="83d4e-133">String</span><span class="sxs-lookup"><span data-stu-id="83d4e-133">String</span></span>|<span data-ttu-id="83d4e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="83d4e-134">Key of the entity.</span></span> <span data-ttu-id="83d4e-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83d4e-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d4e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83d4e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="83d4e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83d4e-137">DateTimeOffset</span></span>|<span data-ttu-id="83d4e-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="83d4e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="83d4e-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83d4e-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d4e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="83d4e-140">roleScopeTagIds</span></span>|<span data-ttu-id="83d4e-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="83d4e-141">String collection</span></span>|<span data-ttu-id="83d4e-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="83d4e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="83d4e-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83d4e-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d4e-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="83d4e-144">supportsScopeTags</span></span>|<span data-ttu-id="83d4e-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="83d4e-145">Boolean</span></span>|<span data-ttu-id="83d4e-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="83d4e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="83d4e-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="83d4e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="83d4e-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="83d4e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="83d4e-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="83d4e-149">This property is read-only.</span></span> <span data-ttu-id="83d4e-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83d4e-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d4e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="83d4e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="83d4e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="83d4e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="83d4e-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="83d4e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="83d4e-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83d4e-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d4e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="83d4e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="83d4e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="83d4e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="83d4e-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="83d4e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="83d4e-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83d4e-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d4e-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="83d4e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="83d4e-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="83d4e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="83d4e-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="83d4e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="83d4e-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83d4e-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d4e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83d4e-163">createdDateTime</span></span>|<span data-ttu-id="83d4e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83d4e-164">DateTimeOffset</span></span>|<span data-ttu-id="83d4e-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="83d4e-165">DateTime the object was created.</span></span> <span data-ttu-id="83d4e-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83d4e-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d4e-167">description</span><span class="sxs-lookup"><span data-stu-id="83d4e-167">description</span></span>|<span data-ttu-id="83d4e-168">String</span><span class="sxs-lookup"><span data-stu-id="83d4e-168">String</span></span>|<span data-ttu-id="83d4e-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="83d4e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="83d4e-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83d4e-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d4e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="83d4e-171">displayName</span></span>|<span data-ttu-id="83d4e-172">Строка</span><span class="sxs-lookup"><span data-stu-id="83d4e-172">String</span></span>|<span data-ttu-id="83d4e-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="83d4e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="83d4e-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83d4e-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d4e-175">version</span><span class="sxs-lookup"><span data-stu-id="83d4e-175">version</span></span>|<span data-ttu-id="83d4e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="83d4e-176">Int32</span></span>|<span data-ttu-id="83d4e-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="83d4e-177">Version of the device configuration.</span></span> <span data-ttu-id="83d4e-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83d4e-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83d4e-179">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="83d4e-179">networkName</span></span>|<span data-ttu-id="83d4e-180">String.</span><span class="sxs-lookup"><span data-stu-id="83d4e-180">String</span></span>|<span data-ttu-id="83d4e-181">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="83d4e-181">Network Name</span></span>|
|<span data-ttu-id="83d4e-182">SSID</span><span class="sxs-lookup"><span data-stu-id="83d4e-182">ssid</span></span>|<span data-ttu-id="83d4e-183">String.</span><span class="sxs-lookup"><span data-stu-id="83d4e-183">String</span></span>|<span data-ttu-id="83d4e-184">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="83d4e-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="83d4e-185">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="83d4e-185">connectAutomatically</span></span>|<span data-ttu-id="83d4e-186">Boolean.</span><span class="sxs-lookup"><span data-stu-id="83d4e-186">Boolean</span></span>|<span data-ttu-id="83d4e-187">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="83d4e-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="83d4e-188">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="83d4e-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="83d4e-189">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="83d4e-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="83d4e-190">Boolean.</span><span class="sxs-lookup"><span data-stu-id="83d4e-190">Boolean</span></span>|<span data-ttu-id="83d4e-191">Подключаться, если сеть не ведет вещание своего имени (SSID).</span><span class="sxs-lookup"><span data-stu-id="83d4e-191">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="83d4e-192">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="83d4e-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="83d4e-193">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="83d4e-193">wiFiSecurityType</span></span>|[<span data-ttu-id="83d4e-194">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="83d4e-194">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="83d4e-195">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="83d4e-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="83d4e-196">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="83d4e-196">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="83d4e-197">proxySettings</span><span class="sxs-lookup"><span data-stu-id="83d4e-197">proxySettings</span></span>|[<span data-ttu-id="83d4e-198">вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="83d4e-198">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="83d4e-199">Тип прокси-сервера для этого подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="83d4e-199">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="83d4e-200">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="83d4e-200">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="83d4e-201">проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="83d4e-201">proxyManualAddress</span></span>|<span data-ttu-id="83d4e-202">String.</span><span class="sxs-lookup"><span data-stu-id="83d4e-202">String</span></span>|<span data-ttu-id="83d4e-203">IP-адрес или DNS-имя узла прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="83d4e-203">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="83d4e-204">проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="83d4e-204">proxyManualPort</span></span>|<span data-ttu-id="83d4e-205">Int32</span><span class="sxs-lookup"><span data-stu-id="83d4e-205">Int32</span></span>|<span data-ttu-id="83d4e-206">Порт прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="83d4e-206">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="83d4e-207">проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="83d4e-207">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="83d4e-208">String.</span><span class="sxs-lookup"><span data-stu-id="83d4e-208">String</span></span>|<span data-ttu-id="83d4e-209">URL-адрес скрипта автоматической настройки прокси-сервера при выборе параметра Автоматическая настройка.</span><span class="sxs-lookup"><span data-stu-id="83d4e-209">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="83d4e-210">Обычно это URL-адрес файла PAC (Автонастройка прокси-сервера).</span><span class="sxs-lookup"><span data-stu-id="83d4e-210">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="83d4e-211">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="83d4e-211">preSharedKey</span></span>|<span data-ttu-id="83d4e-212">String.</span><span class="sxs-lookup"><span data-stu-id="83d4e-212">String</span></span>|<span data-ttu-id="83d4e-213">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="83d4e-213">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="83d4e-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="83d4e-214">Response</span></span>
<span data-ttu-id="83d4e-215">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="83d4e-215">If successful, this method returns a `200 OK` response code and an updated [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83d4e-216">Пример</span><span class="sxs-lookup"><span data-stu-id="83d4e-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="83d4e-217">Запрос</span><span class="sxs-lookup"><span data-stu-id="83d4e-217">Request</span></span>
<span data-ttu-id="83d4e-218">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83d4e-218">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1448

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="83d4e-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="83d4e-219">Response</span></span>
<span data-ttu-id="83d4e-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83d4e-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1620

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
  "id": "516f9ef9-9ef9-516f-f99e-6f51f99e6f51",
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




