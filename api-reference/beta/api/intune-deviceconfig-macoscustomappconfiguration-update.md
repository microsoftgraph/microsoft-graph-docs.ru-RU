---
title: Обновление Макоскустомаппконфигуратион
description: Обновление свойств объекта Макоскустомаппконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c0f19b243a87cc17c161fb21f0b1e2dd5d6f1b1a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283121"
---
# <a name="update-macoscustomappconfiguration"></a><span data-ttu-id="2f633-103">Обновление Макоскустомаппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="2f633-103">Update macOSCustomAppConfiguration</span></span>

<span data-ttu-id="2f633-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f633-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f633-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f633-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f633-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f633-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f633-107">Обновление свойств объекта [макоскустомаппконфигуратион](../resources/intune-deviceconfig-macoscustomappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2f633-107">Update the properties of a [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f633-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2f633-108">Prerequisites</span></span>
<span data-ttu-id="2f633-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f633-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f633-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f633-111">Permission type</span></span>|<span data-ttu-id="2f633-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f633-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f633-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f633-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f633-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f633-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f633-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f633-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f633-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f633-116">Not supported.</span></span>|
|<span data-ttu-id="2f633-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f633-117">Application</span></span>|<span data-ttu-id="2f633-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f633-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f633-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f633-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2f633-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2f633-120">Request headers</span></span>
|<span data-ttu-id="2f633-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f633-121">Header</span></span>|<span data-ttu-id="2f633-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2f633-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f633-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f633-123">Authorization</span></span>|<span data-ttu-id="2f633-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f633-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f633-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2f633-125">Accept</span></span>|<span data-ttu-id="2f633-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f633-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f633-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f633-127">Request body</span></span>
<span data-ttu-id="2f633-128">В тексте запроса добавьте представление объекта [макоскустомаппконфигуратион](../resources/intune-deviceconfig-macoscustomappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f633-128">In the request body, supply a JSON representation for the [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object.</span></span>

<span data-ttu-id="2f633-129">В следующей таблице приведены свойства, необходимые при создании [макоскустомаппконфигуратион](../resources/intune-deviceconfig-macoscustomappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f633-129">The following table shows the properties that are required when you create the [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md).</span></span>

|<span data-ttu-id="2f633-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f633-130">Property</span></span>|<span data-ttu-id="2f633-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2f633-131">Type</span></span>|<span data-ttu-id="2f633-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2f633-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f633-133">id</span><span class="sxs-lookup"><span data-stu-id="2f633-133">id</span></span>|<span data-ttu-id="2f633-134">String</span><span class="sxs-lookup"><span data-stu-id="2f633-134">String</span></span>|<span data-ttu-id="2f633-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2f633-135">Key of the entity.</span></span> <span data-ttu-id="2f633-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f633-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f633-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f633-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2f633-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f633-138">DateTimeOffset</span></span>|<span data-ttu-id="2f633-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2f633-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2f633-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f633-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f633-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2f633-141">roleScopeTagIds</span></span>|<span data-ttu-id="2f633-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2f633-142">String collection</span></span>|<span data-ttu-id="2f633-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2f633-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2f633-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f633-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f633-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="2f633-145">supportsScopeTags</span></span>|<span data-ttu-id="2f633-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f633-146">Boolean</span></span>|<span data-ttu-id="2f633-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="2f633-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2f633-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="2f633-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2f633-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2f633-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2f633-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f633-150">This property is read-only.</span></span> <span data-ttu-id="2f633-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f633-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f633-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2f633-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2f633-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2f633-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2f633-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2f633-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2f633-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f633-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f633-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2f633-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2f633-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2f633-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2f633-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2f633-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2f633-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f633-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f633-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2f633-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2f633-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2f633-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2f633-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2f633-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2f633-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f633-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f633-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f633-164">createdDateTime</span></span>|<span data-ttu-id="2f633-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f633-165">DateTimeOffset</span></span>|<span data-ttu-id="2f633-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2f633-166">DateTime the object was created.</span></span> <span data-ttu-id="2f633-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f633-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f633-168">description</span><span class="sxs-lookup"><span data-stu-id="2f633-168">description</span></span>|<span data-ttu-id="2f633-169">String</span><span class="sxs-lookup"><span data-stu-id="2f633-169">String</span></span>|<span data-ttu-id="2f633-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2f633-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2f633-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f633-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f633-172">displayName</span><span class="sxs-lookup"><span data-stu-id="2f633-172">displayName</span></span>|<span data-ttu-id="2f633-173">String</span><span class="sxs-lookup"><span data-stu-id="2f633-173">String</span></span>|<span data-ttu-id="2f633-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2f633-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2f633-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f633-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f633-176">version</span><span class="sxs-lookup"><span data-stu-id="2f633-176">version</span></span>|<span data-ttu-id="2f633-177">Int32</span><span class="sxs-lookup"><span data-stu-id="2f633-177">Int32</span></span>|<span data-ttu-id="2f633-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2f633-178">Version of the device configuration.</span></span> <span data-ttu-id="2f633-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f633-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f633-180">bundleId</span><span class="sxs-lookup"><span data-stu-id="2f633-180">bundleId</span></span>|<span data-ttu-id="2f633-181">String</span><span class="sxs-lookup"><span data-stu-id="2f633-181">String</span></span>|<span data-ttu-id="2f633-182">Идентификатор пакета для нацеленности.</span><span class="sxs-lookup"><span data-stu-id="2f633-182">Bundle id for targeting.</span></span>|
|<span data-ttu-id="2f633-183">fileName</span><span class="sxs-lookup"><span data-stu-id="2f633-183">fileName</span></span>|<span data-ttu-id="2f633-184">String</span><span class="sxs-lookup"><span data-stu-id="2f633-184">String</span></span>|<span data-ttu-id="2f633-185">Имя файла конфигурации (\*. plist</span><span class="sxs-lookup"><span data-stu-id="2f633-185">Configuration file name (\*.plist</span></span> | <span data-ttu-id="2f633-186">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="2f633-186">\*.xml).</span></span>|
|<span data-ttu-id="2f633-187">конфигуратионксмл</span><span class="sxs-lookup"><span data-stu-id="2f633-187">configurationXml</span></span>|<span data-ttu-id="2f633-188">Binary</span><span class="sxs-lookup"><span data-stu-id="2f633-188">Binary</span></span>|<span data-ttu-id="2f633-189">XML-файл конфигурации.</span><span class="sxs-lookup"><span data-stu-id="2f633-189">Configuration xml.</span></span> <span data-ttu-id="2f633-190">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="2f633-190">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="2f633-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f633-191">Response</span></span>
<span data-ttu-id="2f633-192">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макоскустомаппконфигуратион](../resources/intune-deviceconfig-macoscustomappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f633-192">If successful, this method returns a `200 OK` response code and an updated [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f633-193">Пример</span><span class="sxs-lookup"><span data-stu-id="2f633-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f633-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f633-194">Request</span></span>
<span data-ttu-id="2f633-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f633-195">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f633-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f633-196">Response</span></span>
<span data-ttu-id="2f633-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f633-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




