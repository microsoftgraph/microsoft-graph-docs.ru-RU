---
title: Update androidCustomConfiguration
description: Обновление свойств объекта androidCustomConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f4c0ca3f7f08d8a949cd5f5f2491b1ba938208cf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759915"
---
# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="5a2fd-103">Update androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="5a2fd-103">Update androidCustomConfiguration</span></span>

> <span data-ttu-id="5a2fd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a2fd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a2fd-106">Обновление свойств объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a2fd-106">Update the properties of a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a2fd-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5a2fd-107">Prerequisites</span></span>
<span data-ttu-id="5a2fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a2fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a2fd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a2fd-110">Permission type</span></span>|<span data-ttu-id="5a2fd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a2fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a2fd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a2fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a2fd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a2fd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5a2fd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a2fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a2fd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-115">Not supported.</span></span>|
|<span data-ttu-id="5a2fd-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5a2fd-116">Application</span></span>|<span data-ttu-id="5a2fd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a2fd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a2fd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a2fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5a2fd-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5a2fd-119">Request headers</span></span>
|<span data-ttu-id="5a2fd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a2fd-120">Header</span></span>|<span data-ttu-id="5a2fd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5a2fd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a2fd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a2fd-122">Authorization</span></span>|<span data-ttu-id="5a2fd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a2fd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5a2fd-124">Accept</span></span>|<span data-ttu-id="5a2fd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5a2fd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a2fd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a2fd-126">Request body</span></span>
<span data-ttu-id="5a2fd-127">В теле запроса добавьте представление объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-127">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="5a2fd-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a2fd-128">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="5a2fd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a2fd-129">Property</span></span>|<span data-ttu-id="5a2fd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5a2fd-130">Type</span></span>|<span data-ttu-id="5a2fd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5a2fd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a2fd-132">id</span><span class="sxs-lookup"><span data-stu-id="5a2fd-132">id</span></span>|<span data-ttu-id="5a2fd-133">String</span><span class="sxs-lookup"><span data-stu-id="5a2fd-133">String</span></span>|<span data-ttu-id="5a2fd-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-134">Key of the entity.</span></span> <span data-ttu-id="5a2fd-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a2fd-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a2fd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a2fd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5a2fd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a2fd-137">DateTimeOffset</span></span>|<span data-ttu-id="5a2fd-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5a2fd-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a2fd-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a2fd-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5a2fd-140">roleScopeTagIds</span></span>|<span data-ttu-id="5a2fd-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5a2fd-141">String collection</span></span>|<span data-ttu-id="5a2fd-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5a2fd-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a2fd-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a2fd-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="5a2fd-144">supportsScopeTags</span></span>|<span data-ttu-id="5a2fd-145">Логический</span><span class="sxs-lookup"><span data-stu-id="5a2fd-145">Boolean</span></span>|<span data-ttu-id="5a2fd-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5a2fd-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5a2fd-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5a2fd-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-149">This property is read-only.</span></span> <span data-ttu-id="5a2fd-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a2fd-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a2fd-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5a2fd-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5a2fd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5a2fd-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5a2fd-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5a2fd-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a2fd-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a2fd-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5a2fd-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5a2fd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5a2fd-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5a2fd-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5a2fd-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a2fd-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a2fd-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5a2fd-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5a2fd-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5a2fd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5a2fd-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5a2fd-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a2fd-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a2fd-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a2fd-163">createdDateTime</span></span>|<span data-ttu-id="5a2fd-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a2fd-164">DateTimeOffset</span></span>|<span data-ttu-id="5a2fd-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-165">DateTime the object was created.</span></span> <span data-ttu-id="5a2fd-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a2fd-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a2fd-167">description</span><span class="sxs-lookup"><span data-stu-id="5a2fd-167">description</span></span>|<span data-ttu-id="5a2fd-168">String</span><span class="sxs-lookup"><span data-stu-id="5a2fd-168">String</span></span>|<span data-ttu-id="5a2fd-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5a2fd-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a2fd-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a2fd-171">displayName</span><span class="sxs-lookup"><span data-stu-id="5a2fd-171">displayName</span></span>|<span data-ttu-id="5a2fd-172">Строка</span><span class="sxs-lookup"><span data-stu-id="5a2fd-172">String</span></span>|<span data-ttu-id="5a2fd-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5a2fd-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a2fd-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a2fd-175">version</span><span class="sxs-lookup"><span data-stu-id="5a2fd-175">version</span></span>|<span data-ttu-id="5a2fd-176">Int32</span><span class="sxs-lookup"><span data-stu-id="5a2fd-176">Int32</span></span>|<span data-ttu-id="5a2fd-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-177">Version of the device configuration.</span></span> <span data-ttu-id="5a2fd-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5a2fd-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a2fd-179">omaSettings</span><span class="sxs-lookup"><span data-stu-id="5a2fd-179">omaSettings</span></span>|<span data-ttu-id="5a2fd-180">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5a2fd-180">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="5a2fd-181">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-181">OMA settings.</span></span> <span data-ttu-id="5a2fd-182">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-182">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="5a2fd-183">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a2fd-183">Response</span></span>
<span data-ttu-id="5a2fd-184">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-184">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a2fd-185">Пример</span><span class="sxs-lookup"><span data-stu-id="5a2fd-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a2fd-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a2fd-186">Request</span></span>
<span data-ttu-id="5a2fd-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1294

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5,
      "isReadOnly": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="5a2fd-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a2fd-188">Response</span></span>
<span data-ttu-id="5a2fd-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a2fd-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1466

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5,
      "isReadOnly": true
    }
  ]
}
```




