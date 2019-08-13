---
title: Создание объекта macOSCustomConfiguration
description: Создание объекта macOSCustomConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5a834a941f2f587ba139f2c51f7e886991e44748
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338884"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="fc099-103">Создание объекта macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="fc099-103">Create macOSCustomConfiguration</span></span>

> <span data-ttu-id="fc099-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc099-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc099-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc099-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc099-106">Создание объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc099-106">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc099-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fc099-107">Prerequisites</span></span>
<span data-ttu-id="fc099-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc099-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc099-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc099-110">Permission type</span></span>|<span data-ttu-id="fc099-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc099-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc099-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc099-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fc099-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc099-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fc099-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc099-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc099-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc099-115">Not supported.</span></span>|
|<span data-ttu-id="fc099-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc099-116">Application</span></span>|<span data-ttu-id="fc099-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc099-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc099-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc099-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fc099-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc099-119">Request headers</span></span>
|<span data-ttu-id="fc099-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc099-120">Header</span></span>|<span data-ttu-id="fc099-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fc099-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc099-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc099-122">Authorization</span></span>|<span data-ttu-id="fc099-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc099-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc099-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fc099-124">Accept</span></span>|<span data-ttu-id="fc099-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fc099-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc099-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fc099-126">Request body</span></span>
<span data-ttu-id="fc099-127">В теле запроса добавьте представление объекта macOSCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc099-127">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="fc099-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fc099-128">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="fc099-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc099-129">Property</span></span>|<span data-ttu-id="fc099-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fc099-130">Type</span></span>|<span data-ttu-id="fc099-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fc099-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc099-132">id</span><span class="sxs-lookup"><span data-stu-id="fc099-132">id</span></span>|<span data-ttu-id="fc099-133">Строка</span><span class="sxs-lookup"><span data-stu-id="fc099-133">String</span></span>|<span data-ttu-id="fc099-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fc099-134">Key of the entity.</span></span> <span data-ttu-id="fc099-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc099-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc099-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc099-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fc099-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc099-137">DateTimeOffset</span></span>|<span data-ttu-id="fc099-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fc099-138">DateTime the object was last modified.</span></span> <span data-ttu-id="fc099-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc099-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc099-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fc099-140">roleScopeTagIds</span></span>|<span data-ttu-id="fc099-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fc099-141">String collection</span></span>|<span data-ttu-id="fc099-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fc099-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fc099-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc099-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc099-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="fc099-144">supportsScopeTags</span></span>|<span data-ttu-id="fc099-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc099-145">Boolean</span></span>|<span data-ttu-id="fc099-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="fc099-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fc099-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="fc099-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fc099-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fc099-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fc099-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc099-149">This property is read-only.</span></span> <span data-ttu-id="fc099-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc099-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc099-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fc099-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fc099-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fc099-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fc099-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fc099-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fc099-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc099-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc099-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fc099-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fc099-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fc099-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fc099-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fc099-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fc099-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc099-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc099-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="fc099-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fc099-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="fc099-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fc099-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fc099-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fc099-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc099-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc099-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fc099-163">createdDateTime</span></span>|<span data-ttu-id="fc099-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc099-164">DateTimeOffset</span></span>|<span data-ttu-id="fc099-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fc099-165">DateTime the object was created.</span></span> <span data-ttu-id="fc099-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc099-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc099-167">description</span><span class="sxs-lookup"><span data-stu-id="fc099-167">description</span></span>|<span data-ttu-id="fc099-168">String</span><span class="sxs-lookup"><span data-stu-id="fc099-168">String</span></span>|<span data-ttu-id="fc099-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fc099-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fc099-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc099-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc099-171">displayName</span><span class="sxs-lookup"><span data-stu-id="fc099-171">displayName</span></span>|<span data-ttu-id="fc099-172">Строка</span><span class="sxs-lookup"><span data-stu-id="fc099-172">String</span></span>|<span data-ttu-id="fc099-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fc099-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fc099-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fc099-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc099-175">version</span><span class="sxs-lookup"><span data-stu-id="fc099-175">version</span></span>|<span data-ttu-id="fc099-176">Int32</span><span class="sxs-lookup"><span data-stu-id="fc099-176">Int32</span></span>|<span data-ttu-id="fc099-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fc099-177">Version of the device configuration.</span></span> <span data-ttu-id="fc099-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc099-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc099-179">payloadName</span><span class="sxs-lookup"><span data-stu-id="fc099-179">payloadName</span></span>|<span data-ttu-id="fc099-180">String</span><span class="sxs-lookup"><span data-stu-id="fc099-180">String</span></span>|<span data-ttu-id="fc099-181">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="fc099-181">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="fc099-182">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="fc099-182">payloadFileName</span></span>|<span data-ttu-id="fc099-183">String</span><span class="sxs-lookup"><span data-stu-id="fc099-183">String</span></span>|<span data-ttu-id="fc099-184">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="fc099-184">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="fc099-185">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="fc099-185">\*.xml).</span></span>|
|<span data-ttu-id="fc099-186">payload</span><span class="sxs-lookup"><span data-stu-id="fc099-186">payload</span></span>|<span data-ttu-id="fc099-187">Binary</span><span class="sxs-lookup"><span data-stu-id="fc099-187">Binary</span></span>|<span data-ttu-id="fc099-188">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="fc099-188">Payload.</span></span> <span data-ttu-id="fc099-189">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="fc099-189">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="fc099-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc099-190">Response</span></span>
<span data-ttu-id="fc099-191">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fc099-191">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc099-192">Пример</span><span class="sxs-lookup"><span data-stu-id="fc099-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc099-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc099-193">Request</span></span>
<span data-ttu-id="fc099-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc099-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1146

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
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
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="fc099-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc099-195">Response</span></span>
<span data-ttu-id="fc099-p114">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc099-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1318

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
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
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```






