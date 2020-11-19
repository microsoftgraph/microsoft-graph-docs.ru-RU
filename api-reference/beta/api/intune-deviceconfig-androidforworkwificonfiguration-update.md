---
title: Обновление Андроидфорворквификонфигуратион
description: Обновление свойств объекта Андроидфорворквификонфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f36798000267afe938eb5122b7268dd361a3f030
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49237837"
---
# <a name="update-androidforworkwificonfiguration"></a><span data-ttu-id="dca57-103">Обновление Андроидфорворквификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="dca57-103">Update androidForWorkWiFiConfiguration</span></span>

<span data-ttu-id="dca57-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dca57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dca57-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dca57-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dca57-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dca57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dca57-107">Обновление свойств объекта [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="dca57-107">Update the properties of a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dca57-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dca57-108">Prerequisites</span></span>
<span data-ttu-id="dca57-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dca57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dca57-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dca57-111">Permission type</span></span>|<span data-ttu-id="dca57-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dca57-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dca57-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dca57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dca57-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dca57-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dca57-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dca57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dca57-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dca57-116">Not supported.</span></span>|
|<span data-ttu-id="dca57-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="dca57-117">Application</span></span>|<span data-ttu-id="dca57-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dca57-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dca57-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dca57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="dca57-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dca57-120">Request headers</span></span>
|<span data-ttu-id="dca57-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dca57-121">Header</span></span>|<span data-ttu-id="dca57-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dca57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dca57-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dca57-123">Authorization</span></span>|<span data-ttu-id="dca57-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dca57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dca57-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dca57-125">Accept</span></span>|<span data-ttu-id="dca57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dca57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dca57-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dca57-127">Request body</span></span>
<span data-ttu-id="dca57-128">В тексте запроса добавьте представление объекта [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dca57-128">In the request body, supply a JSON representation for the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

<span data-ttu-id="dca57-129">В следующей таблице приведены свойства, необходимые при создании [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca57-129">The following table shows the properties that are required when you create the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span>

|<span data-ttu-id="dca57-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dca57-130">Property</span></span>|<span data-ttu-id="dca57-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dca57-131">Type</span></span>|<span data-ttu-id="dca57-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dca57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dca57-133">id</span><span class="sxs-lookup"><span data-stu-id="dca57-133">id</span></span>|<span data-ttu-id="dca57-134">String</span><span class="sxs-lookup"><span data-stu-id="dca57-134">String</span></span>|<span data-ttu-id="dca57-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dca57-135">Key of the entity.</span></span> <span data-ttu-id="dca57-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca57-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dca57-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dca57-137">lastModifiedDateTime</span></span>|<span data-ttu-id="dca57-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dca57-138">DateTimeOffset</span></span>|<span data-ttu-id="dca57-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="dca57-139">DateTime the object was last modified.</span></span> <span data-ttu-id="dca57-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca57-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dca57-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dca57-141">roleScopeTagIds</span></span>|<span data-ttu-id="dca57-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="dca57-142">String collection</span></span>|<span data-ttu-id="dca57-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="dca57-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dca57-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca57-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dca57-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="dca57-145">supportsScopeTags</span></span>|<span data-ttu-id="dca57-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca57-146">Boolean</span></span>|<span data-ttu-id="dca57-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="dca57-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="dca57-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="dca57-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="dca57-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="dca57-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="dca57-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dca57-150">This property is read-only.</span></span> <span data-ttu-id="dca57-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca57-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dca57-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="dca57-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="dca57-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="dca57-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="dca57-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="dca57-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="dca57-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca57-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dca57-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="dca57-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="dca57-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="dca57-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="dca57-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="dca57-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="dca57-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca57-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dca57-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="dca57-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="dca57-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="dca57-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="dca57-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="dca57-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="dca57-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca57-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dca57-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dca57-164">createdDateTime</span></span>|<span data-ttu-id="dca57-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dca57-165">DateTimeOffset</span></span>|<span data-ttu-id="dca57-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="dca57-166">DateTime the object was created.</span></span> <span data-ttu-id="dca57-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca57-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dca57-168">description</span><span class="sxs-lookup"><span data-stu-id="dca57-168">description</span></span>|<span data-ttu-id="dca57-169">String</span><span class="sxs-lookup"><span data-stu-id="dca57-169">String</span></span>|<span data-ttu-id="dca57-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dca57-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dca57-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca57-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dca57-172">displayName</span><span class="sxs-lookup"><span data-stu-id="dca57-172">displayName</span></span>|<span data-ttu-id="dca57-173">String</span><span class="sxs-lookup"><span data-stu-id="dca57-173">String</span></span>|<span data-ttu-id="dca57-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dca57-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dca57-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca57-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dca57-176">version</span><span class="sxs-lookup"><span data-stu-id="dca57-176">version</span></span>|<span data-ttu-id="dca57-177">Int32</span><span class="sxs-lookup"><span data-stu-id="dca57-177">Int32</span></span>|<span data-ttu-id="dca57-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dca57-178">Version of the device configuration.</span></span> <span data-ttu-id="dca57-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca57-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dca57-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="dca57-180">networkName</span></span>|<span data-ttu-id="dca57-181">String</span><span class="sxs-lookup"><span data-stu-id="dca57-181">String</span></span>|<span data-ttu-id="dca57-182">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="dca57-182">Network Name</span></span>|
|<span data-ttu-id="dca57-183">SSID</span><span class="sxs-lookup"><span data-stu-id="dca57-183">ssid</span></span>|<span data-ttu-id="dca57-184">String</span><span class="sxs-lookup"><span data-stu-id="dca57-184">String</span></span>|<span data-ttu-id="dca57-185">Это имя Wi-Fiной сети, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="dca57-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="dca57-186">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="dca57-186">connectAutomatically</span></span>|<span data-ttu-id="dca57-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca57-187">Boolean</span></span>|<span data-ttu-id="dca57-188">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="dca57-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="dca57-189">Если задать для этого параметра значение true, запрос пользователя будет пропущен и устройство будет автоматически подключено к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="dca57-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="dca57-190">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="dca57-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="dca57-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca57-191">Boolean</span></span>|<span data-ttu-id="dca57-192">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="dca57-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="dca57-193">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="dca57-193">wiFiSecurityType</span></span>|[<span data-ttu-id="dca57-194">андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="dca57-194">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="dca57-195">Указывает, использует ли конечная точка Wi-Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="dca57-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="dca57-196">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="dca57-196">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="dca57-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="dca57-197">Response</span></span>
<span data-ttu-id="dca57-198">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dca57-198">If successful, this method returns a `200 OK` response code and an updated [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dca57-199">Пример</span><span class="sxs-lookup"><span data-stu-id="dca57-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="dca57-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="dca57-200">Request</span></span>
<span data-ttu-id="dca57-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dca57-201">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1215

{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="dca57-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="dca57-202">Response</span></span>
<span data-ttu-id="dca57-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dca57-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1387

{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
  "id": "58bcfe05-fe05-58bc-05fe-bc5805febc58",
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




