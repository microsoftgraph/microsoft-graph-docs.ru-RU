---
title: Обновление iosEducationDeviceConfiguration
description: Обновление свойств объекта iosEducationDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3521a64b80931449be07287d6c573939e56837a7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47995578"
---
# <a name="update-ioseducationdeviceconfiguration"></a><span data-ttu-id="1be16-103">Обновление iosEducationDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1be16-103">Update iosEducationDeviceConfiguration</span></span>

<span data-ttu-id="1be16-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1be16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1be16-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1be16-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1be16-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1be16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1be16-107">Обновление свойств объекта [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1be16-107">Update the properties of a [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1be16-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1be16-108">Prerequisites</span></span>
<span data-ttu-id="1be16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1be16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1be16-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1be16-111">Permission type</span></span>|<span data-ttu-id="1be16-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1be16-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1be16-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1be16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1be16-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1be16-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1be16-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1be16-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1be16-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1be16-116">Not supported.</span></span>|
|<span data-ttu-id="1be16-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1be16-117">Application</span></span>|<span data-ttu-id="1be16-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1be16-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1be16-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1be16-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1be16-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1be16-120">Request headers</span></span>
|<span data-ttu-id="1be16-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1be16-121">Header</span></span>|<span data-ttu-id="1be16-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1be16-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1be16-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1be16-123">Authorization</span></span>|<span data-ttu-id="1be16-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1be16-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1be16-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1be16-125">Accept</span></span>|<span data-ttu-id="1be16-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1be16-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1be16-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1be16-127">Request body</span></span>
<span data-ttu-id="1be16-128">В тексте запроса добавьте представление объекта [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1be16-128">In the request body, supply a JSON representation for the [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object.</span></span>

<span data-ttu-id="1be16-129">В следующей таблице приведены свойства, необходимые при создании [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1be16-129">The following table shows the properties that are required when you create the [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md).</span></span>

|<span data-ttu-id="1be16-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1be16-130">Property</span></span>|<span data-ttu-id="1be16-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1be16-131">Type</span></span>|<span data-ttu-id="1be16-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1be16-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1be16-133">id</span><span class="sxs-lookup"><span data-stu-id="1be16-133">id</span></span>|<span data-ttu-id="1be16-134">String</span><span class="sxs-lookup"><span data-stu-id="1be16-134">String</span></span>|<span data-ttu-id="1be16-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1be16-135">Key of the entity.</span></span> <span data-ttu-id="1be16-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1be16-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be16-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1be16-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1be16-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1be16-138">DateTimeOffset</span></span>|<span data-ttu-id="1be16-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1be16-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1be16-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1be16-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be16-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1be16-141">roleScopeTagIds</span></span>|<span data-ttu-id="1be16-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1be16-142">String collection</span></span>|<span data-ttu-id="1be16-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1be16-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1be16-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1be16-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be16-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="1be16-145">supportsScopeTags</span></span>|<span data-ttu-id="1be16-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1be16-146">Boolean</span></span>|<span data-ttu-id="1be16-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1be16-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1be16-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="1be16-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1be16-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1be16-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1be16-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1be16-150">This property is read-only.</span></span> <span data-ttu-id="1be16-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1be16-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be16-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1be16-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1be16-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1be16-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1be16-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1be16-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1be16-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1be16-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be16-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1be16-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1be16-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1be16-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1be16-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1be16-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1be16-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1be16-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be16-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1be16-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1be16-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1be16-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1be16-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1be16-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1be16-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1be16-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be16-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1be16-164">createdDateTime</span></span>|<span data-ttu-id="1be16-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1be16-165">DateTimeOffset</span></span>|<span data-ttu-id="1be16-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1be16-166">DateTime the object was created.</span></span> <span data-ttu-id="1be16-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1be16-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be16-168">description</span><span class="sxs-lookup"><span data-stu-id="1be16-168">description</span></span>|<span data-ttu-id="1be16-169">String</span><span class="sxs-lookup"><span data-stu-id="1be16-169">String</span></span>|<span data-ttu-id="1be16-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1be16-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1be16-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1be16-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be16-172">displayName</span><span class="sxs-lookup"><span data-stu-id="1be16-172">displayName</span></span>|<span data-ttu-id="1be16-173">String</span><span class="sxs-lookup"><span data-stu-id="1be16-173">String</span></span>|<span data-ttu-id="1be16-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1be16-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1be16-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1be16-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1be16-176">version</span><span class="sxs-lookup"><span data-stu-id="1be16-176">version</span></span>|<span data-ttu-id="1be16-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1be16-177">Int32</span></span>|<span data-ttu-id="1be16-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1be16-178">Version of the device configuration.</span></span> <span data-ttu-id="1be16-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1be16-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1be16-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="1be16-180">Response</span></span>
<span data-ttu-id="1be16-181">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1be16-181">If successful, this method returns a `200 OK` response code and an updated [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1be16-182">Пример</span><span class="sxs-lookup"><span data-stu-id="1be16-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="1be16-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="1be16-183">Request</span></span>
<span data-ttu-id="1be16-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1be16-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1034

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="1be16-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="1be16-185">Response</span></span>
<span data-ttu-id="1be16-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1be16-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1206

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
  "id": "3d563be4-3be4-3d56-e43b-563de43b563d",
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






