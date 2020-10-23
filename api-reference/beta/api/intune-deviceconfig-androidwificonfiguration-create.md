---
title: Создание Андроидвификонфигуратион
description: Создание нового объекта Андроидвификонфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3acaa21e2369c428ccb114e56f0d74df10774f23
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698934"
---
# <a name="create-androidwificonfiguration"></a><span data-ttu-id="4eb27-103">Создание Андроидвификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="4eb27-103">Create androidWiFiConfiguration</span></span>

<span data-ttu-id="4eb27-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4eb27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4eb27-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eb27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4eb27-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4eb27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4eb27-107">Создание нового объекта [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4eb27-107">Create a new [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4eb27-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4eb27-108">Prerequisites</span></span>
<span data-ttu-id="4eb27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4eb27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4eb27-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4eb27-111">Permission type</span></span>|<span data-ttu-id="4eb27-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4eb27-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4eb27-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4eb27-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4eb27-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4eb27-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4eb27-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4eb27-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4eb27-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eb27-116">Not supported.</span></span>|
|<span data-ttu-id="4eb27-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4eb27-117">Application</span></span>|<span data-ttu-id="4eb27-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4eb27-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4eb27-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4eb27-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4eb27-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4eb27-120">Request headers</span></span>
|<span data-ttu-id="4eb27-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4eb27-121">Header</span></span>|<span data-ttu-id="4eb27-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4eb27-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4eb27-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4eb27-123">Authorization</span></span>|<span data-ttu-id="4eb27-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4eb27-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4eb27-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4eb27-125">Accept</span></span>|<span data-ttu-id="4eb27-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4eb27-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4eb27-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4eb27-127">Request body</span></span>
<span data-ttu-id="4eb27-128">В тексте запроса добавьте представление объекта Андроидвификонфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4eb27-128">In the request body, supply a JSON representation for the androidWiFiConfiguration object.</span></span>

<span data-ttu-id="4eb27-129">В следующей таблице приведены свойства, необходимые при создании Андроидвификонфигуратион.</span><span class="sxs-lookup"><span data-stu-id="4eb27-129">The following table shows the properties that are required when you create the androidWiFiConfiguration.</span></span>

|<span data-ttu-id="4eb27-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4eb27-130">Property</span></span>|<span data-ttu-id="4eb27-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4eb27-131">Type</span></span>|<span data-ttu-id="4eb27-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4eb27-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4eb27-133">id</span><span class="sxs-lookup"><span data-stu-id="4eb27-133">id</span></span>|<span data-ttu-id="4eb27-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4eb27-134">String</span></span>|<span data-ttu-id="4eb27-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4eb27-135">Key of the entity.</span></span> <span data-ttu-id="4eb27-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4eb27-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eb27-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4eb27-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4eb27-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eb27-138">DateTimeOffset</span></span>|<span data-ttu-id="4eb27-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4eb27-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4eb27-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4eb27-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eb27-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4eb27-141">roleScopeTagIds</span></span>|<span data-ttu-id="4eb27-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4eb27-142">String collection</span></span>|<span data-ttu-id="4eb27-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4eb27-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4eb27-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4eb27-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eb27-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4eb27-145">supportsScopeTags</span></span>|<span data-ttu-id="4eb27-146">Логический</span><span class="sxs-lookup"><span data-stu-id="4eb27-146">Boolean</span></span>|<span data-ttu-id="4eb27-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4eb27-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4eb27-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4eb27-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4eb27-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4eb27-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4eb27-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4eb27-150">This property is read-only.</span></span> <span data-ttu-id="4eb27-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4eb27-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eb27-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4eb27-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4eb27-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4eb27-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4eb27-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4eb27-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4eb27-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4eb27-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eb27-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4eb27-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4eb27-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4eb27-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4eb27-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4eb27-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4eb27-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4eb27-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eb27-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4eb27-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4eb27-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4eb27-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4eb27-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4eb27-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4eb27-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4eb27-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eb27-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4eb27-164">createdDateTime</span></span>|<span data-ttu-id="4eb27-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eb27-165">DateTimeOffset</span></span>|<span data-ttu-id="4eb27-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4eb27-166">DateTime the object was created.</span></span> <span data-ttu-id="4eb27-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4eb27-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eb27-168">description</span><span class="sxs-lookup"><span data-stu-id="4eb27-168">description</span></span>|<span data-ttu-id="4eb27-169">Строка</span><span class="sxs-lookup"><span data-stu-id="4eb27-169">String</span></span>|<span data-ttu-id="4eb27-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4eb27-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4eb27-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4eb27-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eb27-172">displayName</span><span class="sxs-lookup"><span data-stu-id="4eb27-172">displayName</span></span>|<span data-ttu-id="4eb27-173">Строка</span><span class="sxs-lookup"><span data-stu-id="4eb27-173">String</span></span>|<span data-ttu-id="4eb27-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4eb27-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4eb27-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4eb27-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eb27-176">version</span><span class="sxs-lookup"><span data-stu-id="4eb27-176">version</span></span>|<span data-ttu-id="4eb27-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4eb27-177">Int32</span></span>|<span data-ttu-id="4eb27-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4eb27-178">Version of the device configuration.</span></span> <span data-ttu-id="4eb27-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4eb27-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eb27-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="4eb27-180">networkName</span></span>|<span data-ttu-id="4eb27-181">Строка</span><span class="sxs-lookup"><span data-stu-id="4eb27-181">String</span></span>|<span data-ttu-id="4eb27-182">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="4eb27-182">Network Name</span></span>|
|<span data-ttu-id="4eb27-183">SSID</span><span class="sxs-lookup"><span data-stu-id="4eb27-183">ssid</span></span>|<span data-ttu-id="4eb27-184">Строка</span><span class="sxs-lookup"><span data-stu-id="4eb27-184">String</span></span>|<span data-ttu-id="4eb27-185">Это имя Wi-Fiной сети, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="4eb27-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="4eb27-186">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="4eb27-186">connectAutomatically</span></span>|<span data-ttu-id="4eb27-187">Логический</span><span class="sxs-lookup"><span data-stu-id="4eb27-187">Boolean</span></span>|<span data-ttu-id="4eb27-188">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="4eb27-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="4eb27-189">Если задать для этого параметра значение true, запрос пользователя будет пропущен и устройство будет автоматически подключено к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="4eb27-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="4eb27-190">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="4eb27-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="4eb27-191">Логический</span><span class="sxs-lookup"><span data-stu-id="4eb27-191">Boolean</span></span>|<span data-ttu-id="4eb27-192">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="4eb27-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="4eb27-193">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="4eb27-193">wiFiSecurityType</span></span>|[<span data-ttu-id="4eb27-194">андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="4eb27-194">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="4eb27-195">Указывает, использует ли конечная точка Wi-Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="4eb27-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="4eb27-196">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="4eb27-196">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="4eb27-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="4eb27-197">Response</span></span>
<span data-ttu-id="4eb27-198">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4eb27-198">If successful, this method returns a `201 Created` response code and a [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4eb27-199">Пример</span><span class="sxs-lookup"><span data-stu-id="4eb27-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="4eb27-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="4eb27-200">Request</span></span>
<span data-ttu-id="4eb27-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4eb27-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4eb27-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="4eb27-202">Response</span></span>
<span data-ttu-id="4eb27-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4eb27-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





