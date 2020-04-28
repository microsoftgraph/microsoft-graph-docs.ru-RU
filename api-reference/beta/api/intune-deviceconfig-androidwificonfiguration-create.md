---
title: Создание Андроидвификонфигуратион
description: Создание нового объекта Андроидвификонфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b9a7641d21e6ea73dae4b23522acbbd2d04bd8f0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43435432"
---
# <a name="create-androidwificonfiguration"></a><span data-ttu-id="32bdc-103">Создание Андроидвификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="32bdc-103">Create androidWiFiConfiguration</span></span>

<span data-ttu-id="32bdc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32bdc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32bdc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32bdc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32bdc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32bdc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32bdc-107">Создание нового объекта [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="32bdc-107">Create a new [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32bdc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="32bdc-108">Prerequisites</span></span>
<span data-ttu-id="32bdc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32bdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32bdc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32bdc-111">Permission type</span></span>|<span data-ttu-id="32bdc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32bdc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32bdc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32bdc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32bdc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32bdc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="32bdc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32bdc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32bdc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32bdc-116">Not supported.</span></span>|
|<span data-ttu-id="32bdc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32bdc-117">Application</span></span>|<span data-ttu-id="32bdc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32bdc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32bdc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32bdc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="32bdc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="32bdc-120">Request headers</span></span>
|<span data-ttu-id="32bdc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32bdc-121">Header</span></span>|<span data-ttu-id="32bdc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="32bdc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32bdc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32bdc-123">Authorization</span></span>|<span data-ttu-id="32bdc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32bdc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32bdc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="32bdc-125">Accept</span></span>|<span data-ttu-id="32bdc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32bdc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32bdc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="32bdc-127">Request body</span></span>
<span data-ttu-id="32bdc-128">В тексте запроса добавьте представление объекта Андроидвификонфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32bdc-128">In the request body, supply a JSON representation for the androidWiFiConfiguration object.</span></span>

<span data-ttu-id="32bdc-129">В следующей таблице приведены свойства, необходимые при создании Андроидвификонфигуратион.</span><span class="sxs-lookup"><span data-stu-id="32bdc-129">The following table shows the properties that are required when you create the androidWiFiConfiguration.</span></span>

|<span data-ttu-id="32bdc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="32bdc-130">Property</span></span>|<span data-ttu-id="32bdc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="32bdc-131">Type</span></span>|<span data-ttu-id="32bdc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="32bdc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32bdc-133">id</span><span class="sxs-lookup"><span data-stu-id="32bdc-133">id</span></span>|<span data-ttu-id="32bdc-134">String</span><span class="sxs-lookup"><span data-stu-id="32bdc-134">String</span></span>|<span data-ttu-id="32bdc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="32bdc-135">Key of the entity.</span></span> <span data-ttu-id="32bdc-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32bdc-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32bdc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32bdc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="32bdc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32bdc-138">DateTimeOffset</span></span>|<span data-ttu-id="32bdc-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="32bdc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="32bdc-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32bdc-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32bdc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="32bdc-141">roleScopeTagIds</span></span>|<span data-ttu-id="32bdc-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="32bdc-142">String collection</span></span>|<span data-ttu-id="32bdc-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="32bdc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="32bdc-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32bdc-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32bdc-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="32bdc-145">supportsScopeTags</span></span>|<span data-ttu-id="32bdc-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="32bdc-146">Boolean</span></span>|<span data-ttu-id="32bdc-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="32bdc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="32bdc-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="32bdc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="32bdc-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="32bdc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="32bdc-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="32bdc-150">This property is read-only.</span></span> <span data-ttu-id="32bdc-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32bdc-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32bdc-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="32bdc-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="32bdc-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="32bdc-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="32bdc-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="32bdc-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="32bdc-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32bdc-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32bdc-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="32bdc-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="32bdc-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="32bdc-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="32bdc-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="32bdc-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="32bdc-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32bdc-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32bdc-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="32bdc-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="32bdc-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="32bdc-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="32bdc-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="32bdc-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="32bdc-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32bdc-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32bdc-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32bdc-164">createdDateTime</span></span>|<span data-ttu-id="32bdc-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32bdc-165">DateTimeOffset</span></span>|<span data-ttu-id="32bdc-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="32bdc-166">DateTime the object was created.</span></span> <span data-ttu-id="32bdc-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32bdc-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32bdc-168">description</span><span class="sxs-lookup"><span data-stu-id="32bdc-168">description</span></span>|<span data-ttu-id="32bdc-169">String</span><span class="sxs-lookup"><span data-stu-id="32bdc-169">String</span></span>|<span data-ttu-id="32bdc-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="32bdc-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="32bdc-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32bdc-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32bdc-172">displayName</span><span class="sxs-lookup"><span data-stu-id="32bdc-172">displayName</span></span>|<span data-ttu-id="32bdc-173">Строка</span><span class="sxs-lookup"><span data-stu-id="32bdc-173">String</span></span>|<span data-ttu-id="32bdc-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="32bdc-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="32bdc-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32bdc-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32bdc-176">version</span><span class="sxs-lookup"><span data-stu-id="32bdc-176">version</span></span>|<span data-ttu-id="32bdc-177">Int32</span><span class="sxs-lookup"><span data-stu-id="32bdc-177">Int32</span></span>|<span data-ttu-id="32bdc-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="32bdc-178">Version of the device configuration.</span></span> <span data-ttu-id="32bdc-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="32bdc-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32bdc-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="32bdc-180">networkName</span></span>|<span data-ttu-id="32bdc-181">String</span><span class="sxs-lookup"><span data-stu-id="32bdc-181">String</span></span>|<span data-ttu-id="32bdc-182">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="32bdc-182">Network Name</span></span>|
|<span data-ttu-id="32bdc-183">SSID</span><span class="sxs-lookup"><span data-stu-id="32bdc-183">ssid</span></span>|<span data-ttu-id="32bdc-184">String</span><span class="sxs-lookup"><span data-stu-id="32bdc-184">String</span></span>|<span data-ttu-id="32bdc-185">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="32bdc-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="32bdc-186">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="32bdc-186">connectAutomatically</span></span>|<span data-ttu-id="32bdc-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="32bdc-187">Boolean</span></span>|<span data-ttu-id="32bdc-188">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="32bdc-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="32bdc-189">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="32bdc-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="32bdc-190">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="32bdc-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="32bdc-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="32bdc-191">Boolean</span></span>|<span data-ttu-id="32bdc-192">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="32bdc-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="32bdc-193">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="32bdc-193">wiFiSecurityType</span></span>|[<span data-ttu-id="32bdc-194">андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="32bdc-194">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="32bdc-195">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="32bdc-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="32bdc-196">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="32bdc-196">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="32bdc-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="32bdc-197">Response</span></span>
<span data-ttu-id="32bdc-198">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="32bdc-198">If successful, this method returns a `201 Created` response code and a [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32bdc-199">Пример</span><span class="sxs-lookup"><span data-stu-id="32bdc-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="32bdc-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="32bdc-200">Request</span></span>
<span data-ttu-id="32bdc-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32bdc-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="32bdc-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="32bdc-202">Response</span></span>
<span data-ttu-id="32bdc-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32bdc-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



