---
title: Создание объекта windowsPhone81CustomConfiguration
description: Создание объекта windowsPhone81CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 20bdb9b445f34b28476753544d676c7ca5009230
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735612"
---
# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="5d953-103">Создание объекта windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="5d953-103">Create windowsPhone81CustomConfiguration</span></span>

<span data-ttu-id="5d953-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d953-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d953-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d953-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d953-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d953-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d953-107">Создание объекта [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5d953-107">Create a new [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d953-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5d953-108">Prerequisites</span></span>
<span data-ttu-id="5d953-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d953-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d953-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d953-111">Permission type</span></span>|<span data-ttu-id="5d953-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d953-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d953-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d953-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5d953-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d953-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5d953-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d953-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d953-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d953-116">Not supported.</span></span>|
|<span data-ttu-id="5d953-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d953-117">Application</span></span>|<span data-ttu-id="5d953-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d953-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d953-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d953-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5d953-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5d953-120">Request headers</span></span>
|<span data-ttu-id="5d953-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5d953-121">Header</span></span>|<span data-ttu-id="5d953-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5d953-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d953-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d953-123">Authorization</span></span>|<span data-ttu-id="5d953-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d953-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d953-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5d953-125">Accept</span></span>|<span data-ttu-id="5d953-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5d953-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d953-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5d953-127">Request body</span></span>
<span data-ttu-id="5d953-128">В теле запроса добавьте представление объекта windowsPhone81CustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d953-128">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="5d953-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsPhone81CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5d953-129">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="5d953-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d953-130">Property</span></span>|<span data-ttu-id="5d953-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5d953-131">Type</span></span>|<span data-ttu-id="5d953-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5d953-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d953-133">id</span><span class="sxs-lookup"><span data-stu-id="5d953-133">id</span></span>|<span data-ttu-id="5d953-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5d953-134">String</span></span>|<span data-ttu-id="5d953-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5d953-135">Key of the entity.</span></span> <span data-ttu-id="5d953-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5d953-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d953-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5d953-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5d953-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d953-138">DateTimeOffset</span></span>|<span data-ttu-id="5d953-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5d953-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5d953-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5d953-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d953-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5d953-141">roleScopeTagIds</span></span>|<span data-ttu-id="5d953-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5d953-142">String collection</span></span>|<span data-ttu-id="5d953-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5d953-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5d953-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5d953-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d953-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="5d953-145">supportsScopeTags</span></span>|<span data-ttu-id="5d953-146">Логический</span><span class="sxs-lookup"><span data-stu-id="5d953-146">Boolean</span></span>|<span data-ttu-id="5d953-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="5d953-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5d953-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="5d953-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5d953-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5d953-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5d953-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5d953-150">This property is read-only.</span></span> <span data-ttu-id="5d953-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5d953-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d953-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5d953-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5d953-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5d953-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5d953-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5d953-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5d953-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5d953-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d953-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5d953-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5d953-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5d953-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5d953-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5d953-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5d953-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5d953-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d953-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5d953-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5d953-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5d953-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5d953-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5d953-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5d953-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5d953-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d953-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5d953-164">createdDateTime</span></span>|<span data-ttu-id="5d953-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d953-165">DateTimeOffset</span></span>|<span data-ttu-id="5d953-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5d953-166">DateTime the object was created.</span></span> <span data-ttu-id="5d953-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5d953-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d953-168">description</span><span class="sxs-lookup"><span data-stu-id="5d953-168">description</span></span>|<span data-ttu-id="5d953-169">Строка</span><span class="sxs-lookup"><span data-stu-id="5d953-169">String</span></span>|<span data-ttu-id="5d953-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5d953-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5d953-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5d953-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d953-172">displayName</span><span class="sxs-lookup"><span data-stu-id="5d953-172">displayName</span></span>|<span data-ttu-id="5d953-173">Строка</span><span class="sxs-lookup"><span data-stu-id="5d953-173">String</span></span>|<span data-ttu-id="5d953-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5d953-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5d953-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5d953-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d953-176">version</span><span class="sxs-lookup"><span data-stu-id="5d953-176">version</span></span>|<span data-ttu-id="5d953-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5d953-177">Int32</span></span>|<span data-ttu-id="5d953-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5d953-178">Version of the device configuration.</span></span> <span data-ttu-id="5d953-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5d953-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5d953-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="5d953-180">omaSettings</span></span>|<span data-ttu-id="5d953-181">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5d953-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="5d953-182">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="5d953-182">OMA settings.</span></span> <span data-ttu-id="5d953-183">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="5d953-183">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="5d953-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d953-184">Response</span></span>
<span data-ttu-id="5d953-185">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5d953-185">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d953-186">Пример</span><span class="sxs-lookup"><span data-stu-id="5d953-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d953-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d953-187">Request</span></span>
<span data-ttu-id="5d953-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d953-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1248

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
      "omaUri": "Oma Uri value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="5d953-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d953-189">Response</span></span>
<span data-ttu-id="5d953-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5d953-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1420

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
      "omaUri": "Oma Uri value"
    }
  ]
}
```





