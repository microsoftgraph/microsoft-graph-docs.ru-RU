---
title: Создание Андроидворкпрофилевификонфигуратион
description: Создание нового объекта Андроидворкпрофилевификонфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a4f3f4a85687fed65c92148f62e57a7c1ad4ff8d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36340536"
---
# <a name="create-androidworkprofilewificonfiguration"></a><span data-ttu-id="ea38c-103">Создание Андроидворкпрофилевификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="ea38c-103">Create androidWorkProfileWiFiConfiguration</span></span>

> <span data-ttu-id="ea38c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea38c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea38c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea38c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea38c-106">Создание нового объекта [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ea38c-106">Create a new [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea38c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ea38c-107">Prerequisites</span></span>
<span data-ttu-id="ea38c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea38c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea38c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea38c-110">Permission type</span></span>|<span data-ttu-id="ea38c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea38c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea38c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea38c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ea38c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea38c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ea38c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea38c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea38c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea38c-115">Not supported.</span></span>|
|<span data-ttu-id="ea38c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea38c-116">Application</span></span>|<span data-ttu-id="ea38c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea38c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea38c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea38c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ea38c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea38c-119">Request headers</span></span>
|<span data-ttu-id="ea38c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea38c-120">Header</span></span>|<span data-ttu-id="ea38c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ea38c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea38c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea38c-122">Authorization</span></span>|<span data-ttu-id="ea38c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea38c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea38c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ea38c-124">Accept</span></span>|<span data-ttu-id="ea38c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ea38c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea38c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ea38c-126">Request body</span></span>
<span data-ttu-id="ea38c-127">В тексте запроса добавьте представление объекта Андроидворкпрофилевификонфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea38c-127">In the request body, supply a JSON representation for the androidWorkProfileWiFiConfiguration object.</span></span>

<span data-ttu-id="ea38c-128">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилевификонфигуратион.</span><span class="sxs-lookup"><span data-stu-id="ea38c-128">The following table shows the properties that are required when you create the androidWorkProfileWiFiConfiguration.</span></span>

|<span data-ttu-id="ea38c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea38c-129">Property</span></span>|<span data-ttu-id="ea38c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ea38c-130">Type</span></span>|<span data-ttu-id="ea38c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ea38c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea38c-132">id</span><span class="sxs-lookup"><span data-stu-id="ea38c-132">id</span></span>|<span data-ttu-id="ea38c-133">String</span><span class="sxs-lookup"><span data-stu-id="ea38c-133">String</span></span>|<span data-ttu-id="ea38c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ea38c-134">Key of the entity.</span></span> <span data-ttu-id="ea38c-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea38c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea38c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea38c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ea38c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea38c-137">DateTimeOffset</span></span>|<span data-ttu-id="ea38c-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ea38c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ea38c-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea38c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea38c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ea38c-140">roleScopeTagIds</span></span>|<span data-ttu-id="ea38c-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ea38c-141">String collection</span></span>|<span data-ttu-id="ea38c-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ea38c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ea38c-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea38c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea38c-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="ea38c-144">supportsScopeTags</span></span>|<span data-ttu-id="ea38c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea38c-145">Boolean</span></span>|<span data-ttu-id="ea38c-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ea38c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ea38c-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="ea38c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ea38c-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ea38c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ea38c-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ea38c-149">This property is read-only.</span></span> <span data-ttu-id="ea38c-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea38c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea38c-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ea38c-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ea38c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ea38c-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ea38c-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ea38c-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ea38c-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea38c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea38c-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ea38c-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ea38c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ea38c-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ea38c-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ea38c-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ea38c-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea38c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea38c-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="ea38c-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ea38c-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="ea38c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ea38c-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ea38c-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ea38c-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea38c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea38c-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea38c-163">createdDateTime</span></span>|<span data-ttu-id="ea38c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea38c-164">DateTimeOffset</span></span>|<span data-ttu-id="ea38c-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ea38c-165">DateTime the object was created.</span></span> <span data-ttu-id="ea38c-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea38c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea38c-167">description</span><span class="sxs-lookup"><span data-stu-id="ea38c-167">description</span></span>|<span data-ttu-id="ea38c-168">String</span><span class="sxs-lookup"><span data-stu-id="ea38c-168">String</span></span>|<span data-ttu-id="ea38c-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ea38c-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ea38c-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea38c-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea38c-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ea38c-171">displayName</span></span>|<span data-ttu-id="ea38c-172">Строка</span><span class="sxs-lookup"><span data-stu-id="ea38c-172">String</span></span>|<span data-ttu-id="ea38c-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ea38c-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ea38c-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea38c-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea38c-175">version</span><span class="sxs-lookup"><span data-stu-id="ea38c-175">version</span></span>|<span data-ttu-id="ea38c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ea38c-176">Int32</span></span>|<span data-ttu-id="ea38c-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ea38c-177">Version of the device configuration.</span></span> <span data-ttu-id="ea38c-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea38c-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea38c-179">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="ea38c-179">networkName</span></span>|<span data-ttu-id="ea38c-180">String</span><span class="sxs-lookup"><span data-stu-id="ea38c-180">String</span></span>|<span data-ttu-id="ea38c-181">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="ea38c-181">Network Name</span></span>|
|<span data-ttu-id="ea38c-182">SSID</span><span class="sxs-lookup"><span data-stu-id="ea38c-182">ssid</span></span>|<span data-ttu-id="ea38c-183">String</span><span class="sxs-lookup"><span data-stu-id="ea38c-183">String</span></span>|<span data-ttu-id="ea38c-184">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="ea38c-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="ea38c-185">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="ea38c-185">connectAutomatically</span></span>|<span data-ttu-id="ea38c-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea38c-186">Boolean</span></span>|<span data-ttu-id="ea38c-187">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="ea38c-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="ea38c-188">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="ea38c-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="ea38c-189">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="ea38c-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="ea38c-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea38c-190">Boolean</span></span>|<span data-ttu-id="ea38c-191">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="ea38c-191">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="ea38c-192">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="ea38c-192">wiFiSecurityType</span></span>|[<span data-ttu-id="ea38c-193">андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="ea38c-193">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="ea38c-194">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="ea38c-194">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="ea38c-195">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="ea38c-195">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="ea38c-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea38c-196">Response</span></span>
<span data-ttu-id="ea38c-197">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea38c-197">If successful, this method returns a `201 Created` response code and a [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea38c-198">Пример</span><span class="sxs-lookup"><span data-stu-id="ea38c-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea38c-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea38c-199">Request</span></span>
<span data-ttu-id="ea38c-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea38c-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="ea38c-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea38c-201">Response</span></span>
<span data-ttu-id="ea38c-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea38c-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






