---
title: Создание Унсуппортеддевицеконфигуратион
description: Создание нового объекта Унсуппортеддевицеконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9a1358eaf63dad3cabf6da98b5c6526b39ee30dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48014849"
---
# <a name="create-unsupporteddeviceconfiguration"></a><span data-ttu-id="0c8fa-103">Создание Унсуппортеддевицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="0c8fa-103">Create unsupportedDeviceConfiguration</span></span>

<span data-ttu-id="0c8fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c8fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c8fa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c8fa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c8fa-107">Создание нового объекта [унсуппортеддевицеконфигуратион](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0c8fa-107">Create a new [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c8fa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0c8fa-108">Prerequisites</span></span>
<span data-ttu-id="0c8fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c8fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c8fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c8fa-111">Permission type</span></span>|<span data-ttu-id="0c8fa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c8fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c8fa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c8fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c8fa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c8fa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c8fa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c8fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c8fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-116">Not supported.</span></span>|
|<span data-ttu-id="0c8fa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c8fa-117">Application</span></span>|<span data-ttu-id="0c8fa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c8fa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c8fa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c8fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0c8fa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0c8fa-120">Request headers</span></span>
|<span data-ttu-id="0c8fa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c8fa-121">Header</span></span>|<span data-ttu-id="0c8fa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0c8fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c8fa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c8fa-123">Authorization</span></span>|<span data-ttu-id="0c8fa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c8fa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0c8fa-125">Accept</span></span>|<span data-ttu-id="0c8fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c8fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c8fa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c8fa-127">Request body</span></span>
<span data-ttu-id="0c8fa-128">В тексте запроса добавьте представление объекта Унсуппортеддевицеконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-128">In the request body, supply a JSON representation for the unsupportedDeviceConfiguration object.</span></span>

<span data-ttu-id="0c8fa-129">В следующей таблице приведены свойства, необходимые при создании Унсуппортеддевицеконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-129">The following table shows the properties that are required when you create the unsupportedDeviceConfiguration.</span></span>

|<span data-ttu-id="0c8fa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c8fa-130">Property</span></span>|<span data-ttu-id="0c8fa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0c8fa-131">Type</span></span>|<span data-ttu-id="0c8fa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0c8fa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c8fa-133">id</span><span class="sxs-lookup"><span data-stu-id="0c8fa-133">id</span></span>|<span data-ttu-id="0c8fa-134">String</span><span class="sxs-lookup"><span data-stu-id="0c8fa-134">String</span></span>|<span data-ttu-id="0c8fa-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-135">Key of the entity.</span></span> <span data-ttu-id="0c8fa-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c8fa-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c8fa-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c8fa-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0c8fa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c8fa-138">DateTimeOffset</span></span>|<span data-ttu-id="0c8fa-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0c8fa-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c8fa-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c8fa-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0c8fa-141">roleScopeTagIds</span></span>|<span data-ttu-id="0c8fa-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0c8fa-142">String collection</span></span>|<span data-ttu-id="0c8fa-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0c8fa-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c8fa-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c8fa-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="0c8fa-145">supportsScopeTags</span></span>|<span data-ttu-id="0c8fa-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c8fa-146">Boolean</span></span>|<span data-ttu-id="0c8fa-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0c8fa-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0c8fa-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0c8fa-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-150">This property is read-only.</span></span> <span data-ttu-id="0c8fa-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c8fa-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c8fa-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0c8fa-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0c8fa-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0c8fa-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0c8fa-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0c8fa-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c8fa-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c8fa-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0c8fa-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0c8fa-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0c8fa-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0c8fa-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0c8fa-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c8fa-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c8fa-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0c8fa-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0c8fa-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0c8fa-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0c8fa-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0c8fa-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c8fa-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c8fa-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c8fa-164">createdDateTime</span></span>|<span data-ttu-id="0c8fa-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c8fa-165">DateTimeOffset</span></span>|<span data-ttu-id="0c8fa-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-166">DateTime the object was created.</span></span> <span data-ttu-id="0c8fa-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c8fa-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c8fa-168">description</span><span class="sxs-lookup"><span data-stu-id="0c8fa-168">description</span></span>|<span data-ttu-id="0c8fa-169">String</span><span class="sxs-lookup"><span data-stu-id="0c8fa-169">String</span></span>|<span data-ttu-id="0c8fa-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0c8fa-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c8fa-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c8fa-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0c8fa-172">displayName</span></span>|<span data-ttu-id="0c8fa-173">String</span><span class="sxs-lookup"><span data-stu-id="0c8fa-173">String</span></span>|<span data-ttu-id="0c8fa-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0c8fa-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c8fa-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c8fa-176">version</span><span class="sxs-lookup"><span data-stu-id="0c8fa-176">version</span></span>|<span data-ttu-id="0c8fa-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0c8fa-177">Int32</span></span>|<span data-ttu-id="0c8fa-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-178">Version of the device configuration.</span></span> <span data-ttu-id="0c8fa-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c8fa-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0c8fa-180">оригиналентититипенаме</span><span class="sxs-lookup"><span data-stu-id="0c8fa-180">originalEntityTypeName</span></span>|<span data-ttu-id="0c8fa-181">String</span><span class="sxs-lookup"><span data-stu-id="0c8fa-181">String</span></span>|<span data-ttu-id="0c8fa-182">Тип сущности, возвращаемой в противном случае.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-182">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="0c8fa-183">details</span><span class="sxs-lookup"><span data-stu-id="0c8fa-183">details</span></span>|<span data-ttu-id="0c8fa-184">Коллекция [унсуппортеддевицеконфигуратиондетаил](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)</span><span class="sxs-lookup"><span data-stu-id="0c8fa-184">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="0c8fa-185">Сведения о том, почему сущность не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-185">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="0c8fa-186">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-186">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="0c8fa-187">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c8fa-187">Response</span></span>
<span data-ttu-id="0c8fa-188">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [унсуппортеддевицеконфигуратион](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-188">If successful, this method returns a `201 Created` response code and a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c8fa-189">Пример</span><span class="sxs-lookup"><span data-stu-id="0c8fa-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c8fa-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c8fa-190">Request</span></span>
<span data-ttu-id="0c8fa-191">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-191">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1291

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
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
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="0c8fa-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c8fa-192">Response</span></span>
<span data-ttu-id="0c8fa-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c8fa-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1463

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
  "id": "f80d6fc8-6fc8-f80d-c86f-0df8c86f0df8",
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
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```






