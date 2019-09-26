---
title: Обновление Андроидвификонфигуратион
description: Обновление свойств объекта Андроидвификонфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc9b45a1bebb155a0a8e8f5679226ef72205d9d9
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37176053"
---
# <a name="update-androidwificonfiguration"></a><span data-ttu-id="1a027-103">Обновление Андроидвификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="1a027-103">Update androidWiFiConfiguration</span></span>

> <span data-ttu-id="1a027-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a027-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a027-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a027-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a027-106">Обновление свойств объекта [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1a027-106">Update the properties of a [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a027-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1a027-107">Prerequisites</span></span>
<span data-ttu-id="1a027-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a027-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a027-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a027-110">Permission type</span></span>|<span data-ttu-id="1a027-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a027-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a027-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a027-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1a027-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a027-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1a027-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a027-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a027-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a027-115">Not supported.</span></span>|
|<span data-ttu-id="1a027-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a027-116">Application</span></span>|<span data-ttu-id="1a027-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a027-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a027-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a027-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1a027-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a027-119">Request headers</span></span>
|<span data-ttu-id="1a027-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1a027-120">Header</span></span>|<span data-ttu-id="1a027-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1a027-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a027-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a027-122">Authorization</span></span>|<span data-ttu-id="1a027-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a027-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a027-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1a027-124">Accept</span></span>|<span data-ttu-id="1a027-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1a027-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a027-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1a027-126">Request body</span></span>
<span data-ttu-id="1a027-127">В тексте запроса добавьте представление объекта [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a027-127">In the request body, supply a JSON representation for the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

<span data-ttu-id="1a027-128">В следующей таблице приведены свойства, необходимые при создании [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a027-128">The following table shows the properties that are required when you create the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span>

|<span data-ttu-id="1a027-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a027-129">Property</span></span>|<span data-ttu-id="1a027-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1a027-130">Type</span></span>|<span data-ttu-id="1a027-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1a027-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a027-132">id</span><span class="sxs-lookup"><span data-stu-id="1a027-132">id</span></span>|<span data-ttu-id="1a027-133">String</span><span class="sxs-lookup"><span data-stu-id="1a027-133">String</span></span>|<span data-ttu-id="1a027-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1a027-134">Key of the entity.</span></span> <span data-ttu-id="1a027-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a027-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a027-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a027-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1a027-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a027-137">DateTimeOffset</span></span>|<span data-ttu-id="1a027-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1a027-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1a027-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a027-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a027-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1a027-140">roleScopeTagIds</span></span>|<span data-ttu-id="1a027-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1a027-141">String collection</span></span>|<span data-ttu-id="1a027-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1a027-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1a027-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a027-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a027-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="1a027-144">supportsScopeTags</span></span>|<span data-ttu-id="1a027-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="1a027-145">Boolean</span></span>|<span data-ttu-id="1a027-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1a027-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1a027-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="1a027-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1a027-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1a027-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1a027-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1a027-149">This property is read-only.</span></span> <span data-ttu-id="1a027-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a027-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a027-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1a027-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1a027-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1a027-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1a027-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1a027-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1a027-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a027-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a027-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1a027-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1a027-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1a027-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1a027-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1a027-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1a027-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a027-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a027-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="1a027-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1a027-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="1a027-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1a027-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1a027-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1a027-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a027-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a027-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a027-163">createdDateTime</span></span>|<span data-ttu-id="1a027-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a027-164">DateTimeOffset</span></span>|<span data-ttu-id="1a027-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1a027-165">DateTime the object was created.</span></span> <span data-ttu-id="1a027-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a027-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a027-167">description</span><span class="sxs-lookup"><span data-stu-id="1a027-167">description</span></span>|<span data-ttu-id="1a027-168">String</span><span class="sxs-lookup"><span data-stu-id="1a027-168">String</span></span>|<span data-ttu-id="1a027-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1a027-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1a027-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a027-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a027-171">displayName</span><span class="sxs-lookup"><span data-stu-id="1a027-171">displayName</span></span>|<span data-ttu-id="1a027-172">Строка</span><span class="sxs-lookup"><span data-stu-id="1a027-172">String</span></span>|<span data-ttu-id="1a027-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1a027-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1a027-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a027-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a027-175">version</span><span class="sxs-lookup"><span data-stu-id="1a027-175">version</span></span>|<span data-ttu-id="1a027-176">Int32</span><span class="sxs-lookup"><span data-stu-id="1a027-176">Int32</span></span>|<span data-ttu-id="1a027-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1a027-177">Version of the device configuration.</span></span> <span data-ttu-id="1a027-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a027-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a027-179">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="1a027-179">networkName</span></span>|<span data-ttu-id="1a027-180">String.</span><span class="sxs-lookup"><span data-stu-id="1a027-180">String</span></span>|<span data-ttu-id="1a027-181">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="1a027-181">Network Name</span></span>|
|<span data-ttu-id="1a027-182">SSID</span><span class="sxs-lookup"><span data-stu-id="1a027-182">ssid</span></span>|<span data-ttu-id="1a027-183">String.</span><span class="sxs-lookup"><span data-stu-id="1a027-183">String</span></span>|<span data-ttu-id="1a027-184">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="1a027-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="1a027-185">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="1a027-185">connectAutomatically</span></span>|<span data-ttu-id="1a027-186">Boolean.</span><span class="sxs-lookup"><span data-stu-id="1a027-186">Boolean</span></span>|<span data-ttu-id="1a027-187">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="1a027-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="1a027-188">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="1a027-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="1a027-189">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="1a027-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="1a027-190">Boolean.</span><span class="sxs-lookup"><span data-stu-id="1a027-190">Boolean</span></span>|<span data-ttu-id="1a027-191">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="1a027-191">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="1a027-192">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="1a027-192">wiFiSecurityType</span></span>|[<span data-ttu-id="1a027-193">андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="1a027-193">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="1a027-194">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="1a027-194">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="1a027-195">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="1a027-195">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="1a027-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a027-196">Response</span></span>
<span data-ttu-id="1a027-197">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a027-197">If successful, this method returns a `200 OK` response code and an updated [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a027-198">Пример</span><span class="sxs-lookup"><span data-stu-id="1a027-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a027-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a027-199">Request</span></span>
<span data-ttu-id="1a027-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a027-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1208

{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
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
  "wiFiSecurityType": "wpaEnterprise"
}
```

### <a name="response"></a><span data-ttu-id="1a027-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a027-201">Response</span></span>
<span data-ttu-id="1a027-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a027-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1380

{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
  "id": "51cfd26f-d26f-51cf-6fd2-cf516fd2cf51",
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
  "wiFiSecurityType": "wpaEnterprise"
}
```




