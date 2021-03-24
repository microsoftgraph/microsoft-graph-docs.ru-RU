---
title: Создание объекта androidCustomConfiguration
description: Создание объекта androidCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1494ad3d3bb26cb411232aa04f388faf4d6e362e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126754"
---
# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="c3502-103">Создание объекта androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="c3502-103">Create androidCustomConfiguration</span></span>

<span data-ttu-id="c3502-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3502-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3502-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3502-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3502-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3502-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3502-107">Создание объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3502-107">Create a new [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3502-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c3502-108">Prerequisites</span></span>
<span data-ttu-id="c3502-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3502-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3502-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3502-111">Permission type</span></span>|<span data-ttu-id="c3502-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3502-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3502-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3502-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3502-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3502-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c3502-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3502-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3502-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3502-116">Not supported.</span></span>|
|<span data-ttu-id="c3502-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c3502-117">Application</span></span>|<span data-ttu-id="c3502-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3502-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3502-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3502-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c3502-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c3502-120">Request headers</span></span>
|<span data-ttu-id="c3502-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3502-121">Header</span></span>|<span data-ttu-id="c3502-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c3502-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3502-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3502-123">Authorization</span></span>|<span data-ttu-id="c3502-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3502-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3502-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c3502-125">Accept</span></span>|<span data-ttu-id="c3502-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3502-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3502-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3502-127">Request body</span></span>
<span data-ttu-id="c3502-128">В тексте запроса добавьте представление объекта androidCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3502-128">In the request body, supply a JSON representation for the androidCustomConfiguration object.</span></span>

<span data-ttu-id="c3502-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c3502-129">The following table shows the properties that are required when you create the androidCustomConfiguration.</span></span>

|<span data-ttu-id="c3502-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3502-130">Property</span></span>|<span data-ttu-id="c3502-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c3502-131">Type</span></span>|<span data-ttu-id="c3502-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c3502-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3502-133">id</span><span class="sxs-lookup"><span data-stu-id="c3502-133">id</span></span>|<span data-ttu-id="c3502-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c3502-134">String</span></span>|<span data-ttu-id="c3502-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c3502-135">Key of the entity.</span></span> <span data-ttu-id="c3502-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3502-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3502-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3502-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c3502-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3502-138">DateTimeOffset</span></span>|<span data-ttu-id="c3502-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c3502-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c3502-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3502-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3502-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c3502-141">roleScopeTagIds</span></span>|<span data-ttu-id="c3502-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c3502-142">String collection</span></span>|<span data-ttu-id="c3502-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="c3502-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c3502-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3502-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3502-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c3502-145">supportsScopeTags</span></span>|<span data-ttu-id="c3502-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3502-146">Boolean</span></span>|<span data-ttu-id="c3502-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c3502-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c3502-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="c3502-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c3502-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c3502-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c3502-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3502-150">This property is read-only.</span></span> <span data-ttu-id="c3502-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3502-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3502-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c3502-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c3502-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c3502-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c3502-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c3502-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c3502-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3502-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3502-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c3502-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c3502-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c3502-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c3502-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c3502-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c3502-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3502-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3502-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c3502-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c3502-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c3502-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c3502-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c3502-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c3502-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3502-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3502-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3502-164">createdDateTime</span></span>|<span data-ttu-id="c3502-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3502-165">DateTimeOffset</span></span>|<span data-ttu-id="c3502-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c3502-166">DateTime the object was created.</span></span> <span data-ttu-id="c3502-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3502-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3502-168">description</span><span class="sxs-lookup"><span data-stu-id="c3502-168">description</span></span>|<span data-ttu-id="c3502-169">Строка</span><span class="sxs-lookup"><span data-stu-id="c3502-169">String</span></span>|<span data-ttu-id="c3502-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c3502-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c3502-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3502-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3502-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c3502-172">displayName</span></span>|<span data-ttu-id="c3502-173">Строка</span><span class="sxs-lookup"><span data-stu-id="c3502-173">String</span></span>|<span data-ttu-id="c3502-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c3502-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c3502-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3502-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3502-176">version</span><span class="sxs-lookup"><span data-stu-id="c3502-176">version</span></span>|<span data-ttu-id="c3502-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c3502-177">Int32</span></span>|<span data-ttu-id="c3502-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c3502-178">Version of the device configuration.</span></span> <span data-ttu-id="c3502-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3502-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3502-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="c3502-180">omaSettings</span></span>|<span data-ttu-id="c3502-181">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c3502-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="c3502-182">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="c3502-182">OMA settings.</span></span> <span data-ttu-id="c3502-183">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="c3502-183">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c3502-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3502-184">Response</span></span>
<span data-ttu-id="c3502-185">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3502-185">If successful, this method returns a `201 Created` response code and a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3502-186">Пример</span><span class="sxs-lookup"><span data-stu-id="c3502-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3502-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3502-187">Request</span></span>
<span data-ttu-id="c3502-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3502-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1269

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
      "isEncrypted": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c3502-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3502-189">Response</span></span>
<span data-ttu-id="c3502-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3502-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1441

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
      "isEncrypted": true
    }
  ]
}
```




