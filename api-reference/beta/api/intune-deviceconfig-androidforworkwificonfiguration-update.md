---
title: Обновление Андроидфорворквификонфигуратион
description: Обновление свойств объекта Андроидфорворквификонфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3b3ea838b9d8596f3d0badd7e9755112db9ac33b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43344718"
---
# <a name="update-androidforworkwificonfiguration"></a><span data-ttu-id="19cd7-103">Обновление Андроидфорворквификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="19cd7-103">Update androidForWorkWiFiConfiguration</span></span>

<span data-ttu-id="19cd7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19cd7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19cd7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19cd7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19cd7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19cd7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19cd7-107">Обновление свойств объекта [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="19cd7-107">Update the properties of a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19cd7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="19cd7-108">Prerequisites</span></span>
<span data-ttu-id="19cd7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19cd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19cd7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19cd7-111">Permission type</span></span>|<span data-ttu-id="19cd7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19cd7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19cd7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19cd7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="19cd7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19cd7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="19cd7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19cd7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19cd7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19cd7-116">Not supported.</span></span>|
|<span data-ttu-id="19cd7-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="19cd7-117">Application</span></span>|<span data-ttu-id="19cd7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19cd7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19cd7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19cd7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="19cd7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="19cd7-120">Request headers</span></span>
|<span data-ttu-id="19cd7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19cd7-121">Header</span></span>|<span data-ttu-id="19cd7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="19cd7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19cd7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19cd7-123">Authorization</span></span>|<span data-ttu-id="19cd7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19cd7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19cd7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="19cd7-125">Accept</span></span>|<span data-ttu-id="19cd7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19cd7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19cd7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19cd7-127">Request body</span></span>
<span data-ttu-id="19cd7-128">В тексте запроса добавьте представление объекта [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19cd7-128">In the request body, supply a JSON representation for the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

<span data-ttu-id="19cd7-129">В следующей таблице приведены свойства, необходимые при создании [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19cd7-129">The following table shows the properties that are required when you create the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span>

|<span data-ttu-id="19cd7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="19cd7-130">Property</span></span>|<span data-ttu-id="19cd7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="19cd7-131">Type</span></span>|<span data-ttu-id="19cd7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="19cd7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19cd7-133">id</span><span class="sxs-lookup"><span data-stu-id="19cd7-133">id</span></span>|<span data-ttu-id="19cd7-134">String</span><span class="sxs-lookup"><span data-stu-id="19cd7-134">String</span></span>|<span data-ttu-id="19cd7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="19cd7-135">Key of the entity.</span></span> <span data-ttu-id="19cd7-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19cd7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19cd7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19cd7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="19cd7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19cd7-138">DateTimeOffset</span></span>|<span data-ttu-id="19cd7-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="19cd7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="19cd7-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19cd7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19cd7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="19cd7-141">roleScopeTagIds</span></span>|<span data-ttu-id="19cd7-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="19cd7-142">String collection</span></span>|<span data-ttu-id="19cd7-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="19cd7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="19cd7-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19cd7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19cd7-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="19cd7-145">supportsScopeTags</span></span>|<span data-ttu-id="19cd7-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="19cd7-146">Boolean</span></span>|<span data-ttu-id="19cd7-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="19cd7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="19cd7-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="19cd7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="19cd7-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="19cd7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="19cd7-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19cd7-150">This property is read-only.</span></span> <span data-ttu-id="19cd7-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19cd7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19cd7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="19cd7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="19cd7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="19cd7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="19cd7-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="19cd7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="19cd7-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19cd7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19cd7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="19cd7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="19cd7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="19cd7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="19cd7-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="19cd7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="19cd7-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19cd7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19cd7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="19cd7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="19cd7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="19cd7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="19cd7-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="19cd7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="19cd7-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19cd7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19cd7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19cd7-164">createdDateTime</span></span>|<span data-ttu-id="19cd7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19cd7-165">DateTimeOffset</span></span>|<span data-ttu-id="19cd7-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="19cd7-166">DateTime the object was created.</span></span> <span data-ttu-id="19cd7-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19cd7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19cd7-168">description</span><span class="sxs-lookup"><span data-stu-id="19cd7-168">description</span></span>|<span data-ttu-id="19cd7-169">String</span><span class="sxs-lookup"><span data-stu-id="19cd7-169">String</span></span>|<span data-ttu-id="19cd7-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="19cd7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="19cd7-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19cd7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19cd7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="19cd7-172">displayName</span></span>|<span data-ttu-id="19cd7-173">Строка</span><span class="sxs-lookup"><span data-stu-id="19cd7-173">String</span></span>|<span data-ttu-id="19cd7-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="19cd7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="19cd7-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19cd7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19cd7-176">version</span><span class="sxs-lookup"><span data-stu-id="19cd7-176">version</span></span>|<span data-ttu-id="19cd7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="19cd7-177">Int32</span></span>|<span data-ttu-id="19cd7-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="19cd7-178">Version of the device configuration.</span></span> <span data-ttu-id="19cd7-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19cd7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19cd7-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="19cd7-180">networkName</span></span>|<span data-ttu-id="19cd7-181">String</span><span class="sxs-lookup"><span data-stu-id="19cd7-181">String</span></span>|<span data-ttu-id="19cd7-182">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="19cd7-182">Network Name</span></span>|
|<span data-ttu-id="19cd7-183">SSID</span><span class="sxs-lookup"><span data-stu-id="19cd7-183">ssid</span></span>|<span data-ttu-id="19cd7-184">String</span><span class="sxs-lookup"><span data-stu-id="19cd7-184">String</span></span>|<span data-ttu-id="19cd7-185">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="19cd7-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="19cd7-186">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="19cd7-186">connectAutomatically</span></span>|<span data-ttu-id="19cd7-187">Логическое</span><span class="sxs-lookup"><span data-stu-id="19cd7-187">Boolean</span></span>|<span data-ttu-id="19cd7-188">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="19cd7-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="19cd7-189">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="19cd7-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="19cd7-190">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="19cd7-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="19cd7-191">Логическое</span><span class="sxs-lookup"><span data-stu-id="19cd7-191">Boolean</span></span>|<span data-ttu-id="19cd7-192">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="19cd7-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="19cd7-193">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="19cd7-193">wiFiSecurityType</span></span>|[<span data-ttu-id="19cd7-194">андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="19cd7-194">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="19cd7-195">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="19cd7-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="19cd7-196">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="19cd7-196">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="19cd7-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="19cd7-197">Response</span></span>
<span data-ttu-id="19cd7-198">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="19cd7-198">If successful, this method returns a `200 OK` response code and an updated [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19cd7-199">Пример</span><span class="sxs-lookup"><span data-stu-id="19cd7-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="19cd7-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="19cd7-200">Request</span></span>
<span data-ttu-id="19cd7-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19cd7-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="19cd7-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="19cd7-202">Response</span></span>
<span data-ttu-id="19cd7-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19cd7-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



