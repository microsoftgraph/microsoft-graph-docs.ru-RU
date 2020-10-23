---
title: Обновление Андроидвификонфигуратион
description: Обновление свойств объекта Андроидвификонфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5ec7f7844218f7a237e0c0ffc881e9f2a28ea315
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707523"
---
# <a name="update-androidwificonfiguration"></a><span data-ttu-id="90b8b-103">Обновление Андроидвификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="90b8b-103">Update androidWiFiConfiguration</span></span>

<span data-ttu-id="90b8b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90b8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90b8b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90b8b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90b8b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90b8b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90b8b-107">Обновление свойств объекта [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="90b8b-107">Update the properties of a [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90b8b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="90b8b-108">Prerequisites</span></span>
<span data-ttu-id="90b8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90b8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90b8b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90b8b-111">Permission type</span></span>|<span data-ttu-id="90b8b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="90b8b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90b8b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90b8b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90b8b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90b8b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="90b8b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90b8b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90b8b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90b8b-116">Not supported.</span></span>|
|<span data-ttu-id="90b8b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90b8b-117">Application</span></span>|<span data-ttu-id="90b8b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90b8b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90b8b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90b8b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="90b8b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="90b8b-120">Request headers</span></span>
|<span data-ttu-id="90b8b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90b8b-121">Header</span></span>|<span data-ttu-id="90b8b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="90b8b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90b8b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90b8b-123">Authorization</span></span>|<span data-ttu-id="90b8b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90b8b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90b8b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="90b8b-125">Accept</span></span>|<span data-ttu-id="90b8b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90b8b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90b8b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="90b8b-127">Request body</span></span>
<span data-ttu-id="90b8b-128">В тексте запроса добавьте представление объекта [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90b8b-128">In the request body, supply a JSON representation for the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

<span data-ttu-id="90b8b-129">В следующей таблице приведены свойства, необходимые при создании [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90b8b-129">The following table shows the properties that are required when you create the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span>

|<span data-ttu-id="90b8b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="90b8b-130">Property</span></span>|<span data-ttu-id="90b8b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="90b8b-131">Type</span></span>|<span data-ttu-id="90b8b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="90b8b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90b8b-133">id</span><span class="sxs-lookup"><span data-stu-id="90b8b-133">id</span></span>|<span data-ttu-id="90b8b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="90b8b-134">String</span></span>|<span data-ttu-id="90b8b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="90b8b-135">Key of the entity.</span></span> <span data-ttu-id="90b8b-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90b8b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90b8b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90b8b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="90b8b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90b8b-138">DateTimeOffset</span></span>|<span data-ttu-id="90b8b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="90b8b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="90b8b-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90b8b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90b8b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="90b8b-141">roleScopeTagIds</span></span>|<span data-ttu-id="90b8b-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="90b8b-142">String collection</span></span>|<span data-ttu-id="90b8b-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="90b8b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="90b8b-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90b8b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90b8b-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="90b8b-145">supportsScopeTags</span></span>|<span data-ttu-id="90b8b-146">Логический</span><span class="sxs-lookup"><span data-stu-id="90b8b-146">Boolean</span></span>|<span data-ttu-id="90b8b-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="90b8b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="90b8b-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="90b8b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="90b8b-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="90b8b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="90b8b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="90b8b-150">This property is read-only.</span></span> <span data-ttu-id="90b8b-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90b8b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90b8b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="90b8b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="90b8b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="90b8b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="90b8b-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="90b8b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="90b8b-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90b8b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90b8b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="90b8b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="90b8b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="90b8b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="90b8b-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="90b8b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="90b8b-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90b8b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90b8b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="90b8b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="90b8b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="90b8b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="90b8b-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="90b8b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="90b8b-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90b8b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90b8b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90b8b-164">createdDateTime</span></span>|<span data-ttu-id="90b8b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90b8b-165">DateTimeOffset</span></span>|<span data-ttu-id="90b8b-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="90b8b-166">DateTime the object was created.</span></span> <span data-ttu-id="90b8b-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90b8b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90b8b-168">description</span><span class="sxs-lookup"><span data-stu-id="90b8b-168">description</span></span>|<span data-ttu-id="90b8b-169">Строка</span><span class="sxs-lookup"><span data-stu-id="90b8b-169">String</span></span>|<span data-ttu-id="90b8b-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="90b8b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="90b8b-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90b8b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90b8b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="90b8b-172">displayName</span></span>|<span data-ttu-id="90b8b-173">Строка</span><span class="sxs-lookup"><span data-stu-id="90b8b-173">String</span></span>|<span data-ttu-id="90b8b-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="90b8b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="90b8b-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90b8b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90b8b-176">version</span><span class="sxs-lookup"><span data-stu-id="90b8b-176">version</span></span>|<span data-ttu-id="90b8b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="90b8b-177">Int32</span></span>|<span data-ttu-id="90b8b-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="90b8b-178">Version of the device configuration.</span></span> <span data-ttu-id="90b8b-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="90b8b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="90b8b-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="90b8b-180">networkName</span></span>|<span data-ttu-id="90b8b-181">Строка</span><span class="sxs-lookup"><span data-stu-id="90b8b-181">String</span></span>|<span data-ttu-id="90b8b-182">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="90b8b-182">Network Name</span></span>|
|<span data-ttu-id="90b8b-183">SSID</span><span class="sxs-lookup"><span data-stu-id="90b8b-183">ssid</span></span>|<span data-ttu-id="90b8b-184">Строка</span><span class="sxs-lookup"><span data-stu-id="90b8b-184">String</span></span>|<span data-ttu-id="90b8b-185">Это имя Wi-Fiной сети, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="90b8b-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="90b8b-186">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="90b8b-186">connectAutomatically</span></span>|<span data-ttu-id="90b8b-187">Логический</span><span class="sxs-lookup"><span data-stu-id="90b8b-187">Boolean</span></span>|<span data-ttu-id="90b8b-188">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="90b8b-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="90b8b-189">Если задать для этого параметра значение true, запрос пользователя будет пропущен и устройство будет автоматически подключено к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="90b8b-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="90b8b-190">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="90b8b-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="90b8b-191">Логический</span><span class="sxs-lookup"><span data-stu-id="90b8b-191">Boolean</span></span>|<span data-ttu-id="90b8b-192">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="90b8b-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="90b8b-193">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="90b8b-193">wiFiSecurityType</span></span>|[<span data-ttu-id="90b8b-194">андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="90b8b-194">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="90b8b-195">Указывает, использует ли конечная точка Wi-Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="90b8b-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="90b8b-196">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="90b8b-196">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="90b8b-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="90b8b-197">Response</span></span>
<span data-ttu-id="90b8b-198">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидвификонфигуратион](../resources/intune-deviceconfig-androidwificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90b8b-198">If successful, this method returns a `200 OK` response code and an updated [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90b8b-199">Пример</span><span class="sxs-lookup"><span data-stu-id="90b8b-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="90b8b-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="90b8b-200">Request</span></span>
<span data-ttu-id="90b8b-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90b8b-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="90b8b-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="90b8b-202">Response</span></span>
<span data-ttu-id="90b8b-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90b8b-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





