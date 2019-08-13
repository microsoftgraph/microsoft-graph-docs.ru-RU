---
title: Создание объекта windows10CustomConfiguration
description: Создание объекта windows10CustomConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 209c312680052f3b514c4d8e5a83c53513e9964e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345381"
---
# <a name="create-windows10customconfiguration"></a><span data-ttu-id="ba9ad-103">Создание объекта windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba9ad-103">Create windows10CustomConfiguration</span></span>

> <span data-ttu-id="ba9ad-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba9ad-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba9ad-106">Создание объекта [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba9ad-106">Create a new [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba9ad-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ba9ad-107">Prerequisites</span></span>
<span data-ttu-id="ba9ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba9ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba9ad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba9ad-110">Permission type</span></span>|<span data-ttu-id="ba9ad-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba9ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba9ad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba9ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba9ad-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba9ad-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ba9ad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba9ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba9ad-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-115">Not supported.</span></span>|
|<span data-ttu-id="ba9ad-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba9ad-116">Application</span></span>|<span data-ttu-id="ba9ad-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba9ad-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba9ad-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba9ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ba9ad-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba9ad-119">Request headers</span></span>
|<span data-ttu-id="ba9ad-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba9ad-120">Header</span></span>|<span data-ttu-id="ba9ad-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ba9ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba9ad-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba9ad-122">Authorization</span></span>|<span data-ttu-id="ba9ad-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba9ad-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ba9ad-124">Accept</span></span>|<span data-ttu-id="ba9ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba9ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba9ad-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ba9ad-126">Request body</span></span>
<span data-ttu-id="ba9ad-127">В тексте запроса добавьте представление объекта windows10CustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-127">In the request body, supply a JSON representation for the windows10CustomConfiguration object.</span></span>

<span data-ttu-id="ba9ad-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта windows10CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-128">The following table shows the properties that are required when you create the windows10CustomConfiguration.</span></span>

|<span data-ttu-id="ba9ad-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba9ad-129">Property</span></span>|<span data-ttu-id="ba9ad-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ba9ad-130">Type</span></span>|<span data-ttu-id="ba9ad-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ba9ad-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba9ad-132">id</span><span class="sxs-lookup"><span data-stu-id="ba9ad-132">id</span></span>|<span data-ttu-id="ba9ad-133">String</span><span class="sxs-lookup"><span data-stu-id="ba9ad-133">String</span></span>|<span data-ttu-id="ba9ad-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-134">Key of the entity.</span></span> <span data-ttu-id="ba9ad-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba9ad-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba9ad-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba9ad-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ba9ad-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba9ad-137">DateTimeOffset</span></span>|<span data-ttu-id="ba9ad-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ba9ad-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba9ad-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba9ad-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ba9ad-140">roleScopeTagIds</span></span>|<span data-ttu-id="ba9ad-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ba9ad-141">String collection</span></span>|<span data-ttu-id="ba9ad-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ba9ad-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba9ad-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba9ad-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="ba9ad-144">supportsScopeTags</span></span>|<span data-ttu-id="ba9ad-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba9ad-145">Boolean</span></span>|<span data-ttu-id="ba9ad-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ba9ad-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ba9ad-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ba9ad-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-149">This property is read-only.</span></span> <span data-ttu-id="ba9ad-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba9ad-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba9ad-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ba9ad-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ba9ad-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ba9ad-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ba9ad-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ba9ad-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba9ad-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba9ad-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ba9ad-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ba9ad-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ba9ad-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ba9ad-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ba9ad-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba9ad-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba9ad-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="ba9ad-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ba9ad-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="ba9ad-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ba9ad-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ba9ad-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba9ad-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba9ad-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ba9ad-163">createdDateTime</span></span>|<span data-ttu-id="ba9ad-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba9ad-164">DateTimeOffset</span></span>|<span data-ttu-id="ba9ad-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-165">DateTime the object was created.</span></span> <span data-ttu-id="ba9ad-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba9ad-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba9ad-167">description</span><span class="sxs-lookup"><span data-stu-id="ba9ad-167">description</span></span>|<span data-ttu-id="ba9ad-168">String</span><span class="sxs-lookup"><span data-stu-id="ba9ad-168">String</span></span>|<span data-ttu-id="ba9ad-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ba9ad-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba9ad-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba9ad-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ba9ad-171">displayName</span></span>|<span data-ttu-id="ba9ad-172">Строка</span><span class="sxs-lookup"><span data-stu-id="ba9ad-172">String</span></span>|<span data-ttu-id="ba9ad-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ba9ad-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba9ad-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba9ad-175">version</span><span class="sxs-lookup"><span data-stu-id="ba9ad-175">version</span></span>|<span data-ttu-id="ba9ad-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ba9ad-176">Int32</span></span>|<span data-ttu-id="ba9ad-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-177">Version of the device configuration.</span></span> <span data-ttu-id="ba9ad-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba9ad-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba9ad-179">omaSettings</span><span class="sxs-lookup"><span data-stu-id="ba9ad-179">omaSettings</span></span>|<span data-ttu-id="ba9ad-180">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ba9ad-180">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="ba9ad-181">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-181">OMA settings.</span></span> <span data-ttu-id="ba9ad-182">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-182">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ba9ad-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba9ad-183">Response</span></span>
<span data-ttu-id="ba9ad-184">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-184">If successful, this method returns a `201 Created` response code and a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba9ad-185">Пример</span><span class="sxs-lookup"><span data-stu-id="ba9ad-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba9ad-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba9ad-186">Request</span></span>
<span data-ttu-id="ba9ad-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1296

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

### <a name="response"></a><span data-ttu-id="ba9ad-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba9ad-188">Response</span></span>
<span data-ttu-id="ba9ad-p114">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1468

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






