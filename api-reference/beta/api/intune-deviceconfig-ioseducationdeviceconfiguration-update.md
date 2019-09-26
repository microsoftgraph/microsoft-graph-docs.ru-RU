---
title: Обновление iosEducationDeviceConfiguration
description: Обновление свойств объекта iosEducationDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3aec9a9459d35c095ee5a35f6d0a90f00fccc2aa
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37167749"
---
# <a name="update-ioseducationdeviceconfiguration"></a><span data-ttu-id="34a84-103">Обновление iosEducationDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="34a84-103">Update iosEducationDeviceConfiguration</span></span>

> <span data-ttu-id="34a84-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34a84-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34a84-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34a84-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34a84-106">Обновление свойств объекта [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="34a84-106">Update the properties of a [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34a84-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="34a84-107">Prerequisites</span></span>
<span data-ttu-id="34a84-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34a84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34a84-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34a84-110">Permission type</span></span>|<span data-ttu-id="34a84-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="34a84-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34a84-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34a84-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34a84-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34a84-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34a84-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34a84-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34a84-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34a84-115">Not supported.</span></span>|
|<span data-ttu-id="34a84-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34a84-116">Application</span></span>|<span data-ttu-id="34a84-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34a84-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34a84-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34a84-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="34a84-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34a84-119">Request headers</span></span>
|<span data-ttu-id="34a84-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34a84-120">Header</span></span>|<span data-ttu-id="34a84-121">Значение</span><span class="sxs-lookup"><span data-stu-id="34a84-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34a84-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34a84-122">Authorization</span></span>|<span data-ttu-id="34a84-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34a84-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34a84-124">Accept</span><span class="sxs-lookup"><span data-stu-id="34a84-124">Accept</span></span>|<span data-ttu-id="34a84-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34a84-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34a84-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="34a84-126">Request body</span></span>
<span data-ttu-id="34a84-127">В тексте запроса добавьте представление объекта [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34a84-127">In the request body, supply a JSON representation for the [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object.</span></span>

<span data-ttu-id="34a84-128">В следующей таблице приведены свойства, необходимые при создании [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a84-128">The following table shows the properties that are required when you create the [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md).</span></span>

|<span data-ttu-id="34a84-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="34a84-129">Property</span></span>|<span data-ttu-id="34a84-130">Тип</span><span class="sxs-lookup"><span data-stu-id="34a84-130">Type</span></span>|<span data-ttu-id="34a84-131">Описание</span><span class="sxs-lookup"><span data-stu-id="34a84-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34a84-132">id</span><span class="sxs-lookup"><span data-stu-id="34a84-132">id</span></span>|<span data-ttu-id="34a84-133">String</span><span class="sxs-lookup"><span data-stu-id="34a84-133">String</span></span>|<span data-ttu-id="34a84-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="34a84-134">Key of the entity.</span></span> <span data-ttu-id="34a84-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a84-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a84-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34a84-136">lastModifiedDateTime</span></span>|<span data-ttu-id="34a84-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34a84-137">DateTimeOffset</span></span>|<span data-ttu-id="34a84-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="34a84-138">DateTime the object was last modified.</span></span> <span data-ttu-id="34a84-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a84-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a84-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="34a84-140">roleScopeTagIds</span></span>|<span data-ttu-id="34a84-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="34a84-141">String collection</span></span>|<span data-ttu-id="34a84-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="34a84-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="34a84-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a84-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a84-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="34a84-144">supportsScopeTags</span></span>|<span data-ttu-id="34a84-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="34a84-145">Boolean</span></span>|<span data-ttu-id="34a84-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="34a84-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="34a84-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="34a84-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="34a84-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="34a84-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="34a84-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="34a84-149">This property is read-only.</span></span> <span data-ttu-id="34a84-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a84-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a84-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="34a84-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="34a84-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="34a84-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="34a84-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="34a84-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="34a84-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a84-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a84-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="34a84-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="34a84-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="34a84-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="34a84-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="34a84-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="34a84-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a84-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a84-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="34a84-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="34a84-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="34a84-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="34a84-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="34a84-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="34a84-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a84-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a84-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34a84-163">createdDateTime</span></span>|<span data-ttu-id="34a84-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34a84-164">DateTimeOffset</span></span>|<span data-ttu-id="34a84-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="34a84-165">DateTime the object was created.</span></span> <span data-ttu-id="34a84-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a84-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a84-167">description</span><span class="sxs-lookup"><span data-stu-id="34a84-167">description</span></span>|<span data-ttu-id="34a84-168">String</span><span class="sxs-lookup"><span data-stu-id="34a84-168">String</span></span>|<span data-ttu-id="34a84-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="34a84-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="34a84-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a84-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a84-171">displayName</span><span class="sxs-lookup"><span data-stu-id="34a84-171">displayName</span></span>|<span data-ttu-id="34a84-172">Строка</span><span class="sxs-lookup"><span data-stu-id="34a84-172">String</span></span>|<span data-ttu-id="34a84-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="34a84-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="34a84-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34a84-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a84-175">version</span><span class="sxs-lookup"><span data-stu-id="34a84-175">version</span></span>|<span data-ttu-id="34a84-176">Int32</span><span class="sxs-lookup"><span data-stu-id="34a84-176">Int32</span></span>|<span data-ttu-id="34a84-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="34a84-177">Version of the device configuration.</span></span> <span data-ttu-id="34a84-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a84-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="34a84-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="34a84-179">Response</span></span>
<span data-ttu-id="34a84-180">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34a84-180">If successful, this method returns a `200 OK` response code and an updated [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34a84-181">Пример</span><span class="sxs-lookup"><span data-stu-id="34a84-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="34a84-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="34a84-182">Request</span></span>
<span data-ttu-id="34a84-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34a84-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1034

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="34a84-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="34a84-184">Response</span></span>
<span data-ttu-id="34a84-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34a84-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1206

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
  "id": "3d563be4-3be4-3d56-e43b-563de43b563d",
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




