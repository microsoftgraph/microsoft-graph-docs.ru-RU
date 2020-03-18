---
title: Обновление Андроидфорворквификонфигуратион
description: Обновление свойств объекта Андроидфорворквификонфигуратион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5e656592fdeac34ce0c6ccc17ee72b92f150732a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759024"
---
# <a name="update-androidforworkwificonfiguration"></a><span data-ttu-id="2bb4b-103">Обновление Андроидфорворквификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="2bb4b-103">Update androidForWorkWiFiConfiguration</span></span>

> <span data-ttu-id="2bb4b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bb4b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bb4b-106">Обновление свойств объекта [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2bb4b-106">Update the properties of a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bb4b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2bb4b-107">Prerequisites</span></span>
<span data-ttu-id="2bb4b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bb4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bb4b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2bb4b-110">Permission type</span></span>|<span data-ttu-id="2bb4b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2bb4b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bb4b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2bb4b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2bb4b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bb4b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2bb4b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2bb4b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bb4b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-115">Not supported.</span></span>|
|<span data-ttu-id="2bb4b-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2bb4b-116">Application</span></span>|<span data-ttu-id="2bb4b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bb4b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bb4b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2bb4b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2bb4b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2bb4b-119">Request headers</span></span>
|<span data-ttu-id="2bb4b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2bb4b-120">Header</span></span>|<span data-ttu-id="2bb4b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2bb4b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bb4b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bb4b-122">Authorization</span></span>|<span data-ttu-id="2bb4b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bb4b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2bb4b-124">Accept</span></span>|<span data-ttu-id="2bb4b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2bb4b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bb4b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2bb4b-126">Request body</span></span>
<span data-ttu-id="2bb4b-127">В тексте запроса добавьте представление объекта [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-127">In the request body, supply a JSON representation for the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

<span data-ttu-id="2bb4b-128">В следующей таблице приведены свойства, необходимые при создании [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bb4b-128">The following table shows the properties that are required when you create the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span>

|<span data-ttu-id="2bb4b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2bb4b-129">Property</span></span>|<span data-ttu-id="2bb4b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2bb4b-130">Type</span></span>|<span data-ttu-id="2bb4b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2bb4b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bb4b-132">id</span><span class="sxs-lookup"><span data-stu-id="2bb4b-132">id</span></span>|<span data-ttu-id="2bb4b-133">String</span><span class="sxs-lookup"><span data-stu-id="2bb4b-133">String</span></span>|<span data-ttu-id="2bb4b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-134">Key of the entity.</span></span> <span data-ttu-id="2bb4b-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bb4b-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2bb4b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2bb4b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2bb4b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bb4b-137">DateTimeOffset</span></span>|<span data-ttu-id="2bb4b-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2bb4b-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bb4b-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2bb4b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2bb4b-140">roleScopeTagIds</span></span>|<span data-ttu-id="2bb4b-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2bb4b-141">String collection</span></span>|<span data-ttu-id="2bb4b-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2bb4b-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bb4b-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2bb4b-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="2bb4b-144">supportsScopeTags</span></span>|<span data-ttu-id="2bb4b-145">Логический</span><span class="sxs-lookup"><span data-stu-id="2bb4b-145">Boolean</span></span>|<span data-ttu-id="2bb4b-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2bb4b-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2bb4b-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2bb4b-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-149">This property is read-only.</span></span> <span data-ttu-id="2bb4b-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bb4b-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2bb4b-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2bb4b-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2bb4b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2bb4b-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2bb4b-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2bb4b-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bb4b-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2bb4b-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2bb4b-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2bb4b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2bb4b-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2bb4b-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2bb4b-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bb4b-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2bb4b-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2bb4b-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2bb4b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2bb4b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2bb4b-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2bb4b-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bb4b-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2bb4b-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2bb4b-163">createdDateTime</span></span>|<span data-ttu-id="2bb4b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bb4b-164">DateTimeOffset</span></span>|<span data-ttu-id="2bb4b-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-165">DateTime the object was created.</span></span> <span data-ttu-id="2bb4b-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bb4b-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2bb4b-167">description</span><span class="sxs-lookup"><span data-stu-id="2bb4b-167">description</span></span>|<span data-ttu-id="2bb4b-168">String</span><span class="sxs-lookup"><span data-stu-id="2bb4b-168">String</span></span>|<span data-ttu-id="2bb4b-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2bb4b-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bb4b-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2bb4b-171">displayName</span><span class="sxs-lookup"><span data-stu-id="2bb4b-171">displayName</span></span>|<span data-ttu-id="2bb4b-172">Строка</span><span class="sxs-lookup"><span data-stu-id="2bb4b-172">String</span></span>|<span data-ttu-id="2bb4b-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2bb4b-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bb4b-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2bb4b-175">version</span><span class="sxs-lookup"><span data-stu-id="2bb4b-175">version</span></span>|<span data-ttu-id="2bb4b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2bb4b-176">Int32</span></span>|<span data-ttu-id="2bb4b-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-177">Version of the device configuration.</span></span> <span data-ttu-id="2bb4b-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bb4b-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2bb4b-179">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="2bb4b-179">networkName</span></span>|<span data-ttu-id="2bb4b-180">String</span><span class="sxs-lookup"><span data-stu-id="2bb4b-180">String</span></span>|<span data-ttu-id="2bb4b-181">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="2bb4b-181">Network Name</span></span>|
|<span data-ttu-id="2bb4b-182">SSID</span><span class="sxs-lookup"><span data-stu-id="2bb4b-182">ssid</span></span>|<span data-ttu-id="2bb4b-183">String</span><span class="sxs-lookup"><span data-stu-id="2bb4b-183">String</span></span>|<span data-ttu-id="2bb4b-184">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="2bb4b-185">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="2bb4b-185">connectAutomatically</span></span>|<span data-ttu-id="2bb4b-186">Логический</span><span class="sxs-lookup"><span data-stu-id="2bb4b-186">Boolean</span></span>|<span data-ttu-id="2bb4b-187">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="2bb4b-188">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="2bb4b-189">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="2bb4b-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="2bb4b-190">Логический</span><span class="sxs-lookup"><span data-stu-id="2bb4b-190">Boolean</span></span>|<span data-ttu-id="2bb4b-191">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-191">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="2bb4b-192">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="2bb4b-192">wiFiSecurityType</span></span>|[<span data-ttu-id="2bb4b-193">андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="2bb4b-193">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="2bb4b-194">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-194">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="2bb4b-195">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-195">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="2bb4b-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bb4b-196">Response</span></span>
<span data-ttu-id="2bb4b-197">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-197">If successful, this method returns a `200 OK` response code and an updated [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bb4b-198">Пример</span><span class="sxs-lookup"><span data-stu-id="2bb4b-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bb4b-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="2bb4b-199">Request</span></span>
<span data-ttu-id="2bb4b-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2bb4b-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bb4b-201">Response</span></span>
<span data-ttu-id="2bb4b-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2bb4b-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




