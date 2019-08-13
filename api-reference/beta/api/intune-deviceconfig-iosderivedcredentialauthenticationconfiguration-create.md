---
title: Создание Иосдериведкредентиалаусентикатионконфигуратион
description: Создание нового объекта Иосдериведкредентиалаусентикатионконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d7f3c5d88da4d512599ce15af972bdb0d83995a3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36339556"
---
# <a name="create-iosderivedcredentialauthenticationconfiguration"></a><span data-ttu-id="01591-103">Создание Иосдериведкредентиалаусентикатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="01591-103">Create iosDerivedCredentialAuthenticationConfiguration</span></span>

> <span data-ttu-id="01591-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01591-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01591-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01591-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01591-106">Создание нового объекта [иосдериведкредентиалаусентикатионконфигуратион](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="01591-106">Create a new [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01591-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="01591-107">Prerequisites</span></span>
<span data-ttu-id="01591-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01591-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01591-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01591-110">Permission type</span></span>|<span data-ttu-id="01591-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01591-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01591-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01591-112">Delegated (work or school account)</span></span>|<span data-ttu-id="01591-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01591-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01591-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01591-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01591-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01591-115">Not supported.</span></span>|
|<span data-ttu-id="01591-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01591-116">Application</span></span>|<span data-ttu-id="01591-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01591-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01591-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01591-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="01591-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01591-119">Request headers</span></span>
|<span data-ttu-id="01591-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01591-120">Header</span></span>|<span data-ttu-id="01591-121">Значение</span><span class="sxs-lookup"><span data-stu-id="01591-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01591-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01591-122">Authorization</span></span>|<span data-ttu-id="01591-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01591-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01591-124">Accept</span><span class="sxs-lookup"><span data-stu-id="01591-124">Accept</span></span>|<span data-ttu-id="01591-125">application/json</span><span class="sxs-lookup"><span data-stu-id="01591-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01591-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01591-126">Request body</span></span>
<span data-ttu-id="01591-127">В тексте запроса добавьте представление объекта Иосдериведкредентиалаусентикатионконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01591-127">In the request body, supply a JSON representation for the iosDerivedCredentialAuthenticationConfiguration object.</span></span>

<span data-ttu-id="01591-128">В следующей таблице приведены свойства, необходимые при создании Иосдериведкредентиалаусентикатионконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="01591-128">The following table shows the properties that are required when you create the iosDerivedCredentialAuthenticationConfiguration.</span></span>

|<span data-ttu-id="01591-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="01591-129">Property</span></span>|<span data-ttu-id="01591-130">Тип</span><span class="sxs-lookup"><span data-stu-id="01591-130">Type</span></span>|<span data-ttu-id="01591-131">Описание</span><span class="sxs-lookup"><span data-stu-id="01591-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01591-132">id</span><span class="sxs-lookup"><span data-stu-id="01591-132">id</span></span>|<span data-ttu-id="01591-133">String</span><span class="sxs-lookup"><span data-stu-id="01591-133">String</span></span>|<span data-ttu-id="01591-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="01591-134">Key of the entity.</span></span> <span data-ttu-id="01591-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01591-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01591-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01591-136">lastModifiedDateTime</span></span>|<span data-ttu-id="01591-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01591-137">DateTimeOffset</span></span>|<span data-ttu-id="01591-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="01591-138">DateTime the object was last modified.</span></span> <span data-ttu-id="01591-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01591-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01591-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="01591-140">roleScopeTagIds</span></span>|<span data-ttu-id="01591-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="01591-141">String collection</span></span>|<span data-ttu-id="01591-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="01591-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="01591-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01591-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01591-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="01591-144">supportsScopeTags</span></span>|<span data-ttu-id="01591-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="01591-145">Boolean</span></span>|<span data-ttu-id="01591-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="01591-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="01591-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="01591-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="01591-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="01591-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="01591-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01591-149">This property is read-only.</span></span> <span data-ttu-id="01591-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01591-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01591-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="01591-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="01591-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="01591-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="01591-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="01591-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="01591-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01591-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01591-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="01591-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="01591-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="01591-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="01591-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="01591-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="01591-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01591-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01591-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="01591-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="01591-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="01591-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="01591-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="01591-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="01591-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01591-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01591-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="01591-163">createdDateTime</span></span>|<span data-ttu-id="01591-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01591-164">DateTimeOffset</span></span>|<span data-ttu-id="01591-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="01591-165">DateTime the object was created.</span></span> <span data-ttu-id="01591-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01591-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01591-167">description</span><span class="sxs-lookup"><span data-stu-id="01591-167">description</span></span>|<span data-ttu-id="01591-168">String</span><span class="sxs-lookup"><span data-stu-id="01591-168">String</span></span>|<span data-ttu-id="01591-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="01591-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="01591-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01591-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01591-171">displayName</span><span class="sxs-lookup"><span data-stu-id="01591-171">displayName</span></span>|<span data-ttu-id="01591-172">Строка</span><span class="sxs-lookup"><span data-stu-id="01591-172">String</span></span>|<span data-ttu-id="01591-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="01591-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="01591-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01591-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01591-175">version</span><span class="sxs-lookup"><span data-stu-id="01591-175">version</span></span>|<span data-ttu-id="01591-176">Int32</span><span class="sxs-lookup"><span data-stu-id="01591-176">Int32</span></span>|<span data-ttu-id="01591-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="01591-177">Version of the device configuration.</span></span> <span data-ttu-id="01591-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01591-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="01591-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="01591-179">Response</span></span>
<span data-ttu-id="01591-180">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иосдериведкредентиалаусентикатионконфигуратион](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01591-180">If successful, this method returns a `201 Created` response code and a [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01591-181">Пример</span><span class="sxs-lookup"><span data-stu-id="01591-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="01591-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="01591-182">Request</span></span>
<span data-ttu-id="01591-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01591-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1050

{
  "@odata.type": "#microsoft.graph.iosDerivedCredentialAuthenticationConfiguration",
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
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="01591-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="01591-184">Response</span></span>
<span data-ttu-id="01591-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01591-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1222

{
  "@odata.type": "#microsoft.graph.iosDerivedCredentialAuthenticationConfiguration",
  "id": "01713f58-3f58-0171-583f-7101583f7101",
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
  "version": 7
}
```






