---
title: Обновление Андроидворкпрофилевификонфигуратион
description: Обновление свойств объекта Андроидворкпрофилевификонфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 780081295ee85acd1207d62babe95bad222f3f01
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534227"
---
# <a name="update-androidworkprofilewificonfiguration"></a><span data-ttu-id="8bc37-103">Обновление Андроидворкпрофилевификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="8bc37-103">Update androidWorkProfileWiFiConfiguration</span></span>

> <span data-ttu-id="8bc37-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bc37-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bc37-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8bc37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bc37-106">Обновление свойств объекта [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8bc37-106">Update the properties of a [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bc37-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8bc37-107">Prerequisites</span></span>
<span data-ttu-id="8bc37-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bc37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bc37-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bc37-110">Permission type</span></span>|<span data-ttu-id="8bc37-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bc37-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bc37-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bc37-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8bc37-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bc37-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8bc37-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bc37-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bc37-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bc37-115">Not supported.</span></span>|
|<span data-ttu-id="8bc37-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8bc37-116">Application</span></span>|<span data-ttu-id="8bc37-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bc37-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bc37-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bc37-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8bc37-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8bc37-119">Request headers</span></span>
|<span data-ttu-id="8bc37-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8bc37-120">Header</span></span>|<span data-ttu-id="8bc37-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8bc37-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bc37-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8bc37-122">Authorization</span></span>|<span data-ttu-id="8bc37-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bc37-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bc37-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8bc37-124">Accept</span></span>|<span data-ttu-id="8bc37-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8bc37-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bc37-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8bc37-126">Request body</span></span>
<span data-ttu-id="8bc37-127">В тексте запроса добавьте представление объекта [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bc37-127">In the request body, supply a JSON representation for the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>

<span data-ttu-id="8bc37-128">В следующей таблице приведены свойства, необходимые при создании [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bc37-128">The following table shows the properties that are required when you create the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span>

|<span data-ttu-id="8bc37-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bc37-129">Property</span></span>|<span data-ttu-id="8bc37-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8bc37-130">Type</span></span>|<span data-ttu-id="8bc37-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8bc37-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bc37-132">id</span><span class="sxs-lookup"><span data-stu-id="8bc37-132">id</span></span>|<span data-ttu-id="8bc37-133">String</span><span class="sxs-lookup"><span data-stu-id="8bc37-133">String</span></span>|<span data-ttu-id="8bc37-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8bc37-134">Key of the entity.</span></span> <span data-ttu-id="8bc37-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bc37-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc37-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bc37-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8bc37-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bc37-137">DateTimeOffset</span></span>|<span data-ttu-id="8bc37-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8bc37-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8bc37-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bc37-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc37-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8bc37-140">roleScopeTagIds</span></span>|<span data-ttu-id="8bc37-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8bc37-141">String collection</span></span>|<span data-ttu-id="8bc37-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8bc37-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8bc37-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bc37-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc37-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="8bc37-144">supportsScopeTags</span></span>|<span data-ttu-id="8bc37-145">Логический</span><span class="sxs-lookup"><span data-stu-id="8bc37-145">Boolean</span></span>|<span data-ttu-id="8bc37-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8bc37-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8bc37-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="8bc37-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8bc37-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8bc37-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8bc37-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8bc37-149">This property is read-only.</span></span> <span data-ttu-id="8bc37-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bc37-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc37-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8bc37-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8bc37-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8bc37-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8bc37-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8bc37-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8bc37-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bc37-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc37-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8bc37-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8bc37-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8bc37-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8bc37-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8bc37-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8bc37-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bc37-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc37-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8bc37-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8bc37-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8bc37-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8bc37-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8bc37-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8bc37-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bc37-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc37-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8bc37-163">createdDateTime</span></span>|<span data-ttu-id="8bc37-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bc37-164">DateTimeOffset</span></span>|<span data-ttu-id="8bc37-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8bc37-165">DateTime the object was created.</span></span> <span data-ttu-id="8bc37-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bc37-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc37-167">description</span><span class="sxs-lookup"><span data-stu-id="8bc37-167">description</span></span>|<span data-ttu-id="8bc37-168">String</span><span class="sxs-lookup"><span data-stu-id="8bc37-168">String</span></span>|<span data-ttu-id="8bc37-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8bc37-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8bc37-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bc37-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc37-171">displayName</span><span class="sxs-lookup"><span data-stu-id="8bc37-171">displayName</span></span>|<span data-ttu-id="8bc37-172">Строка</span><span class="sxs-lookup"><span data-stu-id="8bc37-172">String</span></span>|<span data-ttu-id="8bc37-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8bc37-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8bc37-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bc37-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc37-175">version</span><span class="sxs-lookup"><span data-stu-id="8bc37-175">version</span></span>|<span data-ttu-id="8bc37-176">Int32</span><span class="sxs-lookup"><span data-stu-id="8bc37-176">Int32</span></span>|<span data-ttu-id="8bc37-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8bc37-177">Version of the device configuration.</span></span> <span data-ttu-id="8bc37-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8bc37-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8bc37-179">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="8bc37-179">networkName</span></span>|<span data-ttu-id="8bc37-180">String</span><span class="sxs-lookup"><span data-stu-id="8bc37-180">String</span></span>|<span data-ttu-id="8bc37-181">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="8bc37-181">Network Name</span></span>|
|<span data-ttu-id="8bc37-182">SSID</span><span class="sxs-lookup"><span data-stu-id="8bc37-182">ssid</span></span>|<span data-ttu-id="8bc37-183">String</span><span class="sxs-lookup"><span data-stu-id="8bc37-183">String</span></span>|<span data-ttu-id="8bc37-184">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="8bc37-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="8bc37-185">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="8bc37-185">connectAutomatically</span></span>|<span data-ttu-id="8bc37-186">Логический</span><span class="sxs-lookup"><span data-stu-id="8bc37-186">Boolean</span></span>|<span data-ttu-id="8bc37-187">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="8bc37-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="8bc37-188">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="8bc37-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="8bc37-189">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="8bc37-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="8bc37-190">Логический</span><span class="sxs-lookup"><span data-stu-id="8bc37-190">Boolean</span></span>|<span data-ttu-id="8bc37-191">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="8bc37-191">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="8bc37-192">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="8bc37-192">wiFiSecurityType</span></span>|[<span data-ttu-id="8bc37-193">андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="8bc37-193">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="8bc37-194">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="8bc37-194">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="8bc37-195">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="8bc37-195">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="8bc37-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bc37-196">Response</span></span>
<span data-ttu-id="8bc37-197">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8bc37-197">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bc37-198">Пример</span><span class="sxs-lookup"><span data-stu-id="8bc37-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bc37-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bc37-199">Request</span></span>
<span data-ttu-id="8bc37-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bc37-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1219

{
  "@odata.type": "#microsoft.graph.androidWorkProfileWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="8bc37-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bc37-201">Response</span></span>
<span data-ttu-id="8bc37-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8bc37-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1391

{
  "@odata.type": "#microsoft.graph.androidWorkProfileWiFiConfiguration",
  "id": "8400d131-d131-8400-31d1-008431d10084",
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






