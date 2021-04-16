---
title: Обновление androidForWorkCustomConfiguration
description: Обновление свойств объекта AndroidForWorkCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a91912f9386fde0c3d67d9a6e46f39abff173762
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867240"
---
# <a name="update-androidforworkcustomconfiguration"></a><span data-ttu-id="aee4f-103">Обновление androidForWorkCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="aee4f-103">Update androidForWorkCustomConfiguration</span></span>

<span data-ttu-id="aee4f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aee4f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aee4f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aee4f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aee4f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aee4f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aee4f-107">Обновление свойств объекта [AndroidForWorkCustomConfiguration.](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aee4f-107">Update the properties of a [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aee4f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aee4f-108">Prerequisites</span></span>
<span data-ttu-id="aee4f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aee4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aee4f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aee4f-111">Permission type</span></span>|<span data-ttu-id="aee4f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aee4f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aee4f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aee4f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aee4f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aee4f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aee4f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aee4f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aee4f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aee4f-116">Not supported.</span></span>|
|<span data-ttu-id="aee4f-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="aee4f-117">Application</span></span>|<span data-ttu-id="aee4f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aee4f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aee4f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aee4f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="aee4f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aee4f-120">Request headers</span></span>
|<span data-ttu-id="aee4f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aee4f-121">Header</span></span>|<span data-ttu-id="aee4f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aee4f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aee4f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aee4f-123">Authorization</span></span>|<span data-ttu-id="aee4f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aee4f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aee4f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aee4f-125">Accept</span></span>|<span data-ttu-id="aee4f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aee4f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aee4f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aee4f-127">Request body</span></span>
<span data-ttu-id="aee4f-128">В теле запроса предоставляем представление JSON для [объекта AndroidForWorkCustomConfiguration.](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aee4f-128">In the request body, supply a JSON representation for the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>

<span data-ttu-id="aee4f-129">В следующей таблице показаны свойства, необходимые при создании [androidForWorkCustomConfiguration.](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aee4f-129">The following table shows the properties that are required when you create the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md).</span></span>

|<span data-ttu-id="aee4f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="aee4f-130">Property</span></span>|<span data-ttu-id="aee4f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="aee4f-131">Type</span></span>|<span data-ttu-id="aee4f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="aee4f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aee4f-133">id</span><span class="sxs-lookup"><span data-stu-id="aee4f-133">id</span></span>|<span data-ttu-id="aee4f-134">String</span><span class="sxs-lookup"><span data-stu-id="aee4f-134">String</span></span>|<span data-ttu-id="aee4f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="aee4f-135">Key of the entity.</span></span> <span data-ttu-id="aee4f-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aee4f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee4f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aee4f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="aee4f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aee4f-138">DateTimeOffset</span></span>|<span data-ttu-id="aee4f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="aee4f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="aee4f-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aee4f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee4f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aee4f-141">roleScopeTagIds</span></span>|<span data-ttu-id="aee4f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="aee4f-142">String collection</span></span>|<span data-ttu-id="aee4f-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="aee4f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aee4f-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aee4f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee4f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="aee4f-145">supportsScopeTags</span></span>|<span data-ttu-id="aee4f-146">Логический</span><span class="sxs-lookup"><span data-stu-id="aee4f-146">Boolean</span></span>|<span data-ttu-id="aee4f-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="aee4f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="aee4f-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="aee4f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="aee4f-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="aee4f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="aee4f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aee4f-150">This property is read-only.</span></span> <span data-ttu-id="aee4f-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aee4f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee4f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="aee4f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="aee4f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="aee4f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="aee4f-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="aee4f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="aee4f-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aee4f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee4f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="aee4f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="aee4f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="aee4f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="aee4f-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="aee4f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="aee4f-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aee4f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee4f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="aee4f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="aee4f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="aee4f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="aee4f-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="aee4f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="aee4f-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aee4f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee4f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aee4f-164">createdDateTime</span></span>|<span data-ttu-id="aee4f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aee4f-165">DateTimeOffset</span></span>|<span data-ttu-id="aee4f-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="aee4f-166">DateTime the object was created.</span></span> <span data-ttu-id="aee4f-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aee4f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee4f-168">description</span><span class="sxs-lookup"><span data-stu-id="aee4f-168">description</span></span>|<span data-ttu-id="aee4f-169">String</span><span class="sxs-lookup"><span data-stu-id="aee4f-169">String</span></span>|<span data-ttu-id="aee4f-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aee4f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aee4f-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aee4f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee4f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="aee4f-172">displayName</span></span>|<span data-ttu-id="aee4f-173">String</span><span class="sxs-lookup"><span data-stu-id="aee4f-173">String</span></span>|<span data-ttu-id="aee4f-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aee4f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aee4f-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aee4f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee4f-176">version</span><span class="sxs-lookup"><span data-stu-id="aee4f-176">version</span></span>|<span data-ttu-id="aee4f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="aee4f-177">Int32</span></span>|<span data-ttu-id="aee4f-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="aee4f-178">Version of the device configuration.</span></span> <span data-ttu-id="aee4f-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aee4f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aee4f-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="aee4f-180">omaSettings</span></span>|<span data-ttu-id="aee4f-181">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="aee4f-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="aee4f-182">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="aee4f-182">OMA settings.</span></span> <span data-ttu-id="aee4f-183">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="aee4f-183">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="aee4f-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="aee4f-184">Response</span></span>
<span data-ttu-id="aee4f-185">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект AndroidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="aee4f-185">If successful, this method returns a `200 OK` response code and an updated [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aee4f-186">Пример</span><span class="sxs-lookup"><span data-stu-id="aee4f-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="aee4f-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="aee4f-187">Request</span></span>
<span data-ttu-id="aee4f-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aee4f-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1344

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="aee4f-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="aee4f-189">Response</span></span>
<span data-ttu-id="aee4f-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aee4f-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1516

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
  "id": "cca8b2bb-b2bb-cca8-bbb2-a8ccbbb2a8cc",
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




