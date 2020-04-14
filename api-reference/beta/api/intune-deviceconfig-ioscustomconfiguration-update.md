---
title: Обновление объекта iosCustomConfiguration
description: Обновление свойств объекта iosCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6b9ccc85482bbf32ea8ba403e81f7ccadce0e353
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432869"
---
# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="36f59-103">Обновление объекта iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="36f59-103">Update iosCustomConfiguration</span></span>

<span data-ttu-id="36f59-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36f59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36f59-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36f59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36f59-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36f59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36f59-107">Обновление свойств объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36f59-107">Update the properties of a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36f59-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="36f59-108">Prerequisites</span></span>
<span data-ttu-id="36f59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36f59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36f59-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36f59-111">Permission type</span></span>|<span data-ttu-id="36f59-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="36f59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36f59-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36f59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36f59-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36f59-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="36f59-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36f59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36f59-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36f59-116">Not supported.</span></span>|
|<span data-ttu-id="36f59-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="36f59-117">Application</span></span>|<span data-ttu-id="36f59-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36f59-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36f59-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36f59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="36f59-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="36f59-120">Request headers</span></span>
|<span data-ttu-id="36f59-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36f59-121">Header</span></span>|<span data-ttu-id="36f59-122">Значение</span><span class="sxs-lookup"><span data-stu-id="36f59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36f59-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36f59-123">Authorization</span></span>|<span data-ttu-id="36f59-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36f59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36f59-125">Accept</span><span class="sxs-lookup"><span data-stu-id="36f59-125">Accept</span></span>|<span data-ttu-id="36f59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36f59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36f59-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36f59-127">Request body</span></span>
<span data-ttu-id="36f59-128">В теле запроса добавьте представление объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36f59-128">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="36f59-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36f59-129">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="36f59-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="36f59-130">Property</span></span>|<span data-ttu-id="36f59-131">Тип</span><span class="sxs-lookup"><span data-stu-id="36f59-131">Type</span></span>|<span data-ttu-id="36f59-132">Описание</span><span class="sxs-lookup"><span data-stu-id="36f59-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36f59-133">id</span><span class="sxs-lookup"><span data-stu-id="36f59-133">id</span></span>|<span data-ttu-id="36f59-134">Строка</span><span class="sxs-lookup"><span data-stu-id="36f59-134">String</span></span>|<span data-ttu-id="36f59-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="36f59-135">Key of the entity.</span></span> <span data-ttu-id="36f59-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36f59-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36f59-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="36f59-137">lastModifiedDateTime</span></span>|<span data-ttu-id="36f59-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36f59-138">DateTimeOffset</span></span>|<span data-ttu-id="36f59-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="36f59-139">DateTime the object was last modified.</span></span> <span data-ttu-id="36f59-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36f59-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36f59-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="36f59-141">roleScopeTagIds</span></span>|<span data-ttu-id="36f59-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="36f59-142">String collection</span></span>|<span data-ttu-id="36f59-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="36f59-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="36f59-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36f59-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36f59-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="36f59-145">supportsScopeTags</span></span>|<span data-ttu-id="36f59-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="36f59-146">Boolean</span></span>|<span data-ttu-id="36f59-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="36f59-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="36f59-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="36f59-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="36f59-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="36f59-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="36f59-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="36f59-150">This property is read-only.</span></span> <span data-ttu-id="36f59-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36f59-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36f59-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="36f59-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="36f59-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="36f59-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="36f59-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="36f59-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="36f59-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36f59-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36f59-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="36f59-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="36f59-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="36f59-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="36f59-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="36f59-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="36f59-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36f59-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36f59-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="36f59-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="36f59-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="36f59-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="36f59-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="36f59-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="36f59-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36f59-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36f59-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36f59-164">createdDateTime</span></span>|<span data-ttu-id="36f59-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36f59-165">DateTimeOffset</span></span>|<span data-ttu-id="36f59-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="36f59-166">DateTime the object was created.</span></span> <span data-ttu-id="36f59-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36f59-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36f59-168">description</span><span class="sxs-lookup"><span data-stu-id="36f59-168">description</span></span>|<span data-ttu-id="36f59-169">String</span><span class="sxs-lookup"><span data-stu-id="36f59-169">String</span></span>|<span data-ttu-id="36f59-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="36f59-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="36f59-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36f59-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36f59-172">displayName</span><span class="sxs-lookup"><span data-stu-id="36f59-172">displayName</span></span>|<span data-ttu-id="36f59-173">Строка</span><span class="sxs-lookup"><span data-stu-id="36f59-173">String</span></span>|<span data-ttu-id="36f59-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="36f59-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="36f59-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36f59-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36f59-176">version</span><span class="sxs-lookup"><span data-stu-id="36f59-176">version</span></span>|<span data-ttu-id="36f59-177">Int32</span><span class="sxs-lookup"><span data-stu-id="36f59-177">Int32</span></span>|<span data-ttu-id="36f59-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="36f59-178">Version of the device configuration.</span></span> <span data-ttu-id="36f59-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36f59-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="36f59-180">payloadName</span><span class="sxs-lookup"><span data-stu-id="36f59-180">payloadName</span></span>|<span data-ttu-id="36f59-181">String</span><span class="sxs-lookup"><span data-stu-id="36f59-181">String</span></span>|<span data-ttu-id="36f59-182">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="36f59-182">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="36f59-183">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="36f59-183">payloadFileName</span></span>|<span data-ttu-id="36f59-184">String</span><span class="sxs-lookup"><span data-stu-id="36f59-184">String</span></span>|<span data-ttu-id="36f59-185">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="36f59-185">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="36f59-186">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="36f59-186">\*.xml).</span></span>|
|<span data-ttu-id="36f59-187">payload</span><span class="sxs-lookup"><span data-stu-id="36f59-187">payload</span></span>|<span data-ttu-id="36f59-188">Binary</span><span class="sxs-lookup"><span data-stu-id="36f59-188">Binary</span></span>|<span data-ttu-id="36f59-189">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="36f59-189">Payload.</span></span> <span data-ttu-id="36f59-190">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="36f59-190">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="36f59-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="36f59-191">Response</span></span>
<span data-ttu-id="36f59-192">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="36f59-192">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36f59-193">Пример</span><span class="sxs-lookup"><span data-stu-id="36f59-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="36f59-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="36f59-194">Request</span></span>
<span data-ttu-id="36f59-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36f59-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1144

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="36f59-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="36f59-196">Response</span></span>
<span data-ttu-id="36f59-p114">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36f59-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1316

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
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



