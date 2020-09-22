---
title: Обновление Иосдериведкредентиалаусентикатионконфигуратион
description: Обновление свойств объекта Иосдериведкредентиалаусентикатионконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 358c203e9948671c78b0f63ce2edd01d89141ae6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47995760"
---
# <a name="update-iosderivedcredentialauthenticationconfiguration"></a><span data-ttu-id="64126-103">Обновление Иосдериведкредентиалаусентикатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="64126-103">Update iosDerivedCredentialAuthenticationConfiguration</span></span>

<span data-ttu-id="64126-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64126-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64126-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64126-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64126-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64126-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64126-107">Обновление свойств объекта [иосдериведкредентиалаусентикатионконфигуратион](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="64126-107">Update the properties of a [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64126-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="64126-108">Prerequisites</span></span>
<span data-ttu-id="64126-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64126-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64126-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64126-111">Permission type</span></span>|<span data-ttu-id="64126-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64126-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64126-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64126-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64126-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64126-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64126-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64126-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64126-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64126-116">Not supported.</span></span>|
|<span data-ttu-id="64126-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64126-117">Application</span></span>|<span data-ttu-id="64126-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64126-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64126-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64126-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="64126-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="64126-120">Request headers</span></span>
|<span data-ttu-id="64126-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64126-121">Header</span></span>|<span data-ttu-id="64126-122">Значение</span><span class="sxs-lookup"><span data-stu-id="64126-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64126-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="64126-123">Authorization</span></span>|<span data-ttu-id="64126-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64126-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64126-125">Accept</span><span class="sxs-lookup"><span data-stu-id="64126-125">Accept</span></span>|<span data-ttu-id="64126-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64126-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64126-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="64126-127">Request body</span></span>
<span data-ttu-id="64126-128">В тексте запроса добавьте представление объекта [иосдериведкредентиалаусентикатионконфигуратион](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64126-128">In the request body, supply a JSON representation for the [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object.</span></span>

<span data-ttu-id="64126-129">В следующей таблице приведены свойства, необходимые при создании [иосдериведкредентиалаусентикатионконфигуратион](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64126-129">The following table shows the properties that are required when you create the [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md).</span></span>

|<span data-ttu-id="64126-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="64126-130">Property</span></span>|<span data-ttu-id="64126-131">Тип</span><span class="sxs-lookup"><span data-stu-id="64126-131">Type</span></span>|<span data-ttu-id="64126-132">Описание</span><span class="sxs-lookup"><span data-stu-id="64126-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64126-133">id</span><span class="sxs-lookup"><span data-stu-id="64126-133">id</span></span>|<span data-ttu-id="64126-134">String</span><span class="sxs-lookup"><span data-stu-id="64126-134">String</span></span>|<span data-ttu-id="64126-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="64126-135">Key of the entity.</span></span> <span data-ttu-id="64126-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64126-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64126-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64126-137">lastModifiedDateTime</span></span>|<span data-ttu-id="64126-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64126-138">DateTimeOffset</span></span>|<span data-ttu-id="64126-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="64126-139">DateTime the object was last modified.</span></span> <span data-ttu-id="64126-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64126-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64126-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="64126-141">roleScopeTagIds</span></span>|<span data-ttu-id="64126-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="64126-142">String collection</span></span>|<span data-ttu-id="64126-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="64126-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="64126-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64126-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64126-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="64126-145">supportsScopeTags</span></span>|<span data-ttu-id="64126-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="64126-146">Boolean</span></span>|<span data-ttu-id="64126-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="64126-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="64126-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="64126-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="64126-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="64126-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="64126-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64126-150">This property is read-only.</span></span> <span data-ttu-id="64126-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64126-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64126-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="64126-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="64126-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="64126-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="64126-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="64126-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="64126-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64126-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64126-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="64126-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="64126-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="64126-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="64126-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="64126-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="64126-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64126-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64126-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="64126-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="64126-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="64126-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="64126-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="64126-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="64126-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64126-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64126-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64126-164">createdDateTime</span></span>|<span data-ttu-id="64126-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64126-165">DateTimeOffset</span></span>|<span data-ttu-id="64126-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="64126-166">DateTime the object was created.</span></span> <span data-ttu-id="64126-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64126-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64126-168">description</span><span class="sxs-lookup"><span data-stu-id="64126-168">description</span></span>|<span data-ttu-id="64126-169">String</span><span class="sxs-lookup"><span data-stu-id="64126-169">String</span></span>|<span data-ttu-id="64126-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="64126-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="64126-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64126-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64126-172">displayName</span><span class="sxs-lookup"><span data-stu-id="64126-172">displayName</span></span>|<span data-ttu-id="64126-173">String</span><span class="sxs-lookup"><span data-stu-id="64126-173">String</span></span>|<span data-ttu-id="64126-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="64126-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="64126-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64126-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64126-176">version</span><span class="sxs-lookup"><span data-stu-id="64126-176">version</span></span>|<span data-ttu-id="64126-177">Int32</span><span class="sxs-lookup"><span data-stu-id="64126-177">Int32</span></span>|<span data-ttu-id="64126-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="64126-178">Version of the device configuration.</span></span> <span data-ttu-id="64126-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64126-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="64126-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="64126-180">Response</span></span>
<span data-ttu-id="64126-181">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иосдериведкредентиалаусентикатионконфигуратион](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="64126-181">If successful, this method returns a `200 OK` response code and an updated [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64126-182">Пример</span><span class="sxs-lookup"><span data-stu-id="64126-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="64126-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="64126-183">Request</span></span>
<span data-ttu-id="64126-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64126-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1050

{
  "@odata.type": "#microsoft.graph.iosDerivedCredentialAuthenticationConfiguration",
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
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="64126-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="64126-185">Response</span></span>
<span data-ttu-id="64126-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64126-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1222

{
  "@odata.type": "#microsoft.graph.iosDerivedCredentialAuthenticationConfiguration",
  "id": "01713f58-3f58-0171-583f-7101583f7101",
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
  "version": 7
}
```






