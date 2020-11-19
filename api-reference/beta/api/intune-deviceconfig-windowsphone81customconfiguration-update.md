---
title: Обновление объекта windowsPhone81CustomConfiguration
description: Обновление свойств объекта windowsPhone81CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d73b1b655c55f52aafb82cb996d30134ab7712cf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49235870"
---
# <a name="update-windowsphone81customconfiguration"></a><span data-ttu-id="cc848-103">Обновление объекта windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="cc848-103">Update windowsPhone81CustomConfiguration</span></span>

<span data-ttu-id="cc848-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc848-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc848-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc848-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc848-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc848-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc848-107">Обновление свойств объекта [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc848-107">Update the properties of a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc848-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cc848-108">Prerequisites</span></span>
<span data-ttu-id="cc848-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc848-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc848-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc848-111">Permission type</span></span>|<span data-ttu-id="cc848-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc848-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc848-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc848-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc848-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc848-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cc848-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc848-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc848-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc848-116">Not supported.</span></span>|
|<span data-ttu-id="cc848-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cc848-117">Application</span></span>|<span data-ttu-id="cc848-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc848-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc848-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc848-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cc848-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cc848-120">Request headers</span></span>
|<span data-ttu-id="cc848-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc848-121">Header</span></span>|<span data-ttu-id="cc848-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cc848-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc848-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc848-123">Authorization</span></span>|<span data-ttu-id="cc848-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc848-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc848-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cc848-125">Accept</span></span>|<span data-ttu-id="cc848-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cc848-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc848-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc848-127">Request body</span></span>
<span data-ttu-id="cc848-128">В теле запроса добавьте представление объекта [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc848-128">In the request body, supply a JSON representation for the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

<span data-ttu-id="cc848-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc848-129">The following table shows the properties that are required when you create the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>

|<span data-ttu-id="cc848-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc848-130">Property</span></span>|<span data-ttu-id="cc848-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cc848-131">Type</span></span>|<span data-ttu-id="cc848-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cc848-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc848-133">id</span><span class="sxs-lookup"><span data-stu-id="cc848-133">id</span></span>|<span data-ttu-id="cc848-134">String</span><span class="sxs-lookup"><span data-stu-id="cc848-134">String</span></span>|<span data-ttu-id="cc848-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cc848-135">Key of the entity.</span></span> <span data-ttu-id="cc848-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc848-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc848-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc848-137">lastModifiedDateTime</span></span>|<span data-ttu-id="cc848-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc848-138">DateTimeOffset</span></span>|<span data-ttu-id="cc848-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="cc848-139">DateTime the object was last modified.</span></span> <span data-ttu-id="cc848-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc848-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc848-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cc848-141">roleScopeTagIds</span></span>|<span data-ttu-id="cc848-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cc848-142">String collection</span></span>|<span data-ttu-id="cc848-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="cc848-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cc848-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc848-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc848-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="cc848-145">supportsScopeTags</span></span>|<span data-ttu-id="cc848-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc848-146">Boolean</span></span>|<span data-ttu-id="cc848-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="cc848-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cc848-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="cc848-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cc848-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="cc848-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cc848-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc848-150">This property is read-only.</span></span> <span data-ttu-id="cc848-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc848-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc848-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cc848-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="cc848-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cc848-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="cc848-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cc848-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="cc848-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc848-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc848-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cc848-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="cc848-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cc848-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="cc848-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cc848-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="cc848-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc848-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc848-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="cc848-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="cc848-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="cc848-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="cc848-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cc848-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="cc848-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc848-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc848-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc848-164">createdDateTime</span></span>|<span data-ttu-id="cc848-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc848-165">DateTimeOffset</span></span>|<span data-ttu-id="cc848-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="cc848-166">DateTime the object was created.</span></span> <span data-ttu-id="cc848-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc848-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc848-168">description</span><span class="sxs-lookup"><span data-stu-id="cc848-168">description</span></span>|<span data-ttu-id="cc848-169">String</span><span class="sxs-lookup"><span data-stu-id="cc848-169">String</span></span>|<span data-ttu-id="cc848-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cc848-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cc848-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc848-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc848-172">displayName</span><span class="sxs-lookup"><span data-stu-id="cc848-172">displayName</span></span>|<span data-ttu-id="cc848-173">String</span><span class="sxs-lookup"><span data-stu-id="cc848-173">String</span></span>|<span data-ttu-id="cc848-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cc848-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cc848-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc848-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc848-176">version</span><span class="sxs-lookup"><span data-stu-id="cc848-176">version</span></span>|<span data-ttu-id="cc848-177">Int32</span><span class="sxs-lookup"><span data-stu-id="cc848-177">Int32</span></span>|<span data-ttu-id="cc848-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cc848-178">Version of the device configuration.</span></span> <span data-ttu-id="cc848-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc848-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc848-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="cc848-180">omaSettings</span></span>|<span data-ttu-id="cc848-181">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cc848-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="cc848-182">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="cc848-182">OMA settings.</span></span> <span data-ttu-id="cc848-183">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="cc848-183">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="cc848-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc848-184">Response</span></span>
<span data-ttu-id="cc848-185">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cc848-185">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc848-186">Пример</span><span class="sxs-lookup"><span data-stu-id="cc848-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc848-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc848-187">Request</span></span>
<span data-ttu-id="cc848-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc848-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1276

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
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "isEncrypted": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="cc848-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc848-189">Response</span></span>
<span data-ttu-id="cc848-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc848-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1448

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
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "isEncrypted": true
    }
  ]
}
```




