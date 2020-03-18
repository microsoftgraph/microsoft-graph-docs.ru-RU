---
title: Обновление объекта windows10EnterpriseModernAppManagementConfiguration
description: Обновление свойств объекта windows10EnterpriseModernAppManagementConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8a815db83e86ad5a98a03aa45235621befe04d2b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42739924"
---
# <a name="update-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="baafb-103">Обновление объекта windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="baafb-103">Update windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="baafb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="baafb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="baafb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="baafb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="baafb-106">Обновление свойств объекта [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="baafb-106">Update the properties of a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="baafb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="baafb-107">Prerequisites</span></span>
<span data-ttu-id="baafb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="baafb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baafb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="baafb-110">Permission type</span></span>|<span data-ttu-id="baafb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="baafb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="baafb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="baafb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="baafb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baafb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="baafb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="baafb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="baafb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="baafb-115">Not supported.</span></span>|
|<span data-ttu-id="baafb-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="baafb-116">Application</span></span>|<span data-ttu-id="baafb-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baafb-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="baafb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="baafb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="baafb-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="baafb-119">Request headers</span></span>
|<span data-ttu-id="baafb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="baafb-120">Header</span></span>|<span data-ttu-id="baafb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="baafb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="baafb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="baafb-122">Authorization</span></span>|<span data-ttu-id="baafb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="baafb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="baafb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="baafb-124">Accept</span></span>|<span data-ttu-id="baafb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="baafb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="baafb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="baafb-126">Request body</span></span>
<span data-ttu-id="baafb-127">В теле запроса добавьте представление объекта [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="baafb-127">In the request body, supply a JSON representation for the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

<span data-ttu-id="baafb-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="baafb-128">The following table shows the properties that are required when you create the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span></span>

|<span data-ttu-id="baafb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="baafb-129">Property</span></span>|<span data-ttu-id="baafb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="baafb-130">Type</span></span>|<span data-ttu-id="baafb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="baafb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baafb-132">id</span><span class="sxs-lookup"><span data-stu-id="baafb-132">id</span></span>|<span data-ttu-id="baafb-133">String</span><span class="sxs-lookup"><span data-stu-id="baafb-133">String</span></span>|<span data-ttu-id="baafb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="baafb-134">Key of the entity.</span></span> <span data-ttu-id="baafb-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="baafb-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baafb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="baafb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="baafb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="baafb-137">DateTimeOffset</span></span>|<span data-ttu-id="baafb-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="baafb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="baafb-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="baafb-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baafb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="baafb-140">roleScopeTagIds</span></span>|<span data-ttu-id="baafb-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="baafb-141">String collection</span></span>|<span data-ttu-id="baafb-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="baafb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="baafb-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="baafb-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baafb-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="baafb-144">supportsScopeTags</span></span>|<span data-ttu-id="baafb-145">Логический</span><span class="sxs-lookup"><span data-stu-id="baafb-145">Boolean</span></span>|<span data-ttu-id="baafb-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="baafb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="baafb-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="baafb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="baafb-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="baafb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="baafb-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="baafb-149">This property is read-only.</span></span> <span data-ttu-id="baafb-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="baafb-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baafb-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="baafb-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="baafb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="baafb-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="baafb-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="baafb-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="baafb-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="baafb-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baafb-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="baafb-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="baafb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="baafb-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="baafb-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="baafb-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="baafb-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="baafb-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baafb-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="baafb-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="baafb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="baafb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="baafb-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="baafb-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="baafb-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="baafb-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baafb-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="baafb-163">createdDateTime</span></span>|<span data-ttu-id="baafb-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="baafb-164">DateTimeOffset</span></span>|<span data-ttu-id="baafb-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="baafb-165">DateTime the object was created.</span></span> <span data-ttu-id="baafb-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="baafb-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baafb-167">description</span><span class="sxs-lookup"><span data-stu-id="baafb-167">description</span></span>|<span data-ttu-id="baafb-168">String</span><span class="sxs-lookup"><span data-stu-id="baafb-168">String</span></span>|<span data-ttu-id="baafb-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="baafb-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="baafb-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="baafb-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baafb-171">displayName</span><span class="sxs-lookup"><span data-stu-id="baafb-171">displayName</span></span>|<span data-ttu-id="baafb-172">Строка</span><span class="sxs-lookup"><span data-stu-id="baafb-172">String</span></span>|<span data-ttu-id="baafb-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="baafb-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="baafb-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="baafb-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baafb-175">version</span><span class="sxs-lookup"><span data-stu-id="baafb-175">version</span></span>|<span data-ttu-id="baafb-176">Int32</span><span class="sxs-lookup"><span data-stu-id="baafb-176">Int32</span></span>|<span data-ttu-id="baafb-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="baafb-177">Version of the device configuration.</span></span> <span data-ttu-id="baafb-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="baafb-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baafb-179">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="baafb-179">uninstallBuiltInApps</span></span>|<span data-ttu-id="baafb-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="baafb-180">Boolean</span></span>|<span data-ttu-id="baafb-181">Указывает, следует ли удалить фиксированный список встроенных приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="baafb-181">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="baafb-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="baafb-182">Response</span></span>
<span data-ttu-id="baafb-183">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="baafb-183">If successful, this method returns a `200 OK` response code and an updated [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baafb-184">Пример</span><span class="sxs-lookup"><span data-stu-id="baafb-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="baafb-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="baafb-185">Request</span></span>
<span data-ttu-id="baafb-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="baafb-186">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1087

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
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
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="baafb-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="baafb-187">Response</span></span>
<span data-ttu-id="baafb-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="baafb-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1259

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "id": "d6577687-7687-d657-8776-57d6877657d6",
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
  "uninstallBuiltInApps": true
}
```




