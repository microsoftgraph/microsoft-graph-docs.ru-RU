---
title: Update androidCustomConfiguration
description: Обновление свойств объекта androidCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4c70f4d04272d0c22a20553e916aacede856c4f7
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863782"
---
# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="defaa-103">Update androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="defaa-103">Update androidCustomConfiguration</span></span>

<span data-ttu-id="defaa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="defaa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="defaa-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="defaa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="defaa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="defaa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="defaa-107">Обновление свойств объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="defaa-107">Update the properties of a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="defaa-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="defaa-108">Prerequisites</span></span>
<span data-ttu-id="defaa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="defaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="defaa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="defaa-111">Permission type</span></span>|<span data-ttu-id="defaa-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="defaa-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="defaa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="defaa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="defaa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="defaa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="defaa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="defaa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="defaa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="defaa-116">Not supported.</span></span>|
|<span data-ttu-id="defaa-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="defaa-117">Application</span></span>|<span data-ttu-id="defaa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="defaa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="defaa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="defaa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="defaa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="defaa-120">Request headers</span></span>
|<span data-ttu-id="defaa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="defaa-121">Header</span></span>|<span data-ttu-id="defaa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="defaa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="defaa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="defaa-123">Authorization</span></span>|<span data-ttu-id="defaa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="defaa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="defaa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="defaa-125">Accept</span></span>|<span data-ttu-id="defaa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="defaa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="defaa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="defaa-127">Request body</span></span>
<span data-ttu-id="defaa-128">В теле запроса добавьте представление объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="defaa-128">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="defaa-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="defaa-129">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="defaa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="defaa-130">Property</span></span>|<span data-ttu-id="defaa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="defaa-131">Type</span></span>|<span data-ttu-id="defaa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="defaa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="defaa-133">id</span><span class="sxs-lookup"><span data-stu-id="defaa-133">id</span></span>|<span data-ttu-id="defaa-134">String</span><span class="sxs-lookup"><span data-stu-id="defaa-134">String</span></span>|<span data-ttu-id="defaa-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="defaa-135">Key of the entity.</span></span> <span data-ttu-id="defaa-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="defaa-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="defaa-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="defaa-137">lastModifiedDateTime</span></span>|<span data-ttu-id="defaa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="defaa-138">DateTimeOffset</span></span>|<span data-ttu-id="defaa-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="defaa-139">DateTime the object was last modified.</span></span> <span data-ttu-id="defaa-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="defaa-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="defaa-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="defaa-141">roleScopeTagIds</span></span>|<span data-ttu-id="defaa-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="defaa-142">String collection</span></span>|<span data-ttu-id="defaa-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="defaa-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="defaa-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="defaa-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="defaa-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="defaa-145">supportsScopeTags</span></span>|<span data-ttu-id="defaa-146">Логический</span><span class="sxs-lookup"><span data-stu-id="defaa-146">Boolean</span></span>|<span data-ttu-id="defaa-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="defaa-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="defaa-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="defaa-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="defaa-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="defaa-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="defaa-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="defaa-150">This property is read-only.</span></span> <span data-ttu-id="defaa-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="defaa-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="defaa-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="defaa-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="defaa-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="defaa-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="defaa-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="defaa-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="defaa-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="defaa-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="defaa-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="defaa-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="defaa-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="defaa-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="defaa-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="defaa-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="defaa-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="defaa-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="defaa-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="defaa-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="defaa-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="defaa-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="defaa-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="defaa-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="defaa-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="defaa-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="defaa-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="defaa-164">createdDateTime</span></span>|<span data-ttu-id="defaa-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="defaa-165">DateTimeOffset</span></span>|<span data-ttu-id="defaa-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="defaa-166">DateTime the object was created.</span></span> <span data-ttu-id="defaa-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="defaa-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="defaa-168">description</span><span class="sxs-lookup"><span data-stu-id="defaa-168">description</span></span>|<span data-ttu-id="defaa-169">String</span><span class="sxs-lookup"><span data-stu-id="defaa-169">String</span></span>|<span data-ttu-id="defaa-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="defaa-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="defaa-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="defaa-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="defaa-172">displayName</span><span class="sxs-lookup"><span data-stu-id="defaa-172">displayName</span></span>|<span data-ttu-id="defaa-173">String</span><span class="sxs-lookup"><span data-stu-id="defaa-173">String</span></span>|<span data-ttu-id="defaa-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="defaa-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="defaa-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="defaa-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="defaa-176">version</span><span class="sxs-lookup"><span data-stu-id="defaa-176">version</span></span>|<span data-ttu-id="defaa-177">Int32</span><span class="sxs-lookup"><span data-stu-id="defaa-177">Int32</span></span>|<span data-ttu-id="defaa-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="defaa-178">Version of the device configuration.</span></span> <span data-ttu-id="defaa-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="defaa-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="defaa-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="defaa-180">omaSettings</span></span>|<span data-ttu-id="defaa-181">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="defaa-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="defaa-182">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="defaa-182">OMA settings.</span></span> <span data-ttu-id="defaa-183">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="defaa-183">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="defaa-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="defaa-184">Response</span></span>
<span data-ttu-id="defaa-185">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="defaa-185">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="defaa-186">Пример</span><span class="sxs-lookup"><span data-stu-id="defaa-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="defaa-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="defaa-187">Request</span></span>
<span data-ttu-id="defaa-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="defaa-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1337

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
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "secretReferenceValueId": "Secret Reference Value Id value",
      "isEncrypted": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="defaa-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="defaa-189">Response</span></span>
<span data-ttu-id="defaa-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="defaa-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1509

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
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "secretReferenceValueId": "Secret Reference Value Id value",
      "isEncrypted": true
    }
  ]
}
```




