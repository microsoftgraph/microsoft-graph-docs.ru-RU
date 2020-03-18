---
title: Создание Макоскустомаппконфигуратион
description: Создание нового объекта Макоскустомаппконфигуратион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e05abbf46cf5233c5a47f3f194690a63a5a7404a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42747632"
---
# <a name="create-macoscustomappconfiguration"></a><span data-ttu-id="fe958-103">Создание Макоскустомаппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="fe958-103">Create macOSCustomAppConfiguration</span></span>

> <span data-ttu-id="fe958-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe958-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe958-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe958-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe958-106">Создание нового объекта [макоскустомаппконфигуратион](../resources/intune-deviceconfig-macoscustomappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fe958-106">Create a new [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe958-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fe958-107">Prerequisites</span></span>
<span data-ttu-id="fe958-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe958-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe958-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe958-110">Permission type</span></span>|<span data-ttu-id="fe958-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe958-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe958-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe958-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fe958-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe958-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe958-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe958-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe958-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe958-115">Not supported.</span></span>|
|<span data-ttu-id="fe958-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="fe958-116">Application</span></span>|<span data-ttu-id="fe958-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe958-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe958-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe958-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fe958-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fe958-119">Request headers</span></span>
|<span data-ttu-id="fe958-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe958-120">Header</span></span>|<span data-ttu-id="fe958-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fe958-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe958-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe958-122">Authorization</span></span>|<span data-ttu-id="fe958-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe958-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe958-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fe958-124">Accept</span></span>|<span data-ttu-id="fe958-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fe958-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe958-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe958-126">Request body</span></span>
<span data-ttu-id="fe958-127">В тексте запроса добавьте представление объекта Макоскустомаппконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe958-127">In the request body, supply a JSON representation for the macOSCustomAppConfiguration object.</span></span>

<span data-ttu-id="fe958-128">В следующей таблице приведены свойства, необходимые при создании Макоскустомаппконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="fe958-128">The following table shows the properties that are required when you create the macOSCustomAppConfiguration.</span></span>

|<span data-ttu-id="fe958-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe958-129">Property</span></span>|<span data-ttu-id="fe958-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fe958-130">Type</span></span>|<span data-ttu-id="fe958-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fe958-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe958-132">id</span><span class="sxs-lookup"><span data-stu-id="fe958-132">id</span></span>|<span data-ttu-id="fe958-133">Строка</span><span class="sxs-lookup"><span data-stu-id="fe958-133">String</span></span>|<span data-ttu-id="fe958-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fe958-134">Key of the entity.</span></span> <span data-ttu-id="fe958-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe958-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe958-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe958-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fe958-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe958-137">DateTimeOffset</span></span>|<span data-ttu-id="fe958-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fe958-138">DateTime the object was last modified.</span></span> <span data-ttu-id="fe958-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe958-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe958-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fe958-140">roleScopeTagIds</span></span>|<span data-ttu-id="fe958-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fe958-141">String collection</span></span>|<span data-ttu-id="fe958-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fe958-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fe958-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe958-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe958-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="fe958-144">supportsScopeTags</span></span>|<span data-ttu-id="fe958-145">Логический</span><span class="sxs-lookup"><span data-stu-id="fe958-145">Boolean</span></span>|<span data-ttu-id="fe958-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="fe958-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fe958-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="fe958-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fe958-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fe958-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fe958-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe958-149">This property is read-only.</span></span> <span data-ttu-id="fe958-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe958-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe958-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fe958-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fe958-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fe958-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fe958-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fe958-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fe958-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe958-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe958-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fe958-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fe958-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fe958-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fe958-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fe958-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fe958-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe958-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe958-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fe958-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fe958-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fe958-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fe958-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fe958-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fe958-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe958-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe958-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe958-163">createdDateTime</span></span>|<span data-ttu-id="fe958-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe958-164">DateTimeOffset</span></span>|<span data-ttu-id="fe958-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fe958-165">DateTime the object was created.</span></span> <span data-ttu-id="fe958-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe958-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe958-167">description</span><span class="sxs-lookup"><span data-stu-id="fe958-167">description</span></span>|<span data-ttu-id="fe958-168">String</span><span class="sxs-lookup"><span data-stu-id="fe958-168">String</span></span>|<span data-ttu-id="fe958-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fe958-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fe958-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe958-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe958-171">displayName</span><span class="sxs-lookup"><span data-stu-id="fe958-171">displayName</span></span>|<span data-ttu-id="fe958-172">Строка</span><span class="sxs-lookup"><span data-stu-id="fe958-172">String</span></span>|<span data-ttu-id="fe958-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fe958-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fe958-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe958-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe958-175">version</span><span class="sxs-lookup"><span data-stu-id="fe958-175">version</span></span>|<span data-ttu-id="fe958-176">Int32</span><span class="sxs-lookup"><span data-stu-id="fe958-176">Int32</span></span>|<span data-ttu-id="fe958-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fe958-177">Version of the device configuration.</span></span> <span data-ttu-id="fe958-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe958-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe958-179">bundleId</span><span class="sxs-lookup"><span data-stu-id="fe958-179">bundleId</span></span>|<span data-ttu-id="fe958-180">String</span><span class="sxs-lookup"><span data-stu-id="fe958-180">String</span></span>|<span data-ttu-id="fe958-181">Идентификатор пакета для нацеленности.</span><span class="sxs-lookup"><span data-stu-id="fe958-181">Bundle id for targeting.</span></span>|
|<span data-ttu-id="fe958-182">fileName</span><span class="sxs-lookup"><span data-stu-id="fe958-182">fileName</span></span>|<span data-ttu-id="fe958-183">String</span><span class="sxs-lookup"><span data-stu-id="fe958-183">String</span></span>|<span data-ttu-id="fe958-184">Имя файла конфигурации (\*. plist</span><span class="sxs-lookup"><span data-stu-id="fe958-184">Configuration file name (\*.plist</span></span> | <span data-ttu-id="fe958-185">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="fe958-185">\*.xml).</span></span>|
|<span data-ttu-id="fe958-186">конфигуратионксмл</span><span class="sxs-lookup"><span data-stu-id="fe958-186">configurationXml</span></span>|<span data-ttu-id="fe958-187">Binary</span><span class="sxs-lookup"><span data-stu-id="fe958-187">Binary</span></span>|<span data-ttu-id="fe958-188">XML-файл конфигурации.</span><span class="sxs-lookup"><span data-stu-id="fe958-188">Configuration xml.</span></span> <span data-ttu-id="fe958-189">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="fe958-189">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="fe958-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe958-190">Response</span></span>
<span data-ttu-id="fe958-191">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макоскустомаппконфигуратион](../resources/intune-deviceconfig-macoscustomappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe958-191">If successful, this method returns a `201 Created` response code and a [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe958-192">Пример</span><span class="sxs-lookup"><span data-stu-id="fe958-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe958-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe958-193">Request</span></span>
<span data-ttu-id="fe958-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe958-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="fe958-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe958-195">Response</span></span>
<span data-ttu-id="fe958-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe958-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




