---
title: Создание объекта windowsPhone81CustomConfiguration
description: Создание объекта windowsPhone81CustomConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5f758a5cbf0d10a2f9d96a98d2e74af923b2b442
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946667"
---
# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="40af4-103">Создание объекта windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="40af4-103">Create windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="40af4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40af4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40af4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="40af4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40af4-106">Создание объекта [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40af4-106">Create a new [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40af4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="40af4-107">Prerequisites</span></span>
<span data-ttu-id="40af4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40af4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40af4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40af4-110">Permission type</span></span>|<span data-ttu-id="40af4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="40af4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40af4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40af4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40af4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40af4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="40af4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40af4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40af4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40af4-115">Not supported.</span></span>|
|<span data-ttu-id="40af4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40af4-116">Application</span></span>|<span data-ttu-id="40af4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40af4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40af4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40af4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="40af4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="40af4-119">Request headers</span></span>
|<span data-ttu-id="40af4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40af4-120">Header</span></span>|<span data-ttu-id="40af4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="40af4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40af4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40af4-122">Authorization</span></span>|<span data-ttu-id="40af4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40af4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40af4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="40af4-124">Accept</span></span>|<span data-ttu-id="40af4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="40af4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40af4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="40af4-126">Request body</span></span>
<span data-ttu-id="40af4-127">В теле запроса добавьте представление объекта windowsPhone81CustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40af4-127">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="40af4-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsPhone81CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="40af4-128">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="40af4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="40af4-129">Property</span></span>|<span data-ttu-id="40af4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="40af4-130">Type</span></span>|<span data-ttu-id="40af4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="40af4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40af4-132">id</span><span class="sxs-lookup"><span data-stu-id="40af4-132">id</span></span>|<span data-ttu-id="40af4-133">String</span><span class="sxs-lookup"><span data-stu-id="40af4-133">String</span></span>|<span data-ttu-id="40af4-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="40af4-134">Key of the entity.</span></span> <span data-ttu-id="40af4-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40af4-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40af4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40af4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="40af4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40af4-137">DateTimeOffset</span></span>|<span data-ttu-id="40af4-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="40af4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="40af4-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40af4-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40af4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="40af4-140">roleScopeTagIds</span></span>|<span data-ttu-id="40af4-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="40af4-141">String collection</span></span>|<span data-ttu-id="40af4-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="40af4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="40af4-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40af4-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40af4-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="40af4-144">supportsScopeTags</span></span>|<span data-ttu-id="40af4-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="40af4-145">Boolean</span></span>|<span data-ttu-id="40af4-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="40af4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="40af4-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="40af4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="40af4-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="40af4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="40af4-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="40af4-149">This property is read-only.</span></span> <span data-ttu-id="40af4-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40af4-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40af4-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="40af4-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="40af4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="40af4-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="40af4-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="40af4-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="40af4-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40af4-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40af4-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="40af4-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="40af4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="40af4-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="40af4-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="40af4-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="40af4-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40af4-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40af4-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="40af4-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="40af4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="40af4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="40af4-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="40af4-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="40af4-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40af4-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40af4-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40af4-163">createdDateTime</span></span>|<span data-ttu-id="40af4-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40af4-164">DateTimeOffset</span></span>|<span data-ttu-id="40af4-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="40af4-165">DateTime the object was created.</span></span> <span data-ttu-id="40af4-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40af4-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40af4-167">description</span><span class="sxs-lookup"><span data-stu-id="40af4-167">description</span></span>|<span data-ttu-id="40af4-168">String</span><span class="sxs-lookup"><span data-stu-id="40af4-168">String</span></span>|<span data-ttu-id="40af4-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="40af4-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="40af4-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40af4-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40af4-171">displayName</span><span class="sxs-lookup"><span data-stu-id="40af4-171">displayName</span></span>|<span data-ttu-id="40af4-172">Строка</span><span class="sxs-lookup"><span data-stu-id="40af4-172">String</span></span>|<span data-ttu-id="40af4-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="40af4-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="40af4-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40af4-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40af4-175">version</span><span class="sxs-lookup"><span data-stu-id="40af4-175">version</span></span>|<span data-ttu-id="40af4-176">Int32</span><span class="sxs-lookup"><span data-stu-id="40af4-176">Int32</span></span>|<span data-ttu-id="40af4-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="40af4-177">Version of the device configuration.</span></span> <span data-ttu-id="40af4-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="40af4-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40af4-179">omaSettings</span><span class="sxs-lookup"><span data-stu-id="40af4-179">omaSettings</span></span>|<span data-ttu-id="40af4-180">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="40af4-180">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="40af4-181">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="40af4-181">OMA settings.</span></span> <span data-ttu-id="40af4-182">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="40af4-182">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="40af4-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="40af4-183">Response</span></span>
<span data-ttu-id="40af4-184">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="40af4-184">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40af4-185">Пример</span><span class="sxs-lookup"><span data-stu-id="40af4-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="40af4-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="40af4-186">Request</span></span>
<span data-ttu-id="40af4-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40af4-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1301

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="40af4-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="40af4-188">Response</span></span>
<span data-ttu-id="40af4-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40af4-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1473

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
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





