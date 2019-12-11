---
title: Создание объекта windows10EnterpriseModernAppManagementConfiguration
description: Создание объекта windows10EnterpriseModernAppManagementConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ccc52d3122bd6e7b644bc79efd9ab9bb5f54936
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947493"
---
# <a name="create-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="3a9ec-103">Создание объекта windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="3a9ec-103">Create windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="3a9ec-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a9ec-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a9ec-106">Создание объекта [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a9ec-106">Create a new [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a9ec-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3a9ec-107">Prerequisites</span></span>
<span data-ttu-id="3a9ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a9ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a9ec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a9ec-110">Permission type</span></span>|<span data-ttu-id="3a9ec-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a9ec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a9ec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a9ec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3a9ec-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9ec-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3a9ec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a9ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a9ec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-115">Not supported.</span></span>|
|<span data-ttu-id="3a9ec-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a9ec-116">Application</span></span>|<span data-ttu-id="3a9ec-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9ec-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a9ec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a9ec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3a9ec-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3a9ec-119">Request headers</span></span>
|<span data-ttu-id="3a9ec-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a9ec-120">Header</span></span>|<span data-ttu-id="3a9ec-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3a9ec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a9ec-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a9ec-122">Authorization</span></span>|<span data-ttu-id="3a9ec-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a9ec-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3a9ec-124">Accept</span></span>|<span data-ttu-id="3a9ec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3a9ec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a9ec-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3a9ec-126">Request body</span></span>
<span data-ttu-id="3a9ec-127">В теле запроса добавьте представление объекта windows10EnterpriseModernAppManagementConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-127">In the request body, supply a JSON representation for the windows10EnterpriseModernAppManagementConfiguration object.</span></span>

<span data-ttu-id="3a9ec-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windows10EnterpriseModernAppManagementConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-128">The following table shows the properties that are required when you create the windows10EnterpriseModernAppManagementConfiguration.</span></span>

|<span data-ttu-id="3a9ec-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a9ec-129">Property</span></span>|<span data-ttu-id="3a9ec-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3a9ec-130">Type</span></span>|<span data-ttu-id="3a9ec-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3a9ec-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a9ec-132">id</span><span class="sxs-lookup"><span data-stu-id="3a9ec-132">id</span></span>|<span data-ttu-id="3a9ec-133">String</span><span class="sxs-lookup"><span data-stu-id="3a9ec-133">String</span></span>|<span data-ttu-id="3a9ec-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-134">Key of the entity.</span></span> <span data-ttu-id="3a9ec-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a9ec-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9ec-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a9ec-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3a9ec-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a9ec-137">DateTimeOffset</span></span>|<span data-ttu-id="3a9ec-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3a9ec-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a9ec-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9ec-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3a9ec-140">roleScopeTagIds</span></span>|<span data-ttu-id="3a9ec-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3a9ec-141">String collection</span></span>|<span data-ttu-id="3a9ec-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3a9ec-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a9ec-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9ec-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="3a9ec-144">supportsScopeTags</span></span>|<span data-ttu-id="3a9ec-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a9ec-145">Boolean</span></span>|<span data-ttu-id="3a9ec-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3a9ec-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3a9ec-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3a9ec-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-149">This property is read-only.</span></span> <span data-ttu-id="3a9ec-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a9ec-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9ec-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3a9ec-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3a9ec-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3a9ec-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3a9ec-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3a9ec-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a9ec-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9ec-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3a9ec-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3a9ec-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3a9ec-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3a9ec-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3a9ec-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a9ec-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9ec-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3a9ec-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3a9ec-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3a9ec-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3a9ec-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3a9ec-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a9ec-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9ec-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a9ec-163">createdDateTime</span></span>|<span data-ttu-id="3a9ec-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a9ec-164">DateTimeOffset</span></span>|<span data-ttu-id="3a9ec-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-165">DateTime the object was created.</span></span> <span data-ttu-id="3a9ec-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a9ec-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9ec-167">description</span><span class="sxs-lookup"><span data-stu-id="3a9ec-167">description</span></span>|<span data-ttu-id="3a9ec-168">String</span><span class="sxs-lookup"><span data-stu-id="3a9ec-168">String</span></span>|<span data-ttu-id="3a9ec-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3a9ec-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a9ec-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9ec-171">displayName</span><span class="sxs-lookup"><span data-stu-id="3a9ec-171">displayName</span></span>|<span data-ttu-id="3a9ec-172">Строка</span><span class="sxs-lookup"><span data-stu-id="3a9ec-172">String</span></span>|<span data-ttu-id="3a9ec-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3a9ec-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3a9ec-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9ec-175">version</span><span class="sxs-lookup"><span data-stu-id="3a9ec-175">version</span></span>|<span data-ttu-id="3a9ec-176">Int32</span><span class="sxs-lookup"><span data-stu-id="3a9ec-176">Int32</span></span>|<span data-ttu-id="3a9ec-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-177">Version of the device configuration.</span></span> <span data-ttu-id="3a9ec-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a9ec-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a9ec-179">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="3a9ec-179">uninstallBuiltInApps</span></span>|<span data-ttu-id="3a9ec-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a9ec-180">Boolean</span></span>|<span data-ttu-id="3a9ec-181">Указывает, следует ли удалить фиксированный список встроенных приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-181">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="3a9ec-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a9ec-182">Response</span></span>
<span data-ttu-id="3a9ec-183">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-183">If successful, this method returns a `201 Created` response code and a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a9ec-184">Пример</span><span class="sxs-lookup"><span data-stu-id="3a9ec-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a9ec-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a9ec-185">Request</span></span>
<span data-ttu-id="3a9ec-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-186">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="3a9ec-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a9ec-187">Response</span></span>
<span data-ttu-id="3a9ec-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a9ec-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





