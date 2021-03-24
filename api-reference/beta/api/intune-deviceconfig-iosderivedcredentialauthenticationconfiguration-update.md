---
title: Обновление iosDerivedCredentialAuthenticationConfiguration
description: Обновление свойств объекта iosDerivedCredentialAuthenticationConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cbfdb03868db03f29f22ba7e8e7ede682c37458b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131577"
---
# <a name="update-iosderivedcredentialauthenticationconfiguration"></a><span data-ttu-id="ec580-103">Обновление iosDerivedCredentialAuthenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec580-103">Update iosDerivedCredentialAuthenticationConfiguration</span></span>

<span data-ttu-id="ec580-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec580-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec580-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec580-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec580-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec580-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec580-107">Обновление свойств объекта [iosDerivedCredentialAuthenticationConfiguration.](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ec580-107">Update the properties of a [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec580-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ec580-108">Prerequisites</span></span>
<span data-ttu-id="ec580-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec580-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec580-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec580-111">Permission type</span></span>|<span data-ttu-id="ec580-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec580-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec580-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec580-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec580-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec580-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ec580-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec580-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec580-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec580-116">Not supported.</span></span>|
|<span data-ttu-id="ec580-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ec580-117">Application</span></span>|<span data-ttu-id="ec580-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec580-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec580-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec580-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ec580-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ec580-120">Request headers</span></span>
|<span data-ttu-id="ec580-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ec580-121">Header</span></span>|<span data-ttu-id="ec580-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ec580-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec580-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec580-123">Authorization</span></span>|<span data-ttu-id="ec580-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec580-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec580-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ec580-125">Accept</span></span>|<span data-ttu-id="ec580-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ec580-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec580-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec580-127">Request body</span></span>
<span data-ttu-id="ec580-128">В теле запроса поставляем представление JSON для [объекта iosDerivedCredentialAuthenticationConfiguration.](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ec580-128">In the request body, supply a JSON representation for the [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object.</span></span>

<span data-ttu-id="ec580-129">В следующей таблице показаны свойства, необходимые при создании [iosDerivedCredentialAuthenticationConfiguration.](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ec580-129">The following table shows the properties that are required when you create the [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md).</span></span>

|<span data-ttu-id="ec580-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec580-130">Property</span></span>|<span data-ttu-id="ec580-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ec580-131">Type</span></span>|<span data-ttu-id="ec580-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ec580-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec580-133">id</span><span class="sxs-lookup"><span data-stu-id="ec580-133">id</span></span>|<span data-ttu-id="ec580-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ec580-134">String</span></span>|<span data-ttu-id="ec580-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ec580-135">Key of the entity.</span></span> <span data-ttu-id="ec580-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec580-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec580-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec580-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ec580-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec580-138">DateTimeOffset</span></span>|<span data-ttu-id="ec580-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ec580-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ec580-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec580-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec580-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ec580-141">roleScopeTagIds</span></span>|<span data-ttu-id="ec580-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ec580-142">String collection</span></span>|<span data-ttu-id="ec580-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="ec580-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ec580-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec580-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec580-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ec580-145">supportsScopeTags</span></span>|<span data-ttu-id="ec580-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec580-146">Boolean</span></span>|<span data-ttu-id="ec580-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ec580-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ec580-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="ec580-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ec580-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ec580-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ec580-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec580-150">This property is read-only.</span></span> <span data-ttu-id="ec580-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec580-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec580-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ec580-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ec580-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ec580-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ec580-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ec580-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ec580-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec580-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec580-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ec580-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ec580-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ec580-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ec580-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ec580-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ec580-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec580-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec580-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ec580-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ec580-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ec580-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ec580-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ec580-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ec580-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec580-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec580-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ec580-164">createdDateTime</span></span>|<span data-ttu-id="ec580-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec580-165">DateTimeOffset</span></span>|<span data-ttu-id="ec580-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ec580-166">DateTime the object was created.</span></span> <span data-ttu-id="ec580-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec580-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec580-168">description</span><span class="sxs-lookup"><span data-stu-id="ec580-168">description</span></span>|<span data-ttu-id="ec580-169">Строка</span><span class="sxs-lookup"><span data-stu-id="ec580-169">String</span></span>|<span data-ttu-id="ec580-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ec580-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ec580-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec580-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec580-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ec580-172">displayName</span></span>|<span data-ttu-id="ec580-173">Строка</span><span class="sxs-lookup"><span data-stu-id="ec580-173">String</span></span>|<span data-ttu-id="ec580-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ec580-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ec580-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec580-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec580-176">version</span><span class="sxs-lookup"><span data-stu-id="ec580-176">version</span></span>|<span data-ttu-id="ec580-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ec580-177">Int32</span></span>|<span data-ttu-id="ec580-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ec580-178">Version of the device configuration.</span></span> <span data-ttu-id="ec580-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ec580-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ec580-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec580-180">Response</span></span>
<span data-ttu-id="ec580-181">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ec580-181">If successful, this method returns a `200 OK` response code and an updated [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec580-182">Пример</span><span class="sxs-lookup"><span data-stu-id="ec580-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec580-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec580-183">Request</span></span>
<span data-ttu-id="ec580-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec580-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="ec580-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec580-185">Response</span></span>
<span data-ttu-id="ec580-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec580-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




