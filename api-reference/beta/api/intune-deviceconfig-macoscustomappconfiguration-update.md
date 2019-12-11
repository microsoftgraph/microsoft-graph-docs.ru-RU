---
title: Обновление Макоскустомаппконфигуратион
description: Обновление свойств объекта Макоскустомаппконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3a5b7ce29aef8736f7e4017ea1ac6a316e830a6b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948468"
---
# <a name="update-macoscustomappconfiguration"></a><span data-ttu-id="36cbe-103">Обновление Макоскустомаппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="36cbe-103">Update macOSCustomAppConfiguration</span></span>

> <span data-ttu-id="36cbe-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36cbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36cbe-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36cbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36cbe-106">Обновление свойств объекта [макоскустомаппконфигуратион](../resources/intune-deviceconfig-macoscustomappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="36cbe-106">Update the properties of a [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36cbe-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="36cbe-107">Prerequisites</span></span>
<span data-ttu-id="36cbe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36cbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36cbe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36cbe-110">Permission type</span></span>|<span data-ttu-id="36cbe-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="36cbe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36cbe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36cbe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36cbe-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36cbe-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="36cbe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36cbe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36cbe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36cbe-115">Not supported.</span></span>|
|<span data-ttu-id="36cbe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36cbe-116">Application</span></span>|<span data-ttu-id="36cbe-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36cbe-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36cbe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36cbe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="36cbe-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="36cbe-119">Request headers</span></span>
|<span data-ttu-id="36cbe-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36cbe-120">Header</span></span>|<span data-ttu-id="36cbe-121">Значение</span><span class="sxs-lookup"><span data-stu-id="36cbe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36cbe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36cbe-122">Authorization</span></span>|<span data-ttu-id="36cbe-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36cbe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36cbe-124">Accept</span><span class="sxs-lookup"><span data-stu-id="36cbe-124">Accept</span></span>|<span data-ttu-id="36cbe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36cbe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36cbe-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="36cbe-126">Request body</span></span>
<span data-ttu-id="36cbe-127">В тексте запроса добавьте представление объекта [макоскустомаппконфигуратион](../resources/intune-deviceconfig-macoscustomappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36cbe-127">In the request body, supply a JSON representation for the [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object.</span></span>

<span data-ttu-id="36cbe-128">В следующей таблице приведены свойства, необходимые при создании [макоскустомаппконфигуратион](../resources/intune-deviceconfig-macoscustomappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36cbe-128">The following table shows the properties that are required when you create the [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md).</span></span>

|<span data-ttu-id="36cbe-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="36cbe-129">Property</span></span>|<span data-ttu-id="36cbe-130">Тип</span><span class="sxs-lookup"><span data-stu-id="36cbe-130">Type</span></span>|<span data-ttu-id="36cbe-131">Описание</span><span class="sxs-lookup"><span data-stu-id="36cbe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36cbe-132">id</span><span class="sxs-lookup"><span data-stu-id="36cbe-132">id</span></span>|<span data-ttu-id="36cbe-133">Строка</span><span class="sxs-lookup"><span data-stu-id="36cbe-133">String</span></span>|<span data-ttu-id="36cbe-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="36cbe-134">Key of the entity.</span></span> <span data-ttu-id="36cbe-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36cbe-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36cbe-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="36cbe-136">lastModifiedDateTime</span></span>|<span data-ttu-id="36cbe-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36cbe-137">DateTimeOffset</span></span>|<span data-ttu-id="36cbe-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="36cbe-138">DateTime the object was last modified.</span></span> <span data-ttu-id="36cbe-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36cbe-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36cbe-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="36cbe-140">roleScopeTagIds</span></span>|<span data-ttu-id="36cbe-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="36cbe-141">String collection</span></span>|<span data-ttu-id="36cbe-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="36cbe-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="36cbe-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36cbe-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36cbe-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="36cbe-144">supportsScopeTags</span></span>|<span data-ttu-id="36cbe-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="36cbe-145">Boolean</span></span>|<span data-ttu-id="36cbe-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="36cbe-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="36cbe-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="36cbe-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="36cbe-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="36cbe-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="36cbe-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="36cbe-149">This property is read-only.</span></span> <span data-ttu-id="36cbe-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36cbe-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36cbe-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="36cbe-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="36cbe-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="36cbe-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="36cbe-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="36cbe-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="36cbe-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36cbe-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36cbe-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="36cbe-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="36cbe-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="36cbe-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="36cbe-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="36cbe-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="36cbe-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36cbe-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36cbe-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="36cbe-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="36cbe-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="36cbe-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="36cbe-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="36cbe-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="36cbe-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36cbe-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36cbe-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36cbe-163">createdDateTime</span></span>|<span data-ttu-id="36cbe-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36cbe-164">DateTimeOffset</span></span>|<span data-ttu-id="36cbe-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="36cbe-165">DateTime the object was created.</span></span> <span data-ttu-id="36cbe-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36cbe-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36cbe-167">description</span><span class="sxs-lookup"><span data-stu-id="36cbe-167">description</span></span>|<span data-ttu-id="36cbe-168">String</span><span class="sxs-lookup"><span data-stu-id="36cbe-168">String</span></span>|<span data-ttu-id="36cbe-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="36cbe-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="36cbe-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36cbe-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36cbe-171">displayName</span><span class="sxs-lookup"><span data-stu-id="36cbe-171">displayName</span></span>|<span data-ttu-id="36cbe-172">Строка</span><span class="sxs-lookup"><span data-stu-id="36cbe-172">String</span></span>|<span data-ttu-id="36cbe-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="36cbe-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="36cbe-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36cbe-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36cbe-175">version</span><span class="sxs-lookup"><span data-stu-id="36cbe-175">version</span></span>|<span data-ttu-id="36cbe-176">Int32</span><span class="sxs-lookup"><span data-stu-id="36cbe-176">Int32</span></span>|<span data-ttu-id="36cbe-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="36cbe-177">Version of the device configuration.</span></span> <span data-ttu-id="36cbe-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36cbe-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36cbe-179">bundleId</span><span class="sxs-lookup"><span data-stu-id="36cbe-179">bundleId</span></span>|<span data-ttu-id="36cbe-180">String</span><span class="sxs-lookup"><span data-stu-id="36cbe-180">String</span></span>|<span data-ttu-id="36cbe-181">Идентификатор пакета для нацеленности.</span><span class="sxs-lookup"><span data-stu-id="36cbe-181">Bundle id for targeting.</span></span>|
|<span data-ttu-id="36cbe-182">fileName</span><span class="sxs-lookup"><span data-stu-id="36cbe-182">fileName</span></span>|<span data-ttu-id="36cbe-183">Строка</span><span class="sxs-lookup"><span data-stu-id="36cbe-183">String</span></span>|<span data-ttu-id="36cbe-184">Имя файла конфигурации (\*. plist</span><span class="sxs-lookup"><span data-stu-id="36cbe-184">Configuration file name (\*.plist</span></span> | <span data-ttu-id="36cbe-185">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="36cbe-185">\*.xml).</span></span>|
|<span data-ttu-id="36cbe-186">конфигуратионксмл</span><span class="sxs-lookup"><span data-stu-id="36cbe-186">configurationXml</span></span>|<span data-ttu-id="36cbe-187">Binary</span><span class="sxs-lookup"><span data-stu-id="36cbe-187">Binary</span></span>|<span data-ttu-id="36cbe-188">XML-файл конфигурации.</span><span class="sxs-lookup"><span data-stu-id="36cbe-188">Configuration xml.</span></span> <span data-ttu-id="36cbe-189">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="36cbe-189">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="36cbe-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="36cbe-190">Response</span></span>
<span data-ttu-id="36cbe-191">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макоскустомаппконфигуратион](../resources/intune-deviceconfig-macoscustomappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="36cbe-191">If successful, this method returns a `200 OK` response code and an updated [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36cbe-192">Пример</span><span class="sxs-lookup"><span data-stu-id="36cbe-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="36cbe-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="36cbe-193">Request</span></span>
<span data-ttu-id="36cbe-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36cbe-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1149

{
  "@odata.type": "#microsoft.graph.macOSCustomAppConfiguration",
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
  "bundleId": "Bundle Id value",
  "fileName": "File Name value",
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="36cbe-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="36cbe-195">Response</span></span>
<span data-ttu-id="36cbe-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36cbe-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1321

{
  "@odata.type": "#microsoft.graph.macOSCustomAppConfiguration",
  "id": "1b8a4e02-4e02-1b8a-024e-8a1b024e8a1b",
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
  "bundleId": "Bundle Id value",
  "fileName": "File Name value",
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```





