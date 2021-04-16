---
title: Создание androidForWorkCustomConfiguration
description: Создайте новый объект AndroidForWorkCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cb0a2947da86b346c8d4f5d365385c072f246b77
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865350"
---
# <a name="create-androidforworkcustomconfiguration"></a><span data-ttu-id="92b45-103">Создание androidForWorkCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="92b45-103">Create androidForWorkCustomConfiguration</span></span>

<span data-ttu-id="92b45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92b45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92b45-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92b45-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92b45-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92b45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92b45-107">Создайте новый [объект AndroidForWorkCustomConfiguration.](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92b45-107">Create a new [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92b45-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="92b45-108">Prerequisites</span></span>
<span data-ttu-id="92b45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92b45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92b45-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92b45-111">Permission type</span></span>|<span data-ttu-id="92b45-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="92b45-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92b45-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92b45-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92b45-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92b45-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92b45-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92b45-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92b45-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92b45-116">Not supported.</span></span>|
|<span data-ttu-id="92b45-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="92b45-117">Application</span></span>|<span data-ttu-id="92b45-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92b45-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92b45-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92b45-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="92b45-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="92b45-120">Request headers</span></span>
|<span data-ttu-id="92b45-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92b45-121">Header</span></span>|<span data-ttu-id="92b45-122">Значение</span><span class="sxs-lookup"><span data-stu-id="92b45-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92b45-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92b45-123">Authorization</span></span>|<span data-ttu-id="92b45-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92b45-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92b45-125">Accept</span><span class="sxs-lookup"><span data-stu-id="92b45-125">Accept</span></span>|<span data-ttu-id="92b45-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92b45-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92b45-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92b45-127">Request body</span></span>
<span data-ttu-id="92b45-128">В теле запроса предоставляем представление JSON для объекта AndroidForWorkCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="92b45-128">In the request body, supply a JSON representation for the androidForWorkCustomConfiguration object.</span></span>

<span data-ttu-id="92b45-129">В следующей таблице показаны свойства, необходимые при создании androidForWorkCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="92b45-129">The following table shows the properties that are required when you create the androidForWorkCustomConfiguration.</span></span>

|<span data-ttu-id="92b45-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="92b45-130">Property</span></span>|<span data-ttu-id="92b45-131">Тип</span><span class="sxs-lookup"><span data-stu-id="92b45-131">Type</span></span>|<span data-ttu-id="92b45-132">Описание</span><span class="sxs-lookup"><span data-stu-id="92b45-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92b45-133">id</span><span class="sxs-lookup"><span data-stu-id="92b45-133">id</span></span>|<span data-ttu-id="92b45-134">String</span><span class="sxs-lookup"><span data-stu-id="92b45-134">String</span></span>|<span data-ttu-id="92b45-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="92b45-135">Key of the entity.</span></span> <span data-ttu-id="92b45-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92b45-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92b45-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92b45-137">lastModifiedDateTime</span></span>|<span data-ttu-id="92b45-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92b45-138">DateTimeOffset</span></span>|<span data-ttu-id="92b45-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="92b45-139">DateTime the object was last modified.</span></span> <span data-ttu-id="92b45-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92b45-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92b45-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="92b45-141">roleScopeTagIds</span></span>|<span data-ttu-id="92b45-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="92b45-142">String collection</span></span>|<span data-ttu-id="92b45-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="92b45-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="92b45-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92b45-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92b45-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="92b45-145">supportsScopeTags</span></span>|<span data-ttu-id="92b45-146">Логический</span><span class="sxs-lookup"><span data-stu-id="92b45-146">Boolean</span></span>|<span data-ttu-id="92b45-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="92b45-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="92b45-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="92b45-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="92b45-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="92b45-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="92b45-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92b45-150">This property is read-only.</span></span> <span data-ttu-id="92b45-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92b45-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92b45-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="92b45-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="92b45-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="92b45-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="92b45-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="92b45-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="92b45-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92b45-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92b45-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="92b45-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="92b45-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="92b45-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="92b45-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="92b45-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="92b45-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92b45-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92b45-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="92b45-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="92b45-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="92b45-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="92b45-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="92b45-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="92b45-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92b45-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92b45-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92b45-164">createdDateTime</span></span>|<span data-ttu-id="92b45-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92b45-165">DateTimeOffset</span></span>|<span data-ttu-id="92b45-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="92b45-166">DateTime the object was created.</span></span> <span data-ttu-id="92b45-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92b45-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92b45-168">description</span><span class="sxs-lookup"><span data-stu-id="92b45-168">description</span></span>|<span data-ttu-id="92b45-169">String</span><span class="sxs-lookup"><span data-stu-id="92b45-169">String</span></span>|<span data-ttu-id="92b45-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="92b45-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="92b45-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92b45-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92b45-172">displayName</span><span class="sxs-lookup"><span data-stu-id="92b45-172">displayName</span></span>|<span data-ttu-id="92b45-173">String</span><span class="sxs-lookup"><span data-stu-id="92b45-173">String</span></span>|<span data-ttu-id="92b45-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="92b45-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="92b45-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92b45-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92b45-176">version</span><span class="sxs-lookup"><span data-stu-id="92b45-176">version</span></span>|<span data-ttu-id="92b45-177">Int32</span><span class="sxs-lookup"><span data-stu-id="92b45-177">Int32</span></span>|<span data-ttu-id="92b45-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="92b45-178">Version of the device configuration.</span></span> <span data-ttu-id="92b45-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92b45-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92b45-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="92b45-180">omaSettings</span></span>|<span data-ttu-id="92b45-181">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="92b45-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="92b45-182">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="92b45-182">OMA settings.</span></span> <span data-ttu-id="92b45-183">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="92b45-183">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="92b45-184">Ответ</span><span class="sxs-lookup"><span data-stu-id="92b45-184">Response</span></span>
<span data-ttu-id="92b45-185">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект AndroidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="92b45-185">If successful, this method returns a `201 Created` response code and a [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92b45-186">Пример</span><span class="sxs-lookup"><span data-stu-id="92b45-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="92b45-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="92b45-187">Request</span></span>
<span data-ttu-id="92b45-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92b45-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="92b45-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="92b45-189">Response</span></span>
<span data-ttu-id="92b45-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92b45-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




