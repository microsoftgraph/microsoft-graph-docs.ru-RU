---
title: Создание объекта windows10CustomConfiguration
description: Создание объекта windows10CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 852acc9dc765aed27d413eb9a61e5479e15468a2
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866512"
---
# <a name="create-windows10customconfiguration"></a><span data-ttu-id="459bb-103">Создание объекта windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="459bb-103">Create windows10CustomConfiguration</span></span>

<span data-ttu-id="459bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="459bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="459bb-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="459bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="459bb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="459bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="459bb-107">Создание объекта [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="459bb-107">Create a new [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="459bb-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="459bb-108">Prerequisites</span></span>
<span data-ttu-id="459bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="459bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="459bb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="459bb-111">Permission type</span></span>|<span data-ttu-id="459bb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="459bb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="459bb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="459bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="459bb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="459bb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="459bb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="459bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="459bb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="459bb-116">Not supported.</span></span>|
|<span data-ttu-id="459bb-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="459bb-117">Application</span></span>|<span data-ttu-id="459bb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="459bb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="459bb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="459bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="459bb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="459bb-120">Request headers</span></span>
|<span data-ttu-id="459bb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="459bb-121">Header</span></span>|<span data-ttu-id="459bb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="459bb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="459bb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="459bb-123">Authorization</span></span>|<span data-ttu-id="459bb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="459bb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="459bb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="459bb-125">Accept</span></span>|<span data-ttu-id="459bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="459bb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="459bb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="459bb-127">Request body</span></span>
<span data-ttu-id="459bb-128">В тексте запроса добавьте представление объекта windows10CustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="459bb-128">In the request body, supply a JSON representation for the windows10CustomConfiguration object.</span></span>

<span data-ttu-id="459bb-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта windows10CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="459bb-129">The following table shows the properties that are required when you create the windows10CustomConfiguration.</span></span>

|<span data-ttu-id="459bb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="459bb-130">Property</span></span>|<span data-ttu-id="459bb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="459bb-131">Type</span></span>|<span data-ttu-id="459bb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="459bb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="459bb-133">id</span><span class="sxs-lookup"><span data-stu-id="459bb-133">id</span></span>|<span data-ttu-id="459bb-134">String</span><span class="sxs-lookup"><span data-stu-id="459bb-134">String</span></span>|<span data-ttu-id="459bb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="459bb-135">Key of the entity.</span></span> <span data-ttu-id="459bb-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="459bb-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="459bb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="459bb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="459bb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="459bb-138">DateTimeOffset</span></span>|<span data-ttu-id="459bb-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="459bb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="459bb-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="459bb-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="459bb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="459bb-141">roleScopeTagIds</span></span>|<span data-ttu-id="459bb-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="459bb-142">String collection</span></span>|<span data-ttu-id="459bb-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="459bb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="459bb-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="459bb-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="459bb-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="459bb-145">supportsScopeTags</span></span>|<span data-ttu-id="459bb-146">Логический</span><span class="sxs-lookup"><span data-stu-id="459bb-146">Boolean</span></span>|<span data-ttu-id="459bb-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="459bb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="459bb-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="459bb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="459bb-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="459bb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="459bb-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="459bb-150">This property is read-only.</span></span> <span data-ttu-id="459bb-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="459bb-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="459bb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="459bb-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="459bb-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="459bb-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="459bb-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="459bb-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="459bb-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="459bb-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="459bb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="459bb-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="459bb-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="459bb-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="459bb-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="459bb-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="459bb-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="459bb-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="459bb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="459bb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="459bb-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="459bb-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="459bb-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="459bb-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="459bb-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="459bb-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="459bb-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="459bb-164">createdDateTime</span></span>|<span data-ttu-id="459bb-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="459bb-165">DateTimeOffset</span></span>|<span data-ttu-id="459bb-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="459bb-166">DateTime the object was created.</span></span> <span data-ttu-id="459bb-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="459bb-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="459bb-168">description</span><span class="sxs-lookup"><span data-stu-id="459bb-168">description</span></span>|<span data-ttu-id="459bb-169">String</span><span class="sxs-lookup"><span data-stu-id="459bb-169">String</span></span>|<span data-ttu-id="459bb-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="459bb-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="459bb-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="459bb-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="459bb-172">displayName</span><span class="sxs-lookup"><span data-stu-id="459bb-172">displayName</span></span>|<span data-ttu-id="459bb-173">String</span><span class="sxs-lookup"><span data-stu-id="459bb-173">String</span></span>|<span data-ttu-id="459bb-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="459bb-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="459bb-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="459bb-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="459bb-176">version</span><span class="sxs-lookup"><span data-stu-id="459bb-176">version</span></span>|<span data-ttu-id="459bb-177">Int32</span><span class="sxs-lookup"><span data-stu-id="459bb-177">Int32</span></span>|<span data-ttu-id="459bb-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="459bb-178">Version of the device configuration.</span></span> <span data-ttu-id="459bb-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="459bb-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="459bb-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="459bb-180">omaSettings</span></span>|<span data-ttu-id="459bb-181">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="459bb-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="459bb-182">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="459bb-182">OMA settings.</span></span> <span data-ttu-id="459bb-183">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="459bb-183">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="459bb-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="459bb-184">Response</span></span>
<span data-ttu-id="459bb-185">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="459bb-185">If successful, this method returns a `201 Created` response code and a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="459bb-186">Пример</span><span class="sxs-lookup"><span data-stu-id="459bb-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="459bb-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="459bb-187">Request</span></span>
<span data-ttu-id="459bb-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="459bb-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1339

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="459bb-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="459bb-189">Response</span></span>
<span data-ttu-id="459bb-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="459bb-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1511

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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




