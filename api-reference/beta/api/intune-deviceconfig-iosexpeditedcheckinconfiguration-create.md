---
title: Создание iosExpeditedCheckinConfiguration
description: Создайте новый объект iosExpeditedCheckinConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 97bda095ecbfc6cc0306579fbe5982bdc57eb9b1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148003"
---
# <a name="create-iosexpeditedcheckinconfiguration"></a><span data-ttu-id="428cc-103">Создание iosExpeditedCheckinConfiguration</span><span class="sxs-lookup"><span data-stu-id="428cc-103">Create iosExpeditedCheckinConfiguration</span></span>

<span data-ttu-id="428cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="428cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="428cc-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="428cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="428cc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="428cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="428cc-107">Создайте [новый объект iosExpeditedCheckinConfiguration.](../resources/intune-deviceconfig-iosexpeditedcheckinconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="428cc-107">Create a new [iosExpeditedCheckinConfiguration](../resources/intune-deviceconfig-iosexpeditedcheckinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="428cc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="428cc-108">Prerequisites</span></span>
<span data-ttu-id="428cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="428cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="428cc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="428cc-111">Permission type</span></span>|<span data-ttu-id="428cc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="428cc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="428cc-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="428cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="428cc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="428cc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="428cc-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="428cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="428cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="428cc-116">Not supported.</span></span>|
|<span data-ttu-id="428cc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="428cc-117">Application</span></span>|<span data-ttu-id="428cc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="428cc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="428cc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="428cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="428cc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="428cc-120">Request headers</span></span>
|<span data-ttu-id="428cc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="428cc-121">Header</span></span>|<span data-ttu-id="428cc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="428cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="428cc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="428cc-123">Authorization</span></span>|<span data-ttu-id="428cc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="428cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="428cc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="428cc-125">Accept</span></span>|<span data-ttu-id="428cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="428cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="428cc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="428cc-127">Request body</span></span>
<span data-ttu-id="428cc-128">В теле запроса поставляем представление JSON для объекта iosExpeditedCheckinConfiguration.</span><span class="sxs-lookup"><span data-stu-id="428cc-128">In the request body, supply a JSON representation for the iosExpeditedCheckinConfiguration object.</span></span>

<span data-ttu-id="428cc-129">В следующей таблице показаны свойства, необходимые при создании iosExpeditedCheckinConfiguration.</span><span class="sxs-lookup"><span data-stu-id="428cc-129">The following table shows the properties that are required when you create the iosExpeditedCheckinConfiguration.</span></span>

|<span data-ttu-id="428cc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="428cc-130">Property</span></span>|<span data-ttu-id="428cc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="428cc-131">Type</span></span>|<span data-ttu-id="428cc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="428cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="428cc-133">id</span><span class="sxs-lookup"><span data-stu-id="428cc-133">id</span></span>|<span data-ttu-id="428cc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="428cc-134">String</span></span>|<span data-ttu-id="428cc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="428cc-135">Key of the entity.</span></span> <span data-ttu-id="428cc-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="428cc-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="428cc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="428cc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="428cc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="428cc-138">DateTimeOffset</span></span>|<span data-ttu-id="428cc-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="428cc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="428cc-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="428cc-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="428cc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="428cc-141">roleScopeTagIds</span></span>|<span data-ttu-id="428cc-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="428cc-142">String collection</span></span>|<span data-ttu-id="428cc-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="428cc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="428cc-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="428cc-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="428cc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="428cc-145">supportsScopeTags</span></span>|<span data-ttu-id="428cc-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="428cc-146">Boolean</span></span>|<span data-ttu-id="428cc-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="428cc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="428cc-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="428cc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="428cc-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="428cc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="428cc-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="428cc-150">This property is read-only.</span></span> <span data-ttu-id="428cc-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="428cc-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="428cc-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="428cc-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="428cc-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="428cc-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="428cc-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="428cc-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="428cc-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="428cc-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="428cc-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="428cc-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="428cc-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="428cc-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="428cc-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="428cc-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="428cc-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="428cc-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="428cc-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="428cc-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="428cc-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="428cc-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="428cc-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="428cc-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="428cc-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="428cc-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="428cc-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="428cc-164">createdDateTime</span></span>|<span data-ttu-id="428cc-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="428cc-165">DateTimeOffset</span></span>|<span data-ttu-id="428cc-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="428cc-166">DateTime the object was created.</span></span> <span data-ttu-id="428cc-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="428cc-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="428cc-168">description</span><span class="sxs-lookup"><span data-stu-id="428cc-168">description</span></span>|<span data-ttu-id="428cc-169">Строка</span><span class="sxs-lookup"><span data-stu-id="428cc-169">String</span></span>|<span data-ttu-id="428cc-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="428cc-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="428cc-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="428cc-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="428cc-172">displayName</span><span class="sxs-lookup"><span data-stu-id="428cc-172">displayName</span></span>|<span data-ttu-id="428cc-173">Строка</span><span class="sxs-lookup"><span data-stu-id="428cc-173">String</span></span>|<span data-ttu-id="428cc-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="428cc-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="428cc-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="428cc-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="428cc-176">version</span><span class="sxs-lookup"><span data-stu-id="428cc-176">version</span></span>|<span data-ttu-id="428cc-177">Int32</span><span class="sxs-lookup"><span data-stu-id="428cc-177">Int32</span></span>|<span data-ttu-id="428cc-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="428cc-178">Version of the device configuration.</span></span> <span data-ttu-id="428cc-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="428cc-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="428cc-180">enableExpeditedCheckin</span><span class="sxs-lookup"><span data-stu-id="428cc-180">enableExpeditedCheckin</span></span>|<span data-ttu-id="428cc-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="428cc-181">Boolean</span></span>|<span data-ttu-id="428cc-182">Получает или задает, следует ли включить ускоренную регистрацию устройства. Унаследованный от [appleExpeditedCheckinConfigurationBase](../resources/intune-deviceconfig-appleexpeditedcheckinconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="428cc-182">Gets or sets whether to enable expedited device check-ins. Inherited from [appleExpeditedCheckinConfigurationBase](../resources/intune-deviceconfig-appleexpeditedcheckinconfigurationbase.md)</span></span>|



## <a name="response"></a><span data-ttu-id="428cc-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="428cc-183">Response</span></span>
<span data-ttu-id="428cc-184">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект iosExpeditedCheckinConfiguration](../resources/intune-deviceconfig-iosexpeditedcheckinconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="428cc-184">If successful, this method returns a `201 Created` response code and a [iosExpeditedCheckinConfiguration](../resources/intune-deviceconfig-iosexpeditedcheckinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="428cc-185">Пример</span><span class="sxs-lookup"><span data-stu-id="428cc-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="428cc-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="428cc-186">Request</span></span>
<span data-ttu-id="428cc-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="428cc-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1070

{
  "@odata.type": "#microsoft.graph.iosExpeditedCheckinConfiguration",
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
  "enableExpeditedCheckin": true
}
```

### <a name="response"></a><span data-ttu-id="428cc-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="428cc-188">Response</span></span>
<span data-ttu-id="428cc-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="428cc-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1242

{
  "@odata.type": "#microsoft.graph.iosExpeditedCheckinConfiguration",
  "id": "f833f985-f985-f833-85f9-33f885f933f8",
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
  "enableExpeditedCheckin": true
}
```




